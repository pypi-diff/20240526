# Comparing `tmp/napatrackmater-5.2.4.tar.gz` & `tmp/napatrackmater-5.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napatrackmater-5.2.4.tar", last modified: Fri May 17 20:37:31 2024, max compression
+gzip compressed data, was "napatrackmater-5.2.5.tar", last modified: Sun May 26 15:13:53 2024, max compression
```

## Comparing `napatrackmater-5.2.4.tar` & `napatrackmater-5.2.5.tar`

### file list

```diff
@@ -1,281 +1,281 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.027380 napatrackmater-5.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.983380 napatrackmater-5.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.995380 napatrackmater-5.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/MASTER.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.995380 napatrackmater-5.2.4/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/Notebooks/Track_vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-17 20:37:31.027380 napatrackmater-5.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.999380 napatrackmater-5.2.4/_build/.doctrees/
--rw-r--r--   0 runner    (1001) docker     (127)    33531 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/.doctrees/MASTER.doctree
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.999380 napatrackmater-5.2.4/_build/.doctrees/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    29083 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/.doctrees/Notebooks/Track_vector.doctree
--rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/.doctrees/README.doctree
--rw-r--r--   0 runner    (1001) docker     (127)    36454 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/.doctrees/environment.pickle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.999380 napatrackmater-5.2.4/_build/html/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/.buildinfo
--rw-r--r--   0 runner    (1001) docker     (127)    29915 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/MASTER.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.999380 napatrackmater-5.2.4/_build/html/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    66062 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/Notebooks/Track_vector.html
--rw-r--r--   0 runner    (1001) docker     (127)    18885 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/README.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.999380 napatrackmater-5.2.4/_build/html/_images/
--rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_images/ClusterDistributionPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_images/ClusterNearnessPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_images/ClusterPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_images/FeatureMatrixPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_images/QuadrantDistributionPlot_time_point_97.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.003380 napatrackmater-5.2.4/_build/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_sources/MASTER.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.003380 napatrackmater-5.2.4/_build/html/_sources/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_sources/Notebooks/Track_vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_sources/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.003380 napatrackmater-5.2.4/_build/html/_sphinx_design_static/
--rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_sphinx_design_static/design-tabs.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.007380 napatrackmater-5.2.4/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    14692 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/check-solid.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/copy-button.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/copybutton.css
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/copybutton.js
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/copybutton_funcs.js
--rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/design-tabs.js
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/file.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.007380 napatrackmater-5.2.4/_build/html/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/images/logo_binder.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/images/logo_colab.png
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/images/logo_deepnote.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/images/logo_jupyterhub.svg
--rw-r--r--   0 runner    (1001) docker     (127)   287630 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 runner    (1001) docker     (127)    89476 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/kapoorlablogo.png
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/language_data.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.983380 napatrackmater-5.2.4/_build/html/_static/locales/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.007380 napatrackmater-5.2.4/_build/html/_static/locales/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.983380 napatrackmater-5.2.4/_build/html/_static/locales/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.983380 napatrackmater-5.2.4/_build/html/_static/locales/bn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/bn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.983380 napatrackmater-5.2.4/_build/html/_static/locales/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.983380 napatrackmater-5.2.4/_build/html/_static/locales/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.983380 napatrackmater-5.2.4/_build/html/_static/locales/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.983380 napatrackmater-5.2.4/_build/html/_static/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.983380 napatrackmater-5.2.4/_build/html/_static/locales/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.983380 napatrackmater-5.2.4/_build/html/_static/locales/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.983380 napatrackmater-5.2.4/_build/html/_static/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/id/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/iw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/iw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/lv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/ml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/ml/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/mr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/mr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/ms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/ms/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.011380 napatrackmater-5.2.4/_build/html/_static/locales/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/no/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.987380 napatrackmater-5.2.4/_build/html/_static/locales/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/sl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/sr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/ta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/ta/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/te/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/te/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/tg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/tg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/th/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/tl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/tl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/ur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/vi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/locales/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.015380 napatrackmater-5.2.4/_build/html/_static/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)    39364 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/sbt-webpack-macros.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.019380 napatrackmater-5.2.4/_build/html/_static/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)    80813 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/scripts/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   335757 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/scripts/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (127)    19648 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0 runner    (1001) docker     (127)    13066 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    16634 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/sphinx-thebe.css
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/sphinx-thebe.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.019380 napatrackmater-5.2.4/_build/html/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (127)   176654 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/styles/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)    63341 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/styles/sphinx-book-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/styles/theme.css
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/togglebutton.css
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/togglebutton.js
--rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/underscore.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.991380 napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.019380 napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.019380 napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/css/
--rw-r--r--   0 runner    (1001) docker     (127)   101691 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.023380 napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/
--rw-r--r--   0 runner    (1001) docker     (127)   181264 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   105112 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    60236 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    24028 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   389948 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   154840 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/_static/webpack-macros.html
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (127)    12010 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/search.html
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/html/searchindex.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.995380 napatrackmater-5.2.4/_build/jupyter_execute/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.023380 napatrackmater-5.2.4/_build/jupyter_execute/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    17500 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_build/jupyter_execute/Notebooks/Track_vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.023380 napatrackmater-5.2.4/images/
--rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/images/ClusterDistributionPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/images/ClusterNearnessPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/images/ClusterPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/images/FeatureMatrixPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/images/QuadrantDistributionPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/images/kapoorlablogo.png
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/images/kapoorlogo.png
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-17 20:37:31.027380 napatrackmater-5.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:30.995380 napatrackmater-5.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.027380 napatrackmater-5.2.4/src/napatrackmater/
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/src/napatrackmater/CloudAutoEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/src/napatrackmater/DeepEmbeddedClustering.py
--rw-r--r--   0 runner    (1001) docker     (127)   145682 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/src/napatrackmater/Trackmate.py
--rw-r--r--   0 runner    (1001) docker     (127)   125533 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/src/napatrackmater/Trackvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/src/napatrackmater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/src/napatrackmater/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    24585 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/src/napatrackmater/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/src/napatrackmater/fast_radius_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/src/napatrackmater/fate_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/src/napatrackmater/pretrained.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:37:31.027380 napatrackmater-5.2.4/src/napatrackmater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-17 20:37:30.000000 napatrackmater-5.2.4/src/napatrackmater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-17 20:37:30.000000 napatrackmater-5.2.4/src/napatrackmater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:37:30.000000 napatrackmater-5.2.4/src/napatrackmater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-17 20:37:30.000000 napatrackmater-5.2.4/src/napatrackmater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 20:37:30.000000 napatrackmater-5.2.4/src/napatrackmater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-17 20:37:19.000000 napatrackmater-5.2.4/update_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.604678 napatrackmater-5.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.552677 napatrackmater-5.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.568678 napatrackmater-5.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/MASTER.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.568678 napatrackmater-5.2.5/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/Notebooks/Track_vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-26 15:13:53.604678 napatrackmater-5.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.572677 napatrackmater-5.2.5/_build/.doctrees/
+-rw-r--r--   0 runner    (1001) docker     (127)    33531 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/.doctrees/MASTER.doctree
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.572677 napatrackmater-5.2.5/_build/.doctrees/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    29083 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/.doctrees/Notebooks/Track_vector.doctree
+-rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/.doctrees/README.doctree
+-rw-r--r--   0 runner    (1001) docker     (127)    36454 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/.doctrees/environment.pickle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.572677 napatrackmater-5.2.5/_build/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/.buildinfo
+-rw-r--r--   0 runner    (1001) docker     (127)    29915 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/MASTER.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.572677 napatrackmater-5.2.5/_build/html/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    66062 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/Notebooks/Track_vector.html
+-rw-r--r--   0 runner    (1001) docker     (127)    18885 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/README.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.572677 napatrackmater-5.2.5/_build/html/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_images/ClusterDistributionPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_images/ClusterNearnessPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_images/ClusterPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_images/FeatureMatrixPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_images/QuadrantDistributionPlot_time_point_97.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.576678 napatrackmater-5.2.5/_build/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_sources/MASTER.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.576678 napatrackmater-5.2.5/_build/html/_sources/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_sources/Notebooks/Track_vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_sources/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.576678 napatrackmater-5.2.5/_build/html/_sphinx_design_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_sphinx_design_static/design-tabs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.580678 napatrackmater-5.2.5/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14692 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/check-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/copy-button.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/copybutton.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/copybutton.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/copybutton_funcs.js
+-rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/design-tabs.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/file.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/images/logo_binder.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/images/logo_colab.png
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/images/logo_deepnote.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/images/logo_jupyterhub.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   287630 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89476 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/kapoorlablogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/language_data.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/locales/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.556677 napatrackmater-5.2.5/_build/html/_static/locales/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.556677 napatrackmater-5.2.5/_build/html/_static/locales/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.556677 napatrackmater-5.2.5/_build/html/_static/locales/bn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/bn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.556677 napatrackmater-5.2.5/_build/html/_static/locales/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.556677 napatrackmater-5.2.5/_build/html/_static/locales/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.556677 napatrackmater-5.2.5/_build/html/_static/locales/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.556677 napatrackmater-5.2.5/_build/html/_static/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.556677 napatrackmater-5.2.5/_build/html/_static/locales/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.556677 napatrackmater-5.2.5/_build/html/_static/locales/eo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.556677 napatrackmater-5.2.5/_build/html/_static/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.556677 napatrackmater-5.2.5/_build/html/_static/locales/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.556677 napatrackmater-5.2.5/_build/html/_static/locales/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/id/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/iw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/iw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.584678 napatrackmater-5.2.5/_build/html/_static/locales/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/lv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/ml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/ml/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/mr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/mr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/ms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/ms/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.560677 napatrackmater-5.2.5/_build/html/_static/locales/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/locales/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/locales/sl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/locales/sr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/locales/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/locales/ta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/locales/te/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/te/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/locales/tg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/tg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/locales/th/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/locales/tl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/tl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/locales/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/locales/ur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.588678 napatrackmater-5.2.5/_build/html/_static/locales/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/locales/vi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.592678 napatrackmater-5.2.5/_build/html/_static/locales/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/locales/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.592678 napatrackmater-5.2.5/_build/html/_static/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/locales/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.592678 napatrackmater-5.2.5/_build/html/_static/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39364 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/sbt-webpack-macros.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.592678 napatrackmater-5.2.5/_build/html/_static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    80813 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/scripts/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   335757 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/scripts/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19648 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/scripts/sphinx-book-theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13066 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/scripts/sphinx-book-theme.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    16634 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/sphinx-thebe.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/sphinx-thebe.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.592678 napatrackmater-5.2.5/_build/html/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)   176654 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/styles/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)    63341 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/styles/sphinx-book-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/styles/theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/togglebutton.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/togglebutton.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/underscore.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.564677 napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.592678 napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.596678 napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   101691 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.596678 napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   181264 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   105112 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    60236 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    24028 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   389948 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   154840 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/_static/webpack-macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (127)    12010 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/html/searchindex.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.568678 napatrackmater-5.2.5/_build/jupyter_execute/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.596678 napatrackmater-5.2.5/_build/jupyter_execute/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    17500 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_build/jupyter_execute/Notebooks/Track_vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.600678 napatrackmater-5.2.5/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/images/ClusterDistributionPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/images/ClusterNearnessPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/images/ClusterPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/images/FeatureMatrixPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/images/QuadrantDistributionPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/images/kapoorlablogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/images/kapoorlogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-26 15:13:53.604678 napatrackmater-5.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.568678 napatrackmater-5.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.600678 napatrackmater-5.2.5/src/napatrackmater/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/src/napatrackmater/CloudAutoEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/src/napatrackmater/DeepEmbeddedClustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)   145682 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/src/napatrackmater/Trackmate.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127073 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/src/napatrackmater/Trackvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/src/napatrackmater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/src/napatrackmater/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24585 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/src/napatrackmater/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/src/napatrackmater/fast_radius_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/src/napatrackmater/fate_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/src/napatrackmater/pretrained.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:13:53.604678 napatrackmater-5.2.5/src/napatrackmater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-26 15:13:53.000000 napatrackmater-5.2.5/src/napatrackmater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-26 15:13:53.000000 napatrackmater-5.2.5/src/napatrackmater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 15:13:53.000000 napatrackmater-5.2.5/src/napatrackmater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-26 15:13:53.000000 napatrackmater-5.2.5/src/napatrackmater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-26 15:13:53.000000 napatrackmater-5.2.5/src/napatrackmater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-26 15:13:42.000000 napatrackmater-5.2.5/update_version.py
```

### Comparing `napatrackmater-5.2.4/.github/workflows/deploy.yml` & `napatrackmater-5.2.5/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/.github/workflows/test_and_deploy.yml` & `napatrackmater-5.2.5/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/.gitignore` & `napatrackmater-5.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/.pre-commit-config.yaml` & `napatrackmater-5.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/.travis.yml` & `napatrackmater-5.2.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/Dockerfile` & `napatrackmater-5.2.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/LICENSE` & `napatrackmater-5.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/MASTER.md` & `napatrackmater-5.2.5/MASTER.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/Notebooks/Track_vector.ipynb` & `napatrackmater-5.2.5/Notebooks/Track_vector.ipynb`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/PKG-INFO` & `napatrackmater-5.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 5.2.4
+Version: 5.2.5
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/Kapoorlabs-CAPED/napatrackmater
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/napatrackmater/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/napatrackmater#README.md
@@ -35,14 +35,15 @@
 Requires-Dist: kapoorlabs-lightning
 Requires-Dist: lightning
 Requires-Dist: trimesh
 Requires-Dist: umap-learn
 Requires-Dist: plotly
 Requires-Dist: pymesh
 Requires-Dist: torchsummary
+Requires-Dist: statsmodels
 Requires-Dist: numpy
 Provides-Extra: testing
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-qt; extra == "testing"
 Requires-Dist: napari; extra == "testing"
```

### Comparing `napatrackmater-5.2.4/README.md` & `napatrackmater-5.2.5/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/.doctrees/MASTER.doctree` & `napatrackmater-5.2.5/_build/.doctrees/MASTER.doctree`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/.doctrees/Notebooks/Track_vector.doctree` & `napatrackmater-5.2.5/_build/.doctrees/Notebooks/Track_vector.doctree`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/.doctrees/README.doctree` & `napatrackmater-5.2.5/_build/.doctrees/README.doctree`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/.doctrees/environment.pickle` & `napatrackmater-5.2.5/_build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/MASTER.html` & `napatrackmater-5.2.5/_build/html/MASTER.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/Notebooks/Track_vector.html` & `napatrackmater-5.2.5/_build/html/Notebooks/Track_vector.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/README.html` & `napatrackmater-5.2.5/_build/html/README.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_images/ClusterDistributionPlot_time_point_97.png` & `napatrackmater-5.2.5/_build/html/_images/ClusterDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_images/ClusterNearnessPlot_time_point_97.png` & `napatrackmater-5.2.5/_build/html/_images/ClusterNearnessPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_images/ClusterPlot_time_point_97.png` & `napatrackmater-5.2.5/_build/html/_images/ClusterPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_images/FeatureMatrixPlot_time_point_97.png` & `napatrackmater-5.2.5/_build/html/_images/FeatureMatrixPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_images/QuadrantDistributionPlot_time_point_97.png` & `napatrackmater-5.2.5/_build/html/_images/QuadrantDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_sources/MASTER.md` & `napatrackmater-5.2.5/_build/html/_sources/MASTER.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_sources/Notebooks/Track_vector.ipynb` & `napatrackmater-5.2.5/_build/html/_sources/Notebooks/Track_vector.ipynb`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_sources/README.md` & `napatrackmater-5.2.5/_build/html/_sources/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css` & `napatrackmater-5.2.5/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_sphinx_design_static/design-tabs.js` & `napatrackmater-5.2.5/_build/html/_sphinx_design_static/design-tabs.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/basic.css` & `napatrackmater-5.2.5/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/clipboard.min.js` & `napatrackmater-5.2.5/_build/html/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/copybutton.css` & `napatrackmater-5.2.5/_build/html/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/copybutton.js` & `napatrackmater-5.2.5/_build/html/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/copybutton_funcs.js` & `napatrackmater-5.2.5/_build/html/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css` & `napatrackmater-5.2.5/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/design-tabs.js` & `napatrackmater-5.2.5/_build/html/_static/design-tabs.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/doctools.js` & `napatrackmater-5.2.5/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/images/logo_binder.svg` & `napatrackmater-5.2.5/_build/html/_static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/images/logo_colab.png` & `napatrackmater-5.2.5/_build/html/_static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/images/logo_deepnote.svg` & `napatrackmater-5.2.5/_build/html/_static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/images/logo_jupyterhub.svg` & `napatrackmater-5.2.5/_build/html/_static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/jquery-3.5.1.js` & `napatrackmater-5.2.5/_build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/jquery.js` & `napatrackmater-5.2.5/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/kapoorlablogo.png` & `napatrackmater-5.2.5/_build/html/_static/kapoorlablogo.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/language_data.js` & `napatrackmater-5.2.5/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.5/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css` & `napatrackmater-5.2.5/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/pygments.css` & `napatrackmater-5.2.5/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/scripts/bootstrap.js` & `napatrackmater-5.2.5/_build/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/scripts/bootstrap.js.map` & `napatrackmater-5.2.5/_build/html/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/scripts/pydata-sphinx-theme.js` & `napatrackmater-5.2.5/_build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/scripts/pydata-sphinx-theme.js.map` & `napatrackmater-5.2.5/_build/html/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/scripts/sphinx-book-theme.js` & `napatrackmater-5.2.5/_build/html/_static/scripts/sphinx-book-theme.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/scripts/sphinx-book-theme.js.map` & `napatrackmater-5.2.5/_build/html/_static/scripts/sphinx-book-theme.js.map`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/searchtools.js` & `napatrackmater-5.2.5/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/sphinx-thebe.css` & `napatrackmater-5.2.5/_build/html/_static/sphinx-thebe.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/sphinx-thebe.js` & `napatrackmater-5.2.5/_build/html/_static/sphinx-thebe.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/styles/bootstrap.css` & `napatrackmater-5.2.5/_build/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/styles/pydata-sphinx-theme.css` & `napatrackmater-5.2.5/_build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/styles/sphinx-book-theme.css` & `napatrackmater-5.2.5/_build/html/_static/styles/sphinx-book-theme.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/togglebutton.css` & `napatrackmater-5.2.5/_build/html/_static/togglebutton.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/togglebutton.js` & `napatrackmater-5.2.5/_build/html/_static/togglebutton.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/underscore-1.13.1.js` & `napatrackmater-5.2.5/_build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/underscore.js` & `napatrackmater-5.2.5/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `napatrackmater-5.2.5/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/_static/webpack-macros.html` & `napatrackmater-5.2.5/_build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/genindex.html` & `napatrackmater-5.2.5/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/search.html` & `napatrackmater-5.2.5/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/html/searchindex.js` & `napatrackmater-5.2.5/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_build/jupyter_execute/Notebooks/Track_vector.ipynb` & `napatrackmater-5.2.5/_build/jupyter_execute/Notebooks/Track_vector.ipynb`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/_config.yml` & `napatrackmater-5.2.5/_config.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/images/ClusterDistributionPlot_time_point_97.png` & `napatrackmater-5.2.5/images/ClusterDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/images/ClusterNearnessPlot_time_point_97.png` & `napatrackmater-5.2.5/images/ClusterNearnessPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/images/ClusterPlot_time_point_97.png` & `napatrackmater-5.2.5/images/ClusterPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/images/FeatureMatrixPlot_time_point_97.png` & `napatrackmater-5.2.5/images/FeatureMatrixPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/images/QuadrantDistributionPlot_time_point_97.png` & `napatrackmater-5.2.5/images/QuadrantDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/images/kapoorlablogo.png` & `napatrackmater-5.2.5/images/kapoorlablogo.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/images/kapoorlogo.png` & `napatrackmater-5.2.5/images/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/setup.cfg` & `napatrackmater-5.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 	kapoorlabs-lightning
 	lightning
 	trimesh
 	umap-learn
 	plotly
 	pymesh
 	torchsummary
+	statsmodels
 	numpy
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = setuptools_scm
```

### Comparing `napatrackmater-5.2.4/src/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-5.2.5/src/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/src/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-5.2.5/src/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/src/napatrackmater/Trackmate.py` & `napatrackmater-5.2.5/src/napatrackmater/Trackmate.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/src/napatrackmater/Trackvector.py` & `napatrackmater-5.2.5/src/napatrackmater/Trackvector.py`

 * *Files 0% similar despite different names*

```diff
@@ -2595,14 +2595,68 @@
         concatenated_eigenvectors = np.concatenate((real_part, imag_part), axis=1)
 
         return covariance_matrix, concatenated_eigenvectors
     except Exception as e:
         print(f"Covariance matric computation {e}")
 
 
+
+def train_gbr_neural_net(
+    npz_file,
+    save_path,
+    num_classes=2,
+    batch_size=64,
+    num_workers=0,
+    learning_rate=0.001,
+    epochs=100,
+    accelerator="cuda",
+    devices=1,
+    model_type="simple",
+    growth_rate: int = 32,
+    block_config: tuple = (6, 12, 24, 16),
+    num_init_features: int = 32,
+    bottleneck_size: int = 4,
+    kernel_size: int = 3,
+    experiment_name="mitosis",
+    scheduler_choice="plateau",
+):
+
+    if isinstance(block_config, int):
+        block_config = (block_config,)
+    mitosis_inception = MitosisInception(
+        npz_file=npz_file,
+        num_classes=num_classes,
+        growth_rate=growth_rate,
+        block_config=block_config,
+        num_init_features=num_init_features,
+        bottleneck_size=bottleneck_size,
+        kernel_size=kernel_size,
+        num_workers=num_workers,
+        epochs=epochs,
+        log_path=save_path,
+        batch_size=batch_size,
+        accelerator=accelerator,
+        devices=devices,
+        experiment_name=experiment_name,
+        scheduler_choice=scheduler_choice,
+        learning_rate=learning_rate,
+    )
+
+    mitosis_inception.setup_gbr_datasets()
+    if model_type == "simple":
+        mitosis_inception.setup_mitosisnet_model()
+    else:
+        mitosis_inception.setup_densenet_model()
+
+    mitosis_inception.setup_logger()
+    mitosis_inception.setup_checkpoint()
+    mitosis_inception.setup_adam()
+    mitosis_inception.setup_lightning_model()
+    mitosis_inception.train()
+
 def train_mitosis_neural_net(
     npz_file,
     save_path,
     num_classes=2,
     batch_size=64,
     num_workers=0,
     learning_rate=0.001,
```

### Comparing `napatrackmater-5.2.4/src/napatrackmater/__init__.py` & `napatrackmater-5.2.5/src/napatrackmater/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     TrackVector,
     convert_tracks_to_arrays,
     unsupervised_clustering,
     simple_unsupervised_clustering,
     create_global_gt_dataframe,
     create_gt_analysis_vectors_dict,
     train_mitosis_neural_net,
+    train_gbr_neural_net,
     plot_metrics_from_npz,
     create_analysis_tracklets,
     create_dividing_prediction_tracklets,
     convert_tracks_to_simple_arrays,
     local_track_covaraince,
     cell_fate_recipe,
     core_clustering,
@@ -74,14 +75,15 @@
     "predict_supervised_clustering",
     "convert_tracks_to_arrays",
     "convert_tracks_to_simple_arrays",
     "unsupervised_clustering",
     "simple_unsupervised_clustering",
     "load_json",
     "train_mitosis_neural_net",
+    "train_gbr_neural_net",
     "predict_with_model",
     "plot_metrics_from_npz",
     "load_prediction_data",
     "create_embeddings_with_gt",
     "create_analysis_tracklets",
     "local_track_covaraince",
     "create_dividing_prediction_tracklets",
```

### Comparing `napatrackmater-5.2.4/src/napatrackmater/clustering.py` & `napatrackmater-5.2.5/src/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/src/napatrackmater/fast_radius_regression.py` & `napatrackmater-5.2.5/src/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/src/napatrackmater/fate_mapping.py` & `napatrackmater-5.2.5/src/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/src/napatrackmater/pretrained.py` & `napatrackmater-5.2.5/src/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/src/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-5.2.5/src/napatrackmater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 5.2.4
+Version: 5.2.5
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/Kapoorlabs-CAPED/napatrackmater
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/napatrackmater/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/napatrackmater#README.md
@@ -35,14 +35,15 @@
 Requires-Dist: kapoorlabs-lightning
 Requires-Dist: lightning
 Requires-Dist: trimesh
 Requires-Dist: umap-learn
 Requires-Dist: plotly
 Requires-Dist: pymesh
 Requires-Dist: torchsummary
+Requires-Dist: statsmodels
 Requires-Dist: numpy
 Provides-Extra: testing
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-qt; extra == "testing"
 Requires-Dist: napari; extra == "testing"
```

### Comparing `napatrackmater-5.2.4/src/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-5.2.5/src/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.4/update_version.py` & `napatrackmater-5.2.5/update_version.py`

 * *Files identical despite different names*

