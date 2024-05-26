# Comparing `tmp/neura_library-0.0.5.tar.gz` & `tmp/neura_library-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neura_library-0.0.5.tar", last modified: Wed May  8 15:22:47 2024, max compression
+gzip compressed data, was "neura_library-0.0.6.tar", last modified: Sun May 26 11:56:37 2024, max compression
```

## Comparing `neura_library-0.0.5.tar` & `neura_library-0.0.6.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.853161 neura_library-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-08 15:22:40.000000 neura_library-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-05-08 15:22:47.853161 neura_library-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-08 15:22:40.000000 neura_library-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-08 15:22:40.000000 neura_library-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-08 15:22:40.000000 neura_library-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:22:47.853161 neura_library-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.825161 neura_library-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.853161 neura_library-0.0.5/src/neura_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-05-08 15:22:47.000000 neura_library-0.0.5/src/neura_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-08 15:22:47.000000 neura_library-0.0.5/src/neura_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:22:47.000000 neura_library-0.0.5/src/neura_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-08 15:22:47.000000 neura_library-0.0.5/src/neura_library.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-08 15:22:47.000000 neura_library-0.0.5/src/neura_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 15:22:47.000000 neura_library-0.0.5/src/neura_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.829161 neura_library-0.0.5/src/neuralib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.833161 neura_library-0.0.5/src/neuralib/argp/
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/argp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/argp/_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18987 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/argp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/argp/dispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.833161 neura_library-0.0.5/src/neuralib/atlas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.833161 neura_library-0.0.5/src/neuralib/atlas/brainrender/
--rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/brainrender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/brainrender/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/brainrender/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/brainrender/main_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    13091 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/brainrender/probe_rst.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/brainrender/roi_rst.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/brainrender/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.833161 neura_library-0.0.5/src/neuralib/atlas/ccf/
--rw-r--r--   0 runner    (1001) docker     (127)    15822 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/ccf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33730 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/ccf/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    12990 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/ccf/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/ccf/norm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/ccf/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.833161 neura_library-0.0.5/src/neuralib/atlas/cellatlas/
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/cellatlas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/cellatlas/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.837161 neura_library-0.0.5/src/neuralib/atlas/ibl/
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/ibl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/ibl/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    55607 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.837161 neura_library-0.0.5/src/neuralib/bokeh_model/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11440 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/example_multi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.837161 neura_library-0.0.5/src/neuralib/bokeh_model/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/examples/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/examples/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/examples/view_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/examples/view_animal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/examples/view_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/view_brain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.837161 neura_library-0.0.5/src/neuralib/calimg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.837161 neura_library-0.0.5/src/neuralib/calimg/scan_image/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/scan_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/scan_image/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.837161 neura_library-0.0.5/src/neuralib/calimg/scanbox/
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/scanbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/scanbox/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/scanbox/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.841161 neura_library-0.0.5/src/neuralib/calimg/suite2p/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/suite2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/suite2p/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/suite2p/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/suite2p/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.841161 neura_library-0.0.5/src/neuralib/imglib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/imglib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/imglib/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/imglib/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/imglib/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    13647 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/imglib/labeller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/imglib/norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/imglib/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.841161 neura_library-0.0.5/src/neuralib/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.841161 neura_library-0.0.5/src/neuralib/model/bayes_decoding/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/model/bayes_decoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/model/bayes_decoding/position.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.841161 neura_library-0.0.5/src/neuralib/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/persistence/cli_persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)    27622 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/persistence/persistence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.841161 neura_library-0.0.5/src/neuralib/plot/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/colormap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/venn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.845161 neura_library-0.0.5/src/neuralib/scanner/
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/scanner/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/scanner/czi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/scanner/lsm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.845161 neura_library-0.0.5/src/neuralib/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/segmentation/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.845161 neura_library-0.0.5/src/neuralib/segmentation/cellpose/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/segmentation/cellpose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/segmentation/cellpose/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/segmentation/cellpose/run_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/segmentation/cellpose/run_subproc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.845161 neura_library-0.0.5/src/neuralib/segmentation/stardist/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/segmentation/stardist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/segmentation/stardist/run_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.845161 neura_library-0.0.5/src/neuralib/stimpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/baselog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/baseprot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/camlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/math_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/preference.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/protocol_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    23153 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/stimpy_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/stimpy_git.py
--rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/stimpy_pyv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/stimulus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.849161 neura_library-0.0.5/src/neuralib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.849161 neura_library-0.0.5/src/neuralib/tools/pkl_parq_view/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/tools/pkl_parq_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/tools/pkl_parq_view/main_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.849161 neura_library-0.0.5/src/neuralib/tools/slack_bot/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/tools/slack_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/tools/slack_bot/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.849161 neura_library-0.0.5/src/neuralib/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/cli_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/color_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/profile_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/segement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/util_clazz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/util_cv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/util_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/util_verbose.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.849161 neura_library-0.0.5/src/neuralib/wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.853161 neura_library-0.0.5/src/neuralib/wrapper/deeplabcut/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/deeplabcut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/deeplabcut/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/deeplabcut/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.853161 neura_library-0.0.5/src/neuralib/wrapper/facemap/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/facemap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/facemap/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/facemap/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.853161 neura_library-0.0.5/src/neuralib/wrapper/rastermap/
--rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/rastermap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/rastermap/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.853161 neura_library-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_argp.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_argp_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_csv_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_persistence_autoinc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_protocol_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_pyvstim_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    62204 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_stimpy_bitbucket_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    16421 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_stimpy_github_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_util_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.762143 neura_library-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-26 11:56:33.000000 neura_library-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-05-26 11:56:37.762143 neura_library-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-26 11:56:33.000000 neura_library-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-26 11:56:33.000000 neura_library-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-26 11:56:33.000000 neura_library-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 11:56:37.762143 neura_library-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.734143 neura_library-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.762143 neura_library-0.0.6/src/neura_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-05-26 11:56:37.000000 neura_library-0.0.6/src/neura_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-26 11:56:37.000000 neura_library-0.0.6/src/neura_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 11:56:37.000000 neura_library-0.0.6/src/neura_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-26 11:56:37.000000 neura_library-0.0.6/src/neura_library.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-26 11:56:37.000000 neura_library-0.0.6/src/neura_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 11:56:37.000000 neura_library-0.0.6/src/neura_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.738143 neura_library-0.0.6/src/neuralib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.742143 neura_library-0.0.6/src/neuralib/argp/
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/argp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/argp/_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18987 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/argp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/argp/dispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.742143 neura_library-0.0.6/src/neuralib/atlas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.742143 neura_library-0.0.6/src/neuralib/atlas/brainrender/
+-rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/brainrender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10272 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/brainrender/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/brainrender/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/brainrender/main_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13091 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/brainrender/probe_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/brainrender/roi_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/brainrender/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.742143 neura_library-0.0.6/src/neuralib/atlas/ccf/
+-rw-r--r--   0 runner    (1001) docker     (127)    15822 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/ccf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33730 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/ccf/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12990 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/ccf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/ccf/norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/ccf/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.746143 neura_library-0.0.6/src/neuralib/atlas/cellatlas/
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/cellatlas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/cellatlas/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.746143 neura_library-0.0.6/src/neuralib/atlas/ibl/
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/ibl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/ibl/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55607 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.746143 neura_library-0.0.6/src/neuralib/bokeh_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11440 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/example_multi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.746143 neura_library-0.0.6/src/neuralib/bokeh_model/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/examples/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/examples/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/examples/view_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/examples/view_animal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/examples/view_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/view_brain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.746143 neura_library-0.0.6/src/neuralib/calimg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.746143 neura_library-0.0.6/src/neuralib/calimg/scan_image/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/scan_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/scan_image/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.746143 neura_library-0.0.6/src/neuralib/calimg/scanbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/scanbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/scanbox/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/scanbox/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.750143 neura_library-0.0.6/src/neuralib/calimg/suite2p/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/suite2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/suite2p/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/suite2p/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/suite2p/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.750143 neura_library-0.0.6/src/neuralib/imglib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/imglib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/imglib/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/imglib/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/imglib/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13647 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/imglib/labeller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/imglib/norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/imglib/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.750143 neura_library-0.0.6/src/neuralib/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.750143 neura_library-0.0.6/src/neuralib/model/bayes_decoding/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/model/bayes_decoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/model/bayes_decoding/position.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.750143 neura_library-0.0.6/src/neuralib/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/persistence/cli_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27622 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/persistence/persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.750143 neura_library-0.0.6/src/neuralib/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/venn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.754143 neura_library-0.0.6/src/neuralib/scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/scanner/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/scanner/czi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/scanner/lsm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.754143 neura_library-0.0.6/src/neuralib/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/segmentation/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.754143 neura_library-0.0.6/src/neuralib/segmentation/cellpose/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/segmentation/cellpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/segmentation/cellpose/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/segmentation/cellpose/run_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/segmentation/cellpose/run_subproc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.754143 neura_library-0.0.6/src/neuralib/segmentation/stardist/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/segmentation/stardist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/segmentation/stardist/run_2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.758143 neura_library-0.0.6/src/neuralib/stimpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/baselog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/baseprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/camlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/math_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/preference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/protocol_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22973 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/stimpy_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24923 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/stimpy_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/stimpy_pyv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/stimulus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.758143 neura_library-0.0.6/src/neuralib/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.758143 neura_library-0.0.6/src/neuralib/tools/pkl_parq_view/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/tools/pkl_parq_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/tools/pkl_parq_view/main_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.758143 neura_library-0.0.6/src/neuralib/tools/slack_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/tools/slack_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/tools/slack_bot/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.758143 neura_library-0.0.6/src/neuralib/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/color_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/profile_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/segement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/util_clazz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/util_cv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/util_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/util_verbose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.758143 neura_library-0.0.6/src/neuralib/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.762143 neura_library-0.0.6/src/neuralib/wrapper/deeplabcut/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/deeplabcut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/deeplabcut/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/deeplabcut/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.762143 neura_library-0.0.6/src/neuralib/wrapper/facemap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/facemap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/facemap/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/facemap/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.762143 neura_library-0.0.6/src/neuralib/wrapper/rastermap/
+-rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/rastermap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/rastermap/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.762143 neura_library-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_argp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_argp_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_csv_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_persistence_autoinc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_protocol_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_pyvstim_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62204 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_stimpy_bitbucket_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16421 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_stimpy_github_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_util_func.py
```

### Comparing `neura_library-0.0.5/LICENSE` & `neura_library-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/PKG-INFO` & `neura_library-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neura-library
-Version: 0.0.5
+Version: 0.0.6
 Summary: Utility tools for system neuroscience research, including Open Source Wrapper or Parser
 Author-email: Yu-Ting Wei <ytsimon2004@gmail.com>, Ta-Shun Su <antoniost29@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, YT.WEI
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `neura_library-0.0.5/README.md` & `neura_library-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/pyproject.toml` & `neura_library-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "neura-library"
-version = "0.0.5"
+version = "0.0.6"
 requires-python = ">=3.9"
 description = "Utility tools for system neuroscience research, including Open Source Wrapper or Parser"
 authors = [
     { name = "Yu-Ting Wei", email = "ytsimon2004@gmail.com" },
     { name = "Ta-Shun Su", email = "antoniost29@gmail.com" }
 ]
 license = { file = "LICENSE" }
```

### Comparing `neura_library-0.0.5/src/neura_library.egg-info/PKG-INFO` & `neura_library-0.0.6/src/neura_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neura-library
-Version: 0.0.5
+Version: 0.0.6
 Summary: Utility tools for system neuroscience research, including Open Source Wrapper or Parser
 Author-email: Yu-Ting Wei <ytsimon2004@gmail.com>, Ta-Shun Su <antoniost29@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, YT.WEI
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `neura_library-0.0.5/src/neura_library.egg-info/SOURCES.txt` & `neura_library-0.0.6/src/neura_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/argp/__init__.py` & `neura_library-0.0.6/src/neuralib/argp/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/argp/_type.py` & `neura_library-0.0.6/src/neuralib/argp/_type.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/argp/core.py` & `neura_library-0.0.6/src/neuralib/argp/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/argp/dispatch.py` & `neura_library-0.0.6/src/neuralib/argp/dispatch.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/_structure.py` & `neura_library-0.0.6/src/neuralib/atlas/_structure.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/brainrender/__init__.py` & `neura_library-0.0.6/src/neuralib/atlas/brainrender/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/brainrender/core.py` & `neura_library-0.0.6/src/neuralib/atlas/brainrender/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 __all__ = [
     'ROI_COLORS',
     'RoiType',
     'BrainReconstructor',
 ]
 
-ROI_COLORS = ['purple', 'gold', 'grey']
+ROI_COLORS = ['magenta', 'gold', 'grey']
 DEFAULT_REGION_COLORS = ['lightblue', 'pink', 'turquoise']
 CAMERA_ANGLE_TYPE = Literal['sagittal', 'sagittal2', 'frontal', 'top', 'top_side', 'three_quarters']
 SHADER_STYLE_TYPE = Literal['metallic', 'cartoon', 'plastic', 'shiny', 'glossy']
 
 RoiType: TypeAlias = list[Union[list[np.ndarray], np.ndarray]]
 
 Logger = setup_clogger(caller_name=Path(__file__).name)
```

### Comparing `neura_library-0.0.5/src/neuralib/atlas/brainrender/main_app.py` & `neura_library-0.0.6/src/neuralib/atlas/brainrender/main_app.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/brainrender/probe_rst.py` & `neura_library-0.0.6/src/neuralib/atlas/brainrender/probe_rst.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/brainrender/roi_rst.py` & `neura_library-0.0.6/src/neuralib/atlas/brainrender/roi_rst.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/brainrender/util.py` & `neura_library-0.0.6/src/neuralib/atlas/brainrender/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/ccf/__init__.py` & `neura_library-0.0.6/src/neuralib/atlas/ccf/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/ccf/classifier.py` & `neura_library-0.0.6/src/neuralib/atlas/ccf/classifier.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/ccf/core.py` & `neura_library-0.0.6/src/neuralib/atlas/ccf/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/ccf/norm.py` & `neura_library-0.0.6/src/neuralib/atlas/ccf/norm.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/ccf/query.py` & `neura_library-0.0.6/src/neuralib/atlas/ccf/query.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/cellatlas/__init__.py` & `neura_library-0.0.6/src/neuralib/atlas/cellatlas/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/cellatlas/core.py` & `neura_library-0.0.6/src/neuralib/atlas/cellatlas/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/data.py` & `neura_library-0.0.6/src/neuralib/atlas/data.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/ibl/__init__.py` & `neura_library-0.0.6/src/neuralib/atlas/ibl/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/ibl/plot.py` & `neura_library-0.0.6/src/neuralib/atlas/ibl/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,22 @@
             source_path = IBL_CACHE_DIRECTORY
 
         super().__init__(res_um, scaling, mock, source_path)
 
         self._alpha = alpha
 
     def get_acronym_list(self, mapping: IBL_MAPPING_TYPE) -> list[str]:
-        """get acronym list"""
+        """get acronym list from different mapping type
+
+        :param mapping: `IBL_MAPPING_TYPE`
+        """
+        idx = np.unique(self.regions.mappings[mapping])
         # noinspection PyUnresolvedReferences
-        return list(self.regions.acronym[self.regions.mappings[mapping]])
+        return self.regions.acronym[idx]
+        # return list(self.regions.acronym[self.regions.mappings[mapping]])
 
     def plot_scalar_on_slice(
             self,
             regions: ArrayLike, *,
             values: ArrayLike | None = None,
             coord: int = -570,
             plane: IBL_PLANE_TYPE = 'coronal',
@@ -113,14 +118,18 @@
             regions = np.array(regions)
 
         if values is None:
             values = np.arange(regions.size)
 
         if auto_merge:
             regions = np.unique(self.regions.acronym2acronym(regions, mapping=mapping))
+
+            if any([r not in self.get_acronym_list(mapping) for r in regions]):
+                raise RuntimeError('auto merging error')
+
             values = np.arange(regions.size)
 
         if verbose:
             print(f'Plot region: {list(regions)}')
 
         # noinspection PyTypeChecker
         return plot_scalar_on_slice(
```

### Comparing `neura_library-0.0.5/src/neuralib/atlas/map.py` & `neura_library-0.0.6/src/neuralib/atlas/map.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/plot.py` & `neura_library-0.0.6/src/neuralib/atlas/plot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/util.py` & `neura_library-0.0.6/src/neuralib/atlas/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/atlas/view.py` & `neura_library-0.0.6/src/neuralib/atlas/view.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/bokeh_model/base.py` & `neura_library-0.0.6/src/neuralib/bokeh_model/base.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/bokeh_model/example.py` & `neura_library-0.0.6/src/neuralib/bokeh_model/example.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/bokeh_model/example_multi.py` & `neura_library-0.0.6/src/neuralib/bokeh_model/example_multi.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/bokeh_model/examples/view_all.py` & `neura_library-0.0.6/src/neuralib/bokeh_model/examples/view_all.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/bokeh_model/examples/view_animal.py` & `neura_library-0.0.6/src/neuralib/bokeh_model/examples/view_animal.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/bokeh_model/examples/view_figure.py` & `neura_library-0.0.6/src/neuralib/bokeh_model/examples/view_figure.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/bokeh_model/tool.py` & `neura_library-0.0.6/src/neuralib/bokeh_model/tool.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/bokeh_model/util.py` & `neura_library-0.0.6/src/neuralib/bokeh_model/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/bokeh_model/view_brain.py` & `neura_library-0.0.6/src/neuralib/bokeh_model/view_brain.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/calimg/scan_image/wrapper.py` & `neura_library-0.0.6/src/neuralib/calimg/scan_image/wrapper.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/calimg/scanbox/__init__.py` & `neura_library-0.0.6/src/neuralib/calimg/scanbox/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/calimg/scanbox/core.py` & `neura_library-0.0.6/src/neuralib/calimg/scanbox/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/calimg/scanbox/viewer.py` & `neura_library-0.0.6/src/neuralib/calimg/scanbox/viewer.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/calimg/suite2p/__init__.py` & `neura_library-0.0.6/src/neuralib/calimg/suite2p/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/calimg/suite2p/core.py` & `neura_library-0.0.6/src/neuralib/calimg/suite2p/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/calimg/suite2p/plot.py` & `neura_library-0.0.6/src/neuralib/calimg/suite2p/plot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/calimg/suite2p/signals.py` & `neura_library-0.0.6/src/neuralib/calimg/suite2p/signals.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/imglib/color.py` & `neura_library-0.0.6/src/neuralib/imglib/color.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/imglib/factory.py` & `neura_library-0.0.6/src/neuralib/imglib/factory.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/imglib/io.py` & `neura_library-0.0.6/src/neuralib/imglib/io.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/imglib/labeller.py` & `neura_library-0.0.6/src/neuralib/imglib/labeller.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/imglib/norm.py` & `neura_library-0.0.6/src/neuralib/imglib/norm.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/imglib/transform.py` & `neura_library-0.0.6/src/neuralib/imglib/transform.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/model/bayes_decoding/position.py` & `neura_library-0.0.6/src/neuralib/model/bayes_decoding/position.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/persistence/cli_persistence.py` & `neura_library-0.0.6/src/neuralib/persistence/cli_persistence.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/persistence/persistence.py` & `neura_library-0.0.6/src/neuralib/persistence/persistence.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/plot/animation.py` & `neura_library-0.0.6/src/neuralib/plot/animation.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/plot/colormap.py` & `neura_library-0.0.6/src/neuralib/plot/colormap.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/plot/figure.py` & `neura_library-0.0.6/src/neuralib/plot/figure.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/plot/misc.py` & `neura_library-0.0.6/src/neuralib/plot/misc.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/plot/plot.py` & `neura_library-0.0.6/src/neuralib/plot/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,14 @@
     :param y: (N, )
     :param bins:
     :param ptype
     :return:
     """
 
     if ptype == 'mean':
-
         a, edg = np.histogram(x, weights=y, bins=bins)
         n = np.histogram(x, bins)[0]  # (B, )
 
         weights = np.divide(a, n, out=np.zeros_like(a, dtype=float), where=n != 0)  # avoid true divide
         weights = gaussian_filter1d(weights, 1)
 
         ax.plot(edg[1:], weights, 'r--', alpha=0.5)
```

### Comparing `neura_library-0.0.5/src/neuralib/plot/setting.py` & `neura_library-0.0.6/src/neuralib/plot/setting.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/plot/tools.py` & `neura_library-0.0.6/src/neuralib/plot/tools.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/plot/venn.py` & `neura_library-0.0.6/src/neuralib/plot/venn.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/scanner/__init__.py` & `neura_library-0.0.6/src/neuralib/scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/scanner/core.py` & `neura_library-0.0.6/src/neuralib/scanner/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/scanner/czi.py` & `neura_library-0.0.6/src/neuralib/scanner/czi.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/scanner/lsm.py` & `neura_library-0.0.6/src/neuralib/scanner/lsm.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/segmentation/base.py` & `neura_library-0.0.6/src/neuralib/segmentation/base.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/segmentation/cellpose/core.py` & `neura_library-0.0.6/src/neuralib/segmentation/cellpose/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/segmentation/cellpose/run_api.py` & `neura_library-0.0.6/src/neuralib/segmentation/cellpose/run_api.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/segmentation/cellpose/run_subproc.py` & `neura_library-0.0.6/src/neuralib/segmentation/cellpose/run_subproc.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/segmentation/stardist/run_2d.py` & `neura_library-0.0.6/src/neuralib/segmentation/stardist/run_2d.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/stimpy/__init__.py` & `neura_library-0.0.6/src/neuralib/stimpy/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/stimpy/baselog.py` & `neura_library-0.0.6/src/neuralib/stimpy/baselog.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/stimpy/baseprot.py` & `neura_library-0.0.6/src/neuralib/stimpy/baseprot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/stimpy/camlog.py` & `neura_library-0.0.6/src/neuralib/stimpy/camlog.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/stimpy/event.py` & `neura_library-0.0.6/src/neuralib/stimpy/event.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/stimpy/math_eval.py` & `neura_library-0.0.6/src/neuralib/stimpy/math_eval.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/stimpy/preference.py` & `neura_library-0.0.6/src/neuralib/stimpy/preference.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,19 +107,20 @@
 
     # runtime append
     _controllers_data_folder: Path
     _controllers_protocol_folder: str
     _controllers_folder_read_flag: bool
 
 
-def load_preferences(file: PathLike) -> PreferenceDict:
+def load_preferences(file: PathLike, check_suffix: bool = True) -> PreferenceDict:
     """
     Get stimpy output(parsed) preference file as dict
 
-    :param file: filepath for the .pref
+    :param file: filepath for the .pref or .prefs
+    :param check_suffix: if check the file suffix
     :return: :class:`PreferenceDict`
     """
-    if Path(file).suffix != '.pref':
-        raise ValueError('invalid file type')
+    if check_suffix and Path(file).suffix not in ('.pref', '.prefs'):
+        raise ValueError(f'invalid file type: {Path(file).suffix}')
 
     with open(file, "r") as file:
         return json.load(file)
```

### Comparing `neura_library-0.0.5/src/neuralib/stimpy/protocol_parser.py` & `neura_library-0.0.6/src/neuralib/stimpy/protocol_parser.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/stimpy/session.py` & `neura_library-0.0.6/src/neuralib/stimpy/session.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/stimpy/stimpy_core.py` & `neura_library-0.0.6/src/neuralib/stimpy/stimpy_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import numpy as np
 import polars as pl
 from typing_extensions import Self
 
 from neuralib.plot.figure import plot_figure
 from neuralib.util.util_type import PathLike
 from neuralib.util.util_verbose import fprint
-from neuralib.util.utils import deprecated
 from .baselog import Baselog, LOG_SUFFIX, StimlogBase
 from .baseprot import AbstractStimProtocol
 from .session import Session, SessionInfo, get_protocol_sessions
 from .stimulus import StimPattern
 from .util import unfold_stimuli_condition, try_casting_number
 
 __all__ = ['RiglogData',
@@ -53,37 +52,38 @@
                     3: lambda it: float(it[:-1])
                 }
             )
             np.save(output, riglog)
 
         return np.load(output)
 
-    @deprecated(reason='caller rare')
-    def session_handler(self, session: str | tuple[str, ...]) -> tuple[float, float]:
-        """trigger `select_time_range` for specific time range"""
-        strial = self.stimlog_data().session_trials()
+    def with_sessions(self, session: Session | tuple[Session, ...]) -> Self:
+        """
+        Truncate the instance `dat` with the given session(s)
+
+        :param session: session name(s)
+        :return:
+        """
+        dy = self.stimlog_data().session_trials()
+
         if isinstance(session, str):
-            t0, t1 = strial[session].time
+            t0, t1 = dy[session].time
         elif isinstance(session, tuple):
-            t_all = [strial[s].time for s in session]
+            t_all = np.array([dy[s].time for s in session])
             t0, t1 = np.min(t_all), np.max(t_all)
             fprint(f'get trange from multiple sessions, {session}: t0:{t0}, t1:{t1}')
         else:
-            raise TypeError(f'{type(session)}')
-
-        self.select_time_range(t0, t1)
-
-        return t0, t1
+            raise TypeError('')
 
-    def select_time_range(self, t0: float, t1: float):
-        """overwrite the `instance attr: data` to given time range"""
         t = self.dat[:, 2] / 1000
         mask = np.logical_and(t0 < t, t < t1)
         self.dat = self.dat[mask]
 
+        return self
+
     @property
     def stimlog_file(self) -> Path:
         return self.riglog_file.with_suffix('.stimlog')
 
     def stimlog_data(self) -> StimlogBase:
         if self.__stimlog_cache is None:
             if self.version == 'stimpy-git':
@@ -448,18 +448,19 @@
         except DiodeSignalMissingError as e:
             fprint(f'{repr(e)}, use default value', vtype='warning')
             return default_offset_value
 
     #
     avg_t = float(np.mean(t))
     std_t = float(np.std(t))
+
     if not (0 <= avg_t <= 1):
         fprint(f'{avg_t} too large, might not be properly calculated, check...', vtype='warning')
 
-    fprint(f'avg: {avg_t}, std: {std_t}')
+    fprint(f'DIODE OFFSET avg: {avg_t}s, std: {std_t}s')
 
     if return_sequential:
         return t
     else:
         return avg_t
```

### Comparing `neura_library-0.0.5/src/neuralib/stimpy/stimpy_git.py` & `neura_library-0.0.6/src/neuralib/stimpy/stimpy_git.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 
 import re
+from pathlib import Path
 from typing import Any, Callable, final
 
 import numpy as np
 import polars as pl
 
 from neuralib.util.util_type import PathLike
 from neuralib.util.util_verbose import fprint
 from neuralib.util.utils import deprecated
 from .baselog import StimlogBase
 from .session import Session, SessionInfo, get_protocol_sessions
 from .stimpy_core import RiglogData, StimpyProtocol
 from .stimulus import StimPattern
 
-__all__ = ['StimlogGit']
+__all__ = ['StimlogGit',
+           'load_stimlog']
 
 
 # TODO code 0 options need to be extended
 @final
 class StimlogGit(StimlogBase):
     """class for handle the stimlog file for stimpy **github** version
     (mainly tested in the commits derived from master branch)
@@ -177,17 +179,16 @@
             value = eval(message)
             if len(self.log_header[code]) != len(value):
                 print(f'log category {code} size mismatched at line {line} : {message}')
             else:
                 log_data.setdefault(code, []).append((time, *value))
 
         elif self.log_info[code] == 'StateMachine':
-            # [<States.SHOW_STIM: 2>, <States.SHOW_BLANK: 1>]
             value = eval(message.replace('<', '("').replace(':', '",').replace('>', ')'))
-            # [("States.SHOW_STIM", 2), ("States.SHOW_BLANK", 1)]
+            value = list(map(str, value))
             if len(self.log_header[code]) != len(value):
                 print(f'log category {code} size mismatched at line {line} : {message}')
             else:
                 log_data.setdefault(code, []).append((time, *value))
 
         else:
             print(f'unknown log category : at line {line} : {content}')
@@ -228,25 +229,28 @@
         for code in remove_code:
             del log_data[code]
 
         return log_data
 
     def get_visual_presentation_dataframe(self) -> pl.DataFrame:
         """
-        ┌────────────┬──────────┬──────────┬─────┬───┬──────┬─────┬──────┬─────────┐
-        │ time       ┆ duration ┆ contrast ┆ ori ┆ … ┆ sf   ┆ tf  ┆ opto ┆ pattern │
-        │ ---        ┆ ---      ┆ ---      ┆ --- ┆   ┆ ---  ┆ --- ┆ ---  ┆ ---     │
-        │ f64        ┆ i64      ┆ i64      ┆ i64 ┆   ┆ f64  ┆ i64 ┆ i64  ┆ str     │
-        ╞════════════╪══════════╪══════════╪═════╪═══╪══════╪═════╪══════╪═════════╡
-        │ 18.990026  ┆ 10       ┆ 1        ┆ 0   ┆ … ┆ 0.04 ┆ 10  ┆ 0    ┆ square  │
-        │ 21.000029  ┆ 10       ┆ 1        ┆ 0   ┆ … ┆ 0.04 ┆ 10  ┆ 0    ┆ square  │
-        │ …          ┆ …        ┆ …        ┆ …   ┆ … ┆ …    ┆ …   ┆ …    ┆ …       │
-        │ 619.054972 ┆ 10       ┆ 1        ┆ 0   ┆ … ┆ 0.04 ┆ 50  ┆ 0    ┆ square  │
-        │ 619.084972 ┆ 10       ┆ 1        ┆ 0   ┆ … ┆ 0.04 ┆ 50  ┆ 0    ┆ square  │
-        └────────────┴──────────┴──────────┴─────┴───┴──────┴─────┴──────┴─────────┘
+        Visual presentation dataframe::
+
+            ┌────────────┬──────────┬──────────┬─────┬───┬──────┬─────┬──────┬─────────┐
+            │ time       ┆ duration ┆ contrast ┆ ori ┆ … ┆ sf   ┆ tf  ┆ opto ┆ pattern │
+            │ ---        ┆ ---      ┆ ---      ┆ --- ┆   ┆ ---  ┆ --- ┆ ---  ┆ ---     │
+            │ f64        ┆ i64      ┆ i64      ┆ i64 ┆   ┆ f64  ┆ i64 ┆ i64  ┆ str     │
+            ╞════════════╪══════════╪══════════╪═════╪═══╪══════╪═════╪══════╪═════════╡
+            │ 18.990026  ┆ 10       ┆ 1        ┆ 0   ┆ … ┆ 0.04 ┆ 10  ┆ 0    ┆ square  │
+            │ 21.000029  ┆ 10       ┆ 1        ┆ 0   ┆ … ┆ 0.04 ┆ 10  ┆ 0    ┆ square  │
+            │ …          ┆ …        ┆ …        ┆ …   ┆ … ┆ …    ┆ …   ┆ …    ┆ …       │
+            │ 619.054972 ┆ 10       ┆ 1        ┆ 0   ┆ … ┆ 0.04 ┆ 50  ┆ 0    ┆ square  │
+            │ 619.084972 ┆ 10       ┆ 1        ┆ 0   ┆ … ┆ 0.04 ┆ 50  ┆ 0    ┆ square  │
+            └────────────┴──────────┴──────────┴─────┴───┴──────┴─────┴──────┴─────────┘
+
         :return:
         """
         df = pl.DataFrame().with_columns(
             pl.Series(self.v_present_time).alias('time'),
             pl.Series(self.v_duration).alias('duration'),
             pl.Series(self.v_contrast).alias('contrast'),
             pl.Series(self.v_ori).alias('ori'),
@@ -261,25 +265,28 @@
             pl.Series(self.v_opto).alias('opto'),
             pl.Series(self.v_pattern).alias('pattern')
         )
         return df
 
     def get_photo_indicator_dataframe(self) -> pl.DataFrame:
         """
-        ┌────────────┬───────┬──────┬────────────┬───────┬──────┬────────┬────────┐
-        │ time       ┆ state ┆ size ┆ pos        ┆ units ┆ mode ┆ frames ┆ enable │
-        │ ---        ┆ ---   ┆ ---  ┆ ---        ┆ ---   ┆ ---  ┆ ---    ┆ ---    │
-        │ f64        ┆ bool  ┆ i64  ┆ list[i64]  ┆ str   ┆ i64  ┆ i64    ┆ bool   │
-        ╞════════════╪═══════╪══════╪════════════╪═══════╪══════╪════════╪════════╡
-        │ 18.990026  ┆ false ┆ 60   ┆ [740, 370] ┆ pix   ┆ 0    ┆ 20     ┆ true   │
-        │ 21.000029  ┆ true  ┆ 60   ┆ [740, 370] ┆ pix   ┆ 0    ┆ 20     ┆ true   │
-        │ …          ┆ …     ┆ …    ┆ …          ┆ …     ┆ …    ┆ …      ┆ …      │
-        │ 607.094955 ┆ false ┆ 60   ┆ [740, 370] ┆ pix   ┆ 0    ┆ 20     ┆ true   │
-        │ 609.104958 ┆ true  ┆ 60   ┆ [740, 370] ┆ pix   ┆ 0    ┆ 20     ┆ true   │
-        └────────────┴───────┴──────┴────────────┴───────┴──────┴────────┴────────┘
+        PhotoDiode dataframe::
+
+            ┌────────────┬───────┬──────┬────────────┬───────┬──────┬────────┬────────┐
+            │ time       ┆ state ┆ size ┆ pos        ┆ units ┆ mode ┆ frames ┆ enable │
+            │ ---        ┆ ---   ┆ ---  ┆ ---        ┆ ---   ┆ ---  ┆ ---    ┆ ---    │
+            │ f64        ┆ bool  ┆ i64  ┆ list[i64]  ┆ str   ┆ i64  ┆ i64    ┆ bool   │
+            ╞════════════╪═══════╪══════╪════════════╪═══════╪══════╪════════╪════════╡
+            │ 18.990026  ┆ false ┆ 60   ┆ [740, 370] ┆ pix   ┆ 0    ┆ 20     ┆ true   │
+            │ 21.000029  ┆ true  ┆ 60   ┆ [740, 370] ┆ pix   ┆ 0    ┆ 20     ┆ true   │
+            │ …          ┆ …     ┆ …    ┆ …          ┆ …     ┆ …    ┆ …      ┆ …      │
+            │ 607.094955 ┆ false ┆ 60   ┆ [740, 370] ┆ pix   ┆ 0    ┆ 20     ┆ true   │
+            │ 609.104958 ┆ true  ┆ 60   ┆ [740, 370] ┆ pix   ┆ 0    ┆ 20     ┆ true   │
+            └────────────┴───────┴──────┴────────────┴───────┴──────┴────────┴────────┘
+
         :return:
         """
         df = pl.DataFrame().with_columns(
             pl.Series(self.p_time).alias('time'),
             pl.Series(self.p_state).alias('state'),
             pl.Series(self.p_size).alias('size'),
             pl.Series(self.p_pos).alias('pos'),
@@ -288,47 +295,53 @@
             pl.Series(self.p_frames).alias('frames'),
             pl.Series(self.p_enabled).alias('enable')
         )
         return df
 
     def get_state_machine_dataframe(self) -> pl.DataFrame:
         """
-        ┌────────────┬───────────────────────────┬───────────────────────────┐
-        │ time       ┆ state                     ┆ prev_state                │
-        │ ---        ┆ ---                       ┆ ---                       │
-        │ f64        ┆ object                    ┆ object                    │
-        ╞════════════╪═══════════════════════════╪═══════════════════════════╡
-        │ 18.990026  ┆ ('States.SHOW_BLANK', 1)  ┆ ('States.STIM_SELECT', 0) │
-        │ 20.990029  ┆ ('States.SHOW_STIM', 2)   ┆ ('States.SHOW_BLANK', 1)  │
-        │ …          ┆ …                         ┆ …                         │
-        │ 609.094958 ┆ ('States.SHOW_STIM', 2)   ┆ ('States.SHOW_BLANK', 1)  │
-        │ 619.094972 ┆ ('States.STIM_SELECT', 0) ┆ ('States.SHOW_STIM', 2)   │
-        └────────────┴───────────────────────────┴───────────────────────────┘
+        State Machine dataframe::
+
+            ┌────────────┬───────────────────────────┬───────────────────────────┐
+            │ time       ┆ state                     ┆ prev_state                │
+            │ ---        ┆ ---                       ┆ ---                       │
+            │ f64        ┆ str                       ┆ str                       │
+            ╞════════════╪═══════════════════════════╪═══════════════════════════╡
+            │ 18.990026  ┆ ('States.SHOW_BLANK', 1)  ┆ ('States.STIM_SELECT', 0) │
+            │ 20.990029  ┆ ('States.SHOW_STIM', 2)   ┆ ('States.SHOW_BLANK', 1)  │
+            │ …          ┆ …                         ┆ …                         │
+            │ 609.094958 ┆ ('States.SHOW_STIM', 2)   ┆ ('States.SHOW_BLANK', 1)  │
+            │ 619.094972 ┆ ('States.STIM_SELECT', 0) ┆ ('States.SHOW_STIM', 2)   │
+            └────────────┴───────────────────────────┴───────────────────────────┘
+
         :return:
         """
         df = pl.DataFrame().with_columns(
             pl.Series(it[0] for it in self.log_data[2]).alias('time'),
             pl.Series(it[1] for it in self.log_data[2]).alias('state'),
             pl.Series(it[2] for it in self.log_data[2]).alias('prev_state'),
         )
         return df
 
     def get_log_dict_dataframe(self) -> pl.DataFrame:
         """
-        ┌────────────┬──────────┬──────────┬──────────────┬────────────┐
-        │ time       ┆ block_nr ┆ trial_nr ┆ condition_nr ┆ trial_type │
-        │ ---        ┆ ---      ┆ ---      ┆ ---          ┆ ---        │
-        │ f64        ┆ i64      ┆ i64      ┆ i64          ┆ i64        │
-        ╞════════════╪══════════╪══════════╪══════════════╪════════════╡
-        │ 18.990026  ┆ 0        ┆ 0        ┆ 0            ┆ 1          │
-        │ 30.990043  ┆ 1        ┆ 0        ┆ 0            ┆ 1          │
-        │ …          ┆ …        ┆ …        ┆ …            ┆ …          │
-        │ 595.083939 ┆ 48       ┆ 0        ┆ 0            ┆ 1          │
-        │ 607.094955 ┆ 49       ┆ 0        ┆ 0            ┆ 1          │
-        └────────────┴──────────┴──────────┴──────────────┴────────────┘
+        Log Dict DataFrame::
+
+            ┌────────────┬──────────┬──────────┬──────────────┬────────────┐
+            │ time       ┆ block_nr ┆ trial_nr ┆ condition_nr ┆ trial_type │
+            │ ---        ┆ ---      ┆ ---      ┆ ---          ┆ ---        │
+            │ f64        ┆ i64      ┆ i64      ┆ i64          ┆ i64        │
+            ╞════════════╪══════════╪══════════╪══════════════╪════════════╡
+            │ 18.990026  ┆ 0        ┆ 0        ┆ 0            ┆ 1          │
+            │ 30.990043  ┆ 1        ┆ 0        ┆ 0            ┆ 1          │
+            │ …          ┆ …        ┆ …        ┆ …            ┆ …          │
+            │ 595.083939 ┆ 48       ┆ 0        ┆ 0            ┆ 1          │
+            │ 607.094955 ┆ 49       ┆ 0        ┆ 0            ┆ 1          │
+            └────────────┴──────────┴──────────┴──────────────┴────────────┘
+
         :return:
         """
         df = pl.DataFrame().with_columns(
             pl.Series(it[0] for it in self.log_data[3]).alias('time'),
             pl.Series(it[1] for it in self.log_data[3]).alias('block_nr'),
             pl.Series(it[2] for it in self.log_data[3]).alias('trial_nr'),
             pl.Series(it[3] for it in self.log_data[3]).alias('condition_nr'),
@@ -464,7 +477,81 @@
     offset_t_avg = float(np.mean(offset_t))
     offset_t_std = float(np.std(offset_t))
 
     fprint(f'time offset between stimlog and riglog: {round(offset_t_avg, 3)}')
     fprint(f'offset_std: {round(offset_t_std, 3)}')
 
     return offset_t_avg, offset_t_std
+
+
+def load_stimlog(file: PathLike, string_key: bool = True) -> dict[str | int, pl.DataFrame]:
+    """
+    Load directly the stimlog file (without riglog time offset), and parse data as polars dataframes
+
+    .. code-block:: python
+
+        file = ...
+
+        log = load_stimlog(file, string_key=True)  # get dataframe using keyname
+        print(log['PhotoIndicator'])
+
+        log = load_stimlog(file, string_key=False)  # get dataframe using code int
+        print(log[1])
+
+
+    :param file:
+    :param string_key: show key as str type, otherwise, int type
+    :return: Code:DataFrame dictionary
+    """
+
+    log_info = {}
+    log_header = {}
+    log_data = {}
+
+    with Path(file).open() as f:
+        for line, content in enumerate(f):
+            content = content.strip()
+
+            #
+            m = re.match(r'#+ (.+?)\s*:\s*(.+)', content)
+            if m:
+                info_name = m.group(1)
+                info_value = m.group(2)
+                try:
+                    code = int(info_name)
+                except ValueError:
+                    continue
+                else:
+                    name, header = info_value.split(' ', maxsplit=1)
+                    header = eval(header)
+                    log_info[code] = name
+                    log_header[code] = header
+
+            elif content.startswith('#'):
+                print(f'ignore header line at {line + 1} : {content}')
+                continue
+
+            else:  # data
+                code, time, message = content.split(' ', maxsplit=2)
+                code = int(code)
+                time = float(time)
+
+                if log_info[code] == 'StateMachine':
+                    value = eval(message.replace('<', '("').replace(':', '",').replace('>', ')'))
+                    value = list(map(str, value))
+                    if len(log_header[code]) != len(value):
+                        print(f'log category {code} size mismatched at line {line} : {message}')
+                    else:
+                        log_data.setdefault(code, []).append((time, *value))
+
+                else:
+                    value = eval(message)
+                    if len(log_header[code]) != len(value):
+                        print(f'log category {code} size mismatched at line {line} : {message}')
+                    else:
+                        log_data.setdefault(code, []).append((time, *value))
+
+        return {
+            (log_info[code] if string_key else code):
+                pl.DataFrame(log_data[code], schema=['time'] + log_header[code], strict=False)
+            for code in log_data
+        }
```

### Comparing `neura_library-0.0.5/src/neuralib/stimpy/stimpy_pyv.py` & `neura_library-0.0.6/src/neuralib/stimpy/stimpy_pyv.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/stimpy/stimulus.py` & `neura_library-0.0.6/src/neuralib/stimpy/stimulus.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/stimpy/util.py` & `neura_library-0.0.6/src/neuralib/stimpy/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/tools/pkl_parq_view/main_app.py` & `neura_library-0.0.6/src/neuralib/tools/pkl_parq_view/main_app.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/tools/slack_bot/bot.py` & `neura_library-0.0.6/src/neuralib/tools/slack_bot/bot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/cli_args.py` & `neura_library-0.0.6/src/neuralib/util/cli_args.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/color_logging.py` & `neura_library-0.0.6/src/neuralib/util/color_logging.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/csv.py` & `neura_library-0.0.6/src/neuralib/util/csv.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/func.py` & `neura_library-0.0.6/src/neuralib/util/func.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/gpu.py` & `neura_library-0.0.6/src/neuralib/util/gpu.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/io.py` & `neura_library-0.0.6/src/neuralib/util/io.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/json.py` & `neura_library-0.0.6/src/neuralib/util/json.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/profile_test.py` & `neura_library-0.0.6/src/neuralib/util/profile_test.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/segement.py` & `neura_library-0.0.6/src/neuralib/util/segement.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/table.py` & `neura_library-0.0.6/src/neuralib/util/table.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/tqdm.py` & `neura_library-0.0.6/src/neuralib/util/tqdm.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/util_clazz.py` & `neura_library-0.0.6/src/neuralib/util/util_clazz.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/util_cv2.py` & `neura_library-0.0.6/src/neuralib/util/util_cv2.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/util_type.py` & `neura_library-0.0.6/src/neuralib/util/util_type.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/util_verbose.py` & `neura_library-0.0.6/src/neuralib/util/util_verbose.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/utils.py` & `neura_library-0.0.6/src/neuralib/util/utils.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/util/version.py` & `neura_library-0.0.6/src/neuralib/util/version.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/wrapper/deeplabcut/core.py` & `neura_library-0.0.6/src/neuralib/wrapper/deeplabcut/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/wrapper/deeplabcut/util.py` & `neura_library-0.0.6/src/neuralib/wrapper/deeplabcut/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/wrapper/facemap/__init__.py` & `neura_library-0.0.6/src/neuralib/wrapper/facemap/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/wrapper/facemap/core.py` & `neura_library-0.0.6/src/neuralib/wrapper/facemap/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/wrapper/facemap/plot.py` & `neura_library-0.0.6/src/neuralib/wrapper/facemap/plot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/wrapper/rastermap/__init__.py` & `neura_library-0.0.6/src/neuralib/wrapper/rastermap/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/src/neuralib/wrapper/rastermap/core.py` & `neura_library-0.0.6/src/neuralib/wrapper/rastermap/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/test/test_argp.py` & `neura_library-0.0.6/test/test_argp.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/test/test_argp_dispatch.py` & `neura_library-0.0.6/test/test_argp_dispatch.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/test/test_csv_context_manager.py` & `neura_library-0.0.6/test/test_csv_context_manager.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/test/test_persistence_autoinc.py` & `neura_library-0.0.6/test/test_persistence_autoinc.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/test/test_protocol_parser.py` & `neura_library-0.0.6/test/test_protocol_parser.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/test/test_pyvstim_parser.py` & `neura_library-0.0.6/test/test_pyvstim_parser.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/test/test_stimpy_bitbucket_parser.py` & `neura_library-0.0.6/test/test_stimpy_bitbucket_parser.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/test/test_stimpy_github_parser.py` & `neura_library-0.0.6/test/test_stimpy_github_parser.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.5/test/test_util_func.py` & `neura_library-0.0.6/test/test_util_func.py`

 * *Files identical despite different names*

