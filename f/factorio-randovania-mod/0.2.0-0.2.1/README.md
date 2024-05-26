# Comparing `tmp/factorio_randovania_mod-0.2.0.tar.gz` & `tmp/factorio_randovania_mod-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factorio_randovania_mod-0.2.0.tar", last modified: Thu May 23 21:26:14 2024, max compression
+gzip compressed data, was "factorio_randovania_mod-0.2.1.tar", last modified: Sun May 26 20:36:00 2024, max compression
```

## Comparing `factorio_randovania_mod-0.2.0.tar` & `factorio_randovania_mod-0.2.1.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.470064 factorio_randovania_mod-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.462064 factorio_randovania_mod-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.462064 factorio_randovania_mod-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-23 21:26:14.470064 factorio_randovania_mod-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:26:14.470064 factorio_randovania_mod-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.458064 factorio_randovania_mod-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.466064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/configuration.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.466064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/files/
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/files/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.466064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/control.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/data-updates.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/data.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.462064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/graphics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.466064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/graphics/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.462064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.466064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/locale/en/
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.466064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/prototypes/
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/prototypes/burners.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/prototypes/tech.lua
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 21:26:14.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.466064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-23 21:26:14.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-23 21:26:14.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:26:14.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-23 21:26:14.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 21:26:14.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 21:26:14.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.466064 factorio_randovania_mod-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/tests/test_color_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.757798 factorio_randovania_mod-0.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.757798 factorio_randovania_mod-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.753798 factorio_randovania_mod-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.757798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/__pyinstaller/hook-factorio_randovania_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/configuration.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/files/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/control.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/data-updates.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/data.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.753798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/graphics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/graphics/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.753798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/locale/en/
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/prototypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/prototypes/burners.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/prototypes/tech.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-26 20:36:00.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-26 20:36:00.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-26 20:36:00.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 20:36:00.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-26 20:36:00.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-26 20:36:00.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-26 20:36:00.000000 factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:00.761798 factorio_randovania_mod-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-26 20:35:51.000000 factorio_randovania_mod-0.2.1/tests/test_color_util.py
```

### Comparing `factorio_randovania_mod-0.2.0/.github/dependabot.yml` & `factorio_randovania_mod-0.2.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/.github/workflows/python.yml` & `factorio_randovania_mod-0.2.1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/.gitignore` & `factorio_randovania_mod-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/.pre-commit-config.yaml` & `factorio_randovania_mod-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/LICENSE` & `factorio_randovania_mod-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/PKG-INFO` & `factorio_randovania_mod-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factorio-randovania-mod
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generator of Factorio Randomizer mods for Randovania
 Author: Henrique Gemignani Passos Lima
 Project-URL: Homepage, https://github.com/randovania/factorio-randovania-mod
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `factorio_randovania_mod-0.2.0/pyproject.toml` & `factorio_randovania_mod-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/cli.py` & `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/cli.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/color_util.py` & `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/color_util.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/configuration.pyi` & `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/configuration.pyi`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/creator.py` & `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/creator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import collections
 import configparser
+import os
 import shutil
 import typing
 from pathlib import Path
 
 import PIL.Image
 
 from factorio_randovania_mod import color_util
@@ -121,31 +122,41 @@
         hue_shift(
             base_graphics_path.joinpath(source_path),
             output_path.joinpath("graphics", target_path),
             rotation,
         )
 
 
+def ensure_locale_read(locale: configparser.ConfigParser, files: list[Path]) -> None:
+    filenames = [os.fspath(filename) for filename in files]
+    did_read = locale.read(filenames)
+    if did_read != filenames:
+        missing = set(filenames) - set(did_read)
+        raise FileNotFoundError(str(missing))
+
+
 def create(factorio_path: Path, patch_data: Configuration, output_folder: Path) -> None:
     output_path = output_folder.joinpath("randovania-layout")
     shutil.rmtree(output_path, ignore_errors=True)
 
     original_locale = configparser.ConfigParser()
-    original_locale.read(
+    ensure_locale_read(
+        original_locale,
         [
             factorio_path.joinpath("data/base/locale/en/base.cfg"),
             template_path.joinpath("locale/en/strings.cfg"),
-        ]
+        ],
     )
 
     locale = configparser.ConfigParser()
-    locale.read(
+    ensure_locale_read(
+        locale,
         [
             template_path.joinpath("locale/en/strings.cfg"),
-        ]
+        ],
     )
 
     tech_tree_lua = []
     progressive_sources = collections.defaultdict(list)
     local_unlocks = {}
 
     for tech in patch_data["technologies"]:
```

### Comparing `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/files/schema.json` & `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/files/schema.json`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/control.lua` & `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/control.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/data-updates.lua` & `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/data-updates.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/data.lua` & `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/data.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png` & `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg` & `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/prototypes/burners.lua` & `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/prototypes/burners.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua` & `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/prototypes/tech.lua` & `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_src/prototypes/tech.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_util.py` & `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod/lua_util.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/PKG-INFO` & `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factorio-randovania-mod
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generator of Factorio Randomizer mods for Randovania
 Author: Henrique Gemignani Passos Lima
 Project-URL: Homepage, https://github.com/randovania/factorio-randovania-mod
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/SOURCES.txt` & `factorio_randovania_mod-0.2.1/src/factorio_randovania_mod.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 src/factorio_randovania_mod/version.py
 src/factorio_randovania_mod.egg-info/PKG-INFO
 src/factorio_randovania_mod.egg-info/SOURCES.txt
 src/factorio_randovania_mod.egg-info/dependency_links.txt
 src/factorio_randovania_mod.egg-info/entry_points.txt
 src/factorio_randovania_mod.egg-info/requires.txt
 src/factorio_randovania_mod.egg-info/top_level.txt
+src/factorio_randovania_mod/__pyinstaller/__init__.py
+src/factorio_randovania_mod/__pyinstaller/hook-factorio_randovania_mod.py
 src/factorio_randovania_mod/files/schema.json
 src/factorio_randovania_mod/lua_src/control.lua
 src/factorio_randovania_mod/lua_src/data-updates.lua
 src/factorio_randovania_mod/lua_src/data.lua
 src/factorio_randovania_mod/lua_src/info.json
 src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png
 src/factorio_randovania_mod/lua_src/locale/en/strings.cfg
```

