# Comparing `tmp/nomenklatura-3.9.2.tar.gz` & `tmp/nomenklatura-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-3.9.2.tar", last modified: Sun Jan 14 14:36:47 2024, max compression
+gzip compressed data, was "nomenklatura-3.9.3.tar", last modified: Tue Jan 16 13:08:00 2024, max compression
```

## Comparing `nomenklatura-3.9.2.tar` & `nomenklatura-3.9.3.tar`

### file list

```diff
@@ -1,126 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.347857 nomenklatura-3.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-01-14 14:36:47.347857 nomenklatura-3.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.335857 nomenklatura-3.9.2/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.335857 nomenklatura-3.9.2/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/data/regression-v1.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/data/regression-v2.pkl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.335857 nomenklatura-3.9.2/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.339856 nomenklatura-3.9.2/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/enrich/opencorporates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/enrich/openfigi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/enrich/permid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.339856 nomenklatura-3.9.2/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (127)    15568 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.339856 nomenklatura-3.9.2/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/judgement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.339856 nomenklatura-3.9.2/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.343857 nomenklatura-3.9.2/nomenklatura/matching/compare/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/compare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/compare/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/compare/countries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/compare/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/compare/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/compare/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/compare/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/compare/names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/compare/phonetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/compare/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/logic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.343857 nomenklatura-3.9.2/nomenklatura/matching/name_based/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/name_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/name_based/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/name_based/names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.343857 nomenklatura-3.9.2/nomenklatura/matching/regression_v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/regression_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/regression_v1/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/regression_v1/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/regression_v1/names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/regression_v1/train.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/regression_v1/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.343857 nomenklatura-3.9.2/nomenklatura/matching/regression_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/regression_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/regression_v2/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/regression_v2/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/regression_v2/names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/regression_v2/train.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/regression_v2/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/matching/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.343857 nomenklatura-3.9.2/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.343857 nomenklatura-3.9.2/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    13027 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/senzing.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.343857 nomenklatura-3.9.2/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/statement/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.347857 nomenklatura-3.9.2/nomenklatura/store/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/store/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/store/level.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/store/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/store/redis_.py
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/store/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/store/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.347857 nomenklatura-3.9.2/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:36:47.335857 nomenklatura-3.9.2/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-01-14 14:36:47.000000 nomenklatura-3.9.2/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-01-14 14:36:47.000000 nomenklatura-3.9.2/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 14:36:47.000000 nomenklatura-3.9.2/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-14 14:36:47.000000 nomenklatura-3.9.2/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 14:36:47.000000 nomenklatura-3.9.2/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 14:35:42.000000 nomenklatura-3.9.2/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-01-14 14:36:47.000000 nomenklatura-3.9.2/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-14 14:36:47.000000 nomenklatura-3.9.2/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-14 14:36:47.347857 nomenklatura-3.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-01-14 14:34:28.000000 nomenklatura-3.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.354411 nomenklatura-3.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-01-16 13:08:00.354411 nomenklatura-3.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.342411 nomenklatura-3.9.3/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.342411 nomenklatura-3.9.3/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/data/regression-v1.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/data/regression-v2.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.346411 nomenklatura-3.9.3/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.346411 nomenklatura-3.9.3/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/enrich/opencorporates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/enrich/openfigi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/enrich/permid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.346411 nomenklatura-3.9.3/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15568 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.346411 nomenklatura-3.9.3/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/judgement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.346411 nomenklatura-3.9.3/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.350411 nomenklatura-3.9.3/nomenklatura/matching/compare/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/compare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/compare/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/compare/countries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/compare/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/compare/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/compare/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/compare/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/compare/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/compare/phonetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/compare/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/logic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.350411 nomenklatura-3.9.3/nomenklatura/matching/name_based/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/name_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/name_based/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/name_based/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.350411 nomenklatura-3.9.3/nomenklatura/matching/regression_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/regression_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/regression_v1/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/regression_v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/regression_v1/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/regression_v1/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/regression_v1/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.350411 nomenklatura-3.9.3/nomenklatura/matching/regression_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/regression_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/regression_v2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/regression_v2/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/regression_v2/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/regression_v2/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/regression_v2/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/matching/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.350411 nomenklatura-3.9.3/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.350411 nomenklatura-3.9.3/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13027 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.350411 nomenklatura-3.9.3/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/statement/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.354411 nomenklatura-3.9.3/nomenklatura/store/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/store/level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/store/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/store/redis_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/store/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/store/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.354411 nomenklatura-3.9.3/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:08:00.342411 nomenklatura-3.9.3/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-01-16 13:08:00.000000 nomenklatura-3.9.3/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-01-16 13:08:00.000000 nomenklatura-3.9.3/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 13:08:00.000000 nomenklatura-3.9.3/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-16 13:08:00.000000 nomenklatura-3.9.3/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 13:08:00.000000 nomenklatura-3.9.3/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 13:06:40.000000 nomenklatura-3.9.3/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-01-16 13:08:00.000000 nomenklatura-3.9.3/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-16 13:08:00.000000 nomenklatura-3.9.3/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 13:08:00.354411 nomenklatura-3.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-01-16 13:05:26.000000 nomenklatura-3.9.3/setup.py
```

### Comparing `nomenklatura-3.9.2/LICENSE` & `nomenklatura-3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/PKG-INFO` & `nomenklatura-3.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.9.2
+Version: 3.9.3
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Description-Content-Type: text/markdown
```

### Comparing `nomenklatura-3.9.2/README.md` & `nomenklatura-3.9.3/README.md`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/cache.py` & `nomenklatura-3.9.3/nomenklatura/cache.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/cli.py` & `nomenklatura-3.9.3/nomenklatura/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import orjson
 import yaml
 import click
 import logging
 from pathlib import Path
 from typing import Generator, Iterable, List, Optional, Tuple
 from followthemoney.cli.util import path_writer, InPath, OutPath
 from followthemoney.cli.util import path_entities, write_entity
@@ -15,15 +14,14 @@
 from nomenklatura.dataset import Dataset, DefaultDataset
 from nomenklatura.entity import CompositeEntity as Entity
 from nomenklatura.enrich import Enricher, make_enricher, match, enrich
 from nomenklatura.statement import Statement, CSV, FORMATS
 from nomenklatura.matching import get_algorithm, DefaultAlgorithm
 from nomenklatura.statement import write_statements, read_path_statements
 from nomenklatura.stream import StreamEntity
-from nomenklatura.senzing import senzing_record
 from nomenklatura.xref import xref as run_xref
 from nomenklatura.tui import dedupe_ui
 
 
 log = logging.getLogger(__name__)
 
 ResPath = click.Path(dir_okay=False, writable=True, path_type=Path)
@@ -209,28 +207,14 @@
             stream = path_entities(entities, Entity)
             for proxy in enrich(enricher, resolver_, stream):
                 write_entity(fh, proxy)
     finally:
         enricher.close()
 
 
-@cli.command("export-senzing", help="Export entities to Senzing API format")
-@click.argument("path", type=InPath)
-@click.option("-o", "--outpath", type=OutPath, default="-")
-@click.option("-d", "--dataset", type=str, required=True)
-def export_senzing(path: Path, outpath: Path, dataset: str) -> None:
-    with path_writer(outpath) as outfh:
-        for entity in path_entities(path, Entity):
-            record = senzing_record(dataset, entity)
-            if record is None:
-                continue
-            out = orjson.dumps(record, option=orjson.OPT_APPEND_NEWLINE)
-            outfh.write(out)
-
-
 @cli.command("statements", help="Export entities to statements")
 @click.argument("path", type=InPath)
 @click.option("-o", "--outpath", type=OutPath, default="-")
 @click.option("-d", "--dataset", type=str, required=True)
 @click.option("-f", "--format", type=click.Choice(FORMATS), default=CSV)
 def entity_statements(path: Path, outpath: Path, dataset: str, format: str) -> None:
     def make_statements() -> Generator[Statement, None, None]:
```

### Comparing `nomenklatura-3.9.2/nomenklatura/data/regression-v1.pkl` & `nomenklatura-3.9.3/nomenklatura/data/regression-v1.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/data/regression-v2.pkl` & `nomenklatura-3.9.3/nomenklatura/data/regression-v2.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/dataset/catalog.py` & `nomenklatura-3.9.3/nomenklatura/dataset/catalog.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/dataset/coverage.py` & `nomenklatura-3.9.3/nomenklatura/dataset/coverage.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/dataset/dataset.py` & `nomenklatura-3.9.3/nomenklatura/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/dataset/publisher.py` & `nomenklatura-3.9.3/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/dataset/resource.py` & `nomenklatura-3.9.3/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/dataset/util.py` & `nomenklatura-3.9.3/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/db.py` & `nomenklatura-3.9.3/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/enrich/__init__.py` & `nomenklatura-3.9.3/nomenklatura/enrich/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/enrich/aleph.py` & `nomenklatura-3.9.3/nomenklatura/enrich/aleph.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/enrich/common.py` & `nomenklatura-3.9.3/nomenklatura/enrich/common.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/enrich/nominatim.py` & `nomenklatura-3.9.3/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/enrich/opencorporates.py` & `nomenklatura-3.9.3/nomenklatura/enrich/opencorporates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/enrich/openfigi.py` & `nomenklatura-3.9.3/nomenklatura/enrich/openfigi.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/enrich/permid.py` & `nomenklatura-3.9.3/nomenklatura/enrich/permid.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-3.9.3/nomenklatura/enrich/wikidata/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-3.9.3/nomenklatura/enrich/wikidata/lang.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,16 @@
         lang: Optional[str] = None,
         original: Optional[str] = None,
     ) -> None:
         if text is None or len(text.strip()) == 0:
             text = None
         self.text = text
         self.lang = registry.language.clean(lang)
+        if lang is not None and self.lang is None:
+            self.text = None    
         self.original = original
 
     def __hash__(self) -> int:
         return hash((self.text, self.lang))
 
     def __eq__(self, other: Any) -> bool:
         return hash(self) == hash(other)
```

### Comparing `nomenklatura-3.9.2/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-3.9.3/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-3.9.3/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-3.9.3/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-3.9.3/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/enrich/yente.py` & `nomenklatura-3.9.3/nomenklatura/enrich/yente.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/entity.py` & `nomenklatura-3.9.3/nomenklatura/entity.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/index/entry.py` & `nomenklatura-3.9.3/nomenklatura/index/entry.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/index/index.py` & `nomenklatura-3.9.3/nomenklatura/index/index.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/index/tokenizer.py` & `nomenklatura-3.9.3/nomenklatura/index/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/judgement.py` & `nomenklatura-3.9.3/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/__init__.py` & `nomenklatura-3.9.3/nomenklatura/matching/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/compare/addresses.py` & `nomenklatura-3.9.3/nomenklatura/matching/compare/addresses.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/compare/dates.py` & `nomenklatura-3.9.3/nomenklatura/matching/compare/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/compare/identifiers.py` & `nomenklatura-3.9.3/nomenklatura/matching/compare/identifiers.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/compare/multi.py` & `nomenklatura-3.9.3/nomenklatura/matching/compare/multi.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/compare/names.py` & `nomenklatura-3.9.3/nomenklatura/matching/compare/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/compare/phonetic.py` & `nomenklatura-3.9.3/nomenklatura/matching/compare/phonetic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Optional
 from itertools import product
 from followthemoney.proxy import E
 from followthemoney.types import registry
-from normality.scripts import is_modern_alphabet
+from rigour.text.scripts import is_modern_alphabet
 from fingerprints import clean_name_ascii, clean_entity_prefix
 from nomenklatura.util import name_words, list_intersection, fingerprint_name
 from nomenklatura.util import phonetic_token, metaphone_token, soundex_token
 from nomenklatura.matching.util import type_pair, has_schema
 
 
 def _clean_phonetic_person(original: str) -> Optional[str]:
@@ -20,15 +20,15 @@
 def _clean_phonetic_entity(original: str) -> Optional[str]:
     """Normalize a legal entity name without transliteration."""
     if not is_modern_alphabet(original):
         return None
     return fingerprint_name(original)
 
 
-def _phonetic_tokens(token: str) -> List[str]:
+def _phonetic_person_tokens(token: str) -> List[str]:
     words: List[str] = []
     for word in name_words(_clean_phonetic_person(token), min_length=2):
         words.append(phonetic_token(word))
     return words
 
 
 def _token_names_compare(
@@ -44,16 +44,16 @@
 
 
 def person_name_phonetic_match(query: E, result: E) -> float:
     """Two persons have similar names, using a phonetic algorithm."""
     if not has_schema(query, result, "Person"):
         return 0.0
     query_names_, result_names_ = type_pair(query, result, registry.name)
-    query_names = [_phonetic_tokens(n) for n in query_names_]
-    result_names = [_phonetic_tokens(n) for n in result_names_]
+    query_names = [_phonetic_person_tokens(n) for n in query_names_]
+    result_names = [_phonetic_person_tokens(n) for n in result_names_]
     return _token_names_compare(query_names, result_names)
 
 
 def _metaphone_tokens(token: str) -> List[str]:
     words: List[str] = []
     for word in name_words(_clean_phonetic_entity(token), min_length=2):
         words.append(metaphone_token(word))
```

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/compare/util.py` & `nomenklatura-3.9.3/nomenklatura/matching/compare/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/logic.py` & `nomenklatura-3.9.3/nomenklatura/matching/logic.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/name_based/model.py` & `nomenklatura-3.9.3/nomenklatura/matching/name_based/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/name_based/names.py` & `nomenklatura-3.9.3/nomenklatura/matching/name_based/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/pairs.py` & `nomenklatura-3.9.3/nomenklatura/matching/pairs.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/regression_v1/misc.py` & `nomenklatura-3.9.3/nomenklatura/matching/regression_v1/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/regression_v1/model.py` & `nomenklatura-3.9.3/nomenklatura/matching/regression_v1/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/regression_v1/names.py` & `nomenklatura-3.9.3/nomenklatura/matching/regression_v1/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/regression_v1/train.py` & `nomenklatura-3.9.3/nomenklatura/matching/regression_v1/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/regression_v1/util.py` & `nomenklatura-3.9.3/nomenklatura/matching/regression_v1/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/regression_v2/misc.py` & `nomenklatura-3.9.3/nomenklatura/matching/regression_v2/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/regression_v2/model.py` & `nomenklatura-3.9.3/nomenklatura/matching/regression_v2/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/regression_v2/names.py` & `nomenklatura-3.9.3/nomenklatura/matching/regression_v2/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/regression_v2/train.py` & `nomenklatura-3.9.3/nomenklatura/matching/regression_v2/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/types.py` & `nomenklatura-3.9.3/nomenklatura/matching/types.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/matching/util.py` & `nomenklatura-3.9.3/nomenklatura/matching/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/publish/dates.py` & `nomenklatura-3.9.3/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/publish/edges.py` & `nomenklatura-3.9.3/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/publish/names.py` & `nomenklatura-3.9.3/nomenklatura/publish/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/resolver/edge.py` & `nomenklatura-3.9.3/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/resolver/identifier.py` & `nomenklatura-3.9.3/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/resolver/resolver.py` & `nomenklatura-3.9.3/nomenklatura/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/statement/__init__.py` & `nomenklatura-3.9.3/nomenklatura/statement/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/statement/db.py` & `nomenklatura-3.9.3/nomenklatura/statement/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/statement/serialize.py` & `nomenklatura-3.9.3/nomenklatura/statement/serialize.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/statement/statement.py` & `nomenklatura-3.9.3/nomenklatura/statement/statement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/store/__init__.py` & `nomenklatura-3.9.3/nomenklatura/store/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/store/base.py` & `nomenklatura-3.9.3/nomenklatura/store/base.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/store/level.py` & `nomenklatura-3.9.3/nomenklatura/store/level.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/store/memory.py` & `nomenklatura-3.9.3/nomenklatura/store/memory.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/store/redis_.py` & `nomenklatura-3.9.3/nomenklatura/store/redis_.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/store/sql.py` & `nomenklatura-3.9.3/nomenklatura/store/sql.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/store/util.py` & `nomenklatura-3.9.3/nomenklatura/store/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/stream.py` & `nomenklatura-3.9.3/nomenklatura/stream.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/tui/app.py` & `nomenklatura-3.9.3/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/tui/comparison.py` & `nomenklatura-3.9.3/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/tui/util.py` & `nomenklatura-3.9.3/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura/util.py` & `nomenklatura-3.9.3/nomenklatura/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
 
 @lru_cache(maxsize=1024)
 def metaphone_token(token: str) -> str:
     if token.isalpha() and len(token) > 1:
         out = metaphone(token)
         # doesn't handle non-ascii characters
-        if len(out):
+        if len(out) >= 3:
             return out
     return token.upper()
 
 
 @lru_cache(maxsize=1024)
 def soundex_token(token: str) -> str:
     if token.isalpha() and len(token) > 1:
```

### Comparing `nomenklatura-3.9.2/nomenklatura/xref.py` & `nomenklatura-3.9.3/nomenklatura/xref.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.9.2/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-3.9.3/nomenklatura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.9.2
+Version: 3.9.3
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Description-Content-Type: text/markdown
```

### Comparing `nomenklatura-3.9.2/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-3.9.3/nomenklatura.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 nomenklatura/cache.py
 nomenklatura/cli.py
 nomenklatura/db.py
 nomenklatura/entity.py
 nomenklatura/exceptions.py
 nomenklatura/judgement.py
 nomenklatura/py.typed
-nomenklatura/senzing.py
 nomenklatura/settings.py
 nomenklatura/stream.py
 nomenklatura/util.py
 nomenklatura/xref.py
 nomenklatura.egg-info/PKG-INFO
 nomenklatura.egg-info/SOURCES.txt
 nomenklatura.egg-info/dependency_links.txt
```

### Comparing `nomenklatura-3.9.2/setup.py` & `nomenklatura-3.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="3.9.2",
+    version="3.9.3",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
```

