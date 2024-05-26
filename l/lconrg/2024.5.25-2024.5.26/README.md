# Comparing `tmp/lconrg-2024.5.25.tar.gz` & `tmp/lconrg-2024.5.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lconrg-2024.5.25.tar", max compression
+gzip compressed data, was "lconrg-2024.5.26.tar", max compression
```

## Comparing `lconrg-2024.5.25.tar` & `lconrg-2024.5.26.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1082 2024-05-25 10:43:51.288151 lconrg-2024.5.25/LICENSE
--rw-r--r--   0        0        0     1086 2024-05-25 10:43:51.288151 lconrg-2024.5.25/pyproject.toml
--rw-r--r--   0        0        0        7 2024-05-25 10:43:51.288151 lconrg-2024.5.25/src/lconrg/.python-version
--rw-r--r--   0        0        0      395 2024-05-25 10:43:51.288151 lconrg-2024.5.25/src/lconrg/__init__.py
--rw-r--r--   0        0        0    34884 2024-05-25 10:43:51.288151 lconrg-2024.5.25/src/lconrg/lconrg.py
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 lconrg-2024.5.25/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-26 09:33:47.209445 lconrg-2024.5.26/LICENSE
+-rw-r--r--   0        0        0     1085 2024-05-26 09:33:47.209445 lconrg-2024.5.26/pyproject.toml
+-rw-r--r--   0        0        0        7 2024-05-26 09:33:47.209445 lconrg-2024.5.26/src/lconrg/.python-version
+-rw-r--r--   0        0        0      395 2024-05-26 09:33:47.209445 lconrg-2024.5.26/src/lconrg/__init__.py
+-rw-r--r--   0        0        0    34827 2024-05-26 09:33:47.209445 lconrg-2024.5.26/src/lconrg/lconrg.py
+-rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 lconrg-2024.5.26/PKG-INFO
```

### Comparing `lconrg-2024.5.25/LICENSE` & `lconrg-2024.5.26/LICENSE`

 * *Files identical despite different names*

### Comparing `lconrg-2024.5.25/pyproject.toml` & `lconrg-2024.5.26/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lconrg"
-version = "2024.05.25"
+version = "2024.5.26"
 description = ""
 authors = ["Your Name <you@example.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.11"
 numpy = "^1.22"
 pandas = "^1.4.1"
```

### Comparing `lconrg-2024.5.25/src/lconrg/lconrg.py` & `lconrg-2024.5.26/src/lconrg/lconrg.py`

 * *Files 0% similar despite different names*

```diff
@@ -730,34 +730,31 @@
         lrmc_df = pv_cf[["capital_kgbp", "fixed_opex_kgbp"]]
         srmc = sum(srmc_df.stack().values) / sum(  # type: ignore
             pv_cf.production_GWth.values
         )
         srmc_cap = (  # type: ignore
             sum(srmc_df.stack().values)  # type: ignore
             / sum(pv_cf.capacity_mw.values)  # type: ignore
-            / 1000
         )
         lrmc = sum(lrmc_df.stack().values) / sum(  # type: ignore
             pv_cf.production_GWth.values
         )
         lrmc_cap = (  # type: ignore
             sum(lrmc_df.stack().values)  # type: ignore
             / sum(pv_cf.capacity_mw.values)  # type: ignore
-            / 1000
         )
         lcoe = srmc + lrmc
         lcoe_cap = srmc_cap + lrmc_cap
         full = (
             pv_cf.drop(["production_GWth", "capacity_mw"], axis=1).sum()
             / pv_cf.production_GWth.sum()
         )
         full_cap = (
             pv_cf.drop(["production_GWth", "capacity_mw"], axis=1).sum()
             / pv_cf.capacity_mw.sum()
-            / 1000
         )
 
         LCONRG = namedtuple(
             "LCONRG",
             [
                 "lcoe_gbp_mwh",
                 "srmc_gbp_mwh",
```

