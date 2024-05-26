# Comparing `tmp/dashport-0.7.6.tar.gz` & `tmp/dashport-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashport-0.7.6.tar", last modified: Sun May 12 06:44:45 2024, max compression
+gzip compressed data, was "dashport-0.7.7.tar", last modified: Sun May 26 09:28:27 2024, max compression
```

## Comparing `dashport-0.7.6.tar` & `dashport-0.7.7.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:44:45.094601 dashport-0.7.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:44:45.078601 dashport-0.7.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:44:45.082601 dashport-0.7.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-12 06:44:40.000000 dashport-0.7.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-12 06:44:40.000000 dashport-0.7.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    34459 2024-05-12 06:44:40.000000 dashport-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-12 06:44:45.094601 dashport-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-12 06:44:40.000000 dashport-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:44:45.082601 dashport-0.7.6/dashport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:44:40.000000 dashport-0.7.6/dashport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-12 06:44:40.000000 dashport-0.7.6/dashport/borders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-12 06:44:40.000000 dashport-0.7.6/dashport/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-12 06:44:40.000000 dashport-0.7.6/dashport/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-12 06:44:40.000000 dashport-0.7.6/dashport/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)    10973 2024-05-12 06:44:40.000000 dashport-0.7.6/dashport/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-12 06:44:40.000000 dashport-0.7.6/dashport/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:44:45.086601 dashport-0.7.6/dashport/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:44:40.000000 dashport-0.7.6/dashport/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-12 06:44:40.000000 dashport-0.7.6/dashport/resources/block_elements_table.json
--rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-05-12 06:44:40.000000 dashport-0.7.6/dashport/resources/box_drawing_table.json
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-12 06:44:40.000000 dashport-0.7.6/dashport/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-12 06:44:40.000000 dashport-0.7.6/dashport/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:44:45.094601 dashport-0.7.6/dashport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-12 06:44:45.000000 dashport-0.7.6/dashport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-12 06:44:45.000000 dashport-0.7.6/dashport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 06:44:45.000000 dashport-0.7.6/dashport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-12 06:44:45.000000 dashport-0.7.6/dashport.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:44:45.086601 dashport-0.7.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/buttons.md
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/colors.md
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/dashport.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:44:45.086601 dashport-0.7.6/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/examples/boilerplate.md
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/examples/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/examples/layouts.md
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/examples/util.md
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/examples/views.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:44:45.090601 dashport-0.7.6/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   110554 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/images/Layout_quadrants.png
--rw-r--r--   0 runner    (1001) docker     (127)    66901 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/images/Layout_split_screen_horizontal.png
--rw-r--r--   0 runner    (1001) docker     (127)    76578 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/images/Layout_split_screen_vert.png
--rw-r--r--   0 runner    (1001) docker     (127)    92502 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/images/Layout_three_horizontal.png
--rw-r--r--   0 runner    (1001) docker     (127)   107025 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/images/Layout_three_vert.png
--rw-r--r--   0 runner    (1001) docker     (127)   558852 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/images/color_palette.png
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/layouts.md
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/panels.md
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/strings.md
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-12 06:44:40.000000 dashport-0.7.6/docs/widgets.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:44:45.090601 dashport-0.7.6/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:44:45.090601 dashport-0.7.6/examples/boilerplate/
--rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/boilerplate/basic_window.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      437 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/boilerplate/boilerplate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      433 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/boilerplate/color_example.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/boilerplate/rectangle.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2089 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/boilerplate/using_buttons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:44:45.094601 dashport-0.7.6/examples/layouts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/layouts/arbitrary_panels.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1373 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/layouts/custom_borders.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      578 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/layouts/split_screen_columns.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1896 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/layouts/split_screen_quad.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      561 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/layouts/split_screen_rows.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1262 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/layouts/split_screen_three_horizontal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1260 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/layouts/split_screen_three_vert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:44:45.094601 dashport-0.7.6/examples/util/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1166 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/util/all_ascii_constants.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1010 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/util/all_attributes_curses.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4797 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/util/all_box_drawing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/util/color_palette.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1080 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/util/explore_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:44:45.094601 dashport-0.7.6/examples/views/
--rwxr-xr-x   0 runner    (1001) docker     (127)      830 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/views/interactive_prompt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2541 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/views/multiple_views.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      711 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/views/scroll_panels.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      703 2024-05-12 06:44:40.000000 dashport-0.7.6/examples/views/scroll_text.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 06:44:45.094601 dashport-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-12 06:44:40.000000 dashport-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:28:27.546936 dashport-0.7.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:28:27.534936 dashport-0.7.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:28:27.538936 dashport-0.7.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-26 09:28:19.000000 dashport-0.7.7/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-26 09:28:19.000000 dashport-0.7.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    34459 2024-05-26 09:28:19.000000 dashport-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-26 09:28:27.546936 dashport-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-26 09:28:19.000000 dashport-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:28:27.538936 dashport-0.7.7/dashport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 09:28:19.000000 dashport-0.7.7/dashport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-26 09:28:19.000000 dashport-0.7.7/dashport/borders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-26 09:28:19.000000 dashport-0.7.7/dashport/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-26 09:28:19.000000 dashport-0.7.7/dashport/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-26 09:28:19.000000 dashport-0.7.7/dashport/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10973 2024-05-26 09:28:19.000000 dashport-0.7.7/dashport/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-26 09:28:19.000000 dashport-0.7.7/dashport/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:28:27.538936 dashport-0.7.7/dashport/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 09:28:19.000000 dashport-0.7.7/dashport/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-26 09:28:19.000000 dashport-0.7.7/dashport/resources/block_elements_table.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-05-26 09:28:19.000000 dashport-0.7.7/dashport/resources/box_drawing_table.json
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-26 09:28:19.000000 dashport-0.7.7/dashport/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-26 09:28:19.000000 dashport-0.7.7/dashport/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:28:27.546936 dashport-0.7.7/dashport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-26 09:28:27.000000 dashport-0.7.7/dashport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-26 09:28:27.000000 dashport-0.7.7/dashport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 09:28:27.000000 dashport-0.7.7/dashport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 09:28:27.000000 dashport-0.7.7/dashport.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:28:27.542936 dashport-0.7.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/buttons.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/colors.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/dashport.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:28:27.542936 dashport-0.7.7/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/examples/boilerplate.md
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/examples/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/examples/layouts.md
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/examples/util.md
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/examples/views.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:28:27.542936 dashport-0.7.7/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   110554 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/images/Layout_quadrants.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66901 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/images/Layout_split_screen_horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76578 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/images/Layout_split_screen_vert.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92502 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/images/Layout_three_horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (127)   107025 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/images/Layout_three_vert.png
+-rw-r--r--   0 runner    (1001) docker     (127)   558852 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/images/color_palette.png
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/layouts.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/panels.md
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/strings.md
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-26 09:28:19.000000 dashport-0.7.7/docs/widgets.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:28:27.542936 dashport-0.7.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:28:27.546936 dashport-0.7.7/examples/boilerplate/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/boilerplate/basic_window.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      437 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/boilerplate/boilerplate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      433 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/boilerplate/color_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/boilerplate/rectangle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2089 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/boilerplate/using_buttons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:28:27.546936 dashport-0.7.7/examples/layouts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/layouts/arbitrary_panels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1373 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/layouts/custom_borders.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      578 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/layouts/split_screen_columns.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1896 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/layouts/split_screen_quad.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      561 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/layouts/split_screen_rows.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1262 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/layouts/split_screen_three_horizontal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1260 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/layouts/split_screen_three_vert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:28:27.546936 dashport-0.7.7/examples/util/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1166 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/util/all_ascii_constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1010 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/util/all_attributes_curses.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4797 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/util/all_box_drawing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/util/color_palette.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1080 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/util/explore_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:28:27.546936 dashport-0.7.7/examples/views/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      830 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/views/interactive_prompt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2541 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/views/multiple_views.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      711 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/views/scroll_panels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      703 2024-05-26 09:28:19.000000 dashport-0.7.7/examples/views/scroll_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 09:28:27.546936 dashport-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-26 09:28:19.000000 dashport-0.7.7/setup.py
```

### Comparing `dashport-0.7.6/.github/workflows/publish-to-pypi.yml` & `dashport-0.7.7/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/.gitignore` & `dashport-0.7.7/.gitignore`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/LICENSE` & `dashport-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/PKG-INFO` & `dashport-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashport
-Version: 0.7.6
+Version: 0.7.7
 Summary: Dashport curses wrapper for Python
 Home-page: https://github.com/numbertheory/dashport
 Author: JP Etcheber
 Author-email: jetcheber@gmail.com
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/dashport.svg)](https://badge.fury.io/py/dashport) [![Documentation Status](https://readthedocs.org/projects/dashport/badge/?version=latest)](https://dashport.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `dashport-0.7.6/dashport/borders.py` & `dashport-0.7.7/dashport/borders.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/dashport/characters.py` & `dashport-0.7.7/dashport/characters.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/dashport/colors.py` & `dashport-0.7.7/dashport/colors.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/dashport/dash.py` & `dashport-0.7.7/dashport/dash.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/dashport/layout.py` & `dashport-0.7.7/dashport/layout.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/dashport/prompt.py` & `dashport-0.7.7/dashport/prompt.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,18 @@
         if x == 261:
             app.user_prompt_position += 1
         if x not in invalid_chars and curses.ascii.isprint(x):
             command_line_entered.insert(app.user_prompt_position, chr(x))
             app.user_prompt_position += 1
         if x == backspace_key() and len(command_line_entered) > 0:
             try:
-                command_line_entered.pop(app.user_prompt_position - 1)
+                if platform.system().lower() == "linux":
+                    command_line_entered.pop(app.user_prompt_position - 2)
+                else:
+                    command_line_entered.pop(app.user_prompt_position - 1)
             except IndexError:
                 pass
             app.user_prompt_position -= 1
         app.screen.refresh()
         if x == 127:
             x = 263
         if x == 262:
```

### Comparing `dashport-0.7.6/dashport/resources/block_elements_table.json` & `dashport-0.7.7/dashport/resources/block_elements_table.json`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/dashport/resources/box_drawing_table.json` & `dashport-0.7.7/dashport/resources/box_drawing_table.json`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/dashport/run.py` & `dashport-0.7.7/dashport/run.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/dashport/widgets.py` & `dashport-0.7.7/dashport/widgets.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/dashport.egg-info/PKG-INFO` & `dashport-0.7.7/dashport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashport
-Version: 0.7.6
+Version: 0.7.7
 Summary: Dashport curses wrapper for Python
 Home-page: https://github.com/numbertheory/dashport
 Author: JP Etcheber
 Author-email: jetcheber@gmail.com
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/dashport.svg)](https://badge.fury.io/py/dashport) [![Documentation Status](https://readthedocs.org/projects/dashport/badge/?version=latest)](https://dashport.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `dashport-0.7.6/dashport.egg-info/SOURCES.txt` & `dashport-0.7.7/dashport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/Makefile` & `dashport-0.7.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/buttons.md` & `dashport-0.7.7/docs/buttons.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/colors.md` & `dashport-0.7.7/docs/colors.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/conf.py` & `dashport-0.7.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/dashport.md` & `dashport-0.7.7/docs/dashport.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/examples/boilerplate.md` & `dashport-0.7.7/docs/examples/boilerplate.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/examples/layouts.md` & `dashport-0.7.7/docs/examples/layouts.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/examples/views.md` & `dashport-0.7.7/docs/examples/views.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/images/Layout_quadrants.png` & `dashport-0.7.7/docs/images/Layout_quadrants.png`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/images/Layout_split_screen_horizontal.png` & `dashport-0.7.7/docs/images/Layout_split_screen_horizontal.png`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/images/Layout_split_screen_vert.png` & `dashport-0.7.7/docs/images/Layout_split_screen_vert.png`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/images/Layout_three_horizontal.png` & `dashport-0.7.7/docs/images/Layout_three_horizontal.png`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/images/Layout_three_vert.png` & `dashport-0.7.7/docs/images/Layout_three_vert.png`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/images/color_palette.png` & `dashport-0.7.7/docs/images/color_palette.png`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/index.rst` & `dashport-0.7.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/layouts.md` & `dashport-0.7.7/docs/layouts.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/panels.md` & `dashport-0.7.7/docs/panels.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/strings.md` & `dashport-0.7.7/docs/strings.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/docs/widgets.md` & `dashport-0.7.7/docs/widgets.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/boilerplate/basic_window.py` & `dashport-0.7.7/examples/boilerplate/basic_window.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/boilerplate/rectangle.py` & `dashport-0.7.7/examples/boilerplate/rectangle.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/boilerplate/using_buttons.py` & `dashport-0.7.7/examples/boilerplate/using_buttons.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/layouts/arbitrary_panels.py` & `dashport-0.7.7/examples/layouts/arbitrary_panels.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/layouts/custom_borders.py` & `dashport-0.7.7/examples/layouts/custom_borders.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/layouts/split_screen_columns.py` & `dashport-0.7.7/examples/layouts/split_screen_columns.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/layouts/split_screen_quad.py` & `dashport-0.7.7/examples/layouts/split_screen_quad.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/layouts/split_screen_rows.py` & `dashport-0.7.7/examples/layouts/split_screen_rows.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/layouts/split_screen_three_horizontal.py` & `dashport-0.7.7/examples/layouts/split_screen_three_horizontal.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/layouts/split_screen_three_vert.py` & `dashport-0.7.7/examples/layouts/split_screen_three_vert.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/util/all_ascii_constants.py` & `dashport-0.7.7/examples/util/all_ascii_constants.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/util/all_attributes_curses.py` & `dashport-0.7.7/examples/util/all_attributes_curses.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/util/all_box_drawing.py` & `dashport-0.7.7/examples/util/all_box_drawing.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/util/color_palette.py` & `dashport-0.7.7/examples/util/color_palette.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/util/explore_screen.py` & `dashport-0.7.7/examples/util/explore_screen.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/views/interactive_prompt.py` & `dashport-0.7.7/examples/views/interactive_prompt.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/views/multiple_views.py` & `dashport-0.7.7/examples/views/multiple_views.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/views/scroll_panels.py` & `dashport-0.7.7/examples/views/scroll_panels.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/examples/views/scroll_text.py` & `dashport-0.7.7/examples/views/scroll_text.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.6/setup.py` & `dashport-0.7.7/setup.py`

 * *Files identical despite different names*

