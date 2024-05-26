# Comparing `tmp/apconfig-0.0.109.tar.gz` & `tmp/apconfig-0.0.110.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apconfig-0.0.109.tar", max compression
+gzip compressed data, was "apconfig-0.0.110.tar", max compression
```

## Comparing `apconfig-0.0.109.tar` & `apconfig-0.0.110.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-03-27 10:34:40.761324 apconfig-0.0.109/README.md
--rw-r--r--   0        0        0     3246 2024-05-03 13:24:17.094363 apconfig-0.0.109/apconfig/__init__.py
--rw-r--r--   0        0        0      114 2024-04-05 10:57:51.982200 apconfig-0.0.109/apconfig/utilities.py
--rw-r--r--   0        0        0      305 2024-05-03 13:24:23.726411 apconfig-0.0.109/pyproject.toml
--rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 apconfig-0.0.109/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-27 10:34:40.761324 apconfig-0.0.110/README.md
+-rw-r--r--   0        0        0     3347 2024-05-26 14:37:38.549625 apconfig-0.0.110/apconfig/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-05 10:57:51.982200 apconfig-0.0.110/apconfig/utilities.py
+-rw-r--r--   0        0        0      305 2024-05-26 14:37:38.537625 apconfig-0.0.110/pyproject.toml
+-rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 apconfig-0.0.110/PKG-INFO
```

### Comparing `apconfig-0.0.109/apconfig/__init__.py` & `apconfig-0.0.110/apconfig/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,17 @@
     'trades': tso_trades_streamer_endpoint
 }
 
 tso_utility_topics = [topic for topic in setup_data["algorithms"]["tso"]["utility_topics"]]
 print(tso_utility_topics)
 
 # voting_round_symbol_data_endpoint = setup_data["algorithms"]["data"]["voting_round_symbol_data"]["url"]
+chain_gateway_endpoint = setup_data["algorithms"]["data-connectors"]["flare-chain-gateway"]["url"]
+
+
 
 
 # CHAIN VOTING ROUNDS
 algorithm_prepared_data_buffer = 17
 ml_predictions_buffer = 12
 submission_commit_buffer = 7
```

