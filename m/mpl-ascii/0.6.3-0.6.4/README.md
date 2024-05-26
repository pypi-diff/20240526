# Comparing `tmp/mpl_ascii-0.6.3.tar.gz` & `tmp/mpl_ascii-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_ascii-0.6.3.tar", last modified: Fri May 24 16:57:56 2024, max compression
+gzip compressed data, was "mpl_ascii-0.6.4.tar", last modified: Sun May 26 10:02:00 2024, max compression
```

## Comparing `mpl_ascii-0.6.3.tar` & `mpl_ascii-0.6.4.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:57:56.727309 mpl_ascii-0.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:57:56.711309 mpl_ascii-0.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:57:56.715309 mpl_ascii-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-24 16:57:56.727309 mpl_ascii-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:57:56.723309 mpl_ascii-0.6.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_chart.txt
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_label_5.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_stacked.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/bar_stacked.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/barh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/barh.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/box_plot_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/box_plot_basic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/broken_line_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/broken_line_plot.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/categorical_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/categorical_variables.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/cohere.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/color_bar_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/color_bar_scatter.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/csd_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/csd_demo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/double_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/double_plot.txt
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/errorbars.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/errorbars.txt
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/errorbars_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/errorbars_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/errorbars_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/errorbars_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/errorbars_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/errorbars_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/hist_best_fit_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/hist_best_fit_line.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/hist_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/hist_simple.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/hist_simple_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/hist_simple_colors.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/line_markers.py
--rw-r--r--   0 runner    (1001) docker     (127)    38794 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/line_markers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/lines_multi_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/lines_multi_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/scatter_multi_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/scatter_multi_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/simple_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/simple_plot.txt
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/violin_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/examples/violin_plot.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:57:56.727309 mpl_ascii-0.6.3/mpl_ascii/
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/ascii_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/ax.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/color_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/legend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/poly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/mpl_ascii/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:57:56.727309 mpl_ascii-0.6.3/mpl_ascii.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-24 16:57:56.000000 mpl_ascii-0.6.3/mpl_ascii.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-24 16:57:56.000000 mpl_ascii-0.6.3/mpl_ascii.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:57:56.000000 mpl_ascii-0.6.3/mpl_ascii.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-24 16:57:56.000000 mpl_ascii-0.6.3/mpl_ascii.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 16:57:56.000000 mpl_ascii-0.6.3/mpl_ascii.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 16:57:56.727309 mpl_ascii-0.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:57:56.727309 mpl_ascii-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-24 16:57:51.000000 mpl_ascii-0.6.3/tests/test_overlay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:02:00.152951 mpl_ascii-0.6.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:02:00.132951 mpl_ascii-0.6.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:02:00.132951 mpl_ascii-0.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-26 10:02:00.148951 mpl_ascii-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:02:00.144951 mpl_ascii-0.6.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/bar_chart.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/bar_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/bar_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/bar_label_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/bar_label_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/bar_label_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/bar_label_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/bar_label_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/bar_label_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/bar_label_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/bar_label_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/bar_label_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/bar_label_5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/bar_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/bar_stacked.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/barh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/barh.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/box_plot_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/box_plot_basic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/broken_line_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/broken_line_plot.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/categorical_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/categorical_variables.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/cohere.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/color_bar_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/color_bar_scatter.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/csd_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/csd_demo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/double_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/double_plot.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/errorbars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/errorbars.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/errorbars_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/errorbars_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/errorbars_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/errorbars_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/errorbars_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/errorbars_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/hist_best_fit_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/hist_best_fit_line.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/hist_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/hist_simple.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/hist_simple_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/hist_simple_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/line_markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38794 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/line_markers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/lines_multi_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/lines_multi_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/scatter_multi_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/scatter_multi_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/simple_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/simple_plot.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/violin_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/examples/violin_plot.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:02:00.148951 mpl_ascii-0.6.4/mpl_ascii/
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/mpl_ascii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/mpl_ascii/ascii_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/mpl_ascii/ax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/mpl_ascii/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/mpl_ascii/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/mpl_ascii/color_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/mpl_ascii/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/mpl_ascii/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/mpl_ascii/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/mpl_ascii/legend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/mpl_ascii/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/mpl_ascii/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/mpl_ascii/poly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/mpl_ascii/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/mpl_ascii/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:02:00.148951 mpl_ascii-0.6.4/mpl_ascii.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-26 10:02:00.000000 mpl_ascii-0.6.4/mpl_ascii.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-26 10:02:00.000000 mpl_ascii-0.6.4/mpl_ascii.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 10:02:00.000000 mpl_ascii-0.6.4/mpl_ascii.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-26 10:02:00.000000 mpl_ascii-0.6.4/mpl_ascii.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 10:02:00.000000 mpl_ascii-0.6.4/mpl_ascii.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 10:02:00.152951 mpl_ascii-0.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:02:00.148951 mpl_ascii-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-26 10:01:55.000000 mpl_ascii-0.6.4/tests/test_overlay.py
```

### Comparing `mpl_ascii-0.6.3/.github/workflows/python-package.yml` & `mpl_ascii-0.6.4/.github/workflows/python-package.yml`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         pytest tests
     - name: Acceptance test
       run: |
         make test
 
   build-and-publish:
     needs: test
+    if: github.ref == 'refs/heads/main' || github.event_name == 'release'
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Set up Python
       uses: actions/setup-python@v5
```

### Comparing `mpl_ascii-0.6.3/.gitignore` & `mpl_ascii-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/CHANGELOG.md` & `mpl_ascii-0.6.4/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 
 ### Added
 
 - Add support for colour bars on scatter plots.
 - Add support for contour plots without colors.
 - Add support for text objects in plot.
 
+## [0.6.4] 2024-05-26
+
+### Fixed
+
+- Add fix so if there is a `None` value in only one axis then the line plot does not raise an error and instead skips over it.
+
 ## [0.6.3] 2024-05-24
 
 ### Fixed
 
 - Line plots now handle None values as matplotlib does. If a `None` value is passed into a line plot then it has line break.
 
 ## [0.6.2] 2024-05-19
```

### Comparing `mpl_ascii-0.6.3/LICENSE` & `mpl_ascii-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/Makefile` & `mpl_ascii-0.6.4/Makefile`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/PKG-INFO` & `mpl_ascii-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_ascii
-Version: 0.6.3
+Version: 0.6.4
 Summary: A matplotlib backend that produces plots using only ASCII characters
 Author: Chris Cave
 Maintainer: Chris Cave
 License: MIT License
 Project-URL: Homepage, https://github.com/chriscave/mpl_ascii
 Keywords: matplotlib,plotting,ASCII
 Requires-Python: >=3.7
```

### Comparing `mpl_ascii-0.6.3/README.md` & `mpl_ascii-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/bar_chart.py` & `mpl_ascii-0.6.4/examples/bar_chart.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/bar_chart.txt` & `mpl_ascii-0.6.4/examples/bar_chart.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/bar_color.py` & `mpl_ascii-0.6.4/examples/bar_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/bar_color.txt` & `mpl_ascii-0.6.4/examples/bar_color.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/bar_label_1.py` & `mpl_ascii-0.6.4/examples/bar_label_1.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/bar_label_1.txt` & `mpl_ascii-0.6.4/examples/bar_label_1.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/bar_label_2.py` & `mpl_ascii-0.6.4/examples/bar_label_2.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/bar_label_2.txt` & `mpl_ascii-0.6.4/examples/bar_label_2.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/bar_label_3.py` & `mpl_ascii-0.6.4/examples/bar_label_3.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/bar_label_3.txt` & `mpl_ascii-0.6.4/examples/bar_label_3.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/bar_label_4.py` & `mpl_ascii-0.6.4/examples/bar_label_4.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/bar_label_4.txt` & `mpl_ascii-0.6.4/examples/bar_label_4.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/bar_label_5.py` & `mpl_ascii-0.6.4/examples/bar_label_5.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/bar_label_5.txt` & `mpl_ascii-0.6.4/examples/bar_label_5.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/bar_stacked.py` & `mpl_ascii-0.6.4/examples/bar_stacked.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/bar_stacked.txt` & `mpl_ascii-0.6.4/examples/bar_stacked.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/barh.py` & `mpl_ascii-0.6.4/examples/barh.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/barh.txt` & `mpl_ascii-0.6.4/examples/barh.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/box_plot_basic.py` & `mpl_ascii-0.6.4/examples/box_plot_basic.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/box_plot_basic.txt` & `mpl_ascii-0.6.4/examples/box_plot_basic.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/categorical_variables.py` & `mpl_ascii-0.6.4/examples/categorical_variables.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/categorical_variables.txt` & `mpl_ascii-0.6.4/examples/categorical_variables.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/cohere.py` & `mpl_ascii-0.6.4/examples/cohere.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/cohere.txt` & `mpl_ascii-0.6.4/examples/cohere.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/color_bar_scatter.py` & `mpl_ascii-0.6.4/examples/color_bar_scatter.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/color_bar_scatter.txt` & `mpl_ascii-0.6.4/examples/color_bar_scatter.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/csd_demo.py` & `mpl_ascii-0.6.4/examples/csd_demo.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/csd_demo.txt` & `mpl_ascii-0.6.4/examples/csd_demo.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/double_plot.py` & `mpl_ascii-0.6.4/examples/double_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/double_plot.txt` & `mpl_ascii-0.6.4/examples/double_plot.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/errorbars.txt` & `mpl_ascii-0.6.4/examples/errorbars.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/errorbars_2.py` & `mpl_ascii-0.6.4/examples/errorbars_2.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/errorbars_2.txt` & `mpl_ascii-0.6.4/examples/errorbars_2.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/errorbars_3.py` & `mpl_ascii-0.6.4/examples/errorbars_3.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/errorbars_3.txt` & `mpl_ascii-0.6.4/examples/errorbars_3.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/errorbars_4.py` & `mpl_ascii-0.6.4/examples/errorbars_4.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/errorbars_4.txt` & `mpl_ascii-0.6.4/examples/errorbars_4.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/hist_best_fit_line.py` & `mpl_ascii-0.6.4/examples/hist_best_fit_line.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/hist_best_fit_line.txt` & `mpl_ascii-0.6.4/examples/hist_best_fit_line.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/hist_simple.py` & `mpl_ascii-0.6.4/examples/hist_simple.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/hist_simple.txt` & `mpl_ascii-0.6.4/examples/hist_simple.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/hist_simple_colors.py` & `mpl_ascii-0.6.4/examples/hist_simple_colors.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/hist_simple_colors.txt` & `mpl_ascii-0.6.4/examples/hist_simple_colors.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/line_markers.py` & `mpl_ascii-0.6.4/examples/line_markers.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/line_markers.txt` & `mpl_ascii-0.6.4/examples/line_markers.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/lines_multi_color.py` & `mpl_ascii-0.6.4/examples/lines_multi_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/lines_multi_color.txt` & `mpl_ascii-0.6.4/examples/lines_multi_color.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/scatter_multi_color.py` & `mpl_ascii-0.6.4/examples/scatter_multi_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/scatter_multi_color.txt` & `mpl_ascii-0.6.4/examples/scatter_multi_color.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/simple_plot.py` & `mpl_ascii-0.6.4/examples/simple_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/simple_plot.txt` & `mpl_ascii-0.6.4/examples/simple_plot.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/violin_plot.py` & `mpl_ascii-0.6.4/examples/violin_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/examples/violin_plot.txt` & `mpl_ascii-0.6.4/examples/violin_plot.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/mpl_ascii/__init__.py` & `mpl_ascii-0.6.4/mpl_ascii/__init__.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/mpl_ascii/ascii_canvas.py` & `mpl_ascii-0.6.4/mpl_ascii/ascii_canvas.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/mpl_ascii/ax.py` & `mpl_ascii-0.6.4/mpl_ascii/ax.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/mpl_ascii/bar.py` & `mpl_ascii-0.6.4/mpl_ascii/bar.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/mpl_ascii/color_map.py` & `mpl_ascii-0.6.4/mpl_ascii/color_map.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/mpl_ascii/colorbar.py` & `mpl_ascii-0.6.4/mpl_ascii/colorbar.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/mpl_ascii/draw.py` & `mpl_ascii-0.6.4/mpl_ascii/draw.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/mpl_ascii/format.py` & `mpl_ascii-0.6.4/mpl_ascii/format.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/mpl_ascii/legend.py` & `mpl_ascii-0.6.4/mpl_ascii/legend.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/mpl_ascii/line.py` & `mpl_ascii-0.6.4/mpl_ascii/line.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,30 +92,30 @@
             continue
         ascii_y_data.append(round(linear_transform(y, y_min, y_max, 1, height)))
 
 
     line_canvas_arr = np.full((height, width), fill_value=" ", dtype="object")
 
     for x, y in zip(ascii_x_data, ascii_y_data):
-        if x is None and y is None:
+        if x is None or y is None:
             continue
         row = height - y
         col = x
         line_canvas_arr[row, col] = char
 
     if linestyle == "None":
         return line_canvas_arr
 
     start_points = zip(ascii_x_data[:-1], ascii_y_data[:-1])
     end_points = zip(ascii_x_data[1:], ascii_y_data[1:])
     join_line_points = []
     for start, end in zip(start_points, end_points):
-        if start[0] is None and start[1] is None:
+        if start[0] is None or start[1] is None:
             continue
-        if end[0] is None and end[1] is None:
+        if end[0] is None or end[1] is None:
             continue
         line_points = bresenham_line(start[0], start[1], end[0], end[1])
         if len(line_points) > 2:
             join_line_points += line_points[1:-1]
 
 
     for x,y in join_line_points:
```

### Comparing `mpl_ascii-0.6.3/mpl_ascii/overlay.py` & `mpl_ascii-0.6.4/mpl_ascii/overlay.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/mpl_ascii/poly.py` & `mpl_ascii-0.6.4/mpl_ascii/poly.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/mpl_ascii/scatter.py` & `mpl_ascii-0.6.4/mpl_ascii/scatter.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/mpl_ascii/tools.py` & `mpl_ascii-0.6.4/mpl_ascii/tools.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/mpl_ascii.egg-info/PKG-INFO` & `mpl_ascii-0.6.4/mpl_ascii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_ascii
-Version: 0.6.3
+Version: 0.6.4
 Summary: A matplotlib backend that produces plots using only ASCII characters
 Author: Chris Cave
 Maintainer: Chris Cave
 License: MIT License
 Project-URL: Homepage, https://github.com/chriscave/mpl_ascii
 Keywords: matplotlib,plotting,ASCII
 Requires-Python: >=3.7
```

### Comparing `mpl_ascii-0.6.3/mpl_ascii.egg-info/SOURCES.txt` & `mpl_ascii-0.6.4/mpl_ascii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/pyproject.toml` & `mpl_ascii-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.6.3/tests/test_overlay.py` & `mpl_ascii-0.6.4/tests/test_overlay.py`

 * *Files identical despite different names*

