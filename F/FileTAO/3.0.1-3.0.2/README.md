# Comparing `tmp/FileTAO-3.0.1.tar.gz` & `tmp/FileTAO-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FileTAO-3.0.1.tar", last modified: Wed May 22 22:44:25 2024, max compression
+gzip compressed data, was "FileTAO-3.0.2.tar", last modified: Sun May 26 16:34:40 2024, max compression
```

## Comparing `FileTAO-3.0.1.tar` & `FileTAO-3.0.2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.412089 FileTAO-3.0.1/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.412089 FileTAO-3.0.1/FileTAO.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    67421 2024-05-22 22:44:25.000000 FileTAO-3.0.1/FileTAO.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2099 2024-05-22 22:44:25.000000 FileTAO-3.0.1/FileTAO.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 22:44:25.000000 FileTAO-3.0.1/FileTAO.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       52 2024-05-22 22:44:25.000000 FileTAO-3.0.1/FileTAO.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      379 2024-05-22 22:44:25.000000 FileTAO-3.0.1/FileTAO.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-05-22 22:44:25.000000 FileTAO-3.0.1/FileTAO.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1069 2024-03-31 17:54:51.000000 FileTAO-3.0.1/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    67421 2024-05-22 22:44:25.412089 FileTAO-3.0.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    65567 2024-05-22 14:48:44.000000 FileTAO-3.0.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.404089 FileTAO-3.0.1/neurons/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.1/neurons/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22328 2024-05-22 16:09:56.000000 FileTAO-3.0.1/neurons/api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45035 2024-05-22 15:11:25.000000 FileTAO-3.0.1/neurons/miner.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16973 2024-05-15 15:46:07.000000 FileTAO-3.0.1/neurons/validator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 22:44:25.412089 FileTAO-3.0.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3962 2024-05-15 15:46:07.000000 FileTAO-3.0.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.404089 FileTAO-3.0.1/storage/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2364 2024-05-22 15:11:25.000000 FileTAO-3.0.1/storage/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.404089 FileTAO-3.0.1/storage/api/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      179 2024-05-22 14:46:38.000000 FileTAO-3.0.1/storage/api/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3431 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/api/base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4975 2024-05-22 14:50:05.000000 FileTAO-3.0.1/storage/api/delete_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2552 2024-05-22 14:46:38.000000 FileTAO-3.0.1/storage/api/example.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5923 2024-05-22 15:12:18.000000 FileTAO-3.0.1/storage/api/retrieve_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6841 2024-05-22 14:50:25.000000 FileTAO-3.0.1/storage/api/store_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3991 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/api/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.404089 FileTAO-3.0.1/storage/cli/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1199 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/cli/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8728 2024-05-22 14:46:38.000000 FileTAO-3.0.1/storage/cli/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1602 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/cli/default_values.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6742 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/cli/listcommand.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2274 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/cli/neuroncommand.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9067 2024-05-22 14:46:38.000000 FileTAO-3.0.1/storage/cli/retrievecommand.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4711 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/cli/statscommand.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9471 2024-05-22 14:46:38.000000 FileTAO-3.0.1/storage/cli/storecommand.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2136 2024-05-22 16:09:56.000000 FileTAO-3.0.1/storage/constants.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.408089 FileTAO-3.0.1/storage/indexer/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8064 2024-05-22 15:03:32.000000 FileTAO-3.0.1/storage/indexer/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8056 2024-05-22 16:36:13.000000 FileTAO-3.0.1/storage/indexer/endpoint.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10255 2024-05-22 14:58:41.000000 FileTAO-3.0.1/storage/indexer/redis.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/indexer/sqlite.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.408089 FileTAO-3.0.1/storage/miner/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1240 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/miner/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10763 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/miner/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15278 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/miner/database.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4204 2024-05-22 14:46:38.000000 FileTAO-3.0.1/storage/miner/run.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4619 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/miner/set_weights.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14477 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/miner/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.408089 FileTAO-3.0.1/storage/plot/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/plot/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6672 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/plot/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7921 2024-05-22 16:09:56.000000 FileTAO-3.0.1/storage/protocol.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.408089 FileTAO-3.0.1/storage/shared/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1200 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/shared/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5413 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/shared/checks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7290 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/shared/ecc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17746 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/shared/merkle.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      923 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/shared/subtensor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7992 2024-05-22 14:53:20.000000 FileTAO-3.0.1/storage/shared/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3436 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/shared/weights.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.408089 FileTAO-3.0.1/storage/validator/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1514 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14756 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/bonding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10538 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/challenge.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5864 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/validator/cid.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12139 2024-05-22 14:46:38.000000 FileTAO-3.0.1/storage/validator/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43538 2024-05-22 15:13:14.000000 FileTAO-3.0.1/storage/validator/database.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3113 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/dendrite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3211 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/validator/distribute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15435 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/validator/encryption.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3046 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/validator/event.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6223 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/validator/forward.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9417 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/network.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5072 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/validator/rebalance.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16215 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/retrieve.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12356 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/reward.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8798 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/validator/state.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23047 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/store.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32272 2024-05-22 14:46:38.000000 FileTAO-3.0.1/storage/validator/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8315 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/validator/verify.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6961 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/weights.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.408089 FileTAO-3.0.1/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.408089 FileTAO-3.0.1/tests/integration/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/integration/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.408089 FileTAO-3.0.1/tests/unit/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/unit/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.412089 FileTAO-3.0.1/tests/unit/cli/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/unit/cli/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      407 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/unit/cli/test_cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      442 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/unit/cli/test_neuroncommand.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.412089 FileTAO-3.0.1/tests/unit/validator/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/unit/validator/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      863 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/unit/validator/test_challenge.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1529 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/unit/validator/test_encryption.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1118 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/unit/validator/test_state.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-26 16:34:40.098850 FileTAO-3.0.2/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-26 16:34:40.094850 FileTAO-3.0.2/FileTAO.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    67421 2024-05-26 16:34:40.000000 FileTAO-3.0.2/FileTAO.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2099 2024-05-26 16:34:40.000000 FileTAO-3.0.2/FileTAO.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-26 16:34:40.000000 FileTAO-3.0.2/FileTAO.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       52 2024-05-26 16:34:40.000000 FileTAO-3.0.2/FileTAO.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      379 2024-05-26 16:34:40.000000 FileTAO-3.0.2/FileTAO.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-05-26 16:34:40.000000 FileTAO-3.0.2/FileTAO.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1069 2024-03-31 17:54:51.000000 FileTAO-3.0.2/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    67421 2024-05-26 16:34:40.094850 FileTAO-3.0.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    65567 2024-05-22 14:48:44.000000 FileTAO-3.0.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-26 16:34:40.090850 FileTAO-3.0.2/neurons/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.2/neurons/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22328 2024-05-26 16:14:38.000000 FileTAO-3.0.2/neurons/api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45035 2024-05-26 16:14:38.000000 FileTAO-3.0.2/neurons/miner.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16973 2024-05-15 15:46:07.000000 FileTAO-3.0.2/neurons/validator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-26 16:34:40.098850 FileTAO-3.0.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3962 2024-05-15 15:46:07.000000 FileTAO-3.0.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-26 16:34:40.090850 FileTAO-3.0.2/storage/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2364 2024-05-26 16:29:01.000000 FileTAO-3.0.2/storage/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-26 16:34:40.090850 FileTAO-3.0.2/storage/api/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      179 2024-05-22 14:46:38.000000 FileTAO-3.0.2/storage/api/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3431 2024-05-15 15:46:07.000000 FileTAO-3.0.2/storage/api/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4975 2024-05-22 14:50:05.000000 FileTAO-3.0.2/storage/api/delete_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2552 2024-05-22 14:46:38.000000 FileTAO-3.0.2/storage/api/example.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5923 2024-05-22 15:12:18.000000 FileTAO-3.0.2/storage/api/retrieve_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6841 2024-05-22 14:50:25.000000 FileTAO-3.0.2/storage/api/store_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3991 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/api/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-26 16:34:40.090850 FileTAO-3.0.2/storage/cli/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1199 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/cli/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8728 2024-05-22 14:46:38.000000 FileTAO-3.0.2/storage/cli/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1602 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/cli/default_values.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6742 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/cli/listcommand.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2274 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/cli/neuroncommand.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9067 2024-05-22 14:46:38.000000 FileTAO-3.0.2/storage/cli/retrievecommand.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4711 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/cli/statscommand.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9471 2024-05-22 14:46:38.000000 FileTAO-3.0.2/storage/cli/storecommand.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2136 2024-05-22 16:09:56.000000 FileTAO-3.0.2/storage/constants.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-26 16:34:40.090850 FileTAO-3.0.2/storage/indexer/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8064 2024-05-22 15:03:32.000000 FileTAO-3.0.2/storage/indexer/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8056 2024-05-26 16:14:38.000000 FileTAO-3.0.2/storage/indexer/endpoint.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10255 2024-05-22 14:58:41.000000 FileTAO-3.0.2/storage/indexer/redis.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2024-05-15 15:46:07.000000 FileTAO-3.0.2/storage/indexer/sqlite.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-26 16:34:40.090850 FileTAO-3.0.2/storage/miner/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1240 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/miner/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10763 2024-05-15 15:46:07.000000 FileTAO-3.0.2/storage/miner/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15278 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/miner/database.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4204 2024-05-22 14:46:38.000000 FileTAO-3.0.2/storage/miner/run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4619 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/miner/set_weights.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14477 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/miner/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-26 16:34:40.090850 FileTAO-3.0.2/storage/plot/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/plot/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6672 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/plot/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7921 2024-05-22 16:09:56.000000 FileTAO-3.0.2/storage/protocol.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-26 16:34:40.090850 FileTAO-3.0.2/storage/shared/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1200 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/shared/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5413 2024-05-15 15:46:07.000000 FileTAO-3.0.2/storage/shared/checks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7290 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/shared/ecc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17746 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/shared/merkle.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      923 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/shared/subtensor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7992 2024-05-22 14:53:20.000000 FileTAO-3.0.2/storage/shared/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3436 2024-05-15 15:46:07.000000 FileTAO-3.0.2/storage/shared/weights.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-26 16:34:40.094850 FileTAO-3.0.2/storage/validator/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1514 2024-05-15 15:46:07.000000 FileTAO-3.0.2/storage/validator/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14756 2024-05-15 15:46:07.000000 FileTAO-3.0.2/storage/validator/bonding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10538 2024-05-15 15:46:07.000000 FileTAO-3.0.2/storage/validator/challenge.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5864 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/validator/cid.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12139 2024-05-22 14:46:38.000000 FileTAO-3.0.2/storage/validator/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43538 2024-05-22 15:13:14.000000 FileTAO-3.0.2/storage/validator/database.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3113 2024-05-15 15:46:07.000000 FileTAO-3.0.2/storage/validator/dendrite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3211 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/validator/distribute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15435 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/validator/encryption.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3046 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/validator/event.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6223 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/validator/forward.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9417 2024-05-15 15:46:07.000000 FileTAO-3.0.2/storage/validator/network.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5072 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/validator/rebalance.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16215 2024-05-15 15:46:07.000000 FileTAO-3.0.2/storage/validator/retrieve.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12356 2024-05-15 15:46:07.000000 FileTAO-3.0.2/storage/validator/reward.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8798 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/validator/state.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23047 2024-05-15 15:46:07.000000 FileTAO-3.0.2/storage/validator/store.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32329 2024-05-26 16:14:44.000000 FileTAO-3.0.2/storage/validator/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8315 2024-03-31 17:54:51.000000 FileTAO-3.0.2/storage/validator/verify.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6961 2024-05-15 15:46:07.000000 FileTAO-3.0.2/storage/validator/weights.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-26 16:34:40.094850 FileTAO-3.0.2/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.2/tests/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-26 16:34:40.094850 FileTAO-3.0.2/tests/integration/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.2/tests/integration/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-26 16:34:40.094850 FileTAO-3.0.2/tests/unit/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.2/tests/unit/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-26 16:34:40.094850 FileTAO-3.0.2/tests/unit/cli/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.2/tests/unit/cli/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      407 2024-03-31 17:54:51.000000 FileTAO-3.0.2/tests/unit/cli/test_cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      442 2024-03-31 17:54:51.000000 FileTAO-3.0.2/tests/unit/cli/test_neuroncommand.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-26 16:34:40.094850 FileTAO-3.0.2/tests/unit/validator/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.2/tests/unit/validator/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      863 2024-03-31 17:54:51.000000 FileTAO-3.0.2/tests/unit/validator/test_challenge.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1529 2024-03-31 17:54:51.000000 FileTAO-3.0.2/tests/unit/validator/test_encryption.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1118 2024-03-31 17:54:51.000000 FileTAO-3.0.2/tests/unit/validator/test_state.py
```

### Comparing `FileTAO-3.0.1/FileTAO.egg-info/PKG-INFO` & `FileTAO-3.0.2/FileTAO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FileTAO
-Version: 3.0.1
+Version: 3.0.2
 Summary: Philanthropic storage for the masses. (FileTAO)
 Home-page: https://github.com/ifrit98/storage-subnet
 Author: philanthrope
 Author-email: ifrit98@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `FileTAO-3.0.1/FileTAO.egg-info/SOURCES.txt` & `FileTAO-3.0.2/FileTAO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/LICENSE` & `FileTAO-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/PKG-INFO` & `FileTAO-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FileTAO
-Version: 3.0.1
+Version: 3.0.2
 Summary: Philanthropic storage for the masses. (FileTAO)
 Home-page: https://github.com/ifrit98/storage-subnet
 Author: philanthrope
 Author-email: ifrit98@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `FileTAO-3.0.1/README.md` & `FileTAO-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/neurons/api.py` & `FileTAO-3.0.2/neurons/api.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/neurons/miner.py` & `FileTAO-3.0.2/neurons/miner.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/neurons/validator.py` & `FileTAO-3.0.2/neurons/validator.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/setup.py` & `FileTAO-3.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/__init__.py` & `FileTAO-3.0.2/storage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         return (self.major, self.minor, self.patch) < (
             other.major,
             other.minor,
             other.patch,
         )
 
 
-__version__ = "3.0.1"
+__version__ = "3.0.2"
 version = StorageVersion.from_string(__version__)
 __spec_version__ = version.to_spec_version()
 
 # Import all submodules.
 from . import protocol
 from . import validator
 from . import miner
```

### Comparing `FileTAO-3.0.1/storage/api/base.py` & `FileTAO-3.0.2/storage/api/base.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/api/delete_api.py` & `FileTAO-3.0.2/storage/api/delete_api.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/api/example.py` & `FileTAO-3.0.2/storage/api/example.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/api/retrieve_api.py` & `FileTAO-3.0.2/storage/api/retrieve_api.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/api/store_api.py` & `FileTAO-3.0.2/storage/api/store_api.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/api/utils.py` & `FileTAO-3.0.2/storage/api/utils.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/cli/__init__.py` & `FileTAO-3.0.2/storage/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/cli/cli.py` & `FileTAO-3.0.2/storage/cli/cli.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/cli/default_values.py` & `FileTAO-3.0.2/storage/cli/default_values.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/cli/listcommand.py` & `FileTAO-3.0.2/storage/cli/listcommand.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/cli/neuroncommand.py` & `FileTAO-3.0.2/storage/cli/neuroncommand.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/cli/retrievecommand.py` & `FileTAO-3.0.2/storage/cli/retrievecommand.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/cli/statscommand.py` & `FileTAO-3.0.2/storage/cli/statscommand.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/cli/storecommand.py` & `FileTAO-3.0.2/storage/cli/storecommand.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/constants.py` & `FileTAO-3.0.2/storage/constants.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/indexer/__init__.py` & `FileTAO-3.0.2/storage/indexer/__init__.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/indexer/endpoint.py` & `FileTAO-3.0.2/storage/indexer/endpoint.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/indexer/redis.py` & `FileTAO-3.0.2/storage/indexer/redis.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/indexer/sqlite.py` & `FileTAO-3.0.2/storage/indexer/sqlite.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/miner/__init__.py` & `FileTAO-3.0.2/storage/miner/__init__.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/miner/config.py` & `FileTAO-3.0.2/storage/miner/config.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/miner/database.py` & `FileTAO-3.0.2/storage/miner/database.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/miner/run.py` & `FileTAO-3.0.2/storage/miner/run.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/miner/set_weights.py` & `FileTAO-3.0.2/storage/miner/set_weights.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/miner/utils.py` & `FileTAO-3.0.2/storage/miner/utils.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/plot/utils.py` & `FileTAO-3.0.2/storage/plot/utils.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/protocol.py` & `FileTAO-3.0.2/storage/protocol.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/shared/__init__.py` & `FileTAO-3.0.2/storage/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/shared/checks.py` & `FileTAO-3.0.2/storage/shared/checks.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/shared/ecc.py` & `FileTAO-3.0.2/storage/shared/ecc.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/shared/merkle.py` & `FileTAO-3.0.2/storage/shared/merkle.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/shared/subtensor.py` & `FileTAO-3.0.2/storage/shared/subtensor.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/shared/utils.py` & `FileTAO-3.0.2/storage/shared/utils.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/shared/weights.py` & `FileTAO-3.0.2/storage/shared/weights.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/__init__.py` & `FileTAO-3.0.2/storage/validator/__init__.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/bonding.py` & `FileTAO-3.0.2/storage/validator/bonding.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/challenge.py` & `FileTAO-3.0.2/storage/validator/challenge.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/cid.py` & `FileTAO-3.0.2/storage/validator/cid.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/config.py` & `FileTAO-3.0.2/storage/validator/config.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/database.py` & `FileTAO-3.0.2/storage/validator/database.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/dendrite.py` & `FileTAO-3.0.2/storage/validator/dendrite.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/distribute.py` & `FileTAO-3.0.2/storage/validator/distribute.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/encryption.py` & `FileTAO-3.0.2/storage/validator/encryption.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/event.py` & `FileTAO-3.0.2/storage/validator/event.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/forward.py` & `FileTAO-3.0.2/storage/validator/forward.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/network.py` & `FileTAO-3.0.2/storage/validator/network.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/rebalance.py` & `FileTAO-3.0.2/storage/validator/rebalance.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/retrieve.py` & `FileTAO-3.0.2/storage/validator/retrieve.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/reward.py` & `FileTAO-3.0.2/storage/validator/reward.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/state.py` & `FileTAO-3.0.2/storage/validator/state.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/store.py` & `FileTAO-3.0.2/storage/validator/store.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/utils.py` & `FileTAO-3.0.2/storage/validator/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,21 +128,21 @@
     Args:
         metagraph (:obj: bt.metagraph.Metagraph): Metagraph object
         uid (int): uid to be checked
         vpermit_tao_limit (int): Validator permit tao limit
     Returns:
         bool: True if uid is available, False otherwise
     """
-    # Filter non serving axons.
-    if not metagraph.axons[uid].is_serving:
-        return False
     # Filter validator permit > 1024 stake.
     if metagraph.validator_permit[uid]:
         if metagraph.S[uid] > vpermit_tao_limit:
             return False
+    # Disallow non-serving miner axons by letting them fail early. (Excludes validators)
+    if metagraph.axons[uid].ip == '0.0.0.0':
+        return True
     # Available otherwise.
     return True
 
 
 def ttl_cache(maxsize=128, ttl=10):
     """A simple TTL cache decorator for functions with a single argument."""
```

### Comparing `FileTAO-3.0.1/storage/validator/verify.py` & `FileTAO-3.0.2/storage/validator/verify.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/storage/validator/weights.py` & `FileTAO-3.0.2/storage/validator/weights.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/tests/unit/validator/test_challenge.py` & `FileTAO-3.0.2/tests/unit/validator/test_challenge.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/tests/unit/validator/test_encryption.py` & `FileTAO-3.0.2/tests/unit/validator/test_encryption.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.1/tests/unit/validator/test_state.py` & `FileTAO-3.0.2/tests/unit/validator/test_state.py`

 * *Files identical despite different names*

