# Comparing `tmp/syft-0.8.7b7.tar.gz` & `tmp/syft-0.8.7b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.7b7.tar", last modified: Sun Apr 28 12:46:39 2024, max compression
+gzip compressed data, was "syft-0.8.7b8.tar", last modified: Sun May 26 12:36:35 2024, max compression
```

## Comparing `syft-0.8.7b7.tar` & `syft-0.8.7b8.tar`

### file list

```diff
@@ -1,309 +1,335 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.481117 syft-0.8.7b7/
--rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-04-28 12:43:27.000000 syft-0.8.7b7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-28 12:43:27.000000 syft-0.8.7b7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-28 12:46:39.481117 syft-0.8.7b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18678 2024-04-28 12:44:27.000000 syft-0.8.7b7/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (127)    17508 2024-04-28 12:43:27.000000 syft-0.8.7b7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-28 12:43:27.000000 syft-0.8.7b7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-28 12:46:39.485117 syft-0.8.7b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-28 12:43:27.000000 syft-0.8.7b7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.417117 syft-0.8.7b7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.425117 syft-0.8.7b7/src/syft/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-28 12:43:57.000000 syft-0.8.7b7/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-28 12:43:57.000000 syft-0.8.7b7/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.425117 syft-0.8.7b7/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.429117 syft-0.8.7b7/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42850 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    37060 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18538 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/client/domain_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/client/enclave_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/client/gateway_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/client/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    16329 2024-04-28 12:45:36.000000 syft-0.8.7b7/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/client/sync_decision.py
--rw-r--r--   0 runner    (1001) docker     (127)    19869 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/client/syncing.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.433117 syft-0.8.7b7/src/syft/custom_worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/custom_worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/custom_worker/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/custom_worker/builder_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13899 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/custom_worker/builder_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/custom_worker/builder_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/custom_worker/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/custom_worker/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/custom_worker/runner_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/custom_worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.433117 syft-0.8.7b7/src/syft/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/exceptions/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/exceptions/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/gevent_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.433117 syft-0.8.7b7/src/syft/img/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/img/base64.py
--rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/img/small-grid-symbol-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.433117 syft-0.8.7b7/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/node/enclave.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    63362 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/node/worker_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.433117 syft-0.8.7b7/src/syft/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)    24797 2024-04-28 12:45:36.000000 syft-0.8.7b7/src/syft/protocol/data_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/protocol/protocol_version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.437117 syft-0.8.7b7/src/syft/protocol/releases/
--rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/protocol/releases/0.8.2.json
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/protocol/releases/0.8.3.json
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/protocol/releases/0.8.4.json
--rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/protocol/releases/0.8.6.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.437117 syft-0.8.7b7/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/serde/lib_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/serde/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/serde/third_party.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/serde/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.441117 syft-0.8.7b7/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.441117 syft-0.8.7b7/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/action/action_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/action/action_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    74432 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    39167 2024-04-28 12:45:36.000000 syft-0.8.7b7/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/action/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.445117 syft-0.8.7b7/src/syft/service/api/
--rw-r--r--   0 runner    (1001) docker     (127)    23496 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20772 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/api/api_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/api/api_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.445117 syft-0.8.7b7/src/syft/service/blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/blob_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/blob_storage/remote_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/blob_storage/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/blob_storage/stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.445117 syft-0.8.7b7/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/code/status_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    56556 2024-04-28 12:45:36.000000 syft-0.8.7b7/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    25576 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/code/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.445117 syft-0.8.7b7/src/syft/service/code_history/
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/code_history/code_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/code_history/code_history_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/code_history/code_history_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.449117 syft-0.8.7b7/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.449117 syft-0.8.7b7/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28880 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.449117 syft-0.8.7b7/src/syft/service/enclave/
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/enclave/enclave_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.449117 syft-0.8.7b7/src/syft/service/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/job/html_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/job/job_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    32209 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/job/job_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.449117 syft-0.8.7b7/src/syft/service/log/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/log/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/log/log_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/log/log_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.453117 syft-0.8.7b7/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/metadata/metadata_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/metadata/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.453117 syft-0.8.7b7/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/network/association_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    29706 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/network/network_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/network/node_peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/network/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.453117 syft-0.8.7b7/src/syft/service/notification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14281 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/notification/email_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/notification/notification_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/notification/notification_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/notification/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.453117 syft-0.8.7b7/src/syft/service/notifier/
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/notifier/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/notifier/notifier_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/notifier/notifier_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/notifier/notifier_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/notifier/smtp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.453117 syft-0.8.7b7/src/syft/service/object_search/
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/object_search/migration_state_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/object_search/object_migration_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.453117 syft-0.8.7b7/src/syft/service/output/
--rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/output/output_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.457117 syft-0.8.7b7/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27131 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.457117 syft-0.8.7b7/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49644 2024-04-28 12:45:36.000000 syft-0.8.7b7/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    15758 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.457117 syft-0.8.7b7/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/queue/base_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11540 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/queue/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/queue/queue_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.457117 syft-0.8.7b7/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50592 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16887 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.461117 syft-0.8.7b7/src/syft/service/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/settings/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/settings/settings_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.461117 syft-0.8.7b7/src/syft/service/sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53412 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/sync/diff_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/sync/resolve_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    13943 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/sync/sync_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/sync/sync_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/sync/sync_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.461117 syft-0.8.7b7/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    21117 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/user/user_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.465117 syft-0.8.7b7/src/syft/service/worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/worker/image_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/worker/image_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/worker/image_registry_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/worker/image_registry_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    22317 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/worker/worker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/worker/worker_image_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/worker/worker_image_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/worker/worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/worker/worker_pool_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/worker/worker_pool_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/worker/worker_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/service/worker/worker_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/stable_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.469117 syft-0.8.7b7/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.469117 syft-0.8.7b7/src/syft/store/blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/store/blob_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/store/blob_storage/on_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/store/blob_storage/seaweedfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    26587 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-04-28 12:45:36.000000 syft-0.8.7b7/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)    37008 2024-04-28 12:45:36.000000 syft-0.8.7b7/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-04-28 12:45:36.000000 syft-0.8.7b7/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.473117 syft-0.8.7b7/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11929 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/types/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/types/cache_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/types/dicttuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/types/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/types/syft_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)    37820 2024-04-28 12:45:36.000000 syft-0.8.7b7/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/types/syncable_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.477117 syft-0.8.7b7/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/_std_stream_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.477117 syft-0.8.7b7/src/syft/util/notebook_ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/notebook_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.477117 syft-0.8.7b7/src/syft/util/notebook_ui/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/notebook_ui/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/notebook_ui/components/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/notebook_ui/components/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    34946 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/notebook_ui/notebook_addons.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-28 12:43:27.000000 syft-0.8.7b7/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:46:39.477117 syft-0.8.7b7/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-28 12:46:39.000000 syft-0.8.7b7/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-04-28 12:46:39.000000 syft-0.8.7b7/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:46:39.000000 syft-0.8.7b7/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-28 12:46:39.000000 syft-0.8.7b7/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:43:58.000000 syft-0.8.7b7/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-28 12:46:39.000000 syft-0.8.7b7/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-28 12:46:39.000000 syft-0.8.7b7/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.151306 syft-0.8.7b8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-05-26 12:33:03.000000 syft-0.8.7b8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-26 12:33:03.000000 syft-0.8.7b8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22510 2024-05-26 12:36:35.151306 syft-0.8.7b8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18142 2024-05-26 12:34:23.000000 syft-0.8.7b8/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16925 2024-05-26 12:33:03.000000 syft-0.8.7b8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-26 12:33:03.000000 syft-0.8.7b8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-26 12:36:35.151306 syft-0.8.7b8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-26 12:33:03.000000 syft-0.8.7b8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.087306 syft-0.8.7b8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.095306 syft-0.8.7b8/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-26 12:33:57.000000 syft-0.8.7b8/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-05-26 12:33:57.000000 syft-0.8.7b8/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.087306 syft-0.8.7b8/src/syft/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.095306 syft-0.8.7b8/src/syft/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/css/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/css/itables.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)    41577 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/css/tabulator_pysyft.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.095306 syft-0.8.7b8/src/syft/assets/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/img/small-grid-symbol-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.095306 syft-0.8.7b8/src/syft/assets/jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/jinja/table.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.095306 syft-0.8.7b8/src/syft/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/js/table.js
+-rw-r--r--   0 runner    (1001) docker     (127)   437328 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/js/tabulator.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.099306 syft-0.8.7b8/src/syft/assets/svg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/svg/arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/svg/clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/svg/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/svg/folder.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/svg/info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/svg/request.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/svg/search.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/svg/table.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.099306 syft-0.8.7b8/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.103306 syft-0.8.7b8/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47324 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37620 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18267 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/domain_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8089 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/enclave_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/gateway_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/sync_decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/syncing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.103306 syft-0.8.7b8/src/syft/custom_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/builder_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13899 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/builder_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/builder_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/runner_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.107306 syft-0.8.7b8/src/syft/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/exceptions/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.107306 syft-0.8.7b8/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/enclave.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65150 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/worker_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/orchestra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.107306 syft-0.8.7b8/src/syft/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)    24797 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/protocol/data_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/protocol/protocol_version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.107306 syft-0.8.7b8/src/syft/protocol/releases/
+-rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/protocol/releases/0.8.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/protocol/releases/0.8.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/protocol/releases/0.8.4.json
+-rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/protocol/releases/0.8.6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.111306 syft-0.8.7b8/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/third_party.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.111306 syft-0.8.7b8/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.115306 syft-0.8.7b8/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/action_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/action_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74426 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39167 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.115306 syft-0.8.7b8/src/syft/service/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    24157 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20850 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/api/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/api/api_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.115306 syft-0.8.7b8/src/syft/service/attestation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/attestation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/attestation/attestation_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/attestation/attestation_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.115306 syft-0.8.7b8/src/syft/service/blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/blob_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/blob_storage/remote_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/blob_storage/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/blob_storage/stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.119306 syft-0.8.7b8/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code/status_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57343 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26547 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.119306 syft-0.8.7b8/src/syft/service/code_history/
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code_history/code_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code_history/code_history_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code_history/code_history_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.119306 syft-0.8.7b8/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.119306 syft-0.8.7b8/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27907 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.119306 syft-0.8.7b8/src/syft/service/enclave/
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/enclave/enclave_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.119306 syft-0.8.7b8/src/syft/service/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/job/html_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/job/job_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31391 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/job/job_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.123306 syft-0.8.7b8/src/syft/service/log/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/log/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/log/log_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/log/log_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.123306 syft-0.8.7b8/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/metadata/metadata_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/metadata/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.123306 syft-0.8.7b8/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/network/association_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38178 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/network/network_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/network/node_peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/network/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/network/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.123306 syft-0.8.7b8/src/syft/service/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14281 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notification/email_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notification/notification_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notification/notification_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notification/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.123306 syft-0.8.7b8/src/syft/service/notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notifier/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notifier/notifier_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notifier/notifier_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notifier/notifier_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notifier/smtp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.127306 syft-0.8.7b8/src/syft/service/object_search/
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/object_search/migration_state_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/object_search/object_migration_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.127306 syft-0.8.7b8/src/syft/service/output/
+-rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/output/output_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.127306 syft-0.8.7b8/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28215 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.127306 syft-0.8.7b8/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49945 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15758 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.127306 syft-0.8.7b8/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/queue/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/queue/queue_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34509 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.131306 syft-0.8.7b8/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50857 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16870 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.131306 syft-0.8.7b8/src/syft/service/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/settings/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.131306 syft-0.8.7b8/src/syft/service/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58990 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/sync/diff_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/sync/resolve_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13943 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/sync/sync_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/sync/sync_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/sync/sync_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.131306 syft-0.8.7b8/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21714 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/user/user_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.135306 syft-0.8.7b8/src/syft/service/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/image_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/image_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/image_registry_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/image_registry_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21379 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker_image_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker_image_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9763 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker_pool_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker_pool_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/stable_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.139306 syft-0.8.7b8/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.139306 syft-0.8.7b8/src/syft/store/blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/blob_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/blob_storage/on_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/blob_storage/seaweedfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26625 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36893 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.143306 syft-0.8.7b8/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11929 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/cache_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/dicttuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/syft_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30658 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/syncable_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.143306 syft-0.8.7b8/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/_std_stream_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.147306 syft-0.8.7b8/src/syft/util/notebook_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/notebook_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.147306 syft-0.8.7b8/src/syft/util/notebook_ui/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/notebook_ui/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/notebook_ui/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/notebook_ui/components/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17871 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/notebook_ui/components/table_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/notebook_ui/components/tabulator_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/notebook_ui/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/notebook_ui/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24653 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.147306 syft-0.8.7b8/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22510 2024-05-26 12:36:35.000000 syft-0.8.7b8/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-05-26 12:36:35.000000 syft-0.8.7b8/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 12:36:35.000000 syft-0.8.7b8/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-26 12:36:35.000000 syft-0.8.7b8/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 12:33:58.000000 syft-0.8.7b8/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-26 12:36:35.000000 syft-0.8.7b8/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-26 12:36:35.000000 syft-0.8.7b8/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.7b7/LICENSE` & `syft-0.8.7b8/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/PKG-INFO` & `syft-0.8.7b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.7b7
+Version: 0.8.7b8
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -14,15 +14,14 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
 Requires-Dist: setuptools
 Requires-Dist: bcrypt==4.1.2
 Requires-Dist: boto3==1.34.56
 Requires-Dist: forbiddenfruit==0.1.4
-Requires-Dist: gevent==23.9.1
 Requires-Dist: loguru==0.7.2
 Requires-Dist: networkx==3.2.1
 Requires-Dist: packaging>=23.0
 Requires-Dist: pyarrow==15.0.0
 Requires-Dist: pycapnp==2.0.0b2
 Requires-Dist: pydantic[email]==2.6.0
 Requires-Dist: pydantic-settings==2.2.1
@@ -35,35 +34,34 @@
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: typeguard==4.1.5
 Requires-Dist: typing_extensions==4.10.0
 Requires-Dist: sherlock[filelock]==0.4.1
 Requires-Dist: uvicorn[standard]==0.27.1
 Requires-Dist: fastapi==0.110.0
 Requires-Dist: psutil==5.9.8
-Requires-Dist: hagrid>=0.3
 Requires-Dist: itables==1.7.1
 Requires-Dist: argon2-cffi==23.1.0
 Requires-Dist: matplotlib==3.8.3
-Requires-Dist: jaxlib==0.4.20
-Requires-Dist: jax==0.4.20
 Requires-Dist: numpy<=1.24.4,>=1.23.5; python_version < "3.12"
 Requires-Dist: numpy<1.27,>=1.26.4; python_version >= "3.12"
 Requires-Dist: pandas==2.2.1
 Requires-Dist: docker==6.1.3
 Requires-Dist: kr8s==0.13.5
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: azure-storage-blob==12.19.1
 Requires-Dist: ipywidgets==8.1.2
+Requires-Dist: rich==13.7.1
+Requires-Dist: jinja2==3.1.4
+Requires-Dist: tenacity==8.3.0
 Provides-Extra: data-science
 Requires-Dist: transformers==4.39.3; extra == "data-science"
 Requires-Dist: opendp==0.9.2; extra == "data-science"
 Requires-Dist: evaluate==0.4.1; extra == "data-science"
 Requires-Dist: recordlinkage==0.16; extra == "data-science"
-Requires-Dist: dm-haiku==0.0.10; extra == "data-science"
-Requires-Dist: torch[cpu]==2.2.1; extra == "data-science"
+Requires-Dist: torch==2.3.0; extra == "data-science"
 Provides-Extra: dev
 Requires-Dist: pytest<8; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-xdist[psutil]; extra == "dev"
 Requires-Dist: pytest-parallel; extra == "dev"
 Requires-Dist: pytest-randomly; extra == "dev"
 Requires-Dist: pytest-sugar; extra == "dev"
@@ -108,62 +106,74 @@
 
 <img alt="Syft Logo" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/title_syft_light.png" width="200px" />
 
 Perform data science on `data` that remains in `someone else's` server
 
 # Quickstart
 
-✅ `Linux` ✅ `macOS` ✅ `Windows` ✅ `Docker` ✅ `Podman` ✅ `Kubernetes`
+✅ `Linux` ✅ `macOS` ✅ `Windows` ✅ `Docker` ✅ `Kubernetes`
 
 ## Install Client
 
 ```bash
 $ pip install -U syft[data_science]
 ```
 
 ## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
 sy.requires(">=0.8.6,<0.8.7")
-node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
+node = sy.orchestra.launch(
+    name="my-domain",
+    port=8080,
+    create_producer=True,
+    n_consumers=1,
+    dev_mode=True,
+    reset=True, # resets database
+)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Launch Client
 
 ```python
 import syft as sy
 sy.requires(">=0.8.6,<0.8.7")
-domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
+domain_client = sy.login(
+    port=8080,
+    email="info@openmined.org",
+    password="changethis"
+)
 ```
 
 ## PySyft in 10 minutes
 
 📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api">API Example Notebooks</a>
 
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/04-pytorch-example.ipynb">04-pytorch-example.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/08-code-version.ipynb">08-code-version.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/09-blob-storage.ipynb">09-blob-storage.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/10-container-images.ipynb">10-container-images.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/11-container-images-k8s.ipynb">11-container-images-k8s.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/12-custom-api-endpoint.ipynb">12-custom-api-endpoint.ipynb</a>
 
 ## Deploy Kubernetes Helm Chart
 
 **Note**: Assuming we have a Kubernetes cluster already setup.
 
 #### 1. Add and update Helm repo for Syft
 
@@ -200,44 +210,35 @@
 
 For AWS EKS
 
 ```sh
 helm install ... --set ingress.className="alb"
 ```
 
-For Google GKE we need the [`gce` annotation](https://cloud.google.com/kubernetes-engine/docs/how-to/load-balance-ingress#create-ingress) annotation.
+For Google GKE we need the [`gce` annotation](https://cloud.google.com/kubernetes-engine/docs/how-to/load-balance-ingress#create-ingress).
 
 ```sh
 helm install ... --set ingress.class="gce"
 ```
 
-## Deploy to a Container Engine or Cloud
+## Note:
 
-1. Install our handy 🛵 cli tool which makes deploying a Domain or Gateway server to Docker or VM a one-liner:  
-   `pip install -U hagrid`
+🚨 Our old deployment tool `HAGrid` has been `deprecated`. For the updated deployment options kindly refer to:
 
-2. Then run our interactive jupyter Install 🧙🏽‍♂️ Wizard<sup>BETA</sup>:  
-   `hagrid quickstart`
-
-3. In the tutorial you will learn how to install and deploy:  
-   `PySyft` = our `numpy`-like 🐍 Python library for computing on `private data` in someone else's `Domain`
-
-   `PyGrid` = our 🐳 `docker` / 🐧 `vm` `Domain` & `Gateway` Servers where `private data` lives
+- 📚 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/tutorials/deployments">Deployments</a>
 
 ## Docs and Support
 
 - 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
 - `#support` on <a href="https://slack.openmined.org/">Slack</a>
 
 # Install Notes
 
-- HAGrid 0.3 Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
-- Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
-- PySyft 0.8.1 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
-- PyGrid Requires: 🐳 `docker`, 🦦 `podman` or ☸️ `kubernetes` - Run: `hagrid launch ...`
+- PySyft 0.8.6 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
+- PyGrid Requires: 🐳 `docker` or ☸️ `kubernetes`
 
 # Versions
 
 `0.9.0` - Coming soon...  
 `0.8.7` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
 `0.8.6` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8">API</a>
 
@@ -252,21 +253,17 @@
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
 - `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
 - `0.2.0` - `0.5.0`
 
 PySyft and PyGrid use the same `version` and its best to match them up where possible. We release weekly betas which can be used in each context:
 
-PySyft (Stable): `pip install -U syft`  
-PyGrid (Stable) `hagrid launch ... tag=latest`
-
-PySyft (Beta): `pip install -U syft --pre`  
-PyGrid (Beta): `hagrid launch ... tag=beta`
+PySyft (Stable): `pip install -U syft`
 
-HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually the best.
+PySyft (Beta): `pip install -U syft --pre`
 
 # What is Syft?
 
 <img align="right" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
 
 `Syft` is OpenMined's `open source` stack that provides `secure` and `private` Data Science in Python. Syft decouples `private data` from model training, using techniques like [Federated Learning](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and integration with `Deep Learning` frameworks, so that you as a `Data Scientist` can maintain your current workflow while using these new `privacy-enhancing techniques`.
```

### Comparing `syft-0.8.7b7/PYPI.md` & `syft-0.8.7b8/PYPI.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,62 +3,74 @@
 
 <img alt="Syft Logo" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/title_syft_light.png" width="200px" />
 
 Perform data science on `data` that remains in `someone else's` server
 
 # Quickstart
 
-✅ `Linux` ✅ `macOS` ✅ `Windows` ✅ `Docker` ✅ `Podman` ✅ `Kubernetes`
+✅ `Linux` ✅ `macOS` ✅ `Windows` ✅ `Docker` ✅ `Kubernetes`
 
 ## Install Client
 
 ```bash
 $ pip install -U syft[data_science]
 ```
 
 ## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
 sy.requires(">=0.8.6,<0.8.7")
-node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
+node = sy.orchestra.launch(
+    name="my-domain",
+    port=8080,
+    create_producer=True,
+    n_consumers=1,
+    dev_mode=True,
+    reset=True, # resets database
+)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Launch Client
 
 ```python
 import syft as sy
 sy.requires(">=0.8.6,<0.8.7")
-domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
+domain_client = sy.login(
+    port=8080,
+    email="info@openmined.org",
+    password="changethis"
+)
 ```
 
 ## PySyft in 10 minutes
 
 📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api">API Example Notebooks</a>
 
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/04-pytorch-example.ipynb">04-pytorch-example.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/08-code-version.ipynb">08-code-version.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/09-blob-storage.ipynb">09-blob-storage.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/10-container-images.ipynb">10-container-images.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/11-container-images-k8s.ipynb">11-container-images-k8s.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/12-custom-api-endpoint.ipynb">12-custom-api-endpoint.ipynb</a>
 
 ## Deploy Kubernetes Helm Chart
 
 **Note**: Assuming we have a Kubernetes cluster already setup.
 
 #### 1. Add and update Helm repo for Syft
 
@@ -95,44 +107,35 @@
 
 For AWS EKS
 
 ```sh
 helm install ... --set ingress.className="alb"
 ```
 
-For Google GKE we need the [`gce` annotation](https://cloud.google.com/kubernetes-engine/docs/how-to/load-balance-ingress#create-ingress) annotation.
+For Google GKE we need the [`gce` annotation](https://cloud.google.com/kubernetes-engine/docs/how-to/load-balance-ingress#create-ingress).
 
 ```sh
 helm install ... --set ingress.class="gce"
 ```
 
-## Deploy to a Container Engine or Cloud
+## Note:
 
-1. Install our handy 🛵 cli tool which makes deploying a Domain or Gateway server to Docker or VM a one-liner:  
-   `pip install -U hagrid`
+🚨 Our old deployment tool `HAGrid` has been `deprecated`. For the updated deployment options kindly refer to:
 
-2. Then run our interactive jupyter Install 🧙🏽‍♂️ Wizard<sup>BETA</sup>:  
-   `hagrid quickstart`
-
-3. In the tutorial you will learn how to install and deploy:  
-   `PySyft` = our `numpy`-like 🐍 Python library for computing on `private data` in someone else's `Domain`
-
-   `PyGrid` = our 🐳 `docker` / 🐧 `vm` `Domain` & `Gateway` Servers where `private data` lives
+- 📚 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/tutorials/deployments">Deployments</a>
 
 ## Docs and Support
 
 - 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
 - `#support` on <a href="https://slack.openmined.org/">Slack</a>
 
 # Install Notes
 
-- HAGrid 0.3 Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
-- Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
-- PySyft 0.8.1 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
-- PyGrid Requires: 🐳 `docker`, 🦦 `podman` or ☸️ `kubernetes` - Run: `hagrid launch ...`
+- PySyft 0.8.6 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
+- PyGrid Requires: 🐳 `docker` or ☸️ `kubernetes`
 
 # Versions
 
 `0.9.0` - Coming soon...  
 `0.8.7` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
 `0.8.6` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8">API</a>
 
@@ -147,21 +150,17 @@
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
 - `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
 - `0.2.0` - `0.5.0`
 
 PySyft and PyGrid use the same `version` and its best to match them up where possible. We release weekly betas which can be used in each context:
 
-PySyft (Stable): `pip install -U syft`  
-PyGrid (Stable) `hagrid launch ... tag=latest`
-
-PySyft (Beta): `pip install -U syft --pre`  
-PyGrid (Beta): `hagrid launch ... tag=beta`
+PySyft (Stable): `pip install -U syft`
 
-HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually the best.
+PySyft (Beta): `pip install -U syft --pre`
 
 # What is Syft?
 
 <img align="right" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
 
 `Syft` is OpenMined's `open source` stack that provides `secure` and `private` Data Science in Python. Syft decouples `private data` from model training, using techniques like [Federated Learning](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and integration with `Deep Learning` frameworks, so that you as a `Data Scientist` can maintain your current workflow while using these new `privacy-enhancing techniques`.
```

#### html2text {}

```diff
@@ -2,84 +2,74 @@
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_d_o_c_k_e_r_-_i_m_a_g_e_s_-_b_l_u_e_?_l_o_g_o_=_d_o_c_k_e_r_]_[_h_t_t_p_s_:_/_/
 _g_i_t_h_u_b_._c_o_m_/_O_p_e_n_M_i_n_e_d_/_P_y_S_y_f_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_n_i_g_h_t_l_i_e_s_._y_m_l_/
 _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_d_e_v_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_h_a_t_-_o_n_%_2_0_s_l_a_c_k_-
 _p_u_r_p_l_e_?_l_o_g_o_=_s_l_a_c_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_m_d_b_o_o_k_]
 
 [Syft Logo]Perform data science on `data` that remains in `someone else's`
 server # Quickstart â `Linux` â `macOS` â `Windows` â `Docker` â
-`Podman` â `Kubernetes` ## Install Client ```bash $ pip install -U syft
-[data_science] ``` ## Launch Server ```python # from Jupyter / Python import
-syft as sy sy.requires(">=0.8.6,<0.8.7") node = sy.orchestra.launch(name="my-
-domain", port=8080, dev_mode=True, reset=True) ``` ```bash # or from the
-command line $ syft launch --name=my-domain --port=8080 --reset=True Starting
-syft-node server on 0.0.0.0:8080 ``` ## Launch Client ```python import syft as
-sy sy.requires(">=0.8.6,<0.8.7") domain_client = sy.login(port=8080,
-email="info@openmined.org", password="changethis") ``` ## PySyft in 10 minutes
+`Kubernetes` ## Install Client ```bash $ pip install -U syft[data_science] ```
+## Launch Server ```python # from Jupyter / Python import syft as sy
+sy.requires(">=0.8.6,<0.8.7") node = sy.orchestra.launch( name="my-domain",
+port=8080, create_producer=True, n_consumers=1, dev_mode=True, reset=True, #
+resets database ) ``` ```bash # or from the command line $ syft launch --
+name=my-domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:
+8080 ``` ## Launch Client ```python import syft as sy sy.requires
+(">=0.8.6,<0.8.7") domain_client = sy.login( port=8080,
+email="info@openmined.org", password="changethis" ) ``` ## PySyft in 10 minutes
 ð _A_P_I_ _E_x_a_m_p_l_e_ _N_o_t_e_b_o_o_k_s - _0_0_-_l_o_a_d_-_d_a_t_a_._i_p_y_n_b - _0_1_-_s_u_b_m_i_t_-_c_o_d_e_._i_p_y_n_b - _0_2_-
 _r_e_v_i_e_w_-_c_o_d_e_-_a_n_d_-_a_p_p_r_o_v_e_._i_p_y_n_b - _0_3_-_d_a_t_a_-_s_c_i_e_n_t_i_s_t_-_d_o_w_n_l_o_a_d_-_r_e_s_u_l_t_._i_p_y_n_b - _0_4_-
-_j_a_x_-_e_x_a_m_p_l_e_._i_p_y_n_b - _0_5_-_c_u_s_t_o_m_-_p_o_l_i_c_y_._i_p_y_n_b - _0_6_-_m_u_l_t_i_p_l_e_-_c_o_d_e_-_r_e_q_u_e_s_t_s_._i_p_y_n_b -
-_0_7_-_d_o_m_a_i_n_-_r_e_g_i_s_t_e_r_-_c_o_n_t_r_o_l_-_f_l_o_w_._i_p_y_n_b - _0_8_-_c_o_d_e_-_v_e_r_s_i_o_n_._i_p_y_n_b - _0_9_-_b_l_o_b_-
-_s_t_o_r_a_g_e_._i_p_y_n_b - _1_0_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_._i_p_y_n_b - _1_1_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_-_k_8_s_._i_p_y_n_b ##
-Deploy Kubernetes Helm Chart **Note**: Assuming we have a Kubernetes cluster
-already setup. #### 1. Add and update Helm repo for Syft ```sh helm repo add
-openmined https://openmined.github.io/PySyft/helm helm repo update openmined
-``` #### 2. Search for available Syft versions ```sh helm search repo
-openmined/syft --versions --devel ``` #### 3. Set your preferred Syft Chart
-version ```sh SYFT_VERSION="" ``` #### 4. Provisioning Helm Charts ```sh helm
-install my-domain openmined/syft --version $SYFT_VERSION --namespace syft --
-create-namespace --set ingress.className="traefik" ``` ### Ingress Controllers
-For Azure AKS ```sh helm install ... --set ingress.className="azure-
-application-gateway" ``` For AWS EKS ```sh helm install ... --set
-ingress.className="alb" ``` For Google GKE we need the [`gce` annotation]
-(https://cloud.google.com/kubernetes-engine/docs/how-to/load-balance-
-ingress#create-ingress) annotation. ```sh helm install ... --set
-ingress.class="gce" ``` ## Deploy to a Container Engine or Cloud 1. Install our
-handy ðµ cli tool which makes deploying a Domain or Gateway server to Docker
-or VM a one-liner: `pip install -U hagrid` 2. Then run our interactive jupyter
-Install ð§ð½ââï¸ WizardBETA: `hagrid quickstart` 3. In the tutorial
-you will learn how to install and deploy: `PySyft` = our `numpy`-like ð
-Python library for computing on `private data` in someone else's `Domain`
-`PyGrid` = our ð³ `docker` / ð§ `vm` `Domain` & `Gateway` Servers where
-`private data` lives ## Docs and Support - ð _D_o_c_s - `#support` on _S_l_a_c_k #
-Install Notes - HAGrid 0.3 Requires: ð `python` ð `git` - Run: `pip
-install -U hagrid` - Interactive Install ð§ð½ââï¸ WizardBETA Requires
-ðµ `hagrid`: - Run: `hagrid quickstart` - PySyft 0.8.1 Requires: ð `python
-3.10 - 3.12` - Run: `pip install -U syft` - PyGrid Requires: ð³ `docker`,
-ð¦¦ `podman` or â¸ï¸ `kubernetes` - Run: `hagrid launch ...` # Versions
+_p_y_t_o_r_c_h_-_e_x_a_m_p_l_e_._i_p_y_n_b - _0_5_-_c_u_s_t_o_m_-_p_o_l_i_c_y_._i_p_y_n_b - _0_6_-_m_u_l_t_i_p_l_e_-_c_o_d_e_-
+_r_e_q_u_e_s_t_s_._i_p_y_n_b - _0_7_-_d_o_m_a_i_n_-_r_e_g_i_s_t_e_r_-_c_o_n_t_r_o_l_-_f_l_o_w_._i_p_y_n_b - _0_8_-_c_o_d_e_-_v_e_r_s_i_o_n_._i_p_y_n_b
+- _0_9_-_b_l_o_b_-_s_t_o_r_a_g_e_._i_p_y_n_b - _1_0_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_._i_p_y_n_b - _1_1_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_-
+_k_8_s_._i_p_y_n_b - _1_2_-_c_u_s_t_o_m_-_a_p_i_-_e_n_d_p_o_i_n_t_._i_p_y_n_b ## Deploy Kubernetes Helm Chart
+**Note**: Assuming we have a Kubernetes cluster already setup. #### 1. Add and
+update Helm repo for Syft ```sh helm repo add openmined https://
+openmined.github.io/PySyft/helm helm repo update openmined ``` #### 2. Search
+for available Syft versions ```sh helm search repo openmined/syft --versions --
+devel ``` #### 3. Set your preferred Syft Chart version ```sh SYFT_VERSION=""
+``` #### 4. Provisioning Helm Charts ```sh helm install my-domain openmined/
+syft --version $SYFT_VERSION --namespace syft --create-namespace --set
+ingress.className="traefik" ``` ### Ingress Controllers For Azure AKS ```sh
+helm install ... --set ingress.className="azure-application-gateway" ``` For
+AWS EKS ```sh helm install ... --set ingress.className="alb" ``` For Google GKE
+we need the [`gce` annotation](https://cloud.google.com/kubernetes-engine/docs/
+how-to/load-balance-ingress#create-ingress). ```sh helm install ... --set
+ingress.class="gce" ``` ## Note: ð¨ Our old deployment tool `HAGrid` has been
+`deprecated`. For the updated deployment options kindly refer to: - ð
+_D_e_p_l_o_y_m_e_n_t_s ## Docs and Support - ð _D_o_c_s - `#support` on _S_l_a_c_k # Install
+Notes - PySyft 0.8.6 Requires: ð `python 3.10 - 3.12` - Run: `pip install -
+U syft` - PyGrid Requires: ð³ `docker` or â¸ï¸ `kubernetes` # Versions
 `0.9.0` - Coming soon... `0.8.7` (Beta) - `dev` branch ðð½ _A_P_I - Coming
 soon... `0.8.6` (Stable) - _A_P_I Deprecated: - `0.8.5-post.2` - _A_P_I - `0.8.4` -
 _A_P_I - `0.8.3` - _A_P_I - `0.8.2` - _A_P_I - `0.8.1` - _A_P_I - `0.8.0` - _A_P_I - `0.7.0` -
 _C_o_u_r_s_e_ _3_ _U_p_d_a_t_e_d - `0.6.0` - _C_o_u_r_s_e_ _3 - `0.5.1` - _C_o_u_r_s_e_ _2 + M1 Hotfix -
 `0.2.0` - `0.5.0` PySyft and PyGrid use the same `version` and its best to
 match them up where possible. We release weekly betas which can be used in each
-context: PySyft (Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch
-... tag=latest` PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta):
-`hagrid launch ... tag=beta` HAGrid is a cli / deployment tool so the latest
-version of `hagrid` is usually the best. # What is Syft? [Syft]`Syft` is
-OpenMined's `open source` stack that provides `secure` and `private` Data
-Science in Python. Syft decouples `private data` from model training, using
-techniques like [Federated Learning](https://ai.googleblog.com/2017/04/
-federated-learning-collaborative.html), [Differential Privacy](https://
-en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https:
-//en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-
-like interface and integration with `Deep Learning` frameworks, so that you as
-a `Data Scientist` can maintain your current workflow while using these new
-`privacy-enhancing techniques`. ### Why should I use Syft? `Syft` allows a
-`Data Scientist` to ask `questions` about a `dataset` and, within `privacy
-limits` set by the `data owner`, get `answers` to those `questions`, all
-without obtaining a `copy` of the data itself. We call this process `Remote
-Data Science`. It means in a wide variety of `domains` across society, the
-current `risks` of sharing information (`copying` data) with someone such as,
-privacy invasion, IP theft and blackmail will no longer prevent the vast
-`benefits` such as innovation, insights and scientific discovery which secure
-access will provide. No more cold calls to get `access` to a dataset. No more
-weeks of `wait times` to get a `result` on your `query`. It also means `1000x
-more data` in every domain. PySyft opens the doors to a streamlined Data
-Scientist `workflow`, all with the individual's `privacy` at its heart. #
-Terminology
+context: PySyft (Stable): `pip install -U syft` PySyft (Beta): `pip install -
+U syft --pre` # What is Syft? [Syft]`Syft` is OpenMined's `open source` stack
+that provides `secure` and `private` Data Science in Python. Syft decouples
+`private data` from model training, using techniques like [Federated Learning]
+(https://ai.googleblog.com/2017/04/federated-learning-collaborative.html),
+[Differential Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and
+[Encrypted Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption).
+This is done with a `numpy`-like interface and integration with `Deep Learning`
+frameworks, so that you as a `Data Scientist` can maintain your current
+workflow while using these new `privacy-enhancing techniques`. ### Why should I
+use Syft? `Syft` allows a `Data Scientist` to ask `questions` about a `dataset`
+and, within `privacy limits` set by the `data owner`, get `answers` to those
+`questions`, all without obtaining a `copy` of the data itself. We call this
+process `Remote Data Science`. It means in a wide variety of `domains` across
+society, the current `risks` of sharing information (`copying` data) with
+someone such as, privacy invasion, IP theft and blackmail will no longer
+prevent the vast `benefits` such as innovation, insights and scientific
+discovery which secure access will provide. No more cold calls to get `access`
+to a dataset. No more weeks of `wait times` to get a `result` on your `query`.
+It also means `1000x more data` in every domain. PySyft opens the doors to a
+streamlined Data Scientist `workflow`, all with the individual's `privacy` at
+its heart. # Terminology
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |                  [[IImmaaggee]]             |                 [[IImmaaggee]]              |
 |_ _ _ _ _ _ _ _ _?ð_?_?_?¨_?ð_?_?_?»_?â_?_?_?ð_?_?_?¼_ _DD_aa_tt_aa_ _OO_ww_nn_ee_rr_ss_ _ _ _|_ _ _ _ _ _?ð_?_?_?©_?ð_?_?_?½_?â_?_?_?ð_?_?_?¬_ _DD_aa_tt_aa_ _SS_cc_ii_ee_nn_tt_ii_ss_tt_ss_ _ |
 |Provide `datasets` which they would   |Are end `users` who desire to perform |
 |like to make available for `study` by |`computations` or `answer` a specific |
 |an `outside party` they may or may not|`question` using one or more data     |
 |_`_f_u_l_l_y_ _t_r_u_s_t_`_ _h_a_s_ _g_o_o_d_ _i_n_t_e_n_t_i_o_n_s_._ _ _ _ _|_o_w_n_e_r_s_'_ _`_d_a_t_a_s_e_t_s_`_._ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
```

### Comparing `syft-0.8.7b7/README.md` & `syft-0.8.7b8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,62 +6,74 @@
   <img alt="Syft Logo" src="docs/img/title_syft_light.png" width="200px" />
 </picture>
 
 Perform data science on `data` that remains in `someone else's` server
 
 # Quickstart
 
-✅ `Linux` ✅ `macOS` ✅ `Windows` ✅ `Docker` ✅ `Podman` ✅ `Kubernetes`
+✅ `Linux` ✅ `macOS` ✅ `Windows` ✅ `Docker` ✅ `Kubernetes`
 
 ## Install Client
 
 ```bash
 $ pip install -U syft[data_science]
 ```
 
 ## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
 sy.requires(">=0.8.6,<0.8.7")
-node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
+node = sy.orchestra.launch(
+    name="my-domain",
+    port=8080,
+    create_producer=True,
+    n_consumers=1,
+    dev_mode=True,
+    reset=True, # resets database
+)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Launch Client
 
 ```python
 import syft as sy
 sy.requires(">=0.8.6,<0.8.7")
-domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
+domain_client = sy.login(
+    port=8080,
+    email="info@openmined.org",
+    password="changethis"
+)
 ```
 
 ## PySyft in 10 minutes
 
 📝 <a href="notebooks/api">API Example Notebooks</a>
 
 - <a href="notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
 - <a href="notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
 - <a href="notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
 - <a href="notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
-- <a href="notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
+- <a href="notebooks/api/0.8/04-pytorch-example.ipynb">04-pytorch-example.ipynb</a>
 - <a href="notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
 - <a href="notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
 - <a href="notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
 - <a href="notebooks/api/0.8/08-code-version.ipynb">08-code-version.ipynb</a>
 - <a href="notebooks/api/0.8/09-blob-storage.ipynb">09-blob-storage.ipynb</a>
 - <a href="notebooks/api/0.8/10-container-images.ipynb">10-container-images.ipynb</a>
 - <a href="notebooks/api/0.8/11-container-images-k8s.ipynb">11-container-images-k8s.ipynb</a>
+- <a href="notebooks/api/0.8/12-custom-api-endpoint.ipynb">12-custom-api-endpoint.ipynb</a>
 
 ## Deploy Kubernetes Helm Chart
 
 **Note**: Assuming we have a Kubernetes cluster already setup.
 
 #### 1. Add and update Helm repo for Syft
 
@@ -98,44 +110,35 @@
 
 For AWS EKS
 
 ```sh
 helm install ... --set ingress.className="alb"
 ```
 
-For Google GKE we need the [`gce` annotation](https://cloud.google.com/kubernetes-engine/docs/how-to/load-balance-ingress#create-ingress) annotation.
+For Google GKE we need the [`gce` annotation](https://cloud.google.com/kubernetes-engine/docs/how-to/load-balance-ingress#create-ingress).
 
 ```sh
 helm install ... --set ingress.class="gce"
 ```
 
-## Deploy to a Container Engine or Cloud
+## Note:
 
-1. Install our handy 🛵 cli tool which makes deploying a Domain or Gateway server to Docker or VM a one-liner:  
-   `pip install -U hagrid`
+🚨 Our old deployment tool `HAGrid` has been `deprecated`. For the updated deployment options kindly refer to:
 
-2. Then run our interactive jupyter Install 🧙🏽‍♂️ Wizard<sup>BETA</sup>:  
-   `hagrid quickstart`
-
-3. In the tutorial you will learn how to install and deploy:  
-   `PySyft` = our `numpy`-like 🐍 Python library for computing on `private data` in someone else's `Domain`
-
-   `PyGrid` = our 🐳 `docker` / 🐧 `vm` `Domain` & `Gateway` Servers where `private data` lives
+- 📚 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/tutorials/deployments">Deployments</a>
 
 ## Docs and Support
 
 - 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
 - `#support` on <a href="https://slack.openmined.org/">Slack</a>
 
 # Install Notes
 
-- HAGrid 0.3 Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
-- Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
-- PySyft 0.8.1 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
-- PyGrid Requires: 🐳 `docker`, 🦦 `podman` or ☸️ `kubernetes` - Run: `hagrid launch ...`
+- PySyft 0.8.6 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
+- PyGrid Requires: 🐳 `docker` or ☸️ `kubernetes`
 
 # Versions
 
 `0.9.0` - Coming soon...  
 `0.8.7` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
 `0.8.6` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8">API</a>
 
@@ -150,21 +153,17 @@
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
 - `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
 - `0.2.0` - `0.5.0`
 
 PySyft and PyGrid use the same `version` and its best to match them up where possible. We release weekly betas which can be used in each context:
 
-PySyft (Stable): `pip install -U syft`  
-PyGrid (Stable) `hagrid launch ... tag=latest`
-
-PySyft (Beta): `pip install -U syft --pre`  
-PyGrid (Beta): `hagrid launch ... tag=beta`
+PySyft (Stable): `pip install -U syft`
 
-HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually the best.
+PySyft (Beta): `pip install -U syft --pre`
 
 # What is Syft?
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_big_dark.png">
   <img align="right" src="docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
 </picture>
```

#### html2text {}

```diff
@@ -2,84 +2,74 @@
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_d_o_c_k_e_r_-_i_m_a_g_e_s_-_b_l_u_e_?_l_o_g_o_=_d_o_c_k_e_r_]_[_h_t_t_p_s_:_/_/
 _g_i_t_h_u_b_._c_o_m_/_O_p_e_n_M_i_n_e_d_/_P_y_S_y_f_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_n_i_g_h_t_l_i_e_s_._y_m_l_/
 _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_d_e_v_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_h_a_t_-_o_n_%_2_0_s_l_a_c_k_-
 _p_u_r_p_l_e_?_l_o_g_o_=_s_l_a_c_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_m_d_b_o_o_k_]
 
 [Syft Logo]Perform data science on `data` that remains in `someone else's`
 server # Quickstart â `Linux` â `macOS` â `Windows` â `Docker` â
-`Podman` â `Kubernetes` ## Install Client ```bash $ pip install -U syft
-[data_science] ``` ## Launch Server ```python # from Jupyter / Python import
-syft as sy sy.requires(">=0.8.6,<0.8.7") node = sy.orchestra.launch(name="my-
-domain", port=8080, dev_mode=True, reset=True) ``` ```bash # or from the
-command line $ syft launch --name=my-domain --port=8080 --reset=True Starting
-syft-node server on 0.0.0.0:8080 ``` ## Launch Client ```python import syft as
-sy sy.requires(">=0.8.6,<0.8.7") domain_client = sy.login(port=8080,
-email="info@openmined.org", password="changethis") ``` ## PySyft in 10 minutes
+`Kubernetes` ## Install Client ```bash $ pip install -U syft[data_science] ```
+## Launch Server ```python # from Jupyter / Python import syft as sy
+sy.requires(">=0.8.6,<0.8.7") node = sy.orchestra.launch( name="my-domain",
+port=8080, create_producer=True, n_consumers=1, dev_mode=True, reset=True, #
+resets database ) ``` ```bash # or from the command line $ syft launch --
+name=my-domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:
+8080 ``` ## Launch Client ```python import syft as sy sy.requires
+(">=0.8.6,<0.8.7") domain_client = sy.login( port=8080,
+email="info@openmined.org", password="changethis" ) ``` ## PySyft in 10 minutes
 ð _A_P_I_ _E_x_a_m_p_l_e_ _N_o_t_e_b_o_o_k_s - _0_0_-_l_o_a_d_-_d_a_t_a_._i_p_y_n_b - _0_1_-_s_u_b_m_i_t_-_c_o_d_e_._i_p_y_n_b - _0_2_-
 _r_e_v_i_e_w_-_c_o_d_e_-_a_n_d_-_a_p_p_r_o_v_e_._i_p_y_n_b - _0_3_-_d_a_t_a_-_s_c_i_e_n_t_i_s_t_-_d_o_w_n_l_o_a_d_-_r_e_s_u_l_t_._i_p_y_n_b - _0_4_-
-_j_a_x_-_e_x_a_m_p_l_e_._i_p_y_n_b - _0_5_-_c_u_s_t_o_m_-_p_o_l_i_c_y_._i_p_y_n_b - _0_6_-_m_u_l_t_i_p_l_e_-_c_o_d_e_-_r_e_q_u_e_s_t_s_._i_p_y_n_b -
-_0_7_-_d_o_m_a_i_n_-_r_e_g_i_s_t_e_r_-_c_o_n_t_r_o_l_-_f_l_o_w_._i_p_y_n_b - _0_8_-_c_o_d_e_-_v_e_r_s_i_o_n_._i_p_y_n_b - _0_9_-_b_l_o_b_-
-_s_t_o_r_a_g_e_._i_p_y_n_b - _1_0_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_._i_p_y_n_b - _1_1_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_-_k_8_s_._i_p_y_n_b ##
-Deploy Kubernetes Helm Chart **Note**: Assuming we have a Kubernetes cluster
-already setup. #### 1. Add and update Helm repo for Syft ```sh helm repo add
-openmined https://openmined.github.io/PySyft/helm helm repo update openmined
-``` #### 2. Search for available Syft versions ```sh helm search repo
-openmined/syft --versions --devel ``` #### 3. Set your preferred Syft Chart
-version ```sh SYFT_VERSION="" ``` #### 4. Provisioning Helm Charts ```sh helm
-install my-domain openmined/syft --version $SYFT_VERSION --namespace syft --
-create-namespace --set ingress.className="traefik" ``` ### Ingress Controllers
-For Azure AKS ```sh helm install ... --set ingress.className="azure-
-application-gateway" ``` For AWS EKS ```sh helm install ... --set
-ingress.className="alb" ``` For Google GKE we need the [`gce` annotation]
-(https://cloud.google.com/kubernetes-engine/docs/how-to/load-balance-
-ingress#create-ingress) annotation. ```sh helm install ... --set
-ingress.class="gce" ``` ## Deploy to a Container Engine or Cloud 1. Install our
-handy ðµ cli tool which makes deploying a Domain or Gateway server to Docker
-or VM a one-liner: `pip install -U hagrid` 2. Then run our interactive jupyter
-Install ð§ð½ââï¸ WizardBETA: `hagrid quickstart` 3. In the tutorial
-you will learn how to install and deploy: `PySyft` = our `numpy`-like ð
-Python library for computing on `private data` in someone else's `Domain`
-`PyGrid` = our ð³ `docker` / ð§ `vm` `Domain` & `Gateway` Servers where
-`private data` lives ## Docs and Support - ð _D_o_c_s - `#support` on _S_l_a_c_k #
-Install Notes - HAGrid 0.3 Requires: ð `python` ð `git` - Run: `pip
-install -U hagrid` - Interactive Install ð§ð½ââï¸ WizardBETA Requires
-ðµ `hagrid`: - Run: `hagrid quickstart` - PySyft 0.8.1 Requires: ð `python
-3.10 - 3.12` - Run: `pip install -U syft` - PyGrid Requires: ð³ `docker`,
-ð¦¦ `podman` or â¸ï¸ `kubernetes` - Run: `hagrid launch ...` # Versions
+_p_y_t_o_r_c_h_-_e_x_a_m_p_l_e_._i_p_y_n_b - _0_5_-_c_u_s_t_o_m_-_p_o_l_i_c_y_._i_p_y_n_b - _0_6_-_m_u_l_t_i_p_l_e_-_c_o_d_e_-
+_r_e_q_u_e_s_t_s_._i_p_y_n_b - _0_7_-_d_o_m_a_i_n_-_r_e_g_i_s_t_e_r_-_c_o_n_t_r_o_l_-_f_l_o_w_._i_p_y_n_b - _0_8_-_c_o_d_e_-_v_e_r_s_i_o_n_._i_p_y_n_b
+- _0_9_-_b_l_o_b_-_s_t_o_r_a_g_e_._i_p_y_n_b - _1_0_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_._i_p_y_n_b - _1_1_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_-
+_k_8_s_._i_p_y_n_b - _1_2_-_c_u_s_t_o_m_-_a_p_i_-_e_n_d_p_o_i_n_t_._i_p_y_n_b ## Deploy Kubernetes Helm Chart
+**Note**: Assuming we have a Kubernetes cluster already setup. #### 1. Add and
+update Helm repo for Syft ```sh helm repo add openmined https://
+openmined.github.io/PySyft/helm helm repo update openmined ``` #### 2. Search
+for available Syft versions ```sh helm search repo openmined/syft --versions --
+devel ``` #### 3. Set your preferred Syft Chart version ```sh SYFT_VERSION=""
+``` #### 4. Provisioning Helm Charts ```sh helm install my-domain openmined/
+syft --version $SYFT_VERSION --namespace syft --create-namespace --set
+ingress.className="traefik" ``` ### Ingress Controllers For Azure AKS ```sh
+helm install ... --set ingress.className="azure-application-gateway" ``` For
+AWS EKS ```sh helm install ... --set ingress.className="alb" ``` For Google GKE
+we need the [`gce` annotation](https://cloud.google.com/kubernetes-engine/docs/
+how-to/load-balance-ingress#create-ingress). ```sh helm install ... --set
+ingress.class="gce" ``` ## Note: ð¨ Our old deployment tool `HAGrid` has been
+`deprecated`. For the updated deployment options kindly refer to: - ð
+_D_e_p_l_o_y_m_e_n_t_s ## Docs and Support - ð _D_o_c_s - `#support` on _S_l_a_c_k # Install
+Notes - PySyft 0.8.6 Requires: ð `python 3.10 - 3.12` - Run: `pip install -
+U syft` - PyGrid Requires: ð³ `docker` or â¸ï¸ `kubernetes` # Versions
 `0.9.0` - Coming soon... `0.8.7` (Beta) - `dev` branch ðð½ _A_P_I - Coming
 soon... `0.8.6` (Stable) - _A_P_I Deprecated: - `0.8.5-post.2` - _A_P_I - `0.8.4` -
 _A_P_I - `0.8.3` - _A_P_I - `0.8.2` - _A_P_I - `0.8.1` - _A_P_I - `0.8.0` - _A_P_I - `0.7.0` -
 _C_o_u_r_s_e_ _3_ _U_p_d_a_t_e_d - `0.6.0` - _C_o_u_r_s_e_ _3 - `0.5.1` - _C_o_u_r_s_e_ _2 + M1 Hotfix -
 `0.2.0` - `0.5.0` PySyft and PyGrid use the same `version` and its best to
 match them up where possible. We release weekly betas which can be used in each
-context: PySyft (Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch
-... tag=latest` PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta):
-`hagrid launch ... tag=beta` HAGrid is a cli / deployment tool so the latest
-version of `hagrid` is usually the best. # What is Syft? [Syft]`Syft` is
-OpenMined's `open source` stack that provides `secure` and `private` Data
-Science in Python. Syft decouples `private data` from model training, using
-techniques like [Federated Learning](https://ai.googleblog.com/2017/04/
-federated-learning-collaborative.html), [Differential Privacy](https://
-en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https:
-//en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-
-like interface and integration with `Deep Learning` frameworks, so that you as
-a `Data Scientist` can maintain your current workflow while using these new
-`privacy-enhancing techniques`. ### Why should I use Syft? `Syft` allows a
-`Data Scientist` to ask `questions` about a `dataset` and, within `privacy
-limits` set by the `data owner`, get `answers` to those `questions`, all
-without obtaining a `copy` of the data itself. We call this process `Remote
-Data Science`. It means in a wide variety of `domains` across society, the
-current `risks` of sharing information (`copying` data) with someone such as,
-privacy invasion, IP theft and blackmail will no longer prevent the vast
-`benefits` such as innovation, insights and scientific discovery which secure
-access will provide. No more cold calls to get `access` to a dataset. No more
-weeks of `wait times` to get a `result` on your `query`. It also means `1000x
-more data` in every domain. PySyft opens the doors to a streamlined Data
-Scientist `workflow`, all with the individual's `privacy` at its heart. #
-Terminology
+context: PySyft (Stable): `pip install -U syft` PySyft (Beta): `pip install -
+U syft --pre` # What is Syft? [Syft]`Syft` is OpenMined's `open source` stack
+that provides `secure` and `private` Data Science in Python. Syft decouples
+`private data` from model training, using techniques like [Federated Learning]
+(https://ai.googleblog.com/2017/04/federated-learning-collaborative.html),
+[Differential Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and
+[Encrypted Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption).
+This is done with a `numpy`-like interface and integration with `Deep Learning`
+frameworks, so that you as a `Data Scientist` can maintain your current
+workflow while using these new `privacy-enhancing techniques`. ### Why should I
+use Syft? `Syft` allows a `Data Scientist` to ask `questions` about a `dataset`
+and, within `privacy limits` set by the `data owner`, get `answers` to those
+`questions`, all without obtaining a `copy` of the data itself. We call this
+process `Remote Data Science`. It means in a wide variety of `domains` across
+society, the current `risks` of sharing information (`copying` data) with
+someone such as, privacy invasion, IP theft and blackmail will no longer
+prevent the vast `benefits` such as innovation, insights and scientific
+discovery which secure access will provide. No more cold calls to get `access`
+to a dataset. No more weeks of `wait times` to get a `result` on your `query`.
+It also means `1000x more data` in every domain. PySyft opens the doors to a
+streamlined Data Scientist `workflow`, all with the individual's `privacy` at
+its heart. # Terminology
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |                  [[IImmaaggee]]             |                 [[IImmaaggee]]              |
 |_ _ _ _ _ _ _ _ _?ð_?_?_?¨_?ð_?_?_?»_?â_?_?_?ð_?_?_?¼_ _DD_aa_tt_aa_ _OO_ww_nn_ee_rr_ss_ _ _ _|_ _ _ _ _ _?ð_?_?_?©_?ð_?_?_?½_?â_?_?_?ð_?_?_?¬_ _DD_aa_tt_aa_ _SS_cc_ii_ee_nn_tt_ii_ss_tt_ss_ _ |
 |Provide `datasets` which they would   |Are end `users` who desire to perform |
 |like to make available for `study` by |`computations` or `answer` a specific |
 |an `outside party` they may or may not|`question` using one or more data     |
 |_`_f_u_l_l_y_ _t_r_u_s_t_`_ _h_a_s_ _g_o_o_d_ _i_n_t_e_n_t_i_o_n_s_._ _ _ _ _|_o_w_n_e_r_s_'_ _`_d_a_t_a_s_e_t_s_`_._ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
```

### Comparing `syft-0.8.7b7/setup.cfg` & `syft-0.8.7b8/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.7-beta.7"
+version = attr: "0.8.7-beta.8"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: PYPI.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
@@ -23,15 +23,14 @@
 package_dir = 
 	=src
 syft = 
 	setuptools
 	bcrypt==4.1.2
 	boto3==1.34.56
 	forbiddenfruit==0.1.4
-	gevent==23.9.1
 	loguru==0.7.2
 	networkx==3.2.1
 	packaging>=23.0
 	pyarrow==15.0.0
 	pycapnp==2.0.0b2
 	pydantic[email]==2.6.0
 	pydantic-settings==2.2.1
@@ -44,28 +43,28 @@
 	tqdm==4.66.2
 	typeguard==4.1.5
 	typing_extensions==4.10.0
 	sherlock[filelock]==0.4.1
 	uvicorn[standard]==0.27.1
 	fastapi==0.110.0
 	psutil==5.9.8
-	hagrid>=0.3
 	itables==1.7.1
 	argon2-cffi==23.1.0
 	matplotlib==3.8.3
-	jaxlib==0.4.20
-	jax==0.4.20
 	numpy>=1.23.5,<=1.24.4; python_version<"3.12"
 	numpy>=1.26.4,<1.27; python_version>="3.12"
 	pandas==2.2.1
 	docker==6.1.3
 	kr8s==0.13.5
 	PyYAML==6.0.1
 	azure-storage-blob==12.19.1
 	ipywidgets==8.1.2
+	rich==13.7.1
+	jinja2==3.1.4
+	tenacity==8.3.0
 install_requires = 
 	%(syft)s
 python_requires = >=3.10
 
 [options.packages.find]
 where = src
 exclude = 
@@ -73,16 +72,15 @@
 
 [options.extras_require]
 data_science = 
 	transformers==4.39.3
 	opendp==0.9.2
 	evaluate==0.4.1
 	recordlinkage==0.16
-	dm-haiku==0.0.10
-	torch[cpu]==2.2.1
+	torch==2.3.0
 dev = 
 	%(test_plugins)s
 	%(telemetry)s
 	bandit==1.7.7
 	ruff==0.3.0
 	importlib-metadata==6.8.0
 	isort==5.13.2
@@ -194,16 +192,14 @@
 package = syft
 extensions = 
 	markdown
 
 [files]
 packages = 
 	syft
-data_files = 
-	img = img/*
 
 [mypy]
 python_version = 3.12
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `syft-0.8.7b7/src/syft/VERSION` & `syft-0.8.7b8/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.7-beta.7"
+__version__ = "0.8.7-beta.8"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.7b7/src/syft/abstract_node.py` & `syft-0.8.7b8/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/client/api.py` & `syft-0.8.7b8/src/syft/client/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,32 +44,49 @@
 from ..service.service import UserLibConfigRegistry
 from ..service.service import UserServiceConfigRegistry
 from ..service.user.user_roles import ServiceRole
 from ..service.warnings import APIEndpointWarning
 from ..service.warnings import WarningContext
 from ..types.cache_object import CachedSyftObject
 from ..types.identity import Identity
+from ..types.syft_object import SYFT_OBJECT_VERSION_1
 from ..types.syft_object import SYFT_OBJECT_VERSION_2
 from ..types.syft_object import SyftBaseObject
 from ..types.syft_object import SyftMigrationRegistry
 from ..types.syft_object import SyftObject
 from ..types.uid import LineageID
 from ..types.uid import UID
 from ..util.autoreload import autoreload_enabled
 from ..util.markdown import as_markdown_python_code
+from ..util.table import list_dict_repr_html
 from ..util.telemetry import instrument
 from ..util.util import prompt_warning_message
 from .connection import NodeConnection
 
 if TYPE_CHECKING:
     # relative
     from ..node import Node
     from ..service.job.job_stash import Job
 
 
+IPYNB_BACKGROUND_METHODS = {
+    "getdoc",
+    "_partialmethod",
+    "__name__",
+    "__code__",
+    "__wrapped__",
+    "__custom_documentations__",
+    "__signature__",
+    "__defaults__",
+    "__kwdefaults__",
+}
+
+IPYNB_BACKGROUND_PREFIXES = ["_ipy", "_repr", "__ipython", "__pydantic"]
+
+
 class APIRegistry:
     __api_registry__: dict[tuple, SyftAPI] = OrderedDict()
 
     @classmethod
     def set_api_for(
         cls,
         node_uid: UID | str,
@@ -363,17 +380,21 @@
                 kwargs={},
             )
             endpoint = self.make_call(api_call=api_call)
             if isinstance(endpoint, SyftError):
                 return endpoint._repr_html_()
 
             str_repr = "## API: " + custom_path + "\n"
+            if endpoint.description is not None:
+                text = endpoint.description.text
+            else:
+                text = ""
             str_repr += (
                 "### Description: "
-                + f'<span style="font-weight: lighter;">{endpoint.description}</span><br>'
+                + f'<span style="font-weight: lighter;">{text}</span><br>'
                 + "\n"
             )
             str_repr += "#### Private Code:\n"
             not_accessible_code = "N / A"
             private_code_repr = endpoint.private_function or not_accessible_code
             public_code_repr = endpoint.mock_function or not_accessible_code
             str_repr += as_markdown_python_code(private_code_repr) + "\n"
@@ -577,47 +598,121 @@
         result = wrapper_make_call(api_call=api_call)
         return result
 
     wrapper.__ipython_inspector_signature_override__ = signature
     return wrapper
 
 
+class APISubModulesView(SyftObject):
+    __canonical_name__ = "APISubModulesView"
+    __version__ = SYFT_OBJECT_VERSION_1
+
+    submodule: str = ""
+    endpoints: list[str] = []
+
+    __syft_include_id_coll_repr__ = False
+
+    def _coll_repr_(self) -> dict[str, Any]:
+        return {"submodule": self.submodule, "endpoints": "\n".join(self.endpoints)}
+
+
 @serializable()
 class APIModule:
     _modules: list[str]
     path: str
+    refresh_callback: Callable | None
 
-    def __init__(self, path: str) -> None:
+    def __init__(self, path: str, refresh_callback: Callable | None) -> None:
         self._modules = []
         self.path = path
+        self.refresh_callback = refresh_callback
+
+    def __dir__(self) -> list[str]:
+        return self._modules + ["path"]
+
+    def has_submodule(self, name: str) -> bool:
+        """We use this as hasattr() triggers __getattribute__ which triggers recursion"""
+        try:
+            _ = object.__getattribute__(self, name)
+            return True
+        except AttributeError:
+            return False
 
     def _add_submodule(
         self, attr_name: str, module_or_func: Callable | APIModule
     ) -> None:
         setattr(self, attr_name, module_or_func)
         self._modules.append(attr_name)
 
-    def __getattribute__(self, name: str) -> Any:
+    def __getattr__(self, name: str) -> Any:
         try:
             return object.__getattribute__(self, name)
         except AttributeError:
+            # if we fail, we refresh the api and try again
+            # however, we dont want this to happen all the time because of ipy magic happening
+            # in the background
+            if (
+                self.refresh_callback is not None
+                and name not in IPYNB_BACKGROUND_METHODS
+                and not any(
+                    name.startswith(prefix) for prefix in IPYNB_BACKGROUND_PREFIXES
+                )
+            ):
+                api = self.refresh_callback()
+                try:
+                    # get current path in the module tree
+                    new_current_module = api.services
+                    for submodule in self.path.split("."):
+                        if submodule != "":
+                            new_current_module = getattr(new_current_module, submodule)
+                    # retry getting the attribute, if this fails, we throw an error
+                    return object.__getattribute__(new_current_module, name)
+                except AttributeError:
+                    pass
             raise SyftAttributeError(
                 f"'APIModule' api{self.path} object has no submodule or method '{name}', "
                 "you may not have permission to access the module you are trying to access."
                 "If you think this is an error, try calling `client.refresh()` to update the API."
             )
 
     def __getitem__(self, key: str | int) -> Any:
         if hasattr(self, "get_all"):
             return self.get_all()[key]
         raise NotImplementedError
 
     def _repr_html_(self) -> Any:
+        if self.path == "settings":
+            return self.get()._repr_html_()
+
         if not hasattr(self, "get_all"):
-            return NotImplementedError
+
+            def recursively_get_submodules(
+                module: APIModule | Callable,
+            ) -> list[APIModule | Callable]:
+                children = [module]
+                if isinstance(module, APIModule):
+                    for submodule_name in module._modules:
+                        submodule = getattr(module, submodule_name)
+                        children += recursively_get_submodules(submodule)
+                return children
+
+            views = []
+            for submodule_name in self._modules:
+                submodule = getattr(self, submodule_name)
+                children = recursively_get_submodules(submodule)
+                child_paths = [
+                    x.path for x in children if isinstance(x, RemoteFunction)
+                ]
+                views.append(
+                    APISubModulesView(submodule=submodule_name, endpoints=child_paths)
+                )
+
+            return list_dict_repr_html(views)
+            # return NotImplementedError
+
         results = self.get_all()
         return results._repr_html_()
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         return NotImplementedError
 
 
@@ -735,16 +830,34 @@
     libs: APIModule | None = None
     signing_key: SyftSigningKey | None = None
     # serde / storage rules
     refresh_api_callback: Callable | None = None
     __user_role: ServiceRole = ServiceRole.NONE
     communication_protocol: PROTOCOL_TYPE
 
-    # def __post_init__(self) -> None:
-    #     pass
+    # informs getattr does not have nasty side effects
+    __syft_allow_autocomplete__ = ["services"]
+
+    def __dir__(self) -> list[str]:
+        modules = getattr(self.api_module, "_modules", [])
+        return ["services"] + modules
+
+    def __syft_dir__(self) -> list[str]:
+        modules = getattr(self.api_module, "_modules", [])
+        return ["services"] + modules
+
+    def __getattr__(self, name: str) -> Any:
+        try:
+            return getattr(self.api_module, name)
+        except Exception:
+            raise SyftAttributeError(
+                f"'SyftAPI' object has no submodule or method '{name}', "
+                "you may not have permission to access the module you are trying to access."
+                "If you think this is an error, try calling `client.refresh()` to update the API."
+            )
 
     @staticmethod
     def for_user(
         node: AbstractNode,
         communication_protocol: PROTOCOL_TYPE,
         user_verify_key: SyftVerifyKey | None = None,
     ) -> SyftAPI:
@@ -911,37 +1024,43 @@
 
     def update_api(self, api_call_result: Any) -> None:
         # TODO: hacky stuff with typing and imports to prevent circular imports
         if result_needs_api_update(api_call_result):
             if self.refresh_api_callback is not None:
                 self.refresh_api_callback()
 
-    @staticmethod
     def _add_route(
-        api_module: APIModule, endpoint: APIEndpoint, endpoint_method: Callable
+        self, api_module: APIModule, endpoint: APIEndpoint, endpoint_method: Callable
     ) -> None:
         """Recursively create a module path to the route endpoint."""
 
         _modules = endpoint.module_path.split(".")[:-1] + [endpoint.name]
 
         _self = api_module
         _last_module = _modules.pop()
         while _modules:
             module = _modules.pop(0)
-            if not hasattr(_self, module):
-                submodule_path = f"{_self.path}.{module}"
-                _self._add_submodule(module, APIModule(path=submodule_path))
+            if not _self.has_submodule(module):
+                submodule_path = (
+                    f"{_self.path}.{module}" if _self.path != "" else module
+                )
+                _self._add_submodule(
+                    module,
+                    APIModule(
+                        path=submodule_path, refresh_callback=self.refresh_api_callback
+                    ),
+                )
             _self = getattr(_self, module)
         _self._add_submodule(_last_module, endpoint_method)
 
     def generate_endpoints(self) -> None:
         def build_endpoint_tree(
             endpoints: dict[str, LibEndpoint], communication_protocol: PROTOCOL_TYPE
         ) -> APIModule:
-            api_module = APIModule(path="")
+            api_module = APIModule(path="", refresh_callback=self.refresh_api_callback)
             for _, v in endpoints.items():
                 signature = v.signature
                 if not v.has_self:
                     signature = signature_remove_self(signature)
                 signature = signature_remove_context(signature)
                 if isinstance(v, APIEndpoint):
                     endpoint_function = generate_remote_function(
```

### Comparing `syft-0.8.7b7/src/syft/client/client.py` & `syft-0.8.7b8/src/syft/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # future
 from __future__ import annotations
 
 # stdlib
+import base64
 from collections.abc import Callable
 from copy import deepcopy
 from enum import Enum
 from getpass import getpass
 import json
-import os
 from typing import Any
 from typing import TYPE_CHECKING
 from typing import cast
 
 # third party
 from argon2 import PasswordHasher
 from pydantic import field_validator
@@ -106,14 +106,15 @@
     if credentials is None:
         # generate a random signing key
         credentials = SyftSigningKey.generate()
 
     signed_message: SignedSyftAPICall = call.sign(credentials=credentials)
     signed_result = make_call(signed_message)
     response = debox_signed_syftapicall_response(signed_result)
+
     return response
 
 
 API_PATH = "/api/v2"
 DEFAULT_PYGRID_PORT = 80
 DEFAULT_PYGRID_ADDRESS = f"http://localhost:{DEFAULT_PYGRID_PORT}"
 
@@ -121,14 +122,15 @@
 class Routes(Enum):
     ROUTE_METADATA = f"{API_PATH}/metadata"
     ROUTE_API = f"{API_PATH}/api"
     ROUTE_LOGIN = f"{API_PATH}/login"
     ROUTE_REGISTER = f"{API_PATH}/register"
     ROUTE_API_CALL = f"{API_PATH}/api_call"
     ROUTE_BLOB_STORE = "/blob"
+    STREAM = f"{API_PATH}/stream"
 
 
 @serializable(attrs=["proxy_target_uid", "url"])
 class HTTPConnection(NodeConnection):
     __canonical_name__ = "HTTPConnection"
     __version__ = SYFT_OBJECT_VERSION_2
 
@@ -145,14 +147,23 @@
             if isinstance(v, str | GridURL)
             else v
         )
 
     def with_proxy(self, proxy_target_uid: UID) -> Self:
         return HTTPConnection(url=self.url, proxy_target_uid=proxy_target_uid)
 
+    def stream_via(self, proxy_uid: UID, url_path: str) -> GridURL:
+        # Update the presigned url path to
+        # <gatewayurl>/<peer_uid>/<presigned_url>
+        # url_path_bytes = _serialize(url_path, to_bytes=True)
+
+        url_path_str = base64.urlsafe_b64encode(url_path.encode()).decode()
+        stream_url_path = f"{self.routes.STREAM.value}/{proxy_uid}/{url_path_str}/"
+        return self.url.with_path(stream_url_path)
+
     def get_cache_key(self) -> str:
         return str(self.url)
 
     @property
     def api_url(self) -> GridURL:
         return self.url.with_path(self.routes.ROUTE_API_CALL.value)
 
@@ -202,14 +213,21 @@
             )
 
         # upgrade to tls if available
         self.url = upgrade_tls(self.url, response)
 
         return response.content
 
+    def stream_data(self, credentials: SyftSigningKey) -> Response:
+        url = self.url.with_path(self.routes.STREAM.value)
+        response = self.session.get(
+            str(url), verify=verify_tls(), proxies={}, stream=True
+        )
+        return response
+
     def get_node_metadata(
         self, credentials: SyftSigningKey
     ) -> NodeMetadataJSON | SyftError:
         if self.proxy_target_uid:
             response = forward_message_to_proxy(
                 make_call=self.make_call,
                 proxy_target_uid=self.proxy_target_uid,
@@ -462,25 +480,37 @@
     connection: NodeConnection
     metadata: NodeMetadataJSON | None
     credentials: SyftSigningKey | None
     __logged_in_user: str = ""
     __logged_in_username: str = ""
     __user_role: ServiceRole = ServiceRole.NONE
 
+    # informs getattr does not have nasty side effects
+    __syft_allow_autocomplete__ = [
+        "api",
+        "code",
+        "jobs",
+        "users",
+        "settings",
+        "notifications",
+        "custom_api",
+    ]
+
     def __init__(
         self,
         connection: NodeConnection,
         metadata: NodeMetadataJSON | None = None,
         credentials: SyftSigningKey | None = None,
         api: SyftAPI | None = None,
     ) -> None:
         self.connection = connection
         self.metadata = metadata
         self.credentials: SyftSigningKey | None = credentials
         self._api = api
+        self.services: APIModule | None = None
         self.communication_protocol: int | str | None = None
         self.current_protocol: int | str | None = None
 
         self.post_init()
 
     def get_env(self) -> str:
         return self.api.services.metadata.get_env()
@@ -524,15 +554,15 @@
         project_create = ProjectSubmit(
             name=name,
             description=description,
             shareholders=[self],
             user_email_address=user_email_address,
             members=[self],
         )
-        project = project_create.start()
+        project = project_create.send()
         return project
 
     # TODO: type of request should be REQUEST, but it will give circular import error
     def sync_code_from_request(self, request: Any) -> SyftSuccess | SyftError:
         # relative
         from ..service.code.user_code import UserCode
         from ..service.code.user_code import UserCodeStatusCollection
@@ -660,26 +690,24 @@
 
         if protocol == SyftProtocol.HTTP:
             self_node_route = connection_to_route(self.connection)
             remote_node_route = connection_to_route(client.connection)
             if client.metadata is None:
                 return SyftError(f"client {client}'s metadata is None!")
 
-            result = self.api.services.network.exchange_credentials_with(
+            return self.api.services.network.exchange_credentials_with(
                 self_node_route=self_node_route,
                 remote_node_route=remote_node_route,
                 remote_node_verify_key=client.metadata.to(NodeMetadataV3).verify_key,
             )
         else:
             raise ValueError(
                 f"Invalid Route Exchange SyftProtocol: {protocol}.Supported protocols are {SyftProtocol.all()}"
             )
 
-        return result
-
     @property
     def jobs(self) -> APIModule | None:
         if self.api.has_service("job"):
             return self.api.services.job
         return None
 
     @property
@@ -745,23 +773,14 @@
         self,
         email: str | None = None,
         password: str | None = None,
         cache: bool = True,
         register: bool = False,
         **kwargs: Any,
     ) -> Self:
-        # TODO: Remove this Hack (Note to Rasswanth)
-        # If SYFT_LOGIN_{NODE_NAME}_PASSWORD is set, use that as the password
-        # for the login. This is useful for CI/CD environments to test password
-        # randomization that is implemented by helm charts
-        if self.name is not None and email == "info@openmined.org":
-            pass_env_var = f"SYFT_LOGIN_{self.name}_PASSWORD"
-            if pass_env_var in os.environ:
-                password = os.environ[pass_env_var]
-
         if email is None:
             email = input("Email: ")
         if password is None:
             password = getpass("Password: ")
 
         if register:
             self.register(
@@ -915,34 +934,36 @@
 
     def _fetch_node_metadata(self, credentials: SyftSigningKey) -> None:
         metadata = self.connection.get_node_metadata(credentials=credentials)
         if isinstance(metadata, NodeMetadataJSON):
             metadata.check_version(__version__)
             self.metadata = metadata
 
-    def _fetch_api(self, credentials: SyftSigningKey) -> None:
+    def _fetch_api(self, credentials: SyftSigningKey) -> SyftAPI:
         _api: SyftAPI = self.connection.get_api(
             credentials=credentials,
             communication_protocol=self.communication_protocol,
         )
 
-        def refresh_callback() -> None:
+        def refresh_callback() -> SyftAPI:
             return self._fetch_api(self.credentials)
 
         _api.refresh_api_callback = refresh_callback
 
         if self.credentials is None:
             raise ValueError(f"{self}'s credentials (signing key) is None!")
 
         APIRegistry.set_api_for(
             node_uid=self.id,
             user_verify_key=self.credentials.verify_key,
             api=_api,
         )
         self._api = _api
+        self.services = _api.services
+        return _api
 
 
 @instrument
 def connect(
     url: str | GridURL = DEFAULT_PYGRID_ADDRESS,
     node: AbstractNode | None = None,
     port: int | None = None,
```

### Comparing `syft-0.8.7b7/src/syft/client/connection.py` & `syft-0.8.7b8/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/client/domain_client.py` & `syft-0.8.7b8/src/syft/client/domain_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 # stdlib
 from pathlib import Path
 import re
 from typing import TYPE_CHECKING
 from typing import cast
 
 # third party
-from hagrid.orchestra import NodeHandle
 from loguru import logger
 from tqdm import tqdm
 
 # relative
 from ..abstract_node import NodeSideType
-from ..img.base64 import base64read
 from ..serde.serializable import serializable
 from ..service.action.action_object import ActionObject
 from ..service.code_history.code_history import CodeHistoriesDict
 from ..service.code_history.code_history import UsersCodeHistoriesDict
 from ..service.dataset.dataset import Contributor
 from ..service.dataset.dataset import CreateAsset
 from ..service.dataset.dataset import CreateDataset
@@ -27,26 +25,28 @@
 from ..service.sync.diff_state import ResolvedSyncState
 from ..service.sync.sync_state import SyncState
 from ..service.user.roles import Roles
 from ..service.user.user import UserView
 from ..service.user.user_roles import ServiceRole
 from ..types.blob_storage import BlobFile
 from ..types.uid import UID
-from ..util.fonts import FONT_CSS
+from ..util.assets import load_png_base64
+from ..util.notebook_ui.styles import FONT_CSS
 from ..util.util import get_mb_size
 from ..util.util import prompt_warning_message
 from .api import APIModule
 from .client import SyftClient
 from .client import login
 from .client import login_as_guest
 from .connection import NodeConnection
 from .protocol import SyftProtocol
 
 if TYPE_CHECKING:
     # relative
+    from ..orchestra import NodeHandle
     from ..service.project.project import Project
 
 
 def _get_files_from_glob(glob_path: str) -> list[Path]:
     files = Path().glob(glob_path)
     return [f for f in files if f.is_file() and not f.name.startswith(".")]
 
@@ -118,15 +118,15 @@
             message = (
                 "You're approving a request on "
                 f"{metadata.node_side_type} side {metadata.node_type} "
                 "which may host datasets with private information."
             )
             prompt_warning_message(message=message, confirm=True)
 
-        for asset in tqdm(dataset.asset_list):
+        for asset in tqdm(dataset.asset_list, colour="green"):
             print(f"Uploading: {asset.name}")
             try:
                 twin = TwinObject(
                     private_obj=asset.data,
                     mock_obj=asset.mock,
                     syft_node_location=self.id,
                     syft_client_verify_key=self.verify_key,
@@ -165,14 +165,17 @@
     #                 f"Can't access the api. Please log in to {item.syft_node_location}"
     #             )
     #         return api.services.sync.get_permissions(items)
     #     else:
     #         return {}
 
     def refresh(self) -> None:
+        if self.credentials:
+            self._fetch_node_metadata(self.credentials)
+
         if self._api and self._api.refresh_api_callback:
             self._api.refresh_api_callback()
 
     def get_sync_state(self) -> SyncState | SyftError:
         state: SyncState = self.api.services.sync._get_state()
         if isinstance(state, SyftError):
             return state
@@ -302,107 +305,89 @@
             if isinstance(client, SyftError):
                 return client
 
         res = self.exchange_route(client, protocol=protocol)
         if isinstance(res, SyftSuccess):
             if self.metadata:
                 return SyftSuccess(
-                    message=f"Connected {self.metadata.node_type} '{self.metadata.name}' to gateway '{client.name}'"
+                    message=(
+                        f"Connected {self.metadata.node_type} "
+                        f"'{self.metadata.name}' to gateway '{client.name}'. "
+                        f"{res.message}"
+                    )
                 )
             else:
                 return SyftSuccess(message=f"Connected to '{client.name}' gateway")
+
         return res
 
+    def _get_service_by_name_if_exists(self, name: str) -> APIModule | None:
+        if self.api.has_service(name):
+            return getattr(self.api.services, name)
+        return None
+
     @property
     def data_subject_registry(self) -> APIModule | None:
-        if self.api.has_service("data_subject"):
-            return self.api.services.data_subject
-        return None
+        return self._get_service_by_name_if_exists("data_subject")
 
     @property
     def code(self) -> APIModule | None:
-        # if self.api.refresh_api_callback is not None:
-        #     self.api.refresh_api_callback()
-        if self.api.has_service("code"):
-            return self.api.services.code
-        return None
+        return self._get_service_by_name_if_exists("code")
 
     @property
     def worker(self) -> APIModule | None:
-        if self.api.has_service("worker"):
-            return self.api.services.worker
-        return None
+        return self._get_service_by_name_if_exists("worker")
 
     @property
     def requests(self) -> APIModule | None:
-        if self.api.has_service("request"):
-            return self.api.services.request
-        return None
+        return self._get_service_by_name_if_exists("request")
 
     @property
     def datasets(self) -> APIModule | None:
-        if self.api.has_service("dataset"):
-            return self.api.services.dataset
-        return None
+        return self._get_service_by_name_if_exists("dataset")
 
     @property
     def projects(self) -> APIModule | None:
-        if self.api.has_service("project"):
-            return self.api.services.project
-        return None
+        return self._get_service_by_name_if_exists("project")
 
     @property
     def code_history_service(self) -> APIModule | None:
-        if self.api is not None and self.api.has_service("code_history"):
-            return self.api.services.code_history
-        return None
+        return self._get_service_by_name_if_exists("code_history")
 
     @property
     def code_history(self) -> CodeHistoriesDict:
         return self.api.services.code_history.get_history()
 
     @property
     def code_histories(self) -> UsersCodeHistoriesDict:
         return self.api.services.code_history.get_histories()
 
     @property
     def images(self) -> APIModule | None:
-        if self.api.has_service("worker_image"):
-            return self.api.services.worker_image
-        return None
+        return self._get_service_by_name_if_exists("worker_image")
 
     @property
     def worker_pools(self) -> APIModule | None:
-        if self.api.has_service("worker_pool"):
-            return self.api.services.worker_pool
-        return None
+        return self._get_service_by_name_if_exists("worker_pool")
 
     @property
     def worker_images(self) -> APIModule | None:
-        if self.api.has_service("worker_image"):
-            return self.api.services.worker_image
-        return None
+        return self._get_service_by_name_if_exists("worker_images")
 
     @property
     def sync(self) -> APIModule | None:
-        if self.api.has_service("sync"):
-            return self.api.services.sync
-        return None
+        return self._get_service_by_name_if_exists("sync")
 
     @property
     def code_status(self) -> APIModule | None:
-        if self.api.has_service("code_status"):
-            return self.api.services.code_status
-        return None
+        return self._get_service_by_name_if_exists("code_status")
 
     @property
     def output(self) -> APIModule | None:
-        if self.api.has_service("output"):
-            return self.api.services.output
-        return None
+        return self._get_service_by_name_if_exists("output")
 
     def get_project(
         self,
         name: str | None = None,
         uid: UID | None = None,
     ) -> Project | None:
         """Get project by name or UID"""
@@ -462,15 +447,15 @@
 
         command_list = f"""
         <ul style='padding-left: 1em;'>
             {commands}
         </ul>
         """
 
-        small_grid_symbol_logo = base64read("small-grid-symbol-logo.png")
+        small_grid_symbol_logo = load_png_base64("small-grid-symbol-logo.png")
 
         url = getattr(self.connection, "url", None)
         node_details = f"<strong>URL:</strong> {url}<br />" if url else ""
         if self.metadata is not None:
             node_details += f"<strong>Node Type:</strong> {self.metadata.node_type.capitalize()}<br />"
             node_side_type = (
                 "Low Side"
@@ -478,14 +463,15 @@
                 else "High Side"
             )
             node_details += f"<strong>Node Side Type:</strong> {node_side_type}<br />"
             node_details += (
                 f"<strong>Syft Version:</strong> {self.metadata.syft_version}<br />"
             )
 
+        self._fetch_node_metadata(self.credentials)
         return f"""
         <style>
             {FONT_CSS}
 
             .syft-container {{
                 padding: 5px;
                 font-family: 'Open Sans';
```

### Comparing `syft-0.8.7b7/src/syft/client/enclave_client.py` & `syft-0.8.7b8/src/syft/client/enclave_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # future
 from __future__ import annotations
 
 # stdlib
 from typing import Any
 from typing import TYPE_CHECKING
 
-# third party
-from hagrid.orchestra import NodeHandle
-
 # relative
 from ..abstract_node import NodeSideType
 from ..client.api import APIRegistry
-from ..img.base64 import base64read
 from ..serde.serializable import serializable
 from ..service.metadata.node_metadata import NodeMetadataJSON
 from ..service.network.routes import NodeRouteType
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
 from ..types.syft_object import SYFT_OBJECT_VERSION_3
 from ..types.syft_object import SyftObject
 from ..types.uid import UID
-from ..util.fonts import FONT_CSS
+from ..util.assets import load_png_base64
+from ..util.notebook_ui.styles import FONT_CSS
 from .api import APIModule
 from .client import SyftClient
 from .client import login
 from .client import login_as_guest
 from .protocol import SyftProtocol
 
 if TYPE_CHECKING:
     # relative
+    from ..orchestra import NodeHandle
     from ..service.code.user_code import SubmitUserCode
 
 
 @serializable()
 class EnclaveMetadata(SyftObject):
     __canonical_name__ = "EnclaveMetadata"
     __version__ = SYFT_OBJECT_VERSION_3
@@ -91,17 +89,24 @@
             if isinstance(client, SyftError):
                 return client
 
         self.metadata: NodeMetadataJSON = self.metadata
         res = self.exchange_route(client, protocol=protocol)
 
         if isinstance(res, SyftSuccess):
-            return SyftSuccess(
-                message=f"Connected {self.metadata.node_type} {self.metadata.name} to {client.name} gateway"
-            )
+            if self.metadata:
+                return SyftSuccess(
+                    message=(
+                        f"Connected {self.metadata.node_type} "
+                        f"'{self.metadata.name}' to gateway '{client.name}'. "
+                        f"{res.message}"
+                    )
+                )
+            else:
+                return SyftSuccess(message=f"Connected to '{client.name}' gateway")
 
         return res
 
     def get_enclave_metadata(self) -> EnclaveMetadata:
         return EnclaveMetadata(route=self.connection.route)
 
     def request_code_execution(self, code: SubmitUserCode) -> Any | SyftError:
@@ -160,15 +165,15 @@
 
         command_list = f"""
         <ul style='padding-left: 1em;'>
             {commands}
         </ul>
         """
 
-        small_grid_symbol_logo = base64read("small-grid-symbol-logo.png")
+        small_grid_symbol_logo = load_png_base64("small-grid-symbol-logo.png")
 
         url = getattr(self.connection, "url", None)
         node_details = f"<strong>URL:</strong> {url}<br />" if url else ""
         if self.metadata:
             node_details += f"<strong>Node Type:</strong> {self.metadata.node_type.capitalize()}<br />"
             node_side_type = (
                 "Low Side"
```

### Comparing `syft-0.8.7b7/src/syft/client/gateway_client.py` & `syft-0.8.7b8/src/syft/client/gateway_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # stdlib
 from typing import Any
 
 # relative
 from ..abstract_node import NodeSideType
 from ..abstract_node import NodeType
-from ..img.base64 import base64read
 from ..node.credentials import SyftSigningKey
 from ..serde.serializable import serializable
 from ..service.metadata.node_metadata import NodeMetadataJSON
 from ..service.network.node_peer import NodePeer
 from ..service.response import SyftError
 from ..service.response import SyftException
 from ..types.syft_object import SYFT_OBJECT_VERSION_2
 from ..types.syft_object import SyftObject
-from ..util.fonts import FONT_CSS
+from ..util.assets import load_png_base64
+from ..util.notebook_ui.styles import FONT_CSS
 from .client import SyftClient
 from .connection import NodeConnection
 
 
 @serializable()
 class GatewayClient(SyftClient):
     # TODO: add widget repr for gateway client
@@ -89,15 +89,15 @@
 
         command_list = f"""
         <ul style='padding-left: 1em;'>
             {commands}
         </ul>
         """
 
-        small_grid_symbol_logo = base64read("small-grid-symbol-logo.png")
+        small_grid_symbol_logo = load_png_base64("small-grid-symbol-logo.png")
 
         url = getattr(self.connection, "url", None)
         node_details = f"<strong>URL:</strong> {url}<br />" if url else ""
         if self.metadata:
             node_details += f"<strong>Node Type:</strong> {self.metadata.node_type.capitalize()}<br />"
             node_side_type = (
                 "Low Side"
```

### Comparing `syft-0.8.7b7/src/syft/client/registry.py` & `syft-0.8.7b8/src/syft/client/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,18 +76,18 @@
             url = "http://" + network["host_or_ip"] + ":" + str(network["port"]) + "/"
             try:
                 res = requests.get(url, timeout=DEFAULT_TIMEOUT)  # nosec
                 online = "This is a PyGrid Network node." in res.text
             except Exception:
                 online = False
 
-            # networks without frontend have a /ping route in 0.7.0
+            # networks without frontend
             if not online:
                 try:
-                    ping_url = url + "ping"
+                    ping_url = url + "api/v2/"
                     res = requests.get(ping_url, timeout=DEFAULT_TIMEOUT)  # nosec
                     online = res.status_code == 200
                 except Exception:
                     online = False
 
             if online:
                 version = network.get("version", None)
@@ -185,18 +185,18 @@
             url = "http://" + network["host_or_ip"] + ":" + str(network["port"]) + "/"
             try:
                 res = requests.get(url, timeout=DEFAULT_TIMEOUT)
                 online = "This is a PyGrid Network node." in res.text
             except Exception:
                 online = False
 
-            # networks without frontend have a /ping route in 0.7.0
+            # networks without frontend
             if not online:
                 try:
-                    ping_url = url + "ping"
+                    ping_url = url + "api/v2/"
                     res = requests.get(ping_url, timeout=DEFAULT_TIMEOUT)
                     online = res.status_code == 200
                 except Exception:
                     online = False
 
             if online:
                 version = network.get("version", None)
```

### Comparing `syft-0.8.7b7/src/syft/client/search.py` & `syft-0.8.7b8/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/client/sync_decision.py` & `syft-0.8.7b8/src/syft/client/sync_decision.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/client/user_settings.py` & `syft-0.8.7b8/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/custom_worker/builder.py` & `syft-0.8.7b8/src/syft/custom_worker/builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 __all__ = ["CustomWorkerBuilder"]
 
 
 class CustomWorkerBuilder:
     TYPE_CPU = "cpu"
     TYPE_GPU = "gpu"
 
-    TEMPLATE_DIR_PROD = os.path.expandvars("$APPDIR/grid/")
-    TEMPLATE_DIR_DEV = "../../../../../grid/backend/"
+    TEMPLATE_DIR_PROD = os.path.expandvars("$APPDIR/grid/images/")
+    TEMPLATE_DIR_DEV = "../../../../../grid/backend/grid/images/"
 
     CUSTOM_IMAGE_PREFIX = "custom-worker"
 
     BUILD_MAX_WAIT = 30 * 60
 
     @cached_property
     def builder(self) -> BuilderBase:
@@ -98,15 +98,15 @@
         # Builds a Docker pre-made CPU/GPU image template using a CustomWorkerConfig
         # remove once GPU is supported
         if config.build.gpu:
             raise Exception("GPU custom worker is not supported yet")
 
         type = self.TYPE_GPU if config.build.gpu else self.TYPE_CPU
 
-        dockerfile_path = self._find_template_path(type)
+        dockerfile_path = self.find_worker_image(type)
 
         imgtag = config.get_signature()[:8]
 
         build_args = {
             "PYTHON_VERSION": config.build.python_version,
             "SYSTEM_PACKAGES": config.build.merged_system_pkgs(),
             "PIP_PACKAGES": config.build.merged_python_pkgs(),
@@ -115,19 +115,19 @@
 
         return self.builder.build_image(
             tag=f"{self.CUSTOM_IMAGE_PREFIX}-{type}:{imgtag}",
             dockerfile_path=dockerfile_path,
             buildargs=build_args,
         )
 
-    def _find_template_path(self, type: str) -> Path:
+    def find_worker_image(self, type: str) -> Path:
         """
         Find the Worker Dockerfile and it's context path
         - PROD will be in `$APPDIR/grid/`
-        - DEV will be in `packages/grid/backend`
+        - DEV will be in `packages/grid/backend/grid/images`
         - In both the cases context dir does not matter (unless we're calling COPY)
 
         Args:
             type (str): The type of worker.
         Returns:
             Path: The path to the Dockerfile.
         """
```

### Comparing `syft-0.8.7b7/src/syft/custom_worker/builder_docker.py` & `syft-0.8.7b8/src/syft/custom_worker/builder_docker.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 
         # Core docker build call. Func kwargs should match with Docker SDK's BuildApiMixin
         with contextlib.closing(docker.from_env()) as client:
             image_result, logs = client.images.build(
                 tag=tag,
                 timeout=BUILD_IMAGE_TIMEOUT_SEC,
                 buildargs=buildargs,
+                rm=True,
+                labels={"orgs.openmined.syft": f"Build image {tag}"},
                 **kwargs,
             )
             return ImageBuildResult(
                 # An image that is built locally will not have a RepoDigests until pushed to a v2 registry
                 # https://stackoverflow.com/a/39812035
                 image_hash=image_result.id,
                 logs=self._parse_output(logs),
```

### Comparing `syft-0.8.7b7/src/syft/custom_worker/builder_k8s.py` & `syft-0.8.7b8/src/syft/custom_worker/builder_k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/custom_worker/builder_types.py` & `syft-0.8.7b8/src/syft/custom_worker/builder_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/custom_worker/config.py` & `syft-0.8.7b8/src/syft/custom_worker/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,17 @@
             return f"prebuilt tag='{self.tag}' description='{self.description}'"
         else:
             return f"prebuilt tag='{self.tag}'"
 
     def set_description(self, description_text: str) -> None:
         self.description = description_text
 
+    def __hash__(self) -> int:
+        return hash(self.tag)
+
 
 @serializable()
 class DockerWorkerConfig(WorkerConfig):
     dockerfile: str
     file_name: str | None = None
     description: str | None = None
 
@@ -171,14 +174,16 @@
                     return SyftError(
                         "Cannot reach docker server. Please check if docker is running."
                     )
 
                 kwargs["fileobj"] = io.BytesIO(self.dockerfile.encode("utf-8"))
                 _, logs = client.images.build(
                     tag=tag,
+                    rm=True,
+                    labels={"orgs.openmined.syft": "Test image build"},
                     **kwargs,
                 )
                 return SyftSuccess(message=iterator_to_string(iterator=logs))
         except Exception as e:
             # stdlib
             import traceback
```

### Comparing `syft-0.8.7b7/src/syft/custom_worker/k8s.py` & `syft-0.8.7b8/src/syft/custom_worker/k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/custom_worker/runner_k8s.py` & `syft-0.8.7b8/src/syft/custom_worker/runner_k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/custom_worker/utils.py` & `syft-0.8.7b8/src/syft/custom_worker/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/exceptions/exception.py` & `syft-0.8.7b8/src/syft/exceptions/exception.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/img/logo.png` & `syft-0.8.7b8/src/syft/assets/img/logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/img/small-grid-symbol-logo.png` & `syft-0.8.7b8/src/syft/assets/img/small-grid-symbol-logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/node/credentials.py` & `syft-0.8.7b8/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/node/node.py` & `syft-0.8.7b8/src/syft/node/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # future
 from __future__ import annotations
 
 # stdlib
 from collections import OrderedDict
-from collections import defaultdict
 from collections.abc import Callable
 from datetime import datetime
 from functools import partial
 import hashlib
 import os
 from pathlib import Path
 import shutil
@@ -42,14 +41,15 @@
 from ..service.action.action_object import ActionObject
 from ..service.action.action_service import ActionService
 from ..service.action.action_store import ActionStore
 from ..service.action.action_store import DictActionStore
 from ..service.action.action_store import MongoActionStore
 from ..service.action.action_store import SQLiteActionStore
 from ..service.api.api_service import APIService
+from ..service.attestation.attestation_service import AttestationService
 from ..service.blob_storage.service import BlobStorageService
 from ..service.code.status_service import UserCodeStatusService
 from ..service.code.user_code_service import UserCodeService
 from ..service.code.user_code_stash import UserCodeStash
 from ..service.code_history.code_history_service import CodeHistoryService
 from ..service.context import AuthedServiceContext
 from ..service.context import NodeServiceContext
@@ -58,18 +58,20 @@
 from ..service.data_subject.data_subject_member_service import DataSubjectMemberService
 from ..service.data_subject.data_subject_service import DataSubjectService
 from ..service.dataset.dataset_service import DatasetService
 from ..service.enclave.enclave_service import EnclaveService
 from ..service.job.job_service import JobService
 from ..service.job.job_stash import Job
 from ..service.job.job_stash import JobStash
+from ..service.job.job_stash import JobType
 from ..service.log.log_service import LogService
 from ..service.metadata.metadata_service import MetadataService
 from ..service.metadata.node_metadata import NodeMetadataV3
 from ..service.network.network_service import NetworkService
+from ..service.network.utils import PeerHealthCheckTask
 from ..service.notification.notification_service import NotificationService
 from ..service.notifier.notifier_service import NotifierService
 from ..service.object_search.migration_state_service import MigrateStateService
 from ..service.output.output_service import OutputService
 from ..service.policy.policy_service import PolicyService
 from ..service.project.project_service import ProjectService
 from ..service.queue.base_queue import AbstractMessageHandler
@@ -317,14 +319,15 @@
         in_memory_workers: bool = True,
         smtp_username: str | None = None,
         smtp_password: str | None = None,
         email_sender: str | None = None,
         smtp_port: int | None = None,
         smtp_host: str | None = None,
         association_request_auto_approval: bool = False,
+        background_tasks: bool = False,
     ):
         # 🟡 TODO 22: change our ENV variable format and default init args to make this
         # less horrible or add some convenience functions
         self.dev_mode = dev_mode or get_dev_mode()
         self.id = UID.from_string(node_uid_env) if node_uid_env else (id or UID())
         self.packages = ""
         self.processes = processes
@@ -366,18 +369,20 @@
 
         # must call before initializing stores
         if reset:
             self.remove_temp_dir()
 
         use_sqlite = local_db or (processes > 0 and not is_subprocess)
         document_store_config = document_store_config or self.get_default_store(
-            use_sqlite=use_sqlite
+            use_sqlite=use_sqlite,
+            store_type="Document Store",
         )
         action_store_config = action_store_config or self.get_default_store(
-            use_sqlite=use_sqlite
+            use_sqlite=use_sqlite,
+            store_type="Action Store",
         )
         self.init_stores(
             action_store_config=action_store_config,
             document_store_config=document_store_config,
         )
 
         # construct services only after init stores
@@ -403,14 +408,24 @@
 
         self.create_initial_settings(admin_email=root_email)
 
         self.init_queue_manager(queue_config=self.queue_config)
 
         self.init_blob_storage(config=blob_storage_config)
 
+        context = AuthedServiceContext(
+            node=self,
+            credentials=self.verify_key,
+            role=ServiceRole.ADMIN,
+        )
+
+        self.peer_health_manager: PeerHealthCheckTask | None = None
+        if background_tasks:
+            self.run_peer_health_checks(context=context)
+
         # Migrate data before any operation on db
         if migrate:
             self.find_and_migrate_data()
 
         NodeRegistry.set_node_for(self.id, self)
 
     @property
@@ -418,20 +433,23 @@
         path = "/proc/self/cgroup"
         return (
             os.path.exists("/.dockerenv")
             or os.path.isfile(path)
             and any("docker" in line for line in open(path))
         )
 
-    def get_default_store(self, use_sqlite: bool) -> StoreConfig:
+    def get_default_store(self, use_sqlite: bool, store_type: str) -> StoreConfig:
         if use_sqlite:
             path = self.get_temp_dir("db")
+            file_name: str = f"{self.id}.sqlite"
+            if self.dev_mode:
+                print(f"{store_type}'s SQLite DB path: {path/file_name}")
             return SQLiteStoreConfig(
                 client_config=SQLiteStoreClientConfig(
-                    filename=f"{self.id}.sqlite",
+                    filename=file_name,
                     path=path,
                 )
             )
         return DictStoreConfig()
 
     def init_blob_storage(self, config: BlobStorageConfig | None = None) -> None:
         if config is None:
@@ -453,15 +471,22 @@
                 credentials=self.signing_key.verify_key, has_permission=True
             ).ok()
             for remote_profile in remote_profiles:
                 self.blob_store_config.client_config.remote_profiles[
                     remote_profile.profile_name
                 ] = remote_profile
 
+    def run_peer_health_checks(self, context: AuthedServiceContext) -> None:
+        self.peer_health_manager = PeerHealthCheckTask()
+        self.peer_health_manager.run(context=context)
+
     def stop(self) -> None:
+        if self.peer_health_manager is not None:
+            self.peer_health_manager.stop()
+
         for consumer_list in self.queue_manager.consumers.values():
             for c in consumer_list:
                 c.close()
         for p in self.queue_manager.producers.values():
             p.close()
 
         self.queue_manager.producers.clear()
@@ -598,14 +623,15 @@
         thread_workers: bool = False,
         create_producer: bool = False,
         queue_port: int | None = None,
         dev_mode: bool = False,
         migrate: bool = False,
         in_memory_workers: bool = True,
         association_request_auto_approval: bool = False,
+        background_tasks: bool = False,
     ) -> Self:
         uid = UID.with_seed(name)
         name_hash = hashlib.sha256(name.encode("utf8")).digest()
         key = SyftSigningKey(signing_key=SigningKey(name_hash))
         blob_storage_config = None
 
         node_type = NodeType(node_type)
@@ -626,14 +652,15 @@
             thread_workers=thread_workers,
             create_producer=create_producer,
             dev_mode=dev_mode,
             migrate=migrate,
             in_memory_workers=in_memory_workers,
             reset=reset,
             association_request_auto_approval=association_request_auto_approval,
+            background_tasks=background_tasks,
         )
 
     def is_root(self, credentials: SyftVerifyKey) -> bool:
         return credentials == self.verify_key
 
     @property
     def root_client(self) -> SyftClient:
@@ -873,14 +900,15 @@
         #     - The callable must return AbstractService or None
         # - "store" expects a store type
         #     - By default all services get the document store
         #     - Pass a custom "store" to override this
         default_services: list[dict] = [
             {"svc": ActionService, "store": self.action_store},
             {"svc": UserService},
+            {"svc": AttestationService},
             {"svc": WorkerService},
             {"svc": SettingsService},
             {"svc": DatasetService},
             {"svc": UserCodeService},
             {"svc": LogService},
             {"svc": RequestService},
             {"svc": QueueService},
@@ -968,17 +996,21 @@
 
     @property
     def settings(self) -> NodeSettings:
         settings_stash = SettingsStash(store=self.document_store)
         if self.signing_key is None:
             raise ValueError(f"{self} has no signing key")
         settings = settings_stash.get_all(self.signing_key.verify_key)
+        if settings.is_err():
+            raise ValueError(
+                f"Cannot get node settings for '{self.name}'. Error: {settings.err()}"
+            )
         if settings.is_ok() and len(settings.ok()) > 0:
-            settings_data = settings.ok()[0]
-        return settings_data
+            settings = settings.ok()[0]
+        return settings
 
     @property
     def metadata(self) -> NodeMetadataV3:
         name = ""
         organization = ""
         description = ""
         show_warnings = self.enable_warnings
@@ -1111,23 +1143,16 @@
             else:
                 signed_result = client.connection.make_call(api_call)
                 result = debox_signed_syftapicall_response(signed_result=signed_result)
 
                 # relative
                 from ..store.blob_storage import BlobRetrievalByURL
 
-                # In the case of blob storage, the gateway downloads the result and then passes it to
-                # the proxy client
                 if isinstance(result, BlobRetrievalByURL):
-                    blob_route = client.api.connection.to_blob_route(
-                        result.url.url_path
-                    )
-                    result.url = blob_route
-                    final_res = result.read()
-                    return final_res
+                    result.proxy_node_uid = peer.id
 
             return result
 
         return SyftError(message=(f"Node has no route to {node_uid}"))
 
     def get_role_for_credentials(self, credentials: SyftVerifyKey) -> ServiceRole:
         role = self.get_service("userservice").get_role_for_credentials(
@@ -1180,15 +1205,19 @@
 
         if is_blocking or self.is_subprocess:
             credentials: SyftVerifyKey = api_call.credentials
             api_call = api_call.message
 
             role = self.get_role_for_credentials(credentials=credentials)
             context = AuthedServiceContext(
-                node=self, credentials=credentials, role=role, job_id=job_id
+                node=self,
+                credentials=credentials,
+                role=role,
+                job_id=job_id,
+                is_blocking_api_call=is_blocking,
             )
             AuthNodeContextRegistry.set_node_context(self.id, context, credentials)
 
             user_config_registry = UserServiceConfigRegistry.from_role(role)
 
             if api_call.path not in user_config_registry:
                 if ServiceConfigRegistry.path_exists(api_call.path):
@@ -1229,14 +1258,19 @@
         worker_settings = WorkerSettings.from_node(node=self)
 
         if worker_pool is None:
             worker_pool = self.get_default_worker_pool()
         else:
             worker_pool = self.get_worker_pool_by_name(worker_pool)
 
+        if isinstance(worker_pool, SyftError):
+            return worker_pool
+        elif worker_pool is None:
+            return SyftError(message="Worker pool not found")
+
         # Create a Worker pool reference object
         worker_pool_ref = LinkedObject.from_obj(
             worker_pool,
             service_type=SyftWorkerPoolService,
             node_uid=self.id,
         )
         queue_item = APIEndpointQueueItem(
@@ -1251,19 +1285,40 @@
             kwargs={"path": path, **kwargs},
             has_execute_permissions=True,
             worker_pool=worker_pool_ref,  # set worker pool reference as part of queue item
         )
 
         action = Action.from_api_endpoint_execution()
         return self.add_queueitem_to_queue(
-            queue_item,
-            credentials,
-            action,
-            None,
+            queue_item=queue_item,
+            credentials=credentials,
+            action=action,
+            job_type=JobType.TWINAPIJOB,
+        )
+
+    def get_worker_pool_ref_by_name(
+        self, credentials: SyftVerifyKey, worker_pool_name: str | None = None
+    ) -> LinkedObject | SyftError:
+        # If worker pool id is not set, then use default worker pool
+        # Else, get the worker pool for given uid
+        if worker_pool_name is None:
+            worker_pool = self.get_default_worker_pool()
+        else:
+            result = self.pool_stash.get_by_name(credentials, worker_pool_name)
+            if result.is_err():
+                return SyftError(message=f"{result.err()}")
+            worker_pool = result.ok()
+
+        # Create a Worker pool reference object
+        worker_pool_ref = LinkedObject.from_obj(
+            worker_pool,
+            service_type=SyftWorkerPoolService,
+            node_uid=self.id,
         )
+        return worker_pool_ref
 
     def add_action_to_queue(
         self,
         action: Action,
         credentials: SyftVerifyKey,
         parent_job_id: UID | None = None,
         has_execute_permissions: bool = False,
@@ -1280,31 +1335,19 @@
             )
 
             # If result is Ok, then user code object exists
             if result.is_ok() and result.ok() is not None:
                 user_code = result.ok()
                 worker_pool_name = user_code.worker_pool_name
 
-        # If worker pool id is not set, then use default worker pool
-        # Else, get the worker pool for given uid
-        if worker_pool_name is None:
-            worker_pool = self.get_default_worker_pool()
-        else:
-            result = self.pool_stash.get_by_name(credentials, worker_pool_name)
-            if result.is_err():
-                return SyftError(message=f"{result.err()}")
-            worker_pool = result.ok()
-
-        # Create a Worker pool reference object
-        worker_pool_ref = LinkedObject.from_obj(
-            worker_pool,
-            service_type=SyftWorkerPoolService,
-            node_uid=self.id,
+        worker_pool_ref = self.get_worker_pool_ref_by_name(
+            credentials, worker_pool_name
         )
-
+        if isinstance(worker_pool_ref, SyftError):
+            return worker_pool_ref
         queue_item = ActionQueueItem(
             id=task_uid,
             node_uid=self.id,
             syft_client_verify_key=credentials,
             syft_node_location=self.id,
             job_id=job_id,
             worker_settings=worker_settings,
@@ -1314,24 +1357,30 @@
             worker_pool=worker_pool_ref,  # set worker pool reference as part of queue item
         )
         user_id = self.get_service("UserService").get_user_id_for_credentials(
             credentials
         )
 
         return self.add_queueitem_to_queue(
-            queue_item, credentials, action, parent_job_id, user_id
+            queue_item=queue_item,
+            credentials=credentials,
+            action=action,
+            parent_job_id=parent_job_id,
+            user_id=user_id,
         )
 
     def add_queueitem_to_queue(
         self,
+        *,
         queue_item: QueueItem,
         credentials: SyftVerifyKey,
         action: Action | None = None,
         parent_job_id: UID | None = None,
         user_id: UID | None = None,
+        job_type: JobType = JobType.JOB,
     ) -> Job | SyftError:
         log_id = UID()
         role = self.get_role_for_credentials(credentials=credentials)
         context = AuthedServiceContext(node=self, credentials=credentials, role=role)
 
         result_obj = ActionObject.empty()
         if action is not None:
@@ -1357,14 +1406,15 @@
             node_uid=self.id,
             syft_client_verify_key=credentials,
             syft_node_location=self.id,
             log_id=log_id,
             parent_job_id=parent_job_id,
             action=action,
             requested_by=user_id,
+            job_type=job_type,
         )
 
         # 🟡 TODO 36: Needs distributed lock
         self.queue_stash.set_placeholder(credentials, queue_item)
         self.job_stash.set(credentials, job)
 
         log_service = self.get_service("logservice")
@@ -1441,36 +1491,34 @@
 
             return self.add_action_to_queue(
                 action, api_call.credentials, parent_job_id=parent_job_id
             )
 
         else:
             worker_settings = WorkerSettings.from_node(node=self)
-            default_worker_pool = self.get_default_worker_pool()
-            worker_pool = LinkedObject.from_obj(
-                default_worker_pool,
-                service_type=SyftWorkerPoolService,
-                node_uid=self.id,
-            )
+            worker_pool_ref = self.get_worker_pool_ref_by_name(credentials=credentials)
+            if isinstance(worker_pool_ref, SyftError):
+                return worker_pool_ref
+
             queue_item = QueueItem(
                 id=UID(),
                 node_uid=self.id,
                 syft_client_verify_key=api_call.credentials,
                 syft_node_location=self.id,
                 job_id=UID(),
                 worker_settings=worker_settings,
                 service=service_str,
                 method=method_str,
                 args=unsigned_call.args,
                 kwargs=unsigned_call.kwargs,
-                worker_pool=worker_pool,
+                worker_pool=worker_pool_ref,
             )
             return self.add_queueitem_to_queue(
-                queue_item,
-                api_call.credentials,
+                queue_item=queue_item,
+                credentials=api_call.credentials,
                 action=None,
                 parent_job_id=parent_job_id,
             )
 
     @property
     def pool_stash(self) -> SyftWorkerPoolStash:
         return self.get_service(SyftWorkerPoolService).stash
```

### Comparing `syft-0.8.7b7/src/syft/node/routes.py` & `syft-0.8.7b8/src/syft/node/routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 # stdlib
-
-# stdlib
+import base64
+import binascii
 from typing import Annotated
 
 # third party
 from fastapi import APIRouter
 from fastapi import Body
 from fastapi import Depends
+from fastapi import HTTPException
 from fastapi import Request
 from fastapi import Response
 from fastapi.responses import JSONResponse
+from fastapi.responses import StreamingResponse
 from loguru import logger
 from pydantic import ValidationError
+import requests
 
 # relative
 from ..abstract_node import AbstractNode
 from ..protocol.data_protocol import PROTOCOL_TYPE
 from ..serde.deserialize import _deserialize as deserialize
 from ..serde.serialize import _serialize as serialize
 from ..service.context import NodeServiceContext
 from ..service.context import UnauthedServiceContext
 from ..service.metadata.node_metadata import NodeMetadataJSON
 from ..service.response import SyftError
 from ..service.user.user import UserCreate
 from ..service.user.user import UserPrivateKey
 from ..service.user.user_service import UserService
+from ..types.uid import UID
 from ..util.telemetry import TRACE_MODE
 from .credentials import SyftVerifyKey
 from .credentials import UserLoginCredentials
 from .worker import Worker
 
 
 def make_routes(worker: Worker) -> APIRouter:
@@ -42,14 +46,47 @@
             print("Failed to import opentelemetry")
 
     router = APIRouter()
 
     async def get_body(request: Request) -> bytes:
         return await request.body()
 
+    def _blob_url(peer_uid: UID, presigned_url: str) -> str:
+        # relative
+        from ..service.network.node_peer import route_to_connection
+
+        network_service = worker.get_service("NetworkService")
+        peer = network_service.stash.get_by_uid(worker.verify_key, peer_uid).ok()
+        peer_node_route = peer.pick_highest_priority_route()
+        connection = route_to_connection(route=peer_node_route)
+        url = connection.to_blob_route(presigned_url)
+
+        return str(url)
+
+    @router.get("/stream/{peer_uid}/{url_path}/", name="stream")
+    async def stream(peer_uid: str, url_path: str) -> StreamingResponse:
+        try:
+            url_path_parsed = base64.urlsafe_b64decode(url_path.encode()).decode()
+        except binascii.Error:
+            raise HTTPException(404, "Invalid `url_path`.")
+
+        peer_uid_parsed = UID.from_string(peer_uid)
+
+        url = _blob_url(peer_uid=peer_uid_parsed, presigned_url=url_path_parsed)
+
+        try:
+            resp = requests.get(url=url, stream=True)  # nosec
+            resp.raise_for_status()
+        except requests.RequestException:
+            raise HTTPException(404, "Failed to retrieve data from domain.")
+
+        return StreamingResponse(
+            resp.iter_content(chunk_size=None), media_type="text/event-stream"
+        )
+
     @router.get(
         "/",
         name="healthcheck",
         status_code=200,
         response_class=JSONResponse,
     )
     def root() -> dict[str, str]:
```

### Comparing `syft-0.8.7b7/src/syft/node/run.py` & `syft-0.8.7b8/src/syft/node/run.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # stdlib
 import argparse
 
-# third party
-from hagrid.orchestra import NodeHandle
-
 # relative
-from ..client.deploy import Orchestra
+from ..orchestra import NodeHandle
+from ..orchestra import Orchestra
 
 
 def str_to_bool(bool_str: str | None) -> bool:
     result = False
     bool_str = str(bool_str).lower()
     if bool_str == "true" or bool_str == "1":
         result = True
@@ -67,24 +65,16 @@
     parser.add_argument(
         "--tail",
         help="tail mode",
         type=str,
         default="True",
         dest="tail",
     )
-    parser.add_argument(
-        "--cmd",
-        help="cmd mode",
-        type=str,
-        default="False",
-        dest="cmd",
-    )
 
     args = parser.parse_args()
-
     if args.command != "launch":
         print("syft launch is the only command currently supported")
 
     args.dev_mode = str_to_bool(args.dev_mode)
     args.reset = str_to_bool(args.reset)
     args.local_db = str_to_bool(args.local_db)
     args.tail = str_to_bool(args.tail)
@@ -96,12 +86,11 @@
         host=args.host,
         port=args.port,
         dev_mode=args.dev_mode,
         reset=args.reset,
         local_db=args.local_db,
         processes=args.processes,
         tail=args.tail,
-        cmd=args.cmd,
     )
     if not args.tail:
         return node
     return None
```

### Comparing `syft-0.8.7b7/src/syft/node/server.py` & `syft-0.8.7b8/src/syft/node/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     node_side_type: str,
     enable_warnings: bool,
     in_memory_workers: bool,
     queue_port: int | None,
     create_producer: bool,
     association_request_auto_approval: bool,
     n_consumers: int,
+    background_tasks: bool,
 ) -> None:
     async def _run_uvicorn(
         name: str,
         node_type: NodeType,
         host: str,
         port: int,
         reset: bool,
@@ -108,14 +109,15 @@
                 enable_warnings=enable_warnings,
                 migrate=True,
                 in_memory_workers=in_memory_workers,
                 queue_port=queue_port,
                 create_producer=create_producer,
                 n_consumers=n_consumers,
                 association_request_auto_approval=association_request_auto_approval,
+                background_tasks=background_tasks,
             )
         else:
             worker = worker_class(
                 name=name,
                 processes=processes,
                 local_db=True,
                 node_type=node_type,
@@ -123,14 +125,15 @@
                 enable_warnings=enable_warnings,
                 migrate=True,
                 in_memory_workers=in_memory_workers,
                 queue_port=queue_port,
                 create_producer=create_producer,
                 n_consumers=n_consumers,
                 association_request_auto_approval=association_request_auto_approval,
+                background_tasks=background_tasks,
             )
         router = make_routes(worker=worker)
         app = make_app(worker.name, router=router)
 
         if reset:
             try:
                 python_pids = find_python_processes_on_port(port)
@@ -182,14 +185,15 @@
     tail: bool = False,
     enable_warnings: bool = False,
     in_memory_workers: bool = True,
     queue_port: int | None = None,
     create_producer: bool = False,
     n_consumers: int = 0,
     association_request_auto_approval: bool = False,
+    background_tasks: bool = False,
 ) -> tuple[Callable, Callable]:
     server_process = multiprocessing.Process(
         target=run_uvicorn,
         kwargs={
             "name": name,
             "node_type": node_type,
             "host": host,
@@ -200,14 +204,15 @@
             "node_side_type": node_side_type,
             "enable_warnings": enable_warnings,
             "in_memory_workers": in_memory_workers,
             "queue_port": queue_port,
             "create_producer": create_producer,
             "n_consumers": n_consumers,
             "association_request_auto_approval": association_request_auto_approval,
+            "background_tasks": background_tasks,
         },
     )
 
     def stop() -> None:
         print(f"Stopping {name}")
         server_process.terminate()
         server_process.join(3)
```

### Comparing `syft-0.8.7b7/src/syft/node/worker_settings.py` & `syft-0.8.7b8/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/protocol/data_protocol.py` & `syft-0.8.7b8/src/syft/protocol/data_protocol.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/protocol/protocol_version.json` & `syft-0.8.7b8/src/syft/protocol/protocol_version.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964962121212121%*

 * *Differences: {"'dev'": "{'object_versions': {'JobItem': {'6': OrderedDict([('version', 6), ('hash', "*

 * *          "'865a2ed791b8abd20d76e9a6bfae7ae7dad51b5ebfd8ff728aab25af93fa5570'), ('action', "*

 * *          "'add')]), delete: ['5']}, 'CustomAPIView': {'1': {'hash': "*

 * *          "'0b9afdd554f0b353c07256e2522342be1302b395d649f1cbabc555e5baecb150'}}, "*

 * *          "'UpdateTwinAPIEndpoint': {'1': {'hash': "*

 * *          "'6d8effd404f15d4378b1ff3382e0622b9e5a637d9db342d43cfec00fe29c649a'}}, "*

 * *          "'CreateTwinAPIEndpoint': {'1' […]*

```diff
@@ -23,25 +23,32 @@
             "AssociationRequestChange": {
                 "1": {
                     "action": "add",
                     "hash": "508550c43e9e3f30243813c23eb6eec20918923d7ba09498cddbcd7e8bfa4539",
                     "version": 1
                 }
             },
+            "BlobRetrievalByURL": {
+                "5": {
+                    "action": "add",
+                    "hash": "4934bf72bb10ac0a670c87ab735175088274e090819436563543473e64cf15e3",
+                    "version": 5
+                }
+            },
             "CreateTwinAPIEndpoint": {
                 "1": {
                     "action": "add",
-                    "hash": "e735dc30cba1789c3fb109e35aa40ffa873951f8e00b0b971950b1735c27d1ca",
+                    "hash": "55e0a7b0ac428a6abb771ffcb925ee79cdd752a4b83058aa4b71fbef2a9fee63",
                     "version": 1
                 }
             },
             "CustomAPIView": {
                 "1": {
                     "action": "add",
-                    "hash": "8fe9f0fded4dbce033e2b14798a59d8635c3b73b0562f9ea686b1162ed155e91",
+                    "hash": "0b9afdd554f0b353c07256e2522342be1302b395d649f1cbabc555e5baecb150",
                     "version": 1
                 }
             },
             "CustomApiEndpoint": {
                 "1": {
                     "action": "add",
                     "hash": "13617f3dce60fa692421e0d9deda7ffd365ec02d4a062c18510b48457b6eba02",
@@ -81,24 +88,24 @@
             },
             "JobItem": {
                 "4": {
                     "action": "remove",
                     "hash": "6a7cc7c2bb4dd234c1508b0af4d3b403cd3b7b427578a775bf80dc36891923ed",
                     "version": 4
                 },
-                "5": {
+                "6": {
                     "action": "add",
-                    "hash": "82ee08442b09797ed7a3710c31de633bb308b1d2215f51b58a3e01a4c201055d",
-                    "version": 5
+                    "hash": "865a2ed791b8abd20d76e9a6bfae7ae7dad51b5ebfd8ff728aab25af93fa5570",
+                    "version": 6
                 }
             },
             "NodePeer": {
                 "3": {
                     "action": "add",
-                    "hash": "dababb03d2463b6218ae22d55293a60580f5a14bebd0c664d71da104e2f0b835",
+                    "hash": "ec0e39fc77ddb542558519d6a1f7c55f41cc037b6312792333792a04feea57e6",
                     "version": 3
                 }
             },
             "NodeSettings": {
                 "4": {
                     "action": "add",
                     "hash": "318e578f8a9af213a6af0cc2c567b62196b0ff81769d808afff4dd1eb7c372b8",
@@ -163,22 +170,22 @@
                     "hash": "7d368102d0b473009af3b8c46e0ea6d35893c5ebb172b373ad7d52553c12c9fa",
                     "version": 1
                 }
             },
             "TwinAPIEndpoint": {
                 "1": {
                     "action": "add",
-                    "hash": "540468be5db20efe555d2288c9aed60887306ac9b56d6a63c066246bc0010e9c",
+                    "hash": "e538734d20be3b477e188eb91f66600c2e654bb32e34806ef24329e48238bf18",
                     "version": 1
                 }
             },
             "UpdateTwinAPIEndpoint": {
                 "1": {
                     "action": "add",
-                    "hash": "cd0d4d67dc03cf6b78832f33ef584ec0ff8fa0b851629396ba27d7db63130342",
+                    "hash": "6d8effd404f15d4378b1ff3382e0622b9e5a637d9db342d43cfec00fe29c649a",
                     "version": 1
                 }
             },
             "VeilidConnection": {
                 "1": {
                     "action": "remove",
                     "hash": "c1796e7b01c9eae0dbf59cfd5c2c2f0e7eba593e0cea615717246572b27aae4b",
```

### Comparing `syft-0.8.7b7/src/syft/protocol/releases/0.8.2.json` & `syft-0.8.7b8/src/syft/protocol/releases/0.8.2.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/protocol/releases/0.8.3.json` & `syft-0.8.7b8/src/syft/protocol/releases/0.8.3.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/protocol/releases/0.8.4.json` & `syft-0.8.7b8/src/syft/protocol/releases/0.8.4.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/protocol/releases/0.8.6.json` & `syft-0.8.7b8/src/syft/protocol/releases/0.8.6.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/serde/array.py` & `syft-0.8.7b8/src/syft/serde/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,10 +146,9 @@
 # for numpy_scalar_type in numpy_scalar_types:
 #     recursive_serde_register(
 #     numpy_scalar_type,
 #     serialize=lambda x: x.tobytes(),
 #     deserialize=lambda buffer: frombuffer(buffer, dtype=numpy_scalar_type),
 # )
 
-
 # how else do you import a relative file to execute it?
 NOTHING = None
```

### Comparing `syft-0.8.7b7/src/syft/serde/arrow.py` & `syft-0.8.7b8/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/serde/deserialize.py` & `syft-0.8.7b8/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/serde/lib_permissions.py` & `syft-0.8.7b8/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/serde/lib_service_registry.py` & `syft-0.8.7b8/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/serde/mock.py` & `syft-0.8.7b8/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/serde/recursive.py` & `syft-0.8.7b8/src/syft/serde/recursive.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/serde/recursive_primitives.py` & `syft-0.8.7b8/src/syft/serde/recursive_primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from typing import _SpecialGenericAlias
 from typing import _UnionGenericAlias
 from typing import cast
 import weakref
 
 # relative
 from .capnp import get_capnp_schema
-from .recursive import SPOOLED_FILE_MAX_SIZE_SERDE
 from .recursive import chunk_bytes
 from .recursive import combine_bytes
 from .recursive import recursive_serde_register
 from .util import compatible_with_large_file_writes_capnp
 
 iterable_schema = get_capnp_schema("iterable.capnp").Iterable
 kv_iterable_schema = get_capnp_schema("kv_iterable.capnp").KVIterable
```

### Comparing `syft-0.8.7b7/src/syft/serde/serializable.py` & `syft-0.8.7b8/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/serde/serialize.py` & `syft-0.8.7b8/src/syft/serde/serialize.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # stdlib
 import tempfile
 from typing import Any
 
 # relative
-from .recursive import SPOOLED_FILE_MAX_SIZE_SERDE
 from .util import compatible_with_large_file_writes_capnp
 
 
 def _serialize(
     obj: object,
     to_proto: bool = True,
     to_bytes: bool = False,
```

### Comparing `syft-0.8.7b7/src/syft/serde/signature.py` & `syft-0.8.7b8/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/serde/third_party.py` & `syft-0.8.7b8/src/syft/serde/third_party.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 from datetime import time
 import functools
 from importlib.util import find_spec
 from io import BytesIO
 
 # third party
 from dateutil import parser
-from jax import numpy as jnp
-from jaxlib.xla_extension import ArrayImpl
 from nacl.signing import SigningKey
 from nacl.signing import VerifyKey
 import networkx as nx
 from networkx import DiGraph
 import numpy as np
 from pandas import DataFrame
 from pandas import Series
@@ -22,21 +20,22 @@
 import pyarrow.parquet as pq
 import pydantic
 from pydantic._internal._model_construction import ModelMetaclass
 from pymongo.collection import Collection
 from result import Err
 from result import Ok
 from result import Result
-import zmq.green as zmq
 
 # relative
 from ..types.dicttuple import DictTuple
 from ..types.dicttuple import _Meta as _DictTupleMetaClass
 from ..types.syft_metaclass import EmptyType
 from ..types.syft_metaclass import PartialModelMetaclass
+from .array import numpy_deserialize
+from .array import numpy_serialize
 from .deserialize import _deserialize as deserialize
 from .recursive_primitives import _serialize_kv_pairs
 from .recursive_primitives import deserialize_kv
 from .recursive_primitives import deserialize_type
 from .recursive_primitives import recursive_serde_register
 from .recursive_primitives import recursive_serde_register_type
 from .recursive_primitives import serialize_type
@@ -104,15 +103,14 @@
 
 recursive_serde_register(
     Series,
     serialize=lambda x: serialize(DataFrame(x).to_dict(), to_bytes=True),
     deserialize=deserialize_series,
 )
 
-
 recursive_serde_register(
     datetime,
     serialize=lambda x: serialize(x.isoformat(), to_bytes=True),
     deserialize=lambda x: parser.isoparse(deserialize(x, from_bytes=True)),
 )
 
 recursive_serde_register(
@@ -177,40 +175,60 @@
     from IPython.display import Image
 
     recursive_serde_register(Image)
 
 except Exception:  # nosec
     pass
 
-# jax
-recursive_serde_register(
-    ArrayImpl,
-    serialize=lambda x: serialize(np.array(x), to_bytes=True),
-    deserialize=lambda x: jnp.array(deserialize(x, from_bytes=True)),
-)
 
+try:
+    # third party
+    import torch
+    from torch._C import _TensorMeta
+
+    def serialize_torch_tensor_meta(t: _TensorMeta) -> bytes:
+        buffer = BytesIO()
+        torch.save(t, buffer)
+        return buffer.getvalue()
+
+    def deserialize_torch_tensor_meta(buf: bytes) -> _TensorMeta:
+        buffer = BytesIO(buf)
+        return torch.load(buffer)
+
+    recursive_serde_register(
+        _TensorMeta,
+        serialize=serialize_torch_tensor_meta,
+        deserialize=deserialize_torch_tensor_meta,
+    )
+
+    def torch_serialize(tensor: torch.Tensor) -> bytes:
+        return numpy_serialize(tensor.numpy())
+
+    def torch_deserialize(buffer: bytes) -> torch.tensor:
+        np_array = numpy_deserialize(buffer)
+        return torch.from_numpy(np_array)
+
+    recursive_serde_register(
+        torch.Tensor,
+        serialize=torch_serialize,
+        deserialize=lambda data: torch_deserialize(data),
+    )
+
+except Exception:  # nosec
+    pass
 
 # unsure why we have to register the object not the type but this works
 recursive_serde_register(np.core._ufunc_config._unspecified())
 
 recursive_serde_register(
     pydantic.EmailStr,
     serialize=lambda x: x.encode(),
     deserialize=lambda x: pydantic.EmailStr(x.decode()),
 )
 
-recursive_serde_register(
-    zmq._Socket,
-    serialize_attrs=[
-        "_shadow",
-        "_monitor_socket",
-        "_type_name",
-    ],
-)
-recursive_serde_register(zmq._Context)
 
 # how else do you import a relative file to execute it?
 NOTHING = None
 
 
 # TODO: debug serializing after updating a node
 def serialize_networkx_graph(graph: DiGraph) -> bytes:
```

### Comparing `syft-0.8.7b7/src/syft/service/action/action_data_empty.py` & `syft-0.8.7b8/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/action/action_endpoint.py` & `syft-0.8.7b8/src/syft/service/action/action_endpoint.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/action/action_graph.py` & `syft-0.8.7b8/src/syft/service/action/action_graph.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/action/action_graph_service.py` & `syft-0.8.7b8/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/action/action_object.py` & `syft-0.8.7b8/src/syft/service/action/action_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -758,15 +758,15 @@
             if blob_storage_read_method is not None:
                 blob_retrieval_object = blob_storage_read_method(
                     uid=self.syft_blob_storage_entry_id
                 )
                 if isinstance(blob_retrieval_object, SyftError):
                     print(
                         "Could not fetch actionobject data\n",
-                        type(blob_retrieval_object),
+                        blob_retrieval_object,
                     )
                     return blob_retrieval_object
                 # relative
                 from ...store.blob_storage import BlobRetrieval
 
                 if isinstance(blob_retrieval_object, SyftError):
                     return blob_retrieval_object
```

### Comparing `syft-0.8.7b7/src/syft/service/action/action_permissions.py` & `syft-0.8.7b8/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/action/action_service.py` & `syft-0.8.7b8/src/syft/service/action/action_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/action/action_store.py` & `syft-0.8.7b8/src/syft/service/action/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/action/action_types.py` & `syft-0.8.7b8/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/action/numpy.py` & `syft-0.8.7b8/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/action/pandas.py` & `syft-0.8.7b8/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/action/plan.py` & `syft-0.8.7b8/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/action/verification.py` & `syft-0.8.7b8/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/api/api.py` & `syft-0.8.7b8/src/syft/service/api/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from ...types.transforms import TransformContext
 from ...types.transforms import generate_action_object_id
 from ...types.transforms import generate_id
 from ...types.transforms import keep
 from ...types.transforms import transform
 from ...types.uid import UID
 from ..context import AuthedServiceContext
+from ..dataset.dataset import MarkdownDescription
 from ..response import SyftError
 from ..user.user import UserView
 
 NOT_ACCESSIBLE_STRING = "N / A"
 
 
 class HelperFunctionSet:
@@ -80,15 +81,15 @@
 
     path: str
     action_object_id: UID
     signature: Signature
     access: str = "Public"
     mock_function: str | None = None
     private_function: str | None = None
-    description: str | None = None
+    description: MarkdownDescription | None = None
     mock_helper_functions: list[str] | None = None
     private_helper_functions: list[str] | None = None
     worker_pool: str | None = None
     endpoint_timeout: int = 60
 
     __repr_attrs__ = [
         "path",
@@ -171,17 +172,15 @@
             raise ValueError("Code must be a valid Python function.")
 
         return api_code
 
     @field_validator("func_name", check_fields=False)
     @classmethod
     def validate_func_name(cls, func_name: str) -> str:
-        if not re.match(r"^[a-zA-Z_][a-zA-Z0-9_]*$", func_name) or keyword.iskeyword(
-            func_name
-        ):
+        if not str.isidentifier(func_name) or keyword.iskeyword(func_name):
             raise ValueError("Invalid function name.")
         return func_name
 
     @field_validator("settings", check_fields=False)
     @classmethod
     def validate_settings(
         cls, settings: dict[str, Any] | None
@@ -292,16 +291,22 @@
         return data
 
     @field_validator("path", check_fields=False)
     @classmethod
     def validate_path(cls, path: str) -> str:
         # TODO: Check path doesn't collide with system endpoints
 
-        if not re.match(r"^[a-z]+(\.[a-z]+)*$", path):
-            raise ValueError('String must be a path-like string (e.g., "new.endpoint")')
+        if path.startswith(".") or path.endswith("."):
+            raise ValueError("Path cannot start or end with a '.'")
+        if not path.islower():
+            raise ValueError("Path must be lowercase")
+        parts = path.split(".")
+        for part in parts:
+            if not str.isidentifier(part) or keyword.iskeyword(part):
+                raise ValueError(f"Invalid path: {part} is not a valid identifier")
 
         return path
 
     @field_validator("private_function", check_fields=False)
     @classmethod
     def validate_private_function(
         cls, private_function: PrivateAPIEndpoint | None
@@ -324,47 +329,55 @@
     # version
     __canonical_name__ = "UpdateTwinAPIEndpoint"
     __version__ = SYFT_OBJECT_VERSION_1
 
     path: str
     private_function: PrivateAPIEndpoint | None = None
     mock_function: PublicAPIEndpoint
-    description: str | None = None
+    description: MarkdownDescription | None = None
     endpoint_timeout: int = 60
 
 
 @serializable()
 class CreateTwinAPIEndpoint(BaseTwinAPIEndpoint):
     # version
     __canonical_name__ = "CreateTwinAPIEndpoint"
     __version__ = SYFT_OBJECT_VERSION_1
 
     path: str
     private_function: PrivateAPIEndpoint | None = None
     mock_function: PublicAPIEndpoint
     signature: Signature
-    description: str | None = None
+    description: MarkdownDescription | None = None
     worker_pool: str | None = None
     endpoint_timeout: int = 60
 
+    def __init__(
+        self, description: str | MarkdownDescription | None = "", **kwargs: Any
+    ) -> None:
+        if isinstance(description, str):
+            description = MarkdownDescription(text=description)
+
+        super().__init__(**kwargs, description=description)
+
 
 @serializable()
 class TwinAPIEndpoint(SyncableSyftObject):
     # version
     __canonical_name__: str = "TwinAPIEndpoint"
     __version__ = SYFT_OBJECT_VERSION_1
 
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(**kwargs)
 
     path: str
     private_function: PrivateAPIEndpoint | None = None
     mock_function: PublicAPIEndpoint
     signature: Signature
-    description: str | None = None
+    description: MarkdownDescription | None = None
     action_object_id: UID
     worker_pool: str | None = None
     endpoint_timeout: int = 60
 
     __private_sync_attr_mocks__ = {
         "private_function": None,
     }
@@ -622,15 +635,15 @@
     ]
 
 
 def api_endpoint(
     path: str,
     settings: dict[str, str] | None = None,
     helper_functions: list[Callable] | None = None,
-    description: str | None = None,
+    description: MarkdownDescription | None = None,
     worker_pool: str | None = None,
     endpoint_timeout: int = 60,
 ) -> Callable[..., TwinAPIEndpoint | SyftError]:
     def decorator(f: Callable) -> TwinAPIEndpoint | SyftError:
         try:
             helper_functions_dict = {
                 f.__name__: inspect.getsource(f) for f in (helper_functions or [])
@@ -683,15 +696,15 @@
     return decorator
 
 
 def create_new_api_endpoint(
     path: str,
     mock_function: Endpoint,
     private_function: Endpoint | None = None,
-    description: str | None = None,
+    description: MarkdownDescription | None = None,
     worker_pool: str | None = None,
     endpoint_timeout: int = 60,
 ) -> CreateTwinAPIEndpoint | SyftError:
     try:
         # Parse the string to extract the function name
 
         endpoint_signature = mock_function.signature
```

### Comparing `syft-0.8.7b7/src/syft/service/api/api_service.py` & `syft-0.8.7b8/src/syft/service/api/api_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,16 +304,16 @@
         if isinstance(custom_endpoint, SyftError):
             return custom_endpoint
 
         result = context.node.add_api_endpoint_execution_to_queue(
             context.credentials,
             method,
             path,
-            worker_pool=custom_endpoint.worker_pool,
             *args,
+            worker_pool=custom_endpoint.worker_pool,
             **kwargs,
         )
         if isinstance(result, SyftError):
             return result
         # relative
         from ..job.job_stash import JobStatus
 
@@ -331,15 +331,18 @@
             or job.status == JobStatus.PROCESSING
             or job.status == JobStatus.CREATED
         ):
             job = job_service.get(context, job_id)
             time.sleep(0.1)
             if (time.time() - custom_endpoint.endpoint_timeout) > start:
                 return SyftError(
-                    message=f"Function timed out in {custom_endpoint.endpoint_timeout} seconds. Get the Job with id: {job_id} to check results."
+                    message=(
+                        f"Function timed out in {custom_endpoint.endpoint_timeout} seconds. "
+                        + f"Get the Job with id: {job_id} to check results."
+                    )
                 )
 
         if job.status == JobStatus.COMPLETED:
             return job.result
         else:
             return SyftError(message="Function failed to complete.")
```

### Comparing `syft-0.8.7b7/src/syft/service/api/api_stash.py` & `syft-0.8.7b8/src/syft/service/api/api_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/blob_storage/remote_profile.py` & `syft-0.8.7b8/src/syft/service/blob_storage/remote_profile.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/blob_storage/service.py` & `syft-0.8.7b8/src/syft/service/blob_storage/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/blob_storage/stash.py` & `syft-0.8.7b8/src/syft/service/blob_storage/stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/code/code_parse.py` & `syft-0.8.7b8/src/syft/service/code/code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/code/status_service.py` & `syft-0.8.7b8/src/syft/service/code/status_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/code/user_code.py` & `syft-0.8.7b8/src/syft/service/code/user_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from enum import Enum
 import hashlib
 import inspect
 from io import StringIO
 import itertools
 import random
 import sys
+from textwrap import dedent
 from threading import Thread
 import time
 import traceback
 from typing import Any
 from typing import ClassVar
 from typing import TYPE_CHECKING
 from typing import cast
@@ -71,20 +72,22 @@
 from ..policy.policy import OutputPolicy
 from ..policy.policy import SingleExecutionExactOutput
 from ..policy.policy import SubmitUserPolicy
 from ..policy.policy import UserPolicy
 from ..policy.policy import filter_only_uids
 from ..policy.policy import init_policy
 from ..policy.policy import load_policy_code
+from ..policy.policy import partition_by_node
 from ..policy.policy_service import PolicyService
 from ..response import SyftError
 from ..response import SyftInfo
 from ..response import SyftNotReady
 from ..response import SyftSuccess
 from ..response import SyftWarning
+from ..user.user import UserView
 from .code_parse import GlobalsVisitor
 from .code_parse import LaunchJobVisitor
 from .unparse import unparse
 from .utils import submit_subjobs_code
 
 if TYPE_CHECKING:
     # relative
@@ -344,14 +347,26 @@
                 "type": "clipboard",
             },
             "Status": status_badge,
             "Submit time": str(self.submit_time),
         }
 
     @property
+    def user(self) -> UserView | SyftError:
+        api = APIRegistry.api_for(
+            node_uid=self.syft_node_location,
+            user_verify_key=self.syft_client_verify_key,
+        )
+        if api is None:
+            return SyftError(
+                message=f"Can't access Syft API. You must login to {self.syft_node_location}"
+            )
+        return api.services.user.get_by_verify_key(self.user_verify_key)
+
+    @property
     def status(self) -> UserCodeStatusCollection | SyftError:
         # Clientside only
         res = self.status_link.resolve
         return res
 
     def get_status(
         self, context: AuthedServiceContext
@@ -765,23 +780,38 @@
             values["id"] = UID()
         return values
 
     @property
     def kwargs(self) -> dict[Any, Any] | None:
         return self.input_policy_init_kwargs
 
-    def __call__(self, *args: Any, syft_no_node: bool = False, **kwargs: Any) -> Any:
+    def __call__(
+        self,
+        *args: Any,
+        syft_no_node: bool = False,
+        blocking: bool = False,
+        time_alive: int | None = None,
+        n_consumers: int = 2,
+        **kwargs: Any,
+    ) -> Any:
         if syft_no_node:
             return self.local_call(*args, **kwargs)
-        return self._ephemeral_node_call(*args, **kwargs)
+        return self._ephemeral_node_call(
+            *args,
+            time_alive=time_alive,
+            n_consumers=n_consumers,
+            blocking=blocking,
+            **kwargs,
+        )
 
     def local_call(self, *args: Any, **kwargs: Any) -> Any:
         # only run this on the client side
         if self.local_function:
-            tree = ast.parse(inspect.getsource(self.local_function))
+            source = dedent(inspect.getsource(self.local_function))
+            tree = ast.parse(source)
 
             # check there are no globals
             v = GlobalsVisitor()
             v.visit(tree)
 
             # filtered_args = []
             filtered_kwargs = {}
@@ -798,43 +828,36 @@
                 print("Warning: The result you see is computed on MOCK data.")
             return self.local_function(**filtered_kwargs)
         else:
             raise NotImplementedError
 
     def _ephemeral_node_call(
         self,
-        time_alive: int | None = None,
-        n_consumers: int | None = None,
         *args: Any,
+        time_alive: int | None = None,
+        n_consumers: int = 2,
+        blocking: bool = False,
         **kwargs: Any,
     ) -> Any:
         # relative
-        from ... import _orchestra
+        from ...orchestra import Orchestra
 
         # Right now we only create a number of workers
         # In the future we might need to have the same pools/images as well
 
-        if n_consumers is None:
-            print(
-                SyftInfo(
-                    message="Creating a node with n_consumers=2 (the default value)"
-                )
-            )
-            n_consumers = 2
-
-        if time_alive is None and "blocking" in kwargs and not kwargs["blocking"]:
+        if time_alive is None and not blocking:
             print(
                 SyftInfo(
                     message="Closing the node after time_alive=300 (the default value)"
                 )
             )
             time_alive = 300
 
         # This could be changed given the work on containers
-        ep_node = _orchestra().launch(
+        ep_node = Orchestra.launch(
             name=f"ephemeral_node_{self.func_name}_{random.randint(a=0, b=10000)}",  # nosec
             reset=True,
             create_producer=True,
             n_consumers=n_consumers,
             deploy_to="python",
         )
         ep_client = ep_node.login(email="info@openmined.org", password="changethis")  # nosec
@@ -947,34 +970,37 @@
     output_policy: OutputPolicy | UID | None = None,
     share_results_with_owners: bool = False,
     worker_pool_name: str | None = None,
 ) -> Callable:
     if input_policy is None:
         input_policy = EmpyInputPolicy()
 
+    init_input_kwargs = None
     if isinstance(input_policy, CustomInputPolicy):
         input_policy_type = SubmitUserPolicy.from_obj(input_policy)
+        init_input_kwargs = partition_by_node(input_policy.init_kwargs)
     else:
         input_policy_type = type(input_policy)
+        init_input_kwargs = getattr(input_policy, "init_kwargs", {})
 
     if output_policy is None:
         output_policy = SingleExecutionExactOutput()
 
     if isinstance(output_policy, CustomOutputPolicy):
         output_policy_type = SubmitUserPolicy.from_obj(output_policy)
     else:
         output_policy_type = type(output_policy)
 
     def decorator(f: Any) -> SubmitUserCode:
         res = SubmitUserCode(
-            code=inspect.getsource(f),
+            code=dedent(inspect.getsource(f)),
             func_name=f.__name__,
             signature=inspect.signature(f),
             input_policy_type=input_policy_type,
-            input_policy_init_kwargs=getattr(input_policy, "init_kwargs", {}),
+            input_policy_init_kwargs=init_input_kwargs,
             output_policy_type=output_policy_type,
             output_policy_init_kwargs=getattr(output_policy, "init_kwargs", {}),
             local_function=f,
             input_kwargs=f.__code__.co_varnames[: f.__code__.co_argcount],
             worker_pool_name=worker_pool_name,
         )
```

### Comparing `syft-0.8.7b7/src/syft/service/code/user_code_parse.py` & `syft-0.8.7b8/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/code/user_code_service.py` & `syft-0.8.7b8/src/syft/service/code/user_code_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -394,28 +394,50 @@
         kwargs.pop("result_id", None)
         result = self._call(context, uid, **kwargs)
         if result.is_err():
             return SyftError(message=result.err())
         else:
             return result.ok()
 
+    def valid_worker_pool_for_context(
+        self, context: AuthedServiceContext, user_code: UserCode
+    ) -> bool:
+        """This is a temporary fix that is needed until every function is always just ran as job"""
+        # relative
+        from ...node.node import get_default_worker_pool_name
+
+        has_custom_worker_pool = (
+            user_code.worker_pool_name is not None
+        ) and user_code.worker_pool_name != get_default_worker_pool_name()
+        if has_custom_worker_pool and context.is_blocking_api_call:
+            return False
+        else:
+            return True
+
     def _call(
         self,
         context: AuthedServiceContext,
         uid: UID,
         result_id: UID | None = None,
         **kwargs: Any,
     ) -> Result[ActionObject, Err]:
         """Call a User Code Function"""
         try:
             code_result = self.stash.get_by_uid(context.credentials, uid=uid)
             if code_result.is_err():
                 return code_result
             code: UserCode = code_result.ok()
 
+            if not self.valid_worker_pool_for_context(context, code):
+                return Err(
+                    value="You tried to run a syft function attached to a worker pool in blocking mode,"
+                    "which is currently not supported. Run your function with `blocking=False` to run"
+                    " as a job on your worker pool"
+                )
+
             # Set Permissions
             if self.is_execution_on_owned_args(kwargs, context):
                 if self.is_execution_on_owned_args_allowed(context):
                     # handles the case: if we have 1 or more owned args and execution permission
                     # handles the case: if we have 0 owned args and execution permission
                     context.has_execute_permissions = True
                 elif len(kwargs) == 0:
```

### Comparing `syft-0.8.7b7/src/syft/service/code/user_code_stash.py` & `syft-0.8.7b8/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/code/utils.py` & `syft-0.8.7b8/src/syft/service/code/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/code_history/code_history.py` & `syft-0.8.7b8/src/syft/service/code_history/code_history.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from ...client.api import APIRegistry
 from ...client.enclave_client import EnclaveMetadata
 from ...serde.serializable import serializable
 from ...service.user.user_roles import ServiceRole
 from ...types.syft_object import SYFT_OBJECT_VERSION_2
 from ...types.syft_object import SyftObject
 from ...types.syft_object import SyftVerifyKey
-from ...types.syft_object import get_repr_values_table
 from ...types.uid import UID
-from ...util.notebook_ui.notebook_addons import create_table_template
+from ...util.notebook_ui.components.table_template import create_table_template
+from ...util.table import prepare_table_data
 from ..code.user_code import UserCode
 from ..response import SyftError
 
 
 @serializable()
 class CodeHistory(SyftObject):
     # version
@@ -51,24 +51,25 @@
     service_func_name: str
     comment_history: list[str] = []
 
     def _coll_repr_(self) -> dict[str, int]:
         return {"Number of versions": len(self.user_code_history)}
 
     def _repr_html_(self) -> str:
-        rows = get_repr_values_table(self.user_code_history, True)
+        # TODO techdebt: move this to _coll_repr_
+        rows, _ = prepare_table_data(self.user_code_history)
         for i, r in enumerate(rows):
             r["Version"] = f"v{i}"
             raw_code = self.user_code_history[i].raw_code
             n_code_lines = raw_code.count("\n")
             if n_code_lines > 5:
                 raw_code = "\n".join(raw_code.split("\n", 5))
             r["Code"] = raw_code
         # rows = sorted(rows, key=lambda x: x["Version"])
-        return create_table_template(rows, "CodeHistory", table_icon=None)
+        return create_table_template(rows, "CodeHistory", icon=None)
 
     def __getitem__(self, index: int | str) -> UserCode | SyftError:
         if isinstance(index, str):
             raise TypeError(f"index {index} must be an integer, not a string")
         api = APIRegistry.api_for(self.syft_node_location, self.syft_client_verify_key)
         if api is None:
             return SyftError(
@@ -135,8 +136,8 @@
             )
         return api.services.code_history.get_history_for_user(key)
 
     def _repr_html_(self) -> str:
         rows = []
         for user, funcs in self.user_dict.items():
             rows += [{"user": user, "UserCodes": funcs}]
-        return create_table_template(rows, "UserCodeHistory", table_icon=None)
+        return create_table_template(rows, "UserCodeHistory", icon=None)
```

### Comparing `syft-0.8.7b7/src/syft/service/code_history/code_history_service.py` & `syft-0.8.7b8/src/syft/service/code_history/code_history_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/code_history/code_history_stash.py` & `syft-0.8.7b8/src/syft/service/code_history/code_history_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/context.py` & `syft-0.8.7b8/src/syft/service/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     __version__ = SYFT_OBJECT_VERSION_2
 
     credentials: SyftVerifyKey
     role: ServiceRole = ServiceRole.NONE
     job_id: UID | None = None
     extra_kwargs: dict = {}
     has_execute_permissions: bool = False
+    is_blocking_api_call: bool = False
 
     @property
     def dev_mode(self) -> Any:
         return self.node.dev_mode  # type: ignore
 
     def capabilities(self) -> list[ServiceRoleCapability]:
         return ROLE_TO_CAPABILITIES.get(self.role, [])
```

### Comparing `syft-0.8.7b7/src/syft/service/data_subject/data_subject.py` & `syft-0.8.7b8/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.7b8/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.7b8/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.7b8/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/dataset/dataset.py` & `syft-0.8.7b8/src/syft/service/dataset/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # stdlib
 from collections.abc import Callable
 from datetime import datetime
 from enum import Enum
+import textwrap
 from typing import Any
 
 # third party
 from IPython.display import HTML
 from IPython.display import display
 import itables
 import pandas as pd
@@ -29,29 +30,25 @@
 from ...types.transforms import transform
 from ...types.transforms import validate_url
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import ON_SURFACE_HIGHEST
 from ...util.colors import SURFACE
 from ...util.colors import SURFACE_SURFACE
-from ...util.fonts import FONT_CSS
-from ...util.fonts import ITABLES_CSS
 from ...util.markdown import as_markdown_python_code
-from ...util.notebook_ui.notebook_addons import FOLDER_ICON
-from ...util.util import get_mb_size
+from ...util.notebook_ui.icons import Icon
+from ...util.notebook_ui.styles import FONT_CSS
+from ...util.notebook_ui.styles import ITABLES_CSS
 from ..data_subject.data_subject import DataSubject
 from ..data_subject.data_subject import DataSubjectCreate
 from ..data_subject.data_subject_service import DataSubjectService
 from ..response import SyftError
 from ..response import SyftException
 from ..response import SyftSuccess
 
-DATA_SIZE_WARNING_LIMIT = 512
-
-
 NamePartitionKey = PartitionKey(key="name", type_=str)
 
 
 @serializable()
 class Contributor(SyftObject):
     __canonical_name__ = "Contributor"
     __version__ = SYFT_OBJECT_VERSION_2
@@ -325,16 +322,18 @@
     mock_is_real: bool = False
     created_at: DateTime | None = None
     uploader: Contributor | None = None
 
     __repr_attrs__ = ["name"]
     model_config = ConfigDict(validate_assignment=True)
 
-    def __init__(self, description: str | None = "", **data: Any) -> None:
-        super().__init__(**data, description=MarkdownDescription(text=str(description)))
+    def __init__(self, description: str | None = None, **data: Any) -> None:
+        if isinstance(description, str):
+            description = MarkdownDescription(text=description)
+        super().__init__(**data, description=description)
 
     @model_validator(mode="after")
     def __mock_is_real_for_empty_mock_must_be_false(self) -> Self:
         if self.mock_is_real and (
             self.mock is None or _is_action_data_empty(self.mock)
         ):
             self.__dict__["mock_is_real"] = False
@@ -404,21 +403,14 @@
         # if not _is_action_data_empty(self.mock):
         #     data_shape = get_shape_or_len(self.data)
         #     mock_shape = get_shape_or_len(self.mock)
         #     if data_shape != mock_shape:
         #         return SyftError(
         #             message=f"set_obj shape {data_shape} must match set_mock shape {mock_shape}"
         #         )
-        total_size_mb = get_mb_size(self.data) + get_mb_size(self.mock)
-        if total_size_mb > DATA_SIZE_WARNING_LIMIT:
-            print(
-                f"**WARNING**: The total size for asset: '{self.name}' exceeds '{DATA_SIZE_WARNING_LIMIT} MB'. "
-                "This might result in failure to upload dataset. "
-                "Please contact #support on OpenMined slack for further assistance.",
-            )
 
         return SyftSuccess(message="Dataset is Valid")
 
 
 def get_shape_or_len(obj: Any) -> tuple[int, ...] | int | None:
     if hasattr(obj, "shape"):
         shape = getattr(obj, "shape", None)
@@ -452,35 +444,36 @@
     mb_size: float | None = None
     created_at: DateTime = DateTime.now()
     uploader: Contributor
 
     __attr_searchable__ = ["name", "citation", "url", "description", "action_ids"]
     __attr_unique__ = ["name"]
     __repr_attrs__ = ["name", "url", "created_at"]
+    __table_sort_attr__ = "Created at"
 
     def __init__(
         self,
         description: str | MarkdownDescription | None = "",
         **data: Any,
     ) -> None:
         if isinstance(description, str):
             description = MarkdownDescription(text=description)
         super().__init__(**data, description=description)
 
     @property
     def icon(self) -> str:
-        return FOLDER_ICON
+        return Icon.FOLDER.svg
 
     def _coll_repr_(self) -> dict[str, Any]:
         return {
             "Name": self.name,
             "Assets": len(self.asset_list),
             "Size": f"{self.mb_size} (MB)",
             "Url": self.url,
-            "created at": str(self.created_at),
+            "Created at": str(self.created_at),
         }
 
     def _repr_html_(self) -> Any:
         uploaded_by_line = (
             (
                 "<p class='paragraph-sm'><strong>"
                 + f"<span class='pr-8'>Uploaded by:</span></strong>{self.uploader.name} ({self.uploader.email})</p>"
@@ -517,40 +510,23 @@
                 data.append(asset.action_id)
         return data
 
     @property
     def assets(self) -> DictTuple[str, Asset]:
         return DictTuple((asset.name, asset) for asset in self.asset_list)
 
-    def _old_repr_markdown_(self) -> str:
-        _repr_str = f"Syft Dataset: {self.name}\n"
-        _repr_str += "Assets:\n"
-        for asset in self.asset_list:
-            if asset.description is not None:
-                _repr_str += f"\t{asset.name}: {asset.description.text}\n\n"
-            else:
-                _repr_str += f"\t{asset.name}\n\n"
-        if self.citation:
-            _repr_str += f"Citation: {self.citation}\n"
-        if self.url:
-            _repr_str += f"URL: {self.url}\n"
-        if self.description:
-            _repr_str += f"Description: {self.description.text}\n"
-        return as_markdown_python_code(_repr_str)
-
     def _repr_markdown_(self, wrap_as_python: bool = True, indent: int = 0) -> str:
-        # return self._old_repr_markdown_()
-        return self._markdown_()
-
-    def _markdown_(self) -> str:
         _repr_str = f"Syft Dataset: {self.name}\n\n"
         _repr_str += "Assets:\n\n"
         for asset in self.asset_list:
             if asset.description is not None:
-                _repr_str += f"\t{asset.name}: {asset.description.text}\n\n"
+                description_text = textwrap.shorten(
+                    asset.description.text, width=100, placeholder="..."
+                )
+                _repr_str += f"\t{asset.name}: {description_text}\n\n"
             else:
                 _repr_str += f"\t{asset.name}\n\n"
         if self.citation:
             _repr_str += f"Citation: {self.citation}\n\n"
         if self.url:
             _repr_str += f"URL: {self.url}\n\n"
         if self.description:
```

### Comparing `syft-0.8.7b7/src/syft/service/dataset/dataset_service.py` & `syft-0.8.7b8/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.7b8/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/enclave/enclave_service.py` & `syft-0.8.7b8/src/syft/service/enclave/enclave_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/job/html_template.py` & `syft-0.8.7b8/src/syft/service/job/html_template.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # relative
-from ...util.notebook_ui.notebook_addons import CSS_CODE
-from ...util.notebook_ui.notebook_addons import JS_DOWNLOAD_FONTS
+from ...util.notebook_ui.styles import CSS_CODE
+from ...util.notebook_ui.styles import JS_DOWNLOAD_FONTS
 
 type_html = """
             <div class="label label-light-blue"
             style="display: flex; align-items:center; justify-content: center; width: 34px; height:21px; radius:4px;
                 padding: 2px, 6px, 2px, 6px">
             <span style="font-family: DejaVu Sans Mono, sans-serif;
                 font-size: 12px; font-weight: 400; line-height:16.8px">
@@ -150,55 +150,14 @@
         <div class="tablink-border-${identifier} log-tab-header">
             <a onclick="onClick_${identifier}(event, '${logs_tab_id}')" class='tablink-${identifier}'>Logs</a>
         </div>
     </div>
 </div>
 """
 
-LIST_CSS = """
-<style>
-    .syft-widget ul {
-        list-style-type: none;
-        margin: 0;
-        padding: 0;
-        overflow: hidden;
-    }
-
-    .syft-widget li {
-        float: left;
-        border-bottom: solid;
-        border-bottom-color: #CFCDD6;
-    }
-
-    .syft-widget li a {
-        display: block;
-        text-align: center;
-        padding: 14px 16px;
-        color: #CFCDD6
-    }
-    .log-tab-header{
-        border-bottom: solid 2px #ECEBEF;
-        padding: 4px 16px
-    }
-
-    .active-border {
-        border-bottom: solid 2px #1F567A;
-        font-weight: 700;
-    }
-
-    .active {
-        color: #1F567A
-    }
-
-    .syft-widget li a:hover {
-        background-color: #C2DEF0;
-    }
-</style>
-"""
-
 result_html = """<div id="${result_tab_id}" class="tab-${identifier}" style="background: #F4F3F6;
     border-color: #CFCDD6; border-width: 0.5px; border-style: solid; padding: 24px; gap: 8px; margin-top: 24px">
     <div style="font-size: 12px; font-weight: 400; font: DejaVu Sans Mono, sans-serif; line-height: 16.8px">
         ${result}
     </div>
 </div>
 """
@@ -211,18 +170,14 @@
 {JS_DOWNLOAD_FONTS}
 <!-- End JS_DOWNLOAD_FONTS -->
 
 <!-- Start CSS_CODE -->
 {CSS_CODE}
 <!-- End CSS_CODE -->
 
-<!-- Start LIST_CSS -->
-{LIST_CSS}
-<!-- End LIST_CSS -->
-
 <!-- Start header_line_html -->
 {header_line_html}
 <!-- End header_line_html -->
 
 <!-- Start attrs_html -->
 {attrs_html}
 <!-- End attrs_html -->
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-# relative from ...util.notebook_ui.notebook_addons import CSS_CODE from
-...util.notebook_ui.notebook_addons import JS_DOWNLOAD_FONTS type_html = """
+# relative from ...util.notebook_ui.styles import CSS_CODE from
+...util.notebook_ui.styles import JS_DOWNLOAD_FONTS type_html = """
 ${job_type}
 """ header_line_html = ( """
 ${api_header}
 """ + type_html + """ ${user_code_name}
 ${button_html}
 """ ) # noqa: E501 attrs_html = """
 UserCode: ${user_code_name}
@@ -14,14 +14,13 @@
 Subjobs: ${no_subjobs}
 """ logs_html = """
         ${logs_lines_html}
 """ # TODO: add style change for selected tab onclick_html = """
 """ tabs_html = """
 Result
 Logs
-""" LIST_CSS = """
 """ result_html = """
 ${result}
 """ job_repr_template = f"""
-{JS_DOWNLOAD_FONTS} {CSS_CODE} {LIST_CSS} {header_line_html} {attrs_html}
-{tabs_html} {result_html} {logs_html} {onclick_html}
+{JS_DOWNLOAD_FONTS} {CSS_CODE} {header_line_html} {attrs_html} {tabs_html}
+{result_html} {logs_html} {onclick_html}
 """
```

### Comparing `syft-0.8.7b7/src/syft/service/job/job_service.py` & `syft-0.8.7b8/src/syft/service/job/job_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # stdlib
+from collections.abc import Callable
+import inspect
+import time
 from typing import Any
 from typing import cast
 
 # relative
 from ...node.worker_settings import WorkerSettings
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
@@ -24,14 +27,26 @@
 from ..user.user_roles import DATA_SCIENTIST_ROLE_LEVEL
 from ..user.user_roles import GUEST_ROLE_LEVEL
 from .job_stash import Job
 from .job_stash import JobStash
 from .job_stash import JobStatus
 
 
+def wait_until(
+    predicate: Callable[[], bool], timeout: int = 10
+) -> SyftSuccess | SyftError:
+    start = time.time()
+    code_string = inspect.getsource(predicate).strip()
+    while time.time() - start < timeout:
+        if predicate():
+            return SyftSuccess(message=f"Predicate {code_string} is True")
+        time.sleep(1)
+    return SyftError(message=f"Timeout reached for predicate {code_string}")
+
+
 @instrument
 @serializable()
 class JobService(AbstractService):
     store: DocumentStore
     stash: JobStash
 
     def __init__(self, store: DocumentStore) -> None:
@@ -108,43 +123,59 @@
         path="job.restart",
         name="restart",
         roles=DATA_SCIENTIST_ROLE_LEVEL,
     )
     def restart(
         self, context: AuthedServiceContext, uid: UID
     ) -> SyftSuccess | SyftError:
-        res = self.stash.get_by_uid(context.credentials, uid=uid)
-        if res.is_err():
-            return SyftError(message=res.err())
+        job_or_err = self.stash.get_by_uid(context.credentials, uid=uid)
+        if job_or_err.is_err():
+            return SyftError(message=job_or_err.err())
+        if job_or_err.ok() is None:
+            return SyftError(message="Job not found")
+
+        job = job_or_err.ok()
+        if job.parent_job_id is not None:
+            return SyftError(
+                message="Not possible to restart subjobs. Please restart the parent job."
+            )
+        if job.status == JobStatus.PROCESSING:
+            return SyftError(
+                message="Jobs in progress cannot be restarted. "
+                "Please wait for completion or cancel the job via .cancel() to proceed."
+            )
 
-        job = res.ok()
         job.status = JobStatus.CREATED
         self.update(context=context, job=job)
 
         task_uid = UID()
         worker_settings = WorkerSettings.from_node(context.node)
+        worker_pool_ref = context.node.get_worker_pool_ref_by_name(context.credentials)
+        if isinstance(worker_pool_ref, SyftError):
+            return worker_pool_ref
 
         queue_item = ActionQueueItem(
             id=task_uid,
             node_uid=context.node.id,
             syft_client_verify_key=context.credentials,
             syft_node_location=context.node.id,
             job_id=job.id,
             worker_settings=worker_settings,
             args=[],
             kwargs={"action": job.action},
+            worker_pool=worker_pool_ref,
         )
 
         context.node.queue_stash.set_placeholder(context.credentials, queue_item)
         context.node.job_stash.set(context.credentials, job)
 
         log_service = context.node.get_service("logservice")
         result = log_service.restart(context, job.log_id)
-        if result.is_err():
-            return SyftError(message=str(result.err()))
+        if isinstance(result, SyftError):
+            return result
 
         return SyftSuccess(message="Great Success!")
 
     @service_method(
         path="job.update",
         name="update",
         roles=DATA_SCIENTIST_ROLE_LEVEL,
@@ -154,36 +185,70 @@
     ) -> SyftSuccess | SyftError:
         res = self.stash.update(context.credentials, obj=job)
         if res.is_err():
             return SyftError(message=res.err())
         res = res.ok()
         return SyftSuccess(message="Great Success!")
 
+    def _kill(self, context: AuthedServiceContext, job: Job) -> SyftSuccess | SyftError:
+        # set job and subjobs status to TERMINATING
+        # so that MonitorThread can kill them
+        job.status = JobStatus.TERMINATING
+        res = self.stash.update(context.credentials, obj=job)
+        results = [res]
+
+        # attempt to kill all subjobs
+        subjobs_or_err = self.stash.get_by_parent_id(context.credentials, uid=job.id)
+        if subjobs_or_err.is_ok() and subjobs_or_err.ok() is not None:
+            subjobs = subjobs_or_err.ok()
+            for subjob in subjobs:
+                subjob.status = JobStatus.TERMINATING
+                res = self.stash.update(context.credentials, obj=subjob)
+                results.append(res)
+
+        errors = [res.err() for res in results if res.is_err()]
+        if errors:
+            return SyftError(message=f"Failed to kill job: {errors}")
+
+        # wait for job and subjobs to be killed by MonitorThread
+        wait_until(lambda: job.fetched_status == JobStatus.INTERRUPTED)
+        wait_until(
+            lambda: all(
+                subjob.fetched_status == JobStatus.INTERRUPTED for subjob in job.subjobs
+            )
+        )
+
+        return SyftSuccess(message="Job killed successfully!")
+
     @service_method(
         path="job.kill",
         name="kill",
         roles=DATA_SCIENTIST_ROLE_LEVEL,
     )
     def kill(self, context: AuthedServiceContext, id: UID) -> SyftSuccess | SyftError:
-        res = self.stash.get_by_uid(context.credentials, uid=id)
-        if res.is_err():
-            return SyftError(message=res.err())
+        job_or_err = self.stash.get_by_uid(context.credentials, uid=id)
+        if job_or_err.is_err():
+            return SyftError(message=job_or_err.err())
+        if job_or_err.ok() is None:
+            return SyftError(message="Job not found")
 
-        job = res.ok()
-        if job.job_pid is not None and job.status == JobStatus.PROCESSING:
-            job.status = JobStatus.INTERRUPTED
-            res = self.stash.update(context.credentials, obj=job)
-            if res.is_err():
-                return SyftError(message=res.err())
-            return SyftSuccess(message="Job killed successfully!")
-        else:
+        job = job_or_err.ok()
+        if job.parent_job_id is not None:
             return SyftError(
-                message="Job is not running or isn't running in multiprocessing mode."
-                "Killing threads is currently not supported"
+                message="Not possible to cancel subjobs. To stop execution, please cancel the parent job."
             )
+        if job.status != JobStatus.PROCESSING:
+            return SyftError(message="Job is not running")
+        if job.job_pid is None:
+            return SyftError(
+                message="Job termination disabled in dev mode. "
+                "Set 'dev_mode=False' or 'thread_workers=False' to enable."
+            )
+
+        return self._kill(context, job)
 
     @service_method(
         path="job.get_subjobs",
         name="get_subjobs",
         roles=DATA_SCIENTIST_ROLE_LEVEL,
     )
     def get_subjobs(
```

### Comparing `syft-0.8.7b7/src/syft/service/job/job_stash.py` & `syft-0.8.7b8/src/syft/service/job/job_stash.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # stdlib
 from datetime import datetime
 from datetime import timedelta
+from datetime import timezone
 from enum import Enum
 import random
 from string import Template
 from typing import Any
 
 # third party
 from pydantic import Field
@@ -24,16 +25,17 @@
 from ...store.document_store import BaseStash
 from ...store.document_store import DocumentStore
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...store.document_store import QueryKeys
 from ...store.document_store import UIDPartitionKey
 from ...types.datetime import DateTime
+from ...types.datetime import format_timedelta
 from ...types.syft_object import SYFT_OBJECT_VERSION_2
-from ...types.syft_object import SYFT_OBJECT_VERSION_5
+from ...types.syft_object import SYFT_OBJECT_VERSION_6
 from ...types.syft_object import SyftObject
 from ...types.syncable_object import SyncableSyftObject
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import SURFACE
 from ...util.markdown import as_markdown_code
 from ...util.telemetry import instrument
@@ -50,14 +52,15 @@
 
 @serializable()
 class JobStatus(str, Enum):
     CREATED = "created"
     PROCESSING = "processing"
     ERRORED = "errored"
     COMPLETED = "completed"
+    TERMINATING = "terminating"
     INTERRUPTED = "interrupted"
 
 
 def center_content(text: Any) -> str:
     if isinstance(text, str):
         text = text.replace("\n", "<br>")
     center_div = f"""
@@ -69,34 +72,46 @@
     </div>
     """
     center_div = center_div.replace("\n", "")
     return center_div
 
 
 @serializable()
+class JobType(str, Enum):
+    JOB = "job"
+    TWINAPIJOB = "twinapijob"
+
+    def __str__(self) -> str:
+        return self.value
+
+
+@serializable()
 class Job(SyncableSyftObject):
     __canonical_name__ = "JobItem"
-    __version__ = SYFT_OBJECT_VERSION_5
+    __version__ = SYFT_OBJECT_VERSION_6
 
     id: UID
     node_uid: UID
     result: Any | None = None
     resolved: bool = False
     status: JobStatus = JobStatus.CREATED
     log_id: UID | None = None
     parent_job_id: UID | None = None
     n_iters: int | None = 0
     current_iter: int | None = None
-    creation_time: str | None = Field(default_factory=lambda: str(datetime.now()))
+    creation_time: str | None = Field(
+        default_factory=lambda: str(datetime.now(tz=timezone.utc))
+    )
     action: Action | None = None
     job_pid: int | None = None
     job_worker_id: UID | None = None
     updated_at: DateTime | None = None
     user_code_id: UID | None = None
     requested_by: UID | None = None
+    job_type: JobType = JobType.JOB
 
     __attr_searchable__ = ["parent_job_id", "job_worker_id", "status", "user_code_id"]
     __repr_attrs__ = [
         "id",
         "result",
         "resolved",
         "progress",
@@ -186,26 +201,15 @@
             self.current_iter is None
             or self.current_iter == 0
             or self.n_iters is None
             or self.creation_time is None
         ):
             return None
 
-        def format_timedelta(local_timedelta: timedelta) -> str:
-            total_seconds = int(local_timedelta.total_seconds())
-            hours, leftover = divmod(total_seconds, 3600)
-            minutes, seconds = divmod(leftover, 60)
-
-            hours_string = f"{hours}:" if hours != 0 else ""
-            minutes_string = f"{minutes}:".zfill(3)
-            seconds_string = f"{seconds}".zfill(2)
-
-            return f"{hours_string}{minutes_string}{seconds_string}"
-
-        now = datetime.now()
+        now = datetime.now(tz=timezone.utc)
         time_passed = now - datetime.fromisoformat(self.creation_time)
         iter_duration_seconds: float = time_passed.total_seconds() / self.current_iter
         iters_remaining = self.n_iters - self.current_iter
 
         # TODO: Adjust by the number of consumers
         time_remaining = timedelta(seconds=iters_remaining * iter_duration_seconds)
         time_passed_str = format_timedelta(time_passed)
@@ -250,70 +254,52 @@
             for attr in info.__public_metadata_attrs__:
                 setattr(self, attr, getattr(info, attr))
 
         if info.includes_result:
             self.result = info.result
 
     def restart(self, kill: bool = False) -> None:
-        if kill:
-            self.kill()
-        self.fetch()
-        if not self.has_parent:
-            # this is currently the limitation, we will need to implement
-            # killing toplevel jobs later
-            print("Can only kill nested jobs")
-        elif kill or (
-            self.status != JobStatus.PROCESSING and self.status != JobStatus.CREATED
-        ):
-            api = APIRegistry.api_for(
-                node_uid=self.syft_node_location,
-                user_verify_key=self.syft_client_verify_key,
-            )
-            if api is None:
-                raise ValueError(
-                    f"Can't access Syft API. You must login to {self.syft_node_location}"
-                )
-            call = SyftAPICall(
-                node_uid=self.node_uid,
-                path="job.restart",
-                args=[],
-                kwargs={"uid": self.id},
-                blocking=True,
-            )
-
-            api.make_call(call)
-        else:
-            print(
-                "Job is running or scheduled, if you want to kill it use job.kill() first"
+        api = APIRegistry.api_for(
+            node_uid=self.syft_node_location,
+            user_verify_key=self.syft_client_verify_key,
+        )
+        if api is None:
+            raise ValueError(
+                f"Can't access Syft API. You must login to {self.syft_node_location}"
             )
-        return None
+        call = SyftAPICall(
+            node_uid=self.node_uid,
+            path="job.restart",
+            args=[],
+            kwargs={"uid": self.id},
+            blocking=True,
+        )
+        res = api.make_call(call)
+        self.fetch()
+        return res
 
-    def kill(self) -> SyftError | None:
-        if self.job_pid is not None:
-            api = APIRegistry.api_for(
-                node_uid=self.syft_node_location,
-                user_verify_key=self.syft_client_verify_key,
-            )
-            if api is None:
-                return SyftError(
-                    message=f"Can't access Syft API. You must login to {self.syft_node_location}"
-                )
-            call = SyftAPICall(
-                node_uid=self.node_uid,
-                path="job.kill",
-                args=[],
-                kwargs={"id": self.id},
-                blocking=True,
-            )
-            api.make_call(call)
-            return None
-        else:
+    def kill(self) -> SyftError | SyftSuccess:
+        api = APIRegistry.api_for(
+            node_uid=self.syft_node_location,
+            user_verify_key=self.syft_client_verify_key,
+        )
+        if api is None:
             return SyftError(
-                message="Job is not running or isn't running in multiprocessing mode."
+                message=f"Can't access Syft API. You must login to {self.syft_node_location}"
             )
+        call = SyftAPICall(
+            node_uid=self.node_uid,
+            path="job.kill",
+            args=[],
+            kwargs={"id": self.id},
+            blocking=True,
+        )
+        res = api.make_call(call)
+        self.fetch()
+        return res
 
     def fetch(self) -> None:
         api = APIRegistry.api_for(
             node_uid=self.syft_node_location,
             user_verify_key=self.syft_client_verify_key,
         )
         if api is None:
@@ -323,15 +309,17 @@
         call = SyftAPICall(
             node_uid=self.node_uid,
             path="job.get",
             args=[],
             kwargs={"uid": self.id},
             blocking=True,
         )
-        job: Job = api.make_call(call)
+        job: Job | None = api.make_call(call)
+        if job is None:
+            return
         self.resolved = job.resolved
         if job.resolved:
             self.result = job.result
 
         self.status = job.status
         self.n_iters = job.n_iters
         self.current_iter = job.current_iter
@@ -494,18 +482,18 @@
 
         def default_value(value: str) -> str:
             return value if value else "--"
 
         return {
             "Status": self.status_badge(),
             "Job": self.summary_html(),
-            "# Subjobs": center_content(default_value(len(subjobs))),
-            "Progress": center_content(default_value(self.progress)),
-            "ETA": center_content(default_value(self.eta_string)),
-            "Logs": center_content(default_value(logs)),
+            "# Subjobs": default_value(len(subjobs)),
+            "Progress": default_value(self.progress),
+            "ETA": default_value(self.eta_string),
+            "Logs": default_value(logs),
         }
 
     @property
     def has_parent(self) -> bool:
         return self.parent_job_id is not None
 
     def _repr_markdown_(self, wrap_as_python: bool = True, indent: int = 0) -> str:
@@ -527,14 +515,19 @@
     logs:
 
 {logs_w_linenr}
     """
         return as_markdown_code(md)
 
     @property
+    def fetched_status(self) -> JobStatus:
+        self.fetch()
+        return self.status
+
+    @property
     def requesting_user(self) -> UserView | SyftError:
         api = APIRegistry.api_for(
             node_uid=self.syft_node_location,
             user_verify_key=self.syft_client_verify_key,
         )
         if api is None:
             return SyftError(
```

### Comparing `syft-0.8.7b7/src/syft/service/log/log.py` & `syft-0.8.7b8/src/syft/service/log/log.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/log/log_service.py` & `syft-0.8.7b8/src/syft/service/log/log_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/log/log_stash.py` & `syft-0.8.7b8/src/syft/service/log/log_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/metadata/metadata_service.py` & `syft-0.8.7b8/src/syft/service/metadata/metadata_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/metadata/migrations.py` & `syft-0.8.7b8/src/syft/service/metadata/migrations.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/metadata/node_metadata.py` & `syft-0.8.7b8/src/syft/service/metadata/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/network/association_request.py` & `syft-0.8.7b8/src/syft/service/network/association_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     def _run(
         self, context: ChangeContext, apply: bool
     ) -> Result[tuple[bytes, NodePeer], SyftError]:
         # relative
         from .network_service import NetworkService
 
         if not apply:
+            # TODO: implement undo for AssociationRequestChange
             return Err(
                 SyftError(message="Undo not supported for AssociationRequestChange")
             )
 
         service_ctx = context.to_service_ctx()
 
         try:
```

### Comparing `syft-0.8.7b7/src/syft/service/network/network_service.py` & `syft-0.8.7b8/src/syft/service/network/network_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # stdlib
 from collections.abc import Callable
+from enum import Enum
 import secrets
 from typing import Any
 
 # third party
 from result import Err
 from result import Result
 
@@ -30,14 +31,15 @@
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ...util.util import prompt_warning_message
 from ..context import AuthedServiceContext
 from ..data_subject.data_subject import NamePartitionKey
 from ..metadata.node_metadata import NodeMetadataV3
 from ..request.request import Request
+from ..request.request import RequestStatus
 from ..request.request import SubmitRequest
 from ..request.request_service import RequestService
 from ..response import SyftError
 from ..response import SyftInfo
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
@@ -54,14 +56,21 @@
 from .routes import PythonNodeRoute
 
 VerifyKeyPartitionKey = PartitionKey(key="verify_key", type_=SyftVerifyKey)
 NodeTypePartitionKey = PartitionKey(key="node_type", type_=NodeType)
 OrderByNamePartitionKey = PartitionKey(key="name", type_=str)
 
 
+@serializable()
+class NodePeerAssociationStatus(Enum):
+    PEER_ASSOCIATED = "PEER_ASSOCIATED"
+    PEER_ASSOCIATION_PENDING = "PEER_ASSOCIATION_PENDING"
+    PEER_NOT_FOUND = "PEER_NOT_FOUND"
+
+
 @instrument
 @serializable()
 class NetworkStash(BaseUIDStoreStash):
     object_type = NodePeer
     settings: PartitionSettings = PartitionSettings(
         name=NodePeer.__canonical_name__, object_type=NodePeer
     )
@@ -151,53 +160,118 @@
     )
     def exchange_credentials_with(
         self,
         context: AuthedServiceContext,
         self_node_route: NodeRoute,
         remote_node_route: NodeRoute,
         remote_node_verify_key: SyftVerifyKey,
-    ) -> SyftSuccess | SyftError:
-        """Exchange Route With Another Node"""
+    ) -> Request | SyftSuccess | SyftError:
+        """
+        Exchange Route With Another Node. If there is a pending association request, return it
+        """
 
         # Step 1: Validate the Route
         self_node_peer = self_node_route.validate_with_context(context=context)
 
         if isinstance(self_node_peer, SyftError):
             return self_node_peer
 
         # Step 2: Send the Node Peer to the remote node
         # Also give them their own to validate that it belongs to them
         # random challenge prevents replay attacks
         remote_client: SyftClient = remote_node_route.client_with_context(
             context=context
         )
-        random_challenge = secrets.token_bytes(16)
+        remote_node_peer = NodePeer.from_client(remote_client)
+
+        # check locally if the remote node already exists as a peer
+        existing_peer_result = self.stash.get_by_uid(
+            context.node.verify_key, remote_node_peer.id
+        )
+        if (
+            existing_peer_result.is_ok()
+            and (existing_peer := existing_peer_result.ok()) is not None
+        ):
+            msg = [
+                (
+                    f"{existing_peer.node_type} peer '{existing_peer.name}' already exist for "
+                    f"{self_node_peer.node_type} '{self_node_peer.name}'."
+                )
+            ]
+            if existing_peer != remote_node_peer:
+                result = self.stash.create_or_update_peer(
+                    context.node.verify_key,
+                    remote_node_peer,
+                )
+                msg.append(
+                    f"{existing_peer.node_type} peer '{existing_peer.name}' information change detected."
+                )
+                if result.is_err():
+                    msg.append(
+                        f"Attempt to update peer '{existing_peer.name}' information failed."
+                    )
+                    return SyftError(message="\n".join(msg))
+                msg.append(
+                    f"{existing_peer.node_type} peer '{existing_peer.name}' information successfully updated."
+                )
+
+            # Also check remotely if the self node already exists as a peer
+            remote_self_node_peer = remote_client.api.services.network.get_peer_by_name(
+                name=self_node_peer.name
+            )
+            if isinstance(remote_self_node_peer, NodePeer):
+                msg.append(
+                    f"{self_node_peer.node_type} '{self_node_peer.name}' already exist "
+                    f"as a peer for {remote_node_peer.node_type} '{remote_node_peer.name}'."
+                )
+                if remote_self_node_peer != self_node_peer:
+                    result = remote_client.api.services.network.update_peer(
+                        peer=self_node_peer,
+                    )
+                    msg.append(
+                        f"{self_node_peer.node_type} peer '{self_node_peer.name}' information change detected."
+                    )
+                    if isinstance(result, SyftError):
+                        msg.apnpend(
+                            f"Attempt to remotely update {self_node_peer.node_type} peer "
+                            f"'{self_node_peer.name}' information remotely failed."
+                        )
+                        return SyftError(message="\n".join(msg))
+                    msg.append(
+                        f"{self_node_peer.node_type} peer '{self_node_peer.name}' "
+                        f"information successfully updated."
+                    )
+                msg.append(
+                    f"Routes between {remote_node_peer.node_type} '{remote_node_peer.name}' and "
+                    f"{self_node_peer.node_type} '{self_node_peer.name}' already exchanged."
+                )
+                return SyftSuccess(message="\n".join(msg))
 
-        # ask the remote client to add this node (represented by `self_node_peer`) as a peer
+        # If  peer does not exist, ask the remote client to add this node
+        # (represented by `self_node_peer`) as a peer
+        random_challenge = secrets.token_bytes(16)
         remote_res = remote_client.api.services.network.add_peer(
             peer=self_node_peer,
             challenge=random_challenge,
             self_node_route=remote_node_route,
             verify_key=remote_node_verify_key,
         )
 
         if isinstance(remote_res, SyftError):
             return remote_res
 
         association_request_approved = not isinstance(remote_res, Request)
 
-        remote_node_peer = NodePeer.from_client(remote_client)
-
         # save the remote peer for later
         result = self.stash.create_or_update_peer(
             context.node.verify_key,
             remote_node_peer,
         )
         if result.is_err():
-            return SyftError(message=str(result.err()))
+            return SyftError(message="Failed to update route information.")
 
         return (
             SyftSuccess(message="Routes Exchanged")
             if association_request_approved
             else remote_res
         )
 
@@ -205,15 +279,15 @@
     def add_peer(
         self,
         context: AuthedServiceContext,
         peer: NodePeer,
         challenge: bytes,
         self_node_route: NodeRoute,
         verify_key: SyftVerifyKey,
-    ) -> list | SyftError:
+    ) -> Request | SyftSuccess | SyftError:
         """Add a Network Node Peer. Called by a remote node to add
         itself as a peer for the current node.
         """
         # Using the verify_key of the peer to verify the signature
         # It is also our single source of truth for the peer
         if peer.verify_key != context.credentials:
             return SyftError(
@@ -224,27 +298,63 @@
             )
 
         if verify_key != context.node.verify_key:
             return SyftError(
                 message="verify_key does not match the remote node's verify_key for add_peer"
             )
 
+        # check if the peer already is a node peer
+        existing_peer_res = self.stash.get_by_uid(context.node.verify_key, peer.id)
+        if existing_peer_res.is_err():
+            return SyftError(
+                message=f"Failed to query peer from stash: {existing_peer_res.err()}"
+            )
+
+        if isinstance(existing_peer := existing_peer_res.ok(), NodePeer):
+            msg = [
+                f"The peer '{peer.name}' is already associated with '{context.node.name}'"
+            ]
+
+            if existing_peer != peer:
+                result = self.stash.create_or_update_peer(
+                    context.node.verify_key,
+                    peer,
+                )
+                msg.append("Peer information change detected.")
+
+                if result.is_err():
+                    msg.append("Attempt to update peer information failed.")
+                    return SyftError(message="\n".join(msg))
+
+                msg.append("Peer information successfully updated.")
+                return SyftSuccess(message="\n".join(msg))
+
+            return SyftSuccess(message="\n".join(msg))
+
+        # check if the peer already submitted an association request
+        association_requests: list[Request] = self._get_association_requests_by_peer_id(
+            context=context, peer_id=peer.id
+        )
+        if (
+            association_requests
+            and (association_request := association_requests[-1]).status
+            == RequestStatus.PENDING
+        ):
+            return association_request
+        # only create and submit a new request if there is no requests yet
+        # or all previous requests have been rejected
         association_request_change = AssociationRequestChange(
             self_node_route=self_node_route, challenge=challenge, remote_peer=peer
         )
-
         submit_request = SubmitRequest(
             changes=[association_request_change],
             requesting_user_verify_key=context.credentials,
         )
-
         request_submit_method = context.node.get_service_method(RequestService.submit)
-
         request = request_submit_method(context, submit_request)
-
         if (
             isinstance(request, Request)
             and context.node.settings.association_request_auto_approval
         ):
             request_apply_method = context.node.get_service_method(RequestService.apply)
             return request_apply_method(context, uid=request.id)
 
@@ -266,14 +376,46 @@
         challenge_signature = context.node.signing_key.signing_key.sign(
             challenge
         ).signature
 
         return challenge_signature
 
     @service_method(
+        path="network.check_peer_association",
+        name="check_peer_association",
+        roles=GUEST_ROLE_LEVEL,
+    )
+    def check_peer_association(
+        self, context: AuthedServiceContext, peer_id: UID
+    ) -> NodePeerAssociationStatus | SyftError:
+        """Check if a peer exists in the network stash"""
+
+        # get the node peer for the given sender peer_id
+        peer = self.stash.get_by_uid(context.node.verify_key, peer_id)
+        if err := peer.is_err():
+            return SyftError(message=f"Failed to query peer from stash. Err: {err}")
+
+        if isinstance(peer.ok(), NodePeer):
+            return NodePeerAssociationStatus.PEER_ASSOCIATED
+
+        if peer.ok() is None:  # peer is either pending or not found
+            association_requests: list[Request] = (
+                self._get_association_requests_by_peer_id(
+                    context=context, peer_id=peer_id
+                )
+            )
+            if (
+                association_requests
+                and association_requests[-1].status == RequestStatus.PENDING
+            ):
+                return NodePeerAssociationStatus.PEER_ASSOCIATION_PENDING
+
+        return NodePeerAssociationStatus.PEER_NOT_FOUND
+
+    @service_method(
         path="network.get_all_peers", name="get_all_peers", roles=GUEST_ROLE_LEVEL
     )
     def get_all_peers(
         self, context: AuthedServiceContext
     ) -> list[NodePeer] | SyftError:
         """Get all Peers"""
 
@@ -319,28 +461,59 @@
         if result.is_err():
             return SyftError(message=str(result.err()))
 
         # Return peers or an empty list when result is None
         return result.ok() or []
 
     @service_method(
+        path="network.update_peer", name="update_peer", roles=GUEST_ROLE_LEVEL
+    )
+    def update_peer(
+        self,
+        context: AuthedServiceContext,
+        peer: NodePeer,
+    ) -> SyftSuccess | SyftError:
+        result = self.stash.update(
+            credentials=context.node.verify_key,
+            peer=peer,
+        )
+        if result.is_err():
+            return SyftError(
+                message=f"Failed to update peer '{peer.name}'. Error: {result.err()}"
+            )
+        return SyftSuccess(
+            message=f"Peer '{result.ok().name}' information successfully updated."
+        )
+
+    @service_method(
         path="network.delete_peer_by_id",
         name="delete_peer_by_id",
         roles=DATA_OWNER_ROLE_LEVEL,
     )
     def delete_peer_by_id(
         self, context: AuthedServiceContext, uid: UID
     ) -> SyftSuccess | SyftError:
         """Delete Node Peer"""
         result = self.stash.delete_by_uid(context.credentials, uid)
-        if result.is_err():
-            return SyftError(message=str(result.err()))
+        if err := result.is_err():
+            return SyftError(message=f"Failed to delete peer with UID {uid}: {err}.")
+        # Delete all the association requests from this peer
+        association_requests: list[Request] = self._get_association_requests_by_peer_id(
+            context=context, peer_id=uid
+        )
+        for request in association_requests:
+            request_delete_method = context.node.get_service_method(
+                RequestService.delete_by_uid
+            )
+            res = request_delete_method(context, request.id)
+            if isinstance(res, SyftError):
+                return res
         # TODO: Notify the peer (either by email or by other form of notifications)
         # that it has been deleted from the network
-        return SyftSuccess(message=f"Node Peer with id {uid} Deleted")
+        return SyftSuccess(message=f"Node Peer with id {uid} deleted.")
 
     @service_method(path="network.add_route_on_peer", name="add_route_on_peer")
     def add_route_on_peer(
         self,
         context: AuthedServiceContext,
         peer: NodePeer,
         route: NodeRoute,
@@ -406,26 +579,26 @@
         remote_node_peer: NodePeer | SyftError = (
             self._get_remote_node_peer_by_verify_key(context, peer_verify_key)
         )
         if isinstance(remote_node_peer, SyftError):
             return remote_node_peer
         # add and update the priority for the peer
         existed_route: NodeRoute | None = remote_node_peer.update_route(route)
+        if existed_route:
+            return SyftSuccess(
+                message=f"The route already exists between '{context.node.name}' and "
+                f"peer '{remote_node_peer.name}' with id '{existed_route.id}'."
+            )
         # update the peer in the store with the updated routes
         result = self.stash.update(
             credentials=context.node.verify_key,
             peer=remote_node_peer,
         )
         if result.is_err():
             return SyftError(message=str(result.err()))
-        if existed_route:
-            return SyftSuccess(
-                message=f"The route already exists between '{context.node.name}' and "
-                f"peer '{remote_node_peer.name}' with id '{existed_route.id}', so its priority was updated"
-            )
         return SyftSuccess(
             message=f"New route ({str(route)}) with id '{route.id}' "
             f"to peer {remote_node_peer.node_type.value} '{remote_node_peer.name}' "
             f"was added for {str(context.node.node_type)} '{context.node.name}'"
         )
 
     @service_method(path="network.delete_route_on_peer", name="delete_route_on_peer")
@@ -476,15 +649,17 @@
             peer_verify_key=context.credentials,
             route=route,
             route_id=route_id,
             called_by_peer=True,
         )
         return result
 
-    @service_method(path="network.", name="delete_route", roles=GUEST_ROLE_LEVEL)
+    @service_method(
+        path="network.delete_route", name="delete_route", roles=GUEST_ROLE_LEVEL
+    )
     def delete_route(
         self,
         context: AuthedServiceContext,
         peer_verify_key: SyftVerifyKey,
         route: NodeRoute | None = None,
         route_id: UID | None = None,
         called_by_peer: bool = False,
@@ -698,14 +873,37 @@
         remote_node_peer = remote_node_peer.ok()
         if remote_node_peer is None:
             return SyftError(
                 message=f"Can't retrive {remote_node_peer.name} from the store of peers (None)."
             )
         return remote_node_peer
 
+    def _get_association_requests_by_peer_id(
+        self, context: AuthedServiceContext, peer_id: UID
+    ) -> list[Request]:
+        """
+        Get all the association requests from a peer. The association requests are sorted by request_time.
+        """
+        request_get_all_method: Callable = context.node.get_service_method(
+            RequestService.get_all
+        )
+        all_requests: list[Request] = request_get_all_method(context)
+        association_requests: list[Request] = []
+        for request in all_requests:
+            for change in request.changes:
+                if (
+                    isinstance(change, AssociationRequestChange)
+                    and change.remote_peer.id == peer_id
+                ):
+                    association_requests.append(request)
+
+        return sorted(
+            association_requests, key=lambda request: request.request_time.utc_timestamp
+        )
+
 
 TYPE_TO_SERVICE[NodePeer] = NetworkService
 SERVICE_TO_TYPES[NetworkService].update({NodePeer})
 
 
 def from_grid_url(context: TransformContext) -> TransformContext:
     if context.obj is not None and context.output is not None:
```

### Comparing `syft-0.8.7b7/src/syft/service/network/node_peer.py` & `syft-0.8.7b8/src/syft/service/network/node_peer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # stdlib
 from collections.abc import Callable
+from enum import Enum
 
 # third party
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
 from ...abstract_node import NodeType
 from ...client.client import NodeConnection
 from ...client.client import SyftClient
 from ...node.credentials import SyftSigningKey
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...service.response import SyftError
+from ...types.datetime import DateTime
 from ...types.syft_migration import migrate
 from ...types.syft_object import SYFT_OBJECT_VERSION_2
 from ...types.syft_object import SYFT_OBJECT_VERSION_3
 from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
 from ...types.uid import UID
 from ..context import NodeServiceContext
@@ -29,14 +31,21 @@
 from .routes import PythonNodeRoute
 from .routes import VeilidNodeRoute
 from .routes import connection_to_route
 from .routes import route_to_connection
 
 
 @serializable()
+class NodePeerConnectionStatus(Enum):
+    ACTIVE = "ACTIVE"
+    INACTIVE = "INACTIVE"
+    TIMEOUT = "TIMEOUT"
+
+
+@serializable()
 class NodePeerV2(SyftObject):
     # version
     __canonical_name__ = "NodePeer"
     __version__ = SYFT_OBJECT_VERSION_2
 
     __attr_searchable__ = ["name", "node_type"]
     __attr_unique__ = ["verify_key"]
@@ -54,22 +63,32 @@
 class NodePeer(SyftObject):
     # version
     __canonical_name__ = "NodePeer"
     __version__ = SYFT_OBJECT_VERSION_3
 
     __attr_searchable__ = ["name", "node_type"]
     __attr_unique__ = ["verify_key"]
-    __repr_attrs__ = ["name", "node_type", "admin_email"]
+    __repr_attrs__ = [
+        "name",
+        "node_type",
+        "admin_email",
+        "ping_status.value",
+        "ping_status_message",
+        "pinged_timestamp",
+    ]
 
     id: UID | None = None  # type: ignore[assignment]
     name: str
     verify_key: SyftVerifyKey
     node_routes: list[NodeRouteType] = []
     node_type: NodeType
     admin_email: str
+    ping_status: NodePeerConnectionStatus | None = None
+    ping_status_message: str | None = None
+    pinged_timestamp: DateTime | None = None
 
     def existed_route(
         self, route: NodeRouteType | None = None, route_id: UID | None = None
     ) -> tuple[bool, int | None]:
         """Check if a route exists in self.node_routes
 
         Args:
@@ -108,32 +127,32 @@
         Returns:
             NodeRoute: The new route with the updated priority
         """
         current_max_priority: int = max(route.priority for route in self.node_routes)
         route.priority = current_max_priority + 1
         return route
 
-    def update_route(self, new_route: NodeRoute) -> NodeRoute | None:
+    def update_route(self, route: NodeRoute) -> NodeRoute | None:
         """
         Update the route for the node.
-        If the route already exists, updates the priority of the existing route.
-        If it doesn't, it append the new route to the peer's list of node routes.
+        If the route already exists, return it.
+        If the route is new, assign it to have the highest priority
+        before appending it to the peer's list of node routes.
 
         Args:
-            new_route (NodeRoute): The new route to be added to the node.
+            route (NodeRoute): The new route to be added to the peer.
 
         Returns:
             NodeRoute | None: if the route already exists, return it, else returns None
         """
-        new_route = self.assign_highest_priority(new_route)
-        existed, index = self.existed_route(new_route)
-        if existed and index is not None:
-            self.node_routes[index].priority = new_route.priority
-            return self.node_routes[index]
+        existed, _ = self.existed_route(route)
+        if existed:
+            return route
         else:
+            new_route = self.assign_highest_priority(route)
             self.node_routes.append(new_route)
             return None
 
     def update_routes(self, new_routes: list[NodeRoute]) -> None:
         """
         Update multiple routes of the node peer.
```

### Comparing `syft-0.8.7b7/src/syft/service/network/routes.py` & `syft-0.8.7b8/src/syft/service/network/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/notification/email_templates.py` & `syft-0.8.7b8/src/syft/service/notification/email_templates.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/notification/notification_service.py` & `syft-0.8.7b8/src/syft/service/notification/notification_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/notification/notification_stash.py` & `syft-0.8.7b8/src/syft/service/notification/notification_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/notification/notifications.py` & `syft-0.8.7b8/src/syft/service/notification/notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 
     __attr_searchable__ = [
         "from_user_verify_key",
         "to_user_verify_key",
         "status",
     ]
     __repr_attrs__ = ["subject", "status", "created_at", "linked_obj"]
+    __table_sort_attr__ = "Created at"
 
     def _repr_html_(self) -> str:
         return f"""
             <style>
             .syft-request {{color: {SURFACE[options.color_theme]}; line-height: 1;}}
             </style>
             <div class='syft-request'>
@@ -97,15 +98,15 @@
         return None
 
     def _coll_repr_(self) -> dict[str, str]:
         self.linked_obj = cast(LinkedObject, self.linked_obj)
         return {
             "Subject": self.subject,
             "Status": self.determine_status().name.capitalize(),
-            "Created At": str(self.created_at),
+            "Created at": str(self.created_at),
             "Linked object": f"{self.linked_obj.object_type.__canonical_name__} ({self.linked_obj.object_uid})",
         }
 
     def mark_read(self) -> None:
         api: SyftAPI = cast(
             SyftAPI,
             APIRegistry.api_for(
```

### Comparing `syft-0.8.7b7/src/syft/service/notifier/notifier.py` & `syft-0.8.7b8/src/syft/service/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/notifier/notifier_service.py` & `syft-0.8.7b8/src/syft/service/notifier/notifier_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/notifier/notifier_stash.py` & `syft-0.8.7b8/src/syft/service/notifier/notifier_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/notifier/smtp_client.py` & `syft-0.8.7b8/src/syft/service/notifier/smtp_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/object_search/migration_state_service.py` & `syft-0.8.7b8/src/syft/service/object_search/migration_state_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/object_search/object_migration_state.py` & `syft-0.8.7b8/src/syft/service/object_search/object_migration_state.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/output/output_service.py` & `syft-0.8.7b8/src/syft/service/output/output_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/policy/policy.py` & `syft-0.8.7b8/src/syft/service/policy/policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -850,10 +850,30 @@
     except Exception as e:
         raise Exception(f"Exception loading code. {user_policy}. {e}")
 
 
 def init_policy(user_policy: UserPolicy, init_args: dict[str, Any]) -> Any:
     policy_class = load_policy_code(user_policy)
     policy_object = policy_class()
+
+    # Unwrapp {NodeIdentity : {x: y}} -> {x: y}
+    # Tech debt : For input policies, we required to have NodeIdentity args beforehand,
+    # therefore at this stage we had to return back to the normal args.
+    # Maybe there's better way to do it.
+    if len(init_args) and isinstance(list(init_args.keys())[0], NodeIdentity):
+        unwrapped_init_kwargs = init_args
+        if len(init_args) > 1:
+            raise Exception("You shoudn't have more than one Node Identity.")
+        # Otherwise, unwrapp it
+        init_args = init_args[list(init_args.keys())[0]]
+
     init_args = {k: v for k, v in init_args.items() if k != "id"}
+
+    # For input policies, this initializer wouldn't work properly:
+    # 1 - Passing {NodeIdentity: {kwargs:UIDs}} as keyword args doesn't work since keys must be strings
+    # 2 - Passing {kwargs: UIDs} in this initializer would not trigger the partition nodes from the
+    # InputPolicy initializer.
+    # The cleanest way to solve it is by checking if it's an Input Policy, and then, setting it manually.
     policy_object.__user_init__(**init_args)
+    if isinstance(policy_object, InputPolicy):
+        policy_object.init_kwargs = unwrapped_init_kwargs
     return policy_object
```

### Comparing `syft-0.8.7b7/src/syft/service/policy/policy_service.py` & `syft-0.8.7b8/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.7b8/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/project/project.py` & `syft-0.8.7b8/src/syft/service/project/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from ...types.syft_object import short_qual_name
 from ...types.transforms import TransformContext
 from ...types.transforms import rename
 from ...types.transforms import transform
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import SURFACE
+from ...util.decorators import deprecated
 from ...util.markdown import markdown_as_class_with_fields
 from ...util.util import full_name_with_qualname
 from ..code.user_code import SubmitUserCode
 from ..network.network_service import NodePeer
 from ..network.routes import NodeRoute
 from ..network.routes import connection_to_route
 from ..request.request import Request
@@ -1257,15 +1258,21 @@
         return add_code_request_to_project(
             project=self,
             code=obj,
             client=client,
             reason=reason,
         )
 
+    @deprecated(
+        reason="Project.start has been renamed to Project.send", return_syfterror=True
+    )
     def start(self, return_all_projects: bool = False) -> Project | list[Project]:
+        return self.send(return_all_projects=return_all_projects)
+
+    def send(self, return_all_projects: bool = False) -> Project | list[Project]:
         # Currently we are assuming that the first member is the leader
         # This would be changed in our future leaderless approach
         leader = self.clients[0]
         followers = self.clients[1:]
 
         try:
             # Check for DS role across all members
```

### Comparing `syft-0.8.7b7/src/syft/service/project/project_service.py` & `syft-0.8.7b8/src/syft/service/project/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/project/project_stash.py` & `syft-0.8.7b8/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/queue/base_queue.py` & `syft-0.8.7b8/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/queue/queue.py` & `syft-0.8.7b8/src/syft/service/queue/queue.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # stdlib
+from multiprocessing import Process
 import threading
+from threading import Thread
 import time
 from typing import Any
 from typing import cast
 
 # third party
+from loguru import logger
 import psutil
 from result import Err
 from result import Ok
-from result import Result
 
 # relative
 from ...node.credentials import SyftVerifyKey
 from ...node.worker_settings import WorkerSettings
 from ...serde.deserialize import _deserialize as deserialize
 from ...serde.serializable import serializable
 from ...service.context import AuthedServiceContext
 from ...store.document_store import BaseStash
 from ...types.datetime import DateTime
 from ...types.uid import UID
 from ..job.job_stash import Job
-from ..job.job_stash import JobStash
 from ..job.job_stash import JobStatus
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..worker.worker_stash import WorkerStash
 from .base_queue import AbstractMessageHandler
 from .base_queue import BaseQueueManager
 from .base_queue import QueueConfig
@@ -55,28 +56,36 @@
             time.sleep(self.interval)
 
     def monitor(self) -> None:
         # Implement the monitoring logic here
         job = self.worker.job_stash.get_by_uid(
             self.credentials, self.queue_item.job_id
         ).ok()
-        if job is None or job.status != JobStatus.INTERRUPTED:
-            return
-        else:
-            job.resolved = True
+        if job and job.status == JobStatus.TERMINATING:
+            self.terminate(job)
+            for subjob in job.subjobs:
+                self.terminate(subjob)
+
             self.queue_item.status = Status.INTERRUPTED
             self.queue_item.resolved = True
             self.worker.queue_stash.set_result(self.credentials, self.queue_item)
-            self.worker.job_stash.set_result(self.credentials, job)
-            process = psutil.Process(job.job_pid)
-            process.terminate()
+            # How about subjobs of subjobs?
 
     def stop(self) -> None:
         self.stop_requested.set()
 
+    def terminate(self, job: Job) -> None:
+        job.resolved = True
+        job.status = JobStatus.INTERRUPTED
+        self.worker.job_stash.set_result(self.credentials, job)
+        try:
+            psutil.Process(job.job_pid).terminate()
+        except psutil.Error as e:
+            logger.warning(f"Failed to terminate job {job.id}: {e}")
+
 
 @serializable()
 class QueueManager(BaseQueueManager):
     config: QueueConfig
 
     def post_init(self) -> None:
         self.client_config = self.config.client_config
@@ -241,40 +250,14 @@
     worker.queue_stash.set_result(credentials, queue_item)
     worker.job_stash.set_result(credentials, job_item)
 
     # Finish monitor thread
     monitor_thread.stop()
 
 
-def evaluate_can_run_job(
-    job_id: UID, job_stash: JobStash, credentials: SyftVerifyKey
-) -> Result[Job, str]:
-    """Evaluate if a Job can be executed by the user.
-
-    A Job cannot be executed if any of the following are met:
-    - User doesn't have permission to the job.
-    - Job is either marked Completed or result is available.
-    - Job is Cancelled or Interrupted.
-    """
-    res = job_stash.get_by_uid(credentials, job_id)
-
-    # User doesn't have access to job
-    if res.is_err():
-        return res
-
-    job_item = res.ok()
-
-    if job_item.status == JobStatus.COMPLETED or job_item.resolved:
-        return Err(f"Job: {job_id} already Completed.")
-    elif job_item.status == JobStatus.INTERRUPTED:
-        return Err(f"Job interrupted. Job Id: {job_id}")
-
-    return Ok(job_item)
-
-
 @serializable()
 class APICallMessageHandler(AbstractMessageHandler):
     queue_name = "api_call"
 
     @staticmethod
     def handle_message(message: bytes, syft_worker_id: UID) -> None:
         # relative
@@ -300,59 +283,48 @@
         )
 
         # otherwise it reads it from env, resulting in the wrong credentials
         worker.id = worker_settings.id
         worker.signing_key = worker_settings.signing_key
 
         credentials = queue_item.syft_client_verify_key
-
-        res = evaluate_can_run_job(queue_item.job_id, worker.job_stash, credentials)
+        res = worker.job_stash.get_by_uid(credentials, queue_item.job_id)
         if res.is_err():
+            logger.warning(res.err())
             raise Exception(res.value)
         job_item: Job = res.ok()
 
         queue_item.status = Status.PROCESSING
         queue_item.node_uid = worker.id
 
         job_item.status = JobStatus.PROCESSING
         job_item.node_uid = cast(UID, worker.id)
         job_item.updated_at = DateTime.now()
 
-        # try:
-        #     worker_name = os.getenv("DOCKER_WORKER_NAME", None)
-        #     docker_worker = worker.worker_stash.get_worker_by_name(
-        #         credentials, worker_name
-        #     ).ok()
-        #     job_item.job_worker_id = str(docker_worker.container_id)
-        # except Exception:
-        #     job_item.job_worker_id = str(worker.id)
         if syft_worker_id is not None:
             job_item.job_worker_id = syft_worker_id
 
         queue_result = worker.queue_stash.set_result(credentials, queue_item)
         if isinstance(queue_result, SyftError):
             raise Exception(f"{queue_result.err()}")
 
         job_result = worker.job_stash.set_result(credentials, job_item)
         if isinstance(job_result, SyftError):
             raise Exception(f"{job_result.err()}")
 
         if queue_config.thread_workers:
-            # stdlib
-            from threading import Thread
-
             thread = Thread(
                 target=handle_message_multiprocessing,
                 args=(worker_settings, queue_item, credentials),
             )
             thread.start()
             thread.join()
         else:
-            # stdlib
-            from multiprocessing import Process
+            # if psutil.pid_exists(job_item.job_pid):
+            #     psutil.Process(job_item.job_pid).terminate()
 
             process = Process(
                 target=handle_message_multiprocessing,
                 args=(worker_settings, queue_item, credentials),
             )
             process.start()
             job_item.job_pid = process.pid
```

### Comparing `syft-0.8.7b7/src/syft/service/queue/queue_service.py` & `syft-0.8.7b8/src/syft/service/queue/queue_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/queue/queue_stash.py` & `syft-0.8.7b8/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/queue/zmq_queue.py` & `syft-0.8.7b8/src/syft/service/queue/zmq_queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import time
 from time import sleep
 from typing import Any
 
 # third party
 from loguru import logger
 from pydantic import field_validator
+import zmq
 from zmq import Frame
 from zmq import LINGER
 from zmq.error import ContextTerminated
-import zmq.green as zmq
 
 # relative
 from ...serde.deserialize import _deserialize
 from ...serde.serializable import serializable
 from ...serde.serialize import _serialize as serialize
 from ...service.action.action_object import ActionObject
 from ...service.context import AuthedServiceContext
```

### Comparing `syft-0.8.7b7/src/syft/service/request/request.py` & `syft-0.8.7b8/src/syft/service/request/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from ...types.transforms import transform
 from ...types.twin_object import TwinObject
 from ...types.uid import LineageID
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import SURFACE
 from ...util.markdown import markdown_as_class_with_fields
-from ...util.notebook_ui.notebook_addons import REQUEST_ICON
+from ...util.notebook_ui.icons import Icon
 from ...util.util import prompt_warning_message
 from ..action.action_object import ActionObject
 from ..action.action_service import ActionService
 from ..action.action_store import ActionObjectPermission
 from ..action.action_store import ActionPermission
 from ..blob_storage.service import BlobStorageService
 from ..code.user_code import UserCode
@@ -349,14 +349,15 @@
 
     __table_coll_widths__ = [
         "min-content",
         "auto",
         "auto",
         "auto",
         "auto",
+        "auto",
     ]
 
     __attr_searchable__ = [
         "requesting_user_verify_key",
         "approving_user_verify_key",
     ]
     __attr_unique__ = ["request_hash"]
@@ -364,14 +365,15 @@
         "request_time",
         "updated_at",
         "status",
         "changes",
         "requesting_user_verify_key",
     ]
     __exclude_sync_diff_attrs__ = ["node_uid"]
+    __table_sort_attr__ = "Request time"
 
     def _repr_html_(self) -> Any:
         # add changes
         updated_at_line = ""
         if self.updated_at is not None:
             updated_at_line += (
                 f"<p><strong>Created by: </strong>{self.requesting_user_name}</p>"
@@ -463,14 +465,15 @@
             self.requesting_user_email,
             self.requesting_user_institution,
         ]
 
         return {
             "Description": self.html_description,
             "Requested By": "\n".join(user_data),
+            "Creation Time": str(self.request_time),
             "Status": status_badge,
         }
 
     @property
     def code_id(self) -> UID:
         for change in self.changes:
             if isinstance(change, UserCodeStatusChange):
@@ -507,15 +510,15 @@
             # only store the last change
             change_applied_map[change_status.change_id] = change_status.applied
 
         return change_applied_map
 
     @property
     def icon(self) -> str:
-        return REQUEST_ICON
+        return Icon.REQUEST.svg
 
     @property
     def status(self) -> RequestStatus:
         if len(self.history) == 0:
             return RequestStatus.PENDING
 
         all_changes_applied = all(self.current_change_state.values()) and (
@@ -563,19 +566,22 @@
             message = (
                 "You're approving a request on "
                 f"{metadata.node_side_type} side {metadata.node_type} "
                 "which may host datasets with private information."
             )
         if message and metadata and metadata.show_warnings and not disable_warnings:
             prompt_warning_message(message=message, confirm=True)
+        msg = (
+            "Approving request ",
+            f"on change {self.code.service_func_name} " if is_code_request else "",
+            f"for domain {api.node_name}",
+        )
 
-        print(f"Approving request for domain {api.node_name}")
+        print("".join(msg))
         res = api.services.request.apply(self.id, **kwargs)
-        # if isinstance(res, SyftSuccess):
-
         return res
 
     def deny(self, reason: str) -> SyftSuccess | SyftError:
         """Denies the particular request.
 
         Args:
             reason (str): Reason for which the request has been denied.
@@ -1213,26 +1219,27 @@
         for service_func_name, (_, new_node) in node.items():  # type: ignore
             msg = "├──" + "──" * level + f"{service_func_name}<br>"
             msg += self.nested_repr(node=new_node, level=level + 1)
         return msg
 
     def __repr_syft_nested__(self) -> str:
         msg = (
-            f"Request to change <b>{self.code.service_func_name}</b> "
-            f"(Pool Id: <b>{self.code.worker_pool_name}</b>) "
+            f"Request to change <strong>{self.code.service_func_name}</strong> "
+            f"(Pool Id: <strong>{self.code.worker_pool_name}</strong>) "
         )
-        msg += "to permission <strong>RequestStatus.APPROVED.</strong>"
-        if self.nested_solved:
-            if self.link.nested_codes == {}:  # type: ignore
-                msg += "No nested requests."
-            else:
+        msg += "to permission RequestStatus.APPROVED."
+        if self.code.nested_codes is None or self.code.nested_codes == {}:  # type: ignore
+            msg += " No nested requests"
+        else:
+            if self.nested_solved:
+                # else:
                 msg += "<br><br>This change requests the following nested functions calls:<br>"
                 msg += self.nested_repr()
-        else:
-            msg += "Nested Requests not resolved."
+            else:
+                msg += " Nested Requests not resolved"
         return msg
 
     def _repr_markdown_(self, wrap_as_python: bool = True, indent: int = 0) -> str:
         code = self.code
         input_policy_type = (
             code.input_policy_type.__canonical_name__
             if code.input_policy_type is not None
```

### Comparing `syft-0.8.7b7/src/syft/service/request/request_service.py` & `syft-0.8.7b8/src/syft/service/request/request_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,10 +284,23 @@
         result = self.stash.update(context.credentials, request)
         if result.is_ok():
             return result.ok()
         return SyftError(
             message=f"Failed to update Request: <{request.id}>. Error: {result.err()}"
         )
 
+    @service_method(
+        path="request.delete_by_uid",
+        name="delete_by_uid",
+    )
+    def delete_by_uid(
+        self, context: AuthedServiceContext, uid: UID
+    ) -> SyftSuccess | SyftError:
+        """Delete the request with the given uid."""
+        result = self.stash.delete_by_uid(context.credentials, uid)
+        if result.is_err():
+            return SyftError(message=str(result.err()))
+        return SyftSuccess(message=f"Request with id {uid} deleted.")
+
 
 TYPE_TO_SERVICE[Request] = RequestService
 SERVICE_TO_TYPES[RequestService].update({Request})
```

### Comparing `syft-0.8.7b7/src/syft/service/request/request_stash.py` & `syft-0.8.7b8/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/response.py` & `syft-0.8.7b8/src/syft/service/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,17 @@
     @property
     def _repr_html_class_(self) -> str:
         return "alert-danger"
 
     def to_result(self) -> Err:
         return Err(value=self.message)
 
+    def __bool__(self) -> bool:
+        return False
+
 
 @serializable()
 class SyftSuccess(SyftResponseMessage):
     @property
     def _repr_html_class_(self) -> str:
         return "alert-success"
```

### Comparing `syft-0.8.7b7/src/syft/service/service.py` & `syft-0.8.7b8/src/syft/service/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,17 +368,16 @@
                 result = result[0]
             context = kwargs.get("context", None)
             context = args[0] if context is None else context
             attrs_to_attach = {
                 "syft_node_location": context.node.id,
                 "syft_client_verify_key": context.credentials,
             }
-            return attach_attribute_to_syft_object(
-                result=result, attr_dict=attrs_to_attach
-            )
+            attach_attribute_to_syft_object(result=result, attr_dict=attrs_to_attach)
+            return result
 
         if autosplat is not None and len(autosplat) > 0:
             signature = expand_signature(signature=input_signature, autosplat=autosplat)
 
         config = ServiceConfig(
             public_path=_path if path is None else path,
             private_path=_path,
@@ -405,15 +404,15 @@
     def __init_subclass__(cls, **kwargs: Any) -> None:
         super().__init_subclass__(**kwargs)
         if hasattr(cls, "__canonical_name__") and hasattr(cls, "__version__"):
             mapping_string = f"{cls.__canonical_name__}_{cls.__version__}"
             cls.__object_version_registry__[mapping_string] = cls
 
     @classmethod
-    def versioned_class(cls, name: str, version: int) -> type["SyftObject"] | None:
+    def versioned_class(cls, name: str, version: int) -> type[SyftObject] | None:
         mapping_string = f"{name}_{version}"
         if mapping_string not in cls.__object_version_registry__:
             return None
         return cls.__object_version_registry__[mapping_string]
 
     @classmethod
     def add_transform(
@@ -425,15 +424,15 @@
         method: Callable,
     ) -> None:
         mapping_string = f"{klass_from}_{version_from}_x_{klass_to}_{version_to}"
         cls.__object_transform_registry__[mapping_string] = method
 
     @classmethod
     def get_transform(
-        cls, type_from: type["SyftObject"], type_to: type["SyftObject"]
+        cls, type_from: type[SyftObject], type_to: type[SyftObject]
     ) -> Callable:
         klass_from = type_from.__canonical_name__
         version_from = type_from.__version__
         klass_to = type_to.__canonical_name__
         version_to = type_to.__version__
         mapping_string = f"{klass_from}_{version_from}_x_{klass_to}_{version_to}"
         return cls.__object_transform_registry__[mapping_string]
```

### Comparing `syft-0.8.7b7/src/syft/service/settings/settings.py` & `syft-0.8.7b8/src/syft/service/settings/settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # stdlib
-from typing import Callable
+from collections.abc import Callable
+from typing import Any
 
 # relative
 from ...abstract_node import NodeSideType
 from ...abstract_node import NodeType
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...service.worker.utils import DEFAULT_WORKER_POOL_NAME
@@ -12,14 +13,16 @@
 from ...types.syft_object import SYFT_OBJECT_VERSION_2
 from ...types.syft_object import SYFT_OBJECT_VERSION_3
 from ...types.syft_object import SYFT_OBJECT_VERSION_4
 from ...types.syft_object import SyftObject
 from ...types.transforms import drop
 from ...types.transforms import make_set_default
 from ...types.uid import UID
+from ...util import options
+from ...util.colors import SURFACE
 
 
 @serializable()
 class NodeSettingsUpdateV2(PartialSyftObject):
     __canonical_name__ = "NodeSettingsUpdate"
     __version__ = SYFT_OBJECT_VERSION_2
 
@@ -70,14 +73,31 @@
     signup_enabled: bool
     admin_email: str
     node_side_type: NodeSideType = NodeSideType.HIGH_SIDE
     show_warnings: bool
     association_request_auto_approval: bool
     default_worker_pool: str = DEFAULT_WORKER_POOL_NAME
 
+    def _repr_html_(self) -> Any:
+        return f"""
+            <style>
+            .syft-settings {{color: {SURFACE[options.color_theme]};}}
+            </style>
+            <div class='syft-settings'>
+                <h3>Settings</h3>
+                <p><strong>Id: </strong>{self.id}</p>
+                <p><strong>Name: </strong>{self.name}</p>
+                <p><strong>Organization: </strong>{self.organization}</p>
+                <p><strong>Deployed on: </strong>{self.deployed_on}</p>
+                <p><strong>Signup enabled: </strong>{self.signup_enabled}</p>
+                <p><strong>Admin email: </strong>{self.admin_email}</p>
+            </div>
+
+            """
+
 
 @serializable()
 class NodeSettingsV2(SyftObject):
     __canonical_name__ = "NodeSettings"
     __version__ = SYFT_OBJECT_VERSION_3
     __repr_attrs__ = [
         "name",
```

### Comparing `syft-0.8.7b7/src/syft/service/settings/settings_service.py` & `syft-0.8.7b8/src/syft/service/settings/settings_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,25 +60,30 @@
             return result
         else:
             return SyftError(message=result.err())
 
     @service_method(path="settings.update", name="update")
     def update(
         self, context: AuthedServiceContext, settings: NodeSettingsUpdate
-    ) -> Result[Ok, Err]:
+    ) -> Result[SyftSuccess, SyftError]:
         result = self.stash.get_all(context.credentials)
         if result.is_ok():
             current_settings = result.ok()
             if len(current_settings) > 0:
                 new_settings = current_settings[0].model_copy(
                     update=settings.to_dict(exclude_empty=True)
                 )
                 update_result = self.stash.update(context.credentials, new_settings)
                 if update_result.is_ok():
-                    return result
+                    return SyftSuccess(
+                        message=(
+                            "Settings updated successfully. "
+                            + "You must call <client>.refresh() to sync your client with the changes."
+                        )
+                    )
                 else:
                     return SyftError(message=update_result.err())
             else:
                 return SyftError(message="No settings found")
         else:
             return SyftError(message=result.err())
 
@@ -145,14 +150,14 @@
         name="allow_association_request_auto_approval",
     )
     def allow_association_request_auto_approval(
         self, context: AuthedServiceContext, enable: bool
     ) -> SyftSuccess | SyftError:
         new_settings = NodeSettingsUpdate(association_request_auto_approval=enable)
         result = self.update(context, settings=new_settings)
-        if result.is_err():
-            return SyftError(message=result.err())
+        if isinstance(result, SyftError):
+            return result
 
         message = "enabled" if enable else "disabled"
         return SyftSuccess(
             message="Association request auto-approval successfully " + message
         )
```

### Comparing `syft-0.8.7b7/src/syft/service/settings/settings_stash.py` & `syft-0.8.7b8/src/syft/service/settings/settings_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/sync/diff_state.py` & `syft-0.8.7b8/src/syft/service/sync/diff_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 # stdlib
+from collections.abc import Callable
+from collections.abc import Iterable
+from dataclasses import dataclass
+import enum
 import html
+import operator
 import textwrap
 from typing import Any
 from typing import ClassVar
 from typing import Literal
 
 # third party
+from loguru import logger
 import pandas as pd
 from pydantic import model_validator
 from rich import box
 from rich.console import Console
 from rich.console import Group
 from rich.markdown import Markdown
 from rich.padding import Padding
@@ -28,31 +34,33 @@
 from ...types.syft_object import SyftObject
 from ...types.syft_object import short_uid
 from ...types.syncable_object import SyncableSyftObject
 from ...types.uid import LineageID
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import SURFACE
-from ...util.fonts import FONT_CSS
-from ...util.fonts import ITABLES_CSS
 from ...util.notebook_ui.components.sync import SyncTableObject
-from ...util.notebook_ui.notebook_addons import ARROW_ICON
+from ...util.notebook_ui.icons import Icon
+from ...util.notebook_ui.styles import FONT_CSS
+from ...util.notebook_ui.styles import ITABLES_CSS
 from ..action.action_object import ActionObject
 from ..action.action_permissions import ActionObjectPermission
 from ..action.action_permissions import ActionPermission
 from ..action.action_permissions import StoragePermission
 from ..api.api import TwinAPIEndpoint
 from ..code.user_code import UserCode
 from ..code.user_code import UserCodeStatusCollection
 from ..job.job_stash import Job
+from ..job.job_stash import JobType
 from ..log.log import SyftLog
 from ..output.output_service import ExecutionOutput
 from ..request.request import Request
 from ..response import SyftError
 from ..response import SyftSuccess
+from ..user.user import UserView
 from .sync_state import SyncState
 
 sketchy_tab = "‎ " * 4
 
 
 class AttrDiff(SyftObject):
     # version
@@ -802,15 +810,15 @@
 
     def _repr_html_(self) -> str:
         try:
             diffs = self.flatten_visual_hierarchy()
         except Exception as _:
             return SyftError(
                 message=html.escape(
-                    "Could not render batch, please use resolve_single(<batch>) instead."
+                    "Could not render batch, please use resolve(<batch>) instead."
                 )
             )._repr_html_()
 
         return f"""
 <h2> ObjectBatchDiff </h2>
 {diffs._repr_html_()}
 """
@@ -888,15 +896,15 @@
             return f"""{self.hierarchy_str('low')}
 
     {self.hierarchy_str('high')}
     """
         except Exception as _:
             return SyftError(
                 message=html.escape(
-                    "Could not render batch, please use resolve_single(<batch>) instead."
+                    "Could not render batch, please use resolve(<batch>) instead."
                 )
             )._repr_html_()
 
     def _repr_markdown_(self, wrap_as_python: bool = True, indent: int = 0) -> str:
         return ""  # Turns off the _repr_markdown_ of SyftObject
 
     def _get_visual_hierarchy(
@@ -939,27 +947,40 @@
             raise ValueError("No visual root found")
 
         return visual_roots[0]
 
     @property
     def user_code_high(self) -> UserCode | None:
         """return the user code of the high side of this batch, if it exists"""
-        user_codes_high: list[UserCode] = [
-            diff.high_obj
+        user_code_diff = self.user_code_diff
+        if user_code_diff is not None and isinstance(user_code_diff.high_obj, UserCode):
+            return user_code_diff.high_obj
+        return None
+
+    @property
+    def user_code_diff(self) -> ObjectDiff | None:
+        """return the main user code diff of the high side of this batch, if it exists"""
+        user_code_diffs: list[ObjectDiff] = [
+            diff
             for diff in self.get_dependencies(include_roots=True)
-            if isinstance(diff.high_obj, UserCode)
+            if issubclass(diff.obj_type, UserCode)
         ]
 
-        if len(user_codes_high) == 0:
-            user_code_high = None
+        if len(user_code_diffs) == 0:
+            return None
         else:
-            # NOTE we can always assume the first usercode is
-            # not a nested code, because diffs are sorted in depth-first order
-            user_code_high = user_codes_high[0]
-        return user_code_high
+            # main usercode is always the first, batches are sorted in depth-first order
+            return user_code_diffs[0]
+
+    @property
+    def user(self) -> UserView | SyftError:
+        user_code_diff = self.user_code_diff
+        if user_code_diff is not None and isinstance(user_code_diff.low_obj, UserCode):
+            return user_code_diff.low_obj.user
+        return SyftError(message="No user found")
 
     def get_visual_hierarchy(self) -> dict[ObjectDiff, dict]:
         visual_root = self.visual_root
         return {visual_root: self._get_visual_hierarchy(self.visual_root)}  # type: ignore
 
     def _get_obj_str(self, diff_obj: ObjectDiff, level: int, side: str) -> str:
         obj = diff_obj.low_obj if side == "low" else diff_obj.high_obj
@@ -1017,14 +1038,71 @@
                 other_batch.decision == SyncDecision.IGNORE
                 and other_batch.root_id in required_dependencies
             ):
                 print(f"ignoring other batch ({other_batch.root_type.__name__})")
                 other_batch.decision = None
 
 
+class FilterProperty(enum.Enum):
+    USER = enum.auto()
+    TYPE = enum.auto()
+    STATUS = enum.auto()
+    IGNORED = enum.auto()
+
+    def from_batch(self, batch: ObjectDiffBatch) -> Any:
+        if self == FilterProperty.USER:
+            user = batch.user
+            if isinstance(user, UserView):
+                return user.email
+            return None
+        elif self == FilterProperty.TYPE:
+            return batch.root_diff.obj_type.__name__.lower()
+        elif self == FilterProperty.STATUS:
+            return batch.status.lower()
+        elif self == FilterProperty.IGNORED:
+            return batch.is_ignored
+        else:
+            raise ValueError(f"Invalid property: {property}")
+
+
+@dataclass
+class NodeDiffFilter:
+    """
+    Filter to apply to a NodeDiff object to determine if it should be included in a batch.
+
+    Checks for `property op value` , where
+        property: FilterProperty - property to filter on
+        value: Any - value to compare against
+        op: callable[[Any, Any], bool] - comparison operator. Default is `operator.eq`
+
+    If the comparison fails, the batch is excluded.
+    """
+
+    filter_property: FilterProperty
+    filter_value: Any
+    op: Callable[[Any, Any], bool] = operator.eq
+
+    def __call__(self, batch: ObjectDiffBatch) -> bool:
+        filter_value = self.filter_value
+        if isinstance(filter_value, str):
+            filter_value = filter_value.lower()
+
+        try:
+            p = self.filter_property.from_batch(batch)
+            if self.op == operator.contains:
+                # Contains check has reversed arg order: check if p in self.filter_value
+                return p in filter_value
+            else:
+                return self.op(p, filter_value)
+        except Exception as e:
+            # By default, exclude the batch if there is an error
+            logger.debug(f"Error filtering batch {batch} with {self}: {e}")
+            return False
+
+
 class NodeDiff(SyftObject):
     __canonical_name__ = "NodeDiff"
     __version__ = SYFT_OBJECT_VERSION_2
 
     low_node_uid: UID
     high_node_uid: UID
     user_verify_key_low: SyftVerifyKey
@@ -1032,27 +1110,36 @@
     obj_uid_to_diff: dict[UID, ObjectDiff] = {}
     obj_dependencies: dict[UID, list[UID]] = {}
     batches: list[ObjectDiffBatch] = []
     all_batches: list[ObjectDiffBatch] = []
     low_state: SyncState
     high_state: SyncState
     direction: SyncDirection | None
+    filters: list[NodeDiffFilter] = []
 
     include_ignored: bool = False
 
     def __getitem__(self, idx: Any) -> ObjectDiffBatch:
         return self.batches[idx]
 
     @property
     def ignored_batches(self) -> list[ObjectDiffBatch]:
         return [
             batch for batch in self.all_batches if batch.decision == SyncDecision.IGNORE
         ]
 
     @property
+    def active_batches(self) -> Iterable[ObjectDiffBatch]:
+        decisions_to_skip = {SyncDecision.IGNORE, SyncDecision.SKIP}
+        # self.batches might be modified during iteration
+        for batch in self.batches:
+            if batch.decision not in decisions_to_skip:
+                yield batch
+
+    @property
     def ignored_changes(self) -> list[IgnoredBatchView]:
         result = []
         for ignored_batch in self.ignored_batches:
             other_batches = [b for b in self.all_batches if b is not ignored_batch]
             result.append(
                 IgnoredBatchView(batch=ignored_batch, other_batches=other_batches)
             )
@@ -1061,14 +1148,17 @@
     @classmethod
     def from_sync_state(
         cls: type["NodeDiff"],
         low_state: SyncState,
         high_state: SyncState,
         direction: SyncDirection,
         include_ignored: bool = False,
+        include_same: bool = False,
+        filter_by_email: str | None = None,
+        filter_by_type: type | None = None,
         _include_node_status: bool = False,
     ) -> "NodeDiff":
         obj_uid_to_diff = {}
         for obj_id in set(low_state.objects.keys()) | set(high_state.objects.keys()):
             low_obj = low_state.objects.get(obj_id, None)
             high_obj = high_state.objects.get(obj_id, None)
 
@@ -1113,33 +1203,39 @@
             direction=direction,
         )
 
         # TODO: Check if high and low ignored batches are the same else error
         previously_ignored_batches = low_state.ignored_batches
         NodeDiff.apply_previous_ignore_state(all_batches, previously_ignored_batches)
 
-        if not include_ignored:
-            batches = [b for b in all_batches if not b.is_ignored]
-        else:
-            batches = all_batches
-
-        return cls(
+        res = cls(
             low_node_uid=low_state.node_uid,
             high_node_uid=high_state.node_uid,
             user_verify_key_low=low_state.syft_client_verify_key,
             user_verify_key_high=high_state.syft_client_verify_key,
             obj_uid_to_diff=obj_uid_to_diff,
             obj_dependencies=obj_dependencies,
-            batches=batches,
+            batches=all_batches,
             all_batches=all_batches,
             low_state=low_state,
             high_state=high_state,
             direction=direction,
+            filters=[],
+        )
+
+        res._filter(
+            user_email=filter_by_email,
+            obj_type=filter_by_type,
+            include_ignored=include_ignored,
+            include_same=include_same,
+            inplace=True,
         )
 
+        return res
+
     @staticmethod
     def apply_previous_ignore_state(
         batches: list[ObjectDiffBatch], previously_ignored_batches: dict[UID, int]
     ) -> None:
         """
         Loop through all ignored batches in syncstate. If batch did not change, set to ignored
         If another batch needs to exist in order to accept that changed batch: also unignore
@@ -1213,15 +1309,15 @@
         else:
             name1 = "Private Node"
             name2 = "Public Node"
         repr_html = f"""
         <p style="margin-bottom:16px;"></p>
         <div class="diff-state-intro">Comparing sync states</div>
         <p style="margin-bottom:16px;"></p>
-        <div class="diff-state-header"><span>{name1}</span> {ARROW_ICON} <span>{name2}</span></div>
+        <div class="diff-state-header"><span>{name1}</span> {Icon.ARROW.svg} <span>{name2}</span></div>
         <p style="margin-bottom:16px;"></p>
         <div class="diff-state-sub-header"> This would sync <span class="diff-state-orange-text">{n} batches</span> from <i>{name1}</i> to <i>{name2}</i></div>
         """  # noqa: E501
         repr_html = repr_html.replace("\n", "")
 
         res = repr_html + self.batches._repr_html_()
         return res
@@ -1275,15 +1371,20 @@
 
         for diff in obj_uid_to_diff.values():
             diff_obj = diff.low_obj if diff.low_obj is not None else diff.high_obj
             if isinstance(diff_obj, Request | UserCode | TwinAPIEndpoint):
                 # TODO: Figure out nested user codes, do we even need that?
 
                 root_ids.append(diff.object_id)  # type: ignore
-            elif isinstance(diff_obj, Job) and diff_obj.parent_job_id is None:  # type: ignore
+            elif (
+                isinstance(diff_obj, Job)  # type: ignore
+                and diff_obj.parent_job_id is None
+                # ignore Job objects created by TwinAPIEndpoint
+                and diff_obj.job_type != JobType.TWINAPIJOB
+            ):
                 root_ids.append(diff.object_id)  # type: ignore
 
         for root_uid in root_ids:
             batch = ObjectDiffBatch.from_dependencies(
                 root_uid,
                 obj_dependencies,
                 obj_uid_to_diff,
@@ -1304,14 +1405,74 @@
         hierarchies_sorted = NodeDiff._sort_batches(batches)
         return hierarchies_sorted
 
     @property
     def is_same(self) -> bool:
         return all(object_diff.status == "SAME" for object_diff in self.diffs)
 
+    def _apply_filters(
+        self, filters: list[NodeDiffFilter], inplace: bool = True
+    ) -> Self:
+        """
+        Apply filters to the NodeDiff object and return a new NodeDiff object
+        """
+        batches = self.all_batches
+        for filter in filters:
+            batches = [b for b in batches if filter(b)]
+
+        if inplace:
+            self.filters = filters
+            self.batches = batches
+            return self
+        else:
+            return NodeDiff(
+                low_node_uid=self.low_node_uid,
+                high_node_uid=self.high_node_uid,
+                user_verify_key_low=self.user_verify_key_low,
+                user_verify_key_high=self.user_verify_key_high,
+                obj_uid_to_diff=self.obj_uid_to_diff,
+                obj_dependencies=self.obj_dependencies,
+                batches=batches,
+                all_batches=self.all_batches,
+                low_state=self.low_state,
+                high_state=self.high_state,
+                direction=self.direction,
+                filters=filters,
+            )
+
+    def _filter(
+        self,
+        user_email: str | None = None,
+        obj_type: str | type | None = None,
+        include_ignored: bool = False,
+        include_same: bool = False,
+        inplace: bool = True,
+    ) -> Self:
+        new_filters = []
+        if user_email is not None:
+            new_filters.append(
+                NodeDiffFilter(FilterProperty.USER, user_email, operator.eq)
+            )
+        if obj_type is not None:
+            if isinstance(obj_type, type):
+                obj_type = obj_type.__name__
+            new_filters.append(
+                NodeDiffFilter(FilterProperty.TYPE, obj_type, operator.eq)
+            )
+        if not include_ignored:
+            new_filters.append(
+                NodeDiffFilter(FilterProperty.IGNORED, True, operator.ne)
+            )
+        if not include_same:
+            new_filters.append(
+                NodeDiffFilter(FilterProperty.STATUS, "SAME", operator.ne)
+            )
+
+        return self._apply_filters(new_filters, inplace=inplace)
+
 
 class SyncInstruction(SyftObject):
     __canonical_name__ = "SyncDecision"
     __version__ = SYFT_OBJECT_VERSION_2
 
     diff: ObjectDiff
     decision: SyncDecision | None
```

### Comparing `syft-0.8.7b7/src/syft/service/sync/resolve_widget.py` & `syft-0.8.7b8/src/syft/service/sync/resolve_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,33 +11,29 @@
 from ipywidgets import Checkbox
 from ipywidgets import HBox
 from ipywidgets import HTML
 from ipywidgets import Layout
 from ipywidgets import VBox
 
 # relative
-from ...client.sync_decision import SyncDecision
 from ...client.sync_decision import SyncDirection
-from ...node.credentials import SyftVerifyKey
 from ...types.uid import UID
 from ...util.notebook_ui.components.sync import Alert
-from ...util.notebook_ui.components.sync import Badge
 from ...util.notebook_ui.components.sync import CopyIDButton
 from ...util.notebook_ui.components.sync import MainDescription
 from ...util.notebook_ui.components.sync import SyncWidgetHeader
-from ...util.notebook_ui.notebook_addons import CSS_CODE
+from ...util.notebook_ui.components.sync import TypeLabel
+from ...util.notebook_ui.styles import CSS_CODE
 from ..action.action_object import ActionObject
 from ..api.api import TwinAPIEndpoint
 from ..log.log import SyftLog
 from ..response import SyftError
 from ..response import SyftSuccess
 from .diff_state import ObjectDiff
 from .diff_state import ObjectDiffBatch
-from .diff_state import ResolvedSyncState
-from .diff_state import SyncInstruction
 
 # Standard div Jupyter Lab uses for notebook outputs
 # This is needed to use alert styles from SyftSuccess and SyftError
 NOTEBOOK_OUTPUT_DIV = """
 <div class="lm-Widget
             jp-RenderedHTMLCommon
             jp-RenderedHTML
@@ -243,15 +239,15 @@
         return isinstance(self.diff.non_empty_object, SyftLog | ActionObject)
 
     @property
     def title(self) -> str:
         object = self.diff.non_empty_object
         if object is None:
             return "n/a"
-        type_html = Badge(object=object).to_html()
+        type_html = TypeLabel(object=object).to_html()
         description_html = MainDescription(object=object).to_html()
         copy_id_button = CopyIDButton(copy_text=str(object.id.id), max_width=60)
 
         second_line_html = f"""
             <div class="widget-header2">
             <div class="widget-header2-2">
             {type_html} {description_html}
@@ -447,48 +443,14 @@
         return {
             uid: widget.share_private_data for uid, widget in self.id2widget.items()
         }
 
     def get_mockify_state(self) -> dict[UID, bool]:
         return {uid: widget.mockify for uid, widget in self.id2widget.items()}
 
-    def click_ignore(self, *args: list, **kwargs: dict) -> SyftSuccess | SyftError:
-        # relative
-        from ...client.syncing import handle_ignore_batch
-
-        if self.is_synced:
-            return SyftError(
-                message="The changes in this widget have already been synced."
-            )
-
-        res = handle_ignore_batch(
-            obj_diff_batch=self.obj_diff_batch,
-            all_batches=self.obj_diff_batch.global_batches,
-        )
-
-        self.set_widget_result_state(res)
-        return res
-
-    def click_unignore(self, *args: list, **kwargs: dict) -> SyftSuccess | SyftError:
-        # relative
-        from ...client.syncing import handle_unignore_batch
-
-        if self.is_synced:
-            return SyftError(
-                message="The changes in this widget have already been synced."
-            )
-
-        res = handle_unignore_batch(
-            obj_diff_batch=self.obj_diff_batch,
-            all_batches=self.obj_diff_batch.global_batches,
-        )
-
-        self.set_widget_result_state(res)
-        return res
-
     def click_sync(self, *args: list, **kwargs: dict) -> SyftSuccess | SyftError:
         # relative
         from ...client.syncing import handle_sync_batch
 
         if self.is_synced:
             return SyftError(
                 message="The changes in this widget have already been synced."
```

### Comparing `syft-0.8.7b7/src/syft/service/sync/sync_service.py` & `syft-0.8.7b8/src/syft/service/sync/sync_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/sync/sync_stash.py` & `syft-0.8.7b8/src/syft/service/sync/sync_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/sync/sync_state.py` & `syft-0.8.7b8/src/syft/service/sync/sync_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 from ...types.syft_object import SYFT_OBJECT_VERSION_2
 from ...types.syft_object import SyftObject
 from ...types.syncable_object import SyncableSyftObject
 from ...types.uid import LineageID
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import SURFACE
-from ...util.fonts import FONT_CSS
-from ...util.fonts import ITABLES_CSS
 from ...util.notebook_ui.components.sync import SyncTableObject
+from ...util.notebook_ui.styles import FONT_CSS
+from ...util.notebook_ui.styles import ITABLES_CSS
 from ..context import AuthedServiceContext
 
 
 def get_hierarchy_level_prefix(level: int) -> str:
     if level == 0:
         return ""
     else:
```

### Comparing `syft-0.8.7b7/src/syft/service/user/user.py` & `syft-0.8.7b8/src/syft/service/user/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/user/user_roles.py` & `syft-0.8.7b8/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/user/user_service.py` & `syft-0.8.7b8/src/syft/service/user/user_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from .user import UserPrivateKey
 from .user import UserSearch
 from .user import UserUpdate
 from .user import UserView
 from .user import UserViewPage
 from .user import check_pwd
 from .user import salt_and_hash_password
+from .user_roles import ADMIN_ROLE_LEVEL
 from .user_roles import DATA_OWNER_ROLE_LEVEL
 from .user_roles import DATA_SCIENTIST_ROLE_LEVEL
 from .user_roles import GUEST_ROLE_LEVEL
 from .user_roles import ServiceRole
 from .user_roles import ServiceRoleCapability
 from .user_stash import UserStash
 
@@ -216,15 +217,31 @@
         path="user.get_current_user", name="get_current_user", roles=GUEST_ROLE_LEVEL
     )
     def get_current_user(self, context: AuthedServiceContext) -> UserView | SyftError:
         result = self.stash.get_by_verify_key(
             credentials=context.credentials, verify_key=context.credentials
         )
         if result.is_ok():
-            # this seems weird that we get back None as Ok(None)
+            user = result.ok()
+            if user:
+                return user.to(UserView)
+            else:
+                SyftError(message="User not found!")
+        return SyftError(message=str(result.err()))
+
+    @service_method(
+        path="user.get_by_verify_key", name="get_by_verify_key", roles=ADMIN_ROLE_LEVEL
+    )
+    def get_by_verify_key_endpoint(
+        self, context: AuthedServiceContext, verify_key: SyftVerifyKey
+    ) -> UserView | SyftError:
+        result = self.stash.get_by_verify_key(
+            credentials=context.credentials, verify_key=verify_key
+        )
+        if result.is_ok():
             user = result.ok()
             if user:
                 return user.to(UserView)
             else:
                 SyftError(message="User not found!")
         return SyftError(message=str(result.err()))
```

### Comparing `syft-0.8.7b7/src/syft/service/user/user_stash.py` & `syft-0.8.7b8/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/warnings.py` & `syft-0.8.7b8/src/syft/service/warnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/worker/image_identifier.py` & `syft-0.8.7b8/src/syft/service/worker/image_identifier.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/worker/image_registry.py` & `syft-0.8.7b8/src/syft/service/worker/image_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/worker/image_registry_service.py` & `syft-0.8.7b8/src/syft/service/worker/image_registry_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/worker/image_registry_stash.py` & `syft-0.8.7b8/src/syft/service/worker/image_registry_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/worker/utils.py` & `syft-0.8.7b8/src/syft/service/worker/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from kr8s.objects import Pod
 
 # relative
 from ...abstract_node import AbstractNode
 from ...custom_worker.builder import CustomWorkerBuilder
 from ...custom_worker.builder_types import ImageBuildResult
 from ...custom_worker.builder_types import ImagePushResult
-from ...custom_worker.config import DockerWorkerConfig
 from ...custom_worker.config import PrebuiltWorkerConfig
 from ...custom_worker.k8s import KubeUtils
 from ...custom_worker.k8s import PodStatus
 from ...custom_worker.runner_k8s import KubernetesRunner
 from ...node.credentials import SyftVerifyKey
 from ...types.uid import UID
 from ...util.util import get_queue_address
@@ -78,29 +77,44 @@
     # Inspect the existing container
     details = backend_container.attrs
 
     host_config = details["HostConfig"]
     environment = details["Config"]["Env"]
 
     # Extract Volume Binds
+    vol_binds = {}
+
+    # ignore any irrelevant binds for the worker like
+    # packages/grid/backend/grid:/root/app/grid
+    # packages/syft:/root/app/syft
+    # packages/grid/data/package-cache:/root/.cache
+    valid_binds = {
+        "/var/run/docker.sock",
+        "/root/.cache",
+    }
+
     for vol in host_config["Binds"]:
         parts = vol.split(":")
         key = parts[0]
         bind = parts[1]
         mode = parts[2]
-        if "/storage" in bind:
+
+        if "/root/data/creds" in vol:
             # we need this because otherwise we are using the same node private key
             # which will make account creation fail
-            worker_postfix = worker_name.split("-", 1)[1]
-            key = f"{key}-{worker_postfix}"
-        extracted_config["volume_binds"][key] = {"bind": bind, "mode": mode}
+            key = f"{key}-{worker_name}"
+        elif bind not in valid_binds:
+            continue
+
+        vol_binds[key] = {"bind": bind, "mode": mode}
 
     # Extract Environment Variables
     extracted_config["environment"] = dict([e.split("=", 1) for e in environment])
     extracted_config["network_mode"] = f"container:{backend_container.id}"
+    extracted_config["volume_binds"] = vol_binds
 
     return extracted_config
 
 
 def get_free_tcp_port() -> int:
     with socketserver.TCPServer(("localhost", 0), None) as s:
         free_port = s.server_address[1]
@@ -531,55 +545,28 @@
 
 def create_default_image(
     credentials: SyftVerifyKey,
     image_stash: SyftWorkerImageStash,
     tag: str,
     in_kubernetes: bool = False,
 ) -> SyftError | SyftWorkerImage:
-    # TODO: Hardcode worker dockerfile since not able to COPY
-    # worker_cpu.dockerfile to backend in backend.dockerfile.
-
-    # default_cpu_dockerfile = get_syft_cpu_dockerfile()
-    # DockerWorkerConfig.from_path(default_cpu_dockerfile)
-
     if not in_kubernetes:
-        default_cpu_dockerfile = f"""ARG SYFT_VERSION_TAG='{tag}' \n"""
-        default_cpu_dockerfile += """FROM openmined/grid-backend:${SYFT_VERSION_TAG}
-        ARG PYTHON_VERSION="3.12"
-        ARG SYSTEM_PACKAGES=""
-        ARG PIP_PACKAGES="pip --dry-run"
-        ARG CUSTOM_CMD='echo "No custom commands passed"'
-
-        # Worker specific environment variables go here
-        ENV SYFT_WORKER="true"
-        ENV DOCKER_TAG=${SYFT_VERSION_TAG}
-
-        RUN apk update && \
-            apk add ${SYSTEM_PACKAGES} && \
-            pip install --user ${PIP_PACKAGES} && \
-            bash -c "$CUSTOM_CMD"
-        """
-        worker_config = DockerWorkerConfig(dockerfile=default_cpu_dockerfile)
-        _new_image = SyftWorkerImage(
-            config=worker_config,
-            created_by=credentials,
-        )
-    else:
-        # in k8s we don't need to build the image, just the tag of backend is enough
-        worker_config = PrebuiltWorkerConfig(
-            tag=tag,
-            description="Prebuilt default worker image",
-        )
+        tag = f"openmined/grid-backend:{tag}"
 
-        # create SyftWorkerImage from a pre-built image
-        _new_image = SyftWorkerImage(
-            config=worker_config,
-            created_by=credentials,
-            image_identifier=SyftWorkerImageIdentifier.from_str(tag),
-        )
+    worker_config = PrebuiltWorkerConfig(
+        tag=tag,
+        description="Prebuilt default worker image",
+    )
+
+    # create SyftWorkerImage from a pre-built image
+    _new_image = SyftWorkerImage(
+        config=worker_config,
+        created_by=credentials,
+        image_identifier=SyftWorkerImageIdentifier.from_str(tag),
+    )
 
     result = image_stash.get_by_docker_config(
         credentials=credentials,
         config=worker_config,
     )
 
     if result.ok() is None:
@@ -605,16 +592,14 @@
     if image.image_identifier is not None:
         full_tag = image.image_identifier.full_name_with_tag
         try:
             builder = CustomWorkerBuilder()
             return builder.build_image(
                 config=image.config,
                 tag=full_tag,
-                # rm=True,
-                # forcerm=True,
                 **kwargs,
             )
         except docker.errors.APIError as e:
             return SyftError(
                 message=f"Docker API error when building '{full_tag}'. Reason - {e}"
             )
         except docker.errors.DockerException as e:
```

### Comparing `syft-0.8.7b7/src/syft/service/worker/worker.py` & `syft-0.8.7b8/src/syft/service/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/worker/worker_image.py` & `syft-0.8.7b8/src/syft/service/worker/worker_image.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/worker/worker_image_service.py` & `syft-0.8.7b8/src/syft/service/worker/worker_image_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/worker/worker_image_stash.py` & `syft-0.8.7b8/src/syft/service/worker/worker_image_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/worker/worker_pool.py` & `syft-0.8.7b8/src/syft/service/worker/worker_pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from ...types.datetime import DateTime
 from ...types.syft_object import SYFT_OBJECT_VERSION_2
 from ...types.syft_object import SyftObject
 from ...types.syft_object import short_uid
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import SURFACE
-from ...util.fonts import FONT_CSS
-from ...util.fonts import ITABLES_CSS
+from ...util.notebook_ui.styles import FONT_CSS
+from ...util.notebook_ui.styles import ITABLES_CSS
 from ..response import SyftError
 from .worker_image import SyftWorkerImage
 
 
 @serializable()
 class WorkerStatus(Enum):
     PENDING = "Pending"
@@ -150,14 +150,15 @@
     __repr_attrs__ = [
         "name",
         "image",
         "max_count",
         "workers",
         "created_at",
     ]
+    __table_sort_attr__ = "Created at"
 
     name: str
     image_id: UID | None = None
     max_count: int
     worker_list: list[LinkedObject]
     created_at: DateTime = DateTime.now()
```

### Comparing `syft-0.8.7b7/src/syft/service/worker/worker_pool_service.py` & `syft-0.8.7b8/src/syft/service/worker/worker_pool_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/worker/worker_pool_stash.py` & `syft-0.8.7b8/src/syft/service/worker/worker_pool_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/worker/worker_service.py` & `syft-0.8.7b8/src/syft/service/worker/worker_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/service/worker/worker_stash.py` & `syft-0.8.7b8/src/syft/service/worker/worker_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/store/blob_storage/__init__.py` & `syft-0.8.7b8/src/syft/store/blob_storage/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 - get a BlobRetrieval from the id of the BlobStorageEntry of the SyftObject
   `blob_retrieval = api.services.blob_storage.read(blob_storage_entry_id)`
 - use `BlobRetrieval.read` to retrieve the SyftObject `syft_object = blob_retrieval.read()`
 """
 
 # stdlib
+from collections.abc import Callable
 from collections.abc import Generator
 from io import BytesIO
 from typing import Any
 
 # third party
 from pydantic import BaseModel
 import requests
@@ -59,18 +60,22 @@
 from ...types.blob_storage import BlobFile
 from ...types.blob_storage import BlobFileType
 from ...types.blob_storage import BlobStorageEntry
 from ...types.blob_storage import CreateBlobStorageEntry
 from ...types.blob_storage import DEFAULT_CHUNK_SIZE
 from ...types.blob_storage import SecureFilePathLocation
 from ...types.grid_url import GridURL
+from ...types.syft_migration import migrate
 from ...types.syft_object import SYFT_OBJECT_VERSION_2
 from ...types.syft_object import SYFT_OBJECT_VERSION_3
 from ...types.syft_object import SYFT_OBJECT_VERSION_4
+from ...types.syft_object import SYFT_OBJECT_VERSION_5
 from ...types.syft_object import SyftObject
+from ...types.transforms import drop
+from ...types.transforms import make_set_default
 from ...types.uid import UID
 
 DEFAULT_TIMEOUT = 10
 MAX_RETRIES = 20
 
 
 @serializable()
@@ -139,20 +144,29 @@
                 )
             else:
                 print(f"Max retries reached. Failed with error: {e}")
                 raise
 
 
 @serializable()
-class BlobRetrievalByURL(BlobRetrieval):
+class BlobRetrievalByURLV4(BlobRetrieval):
     __canonical_name__ = "BlobRetrievalByURL"
     __version__ = SYFT_OBJECT_VERSION_4
 
     url: GridURL | str
 
+
+@serializable()
+class BlobRetrievalByURL(BlobRetrieval):
+    __canonical_name__ = "BlobRetrievalByURL"
+    __version__ = SYFT_OBJECT_VERSION_5
+
+    url: GridURL | str
+    proxy_node_uid: UID | None = None
+
     def read(self) -> SyftObject | SyftError:
         if self.type_ is BlobFileType:
             return BlobFile(
                 file_name=self.file_name,
                 syft_client_verify_key=self.syft_client_verify_key,
                 syft_node_location=self.syft_node_location,
                 syft_blob_storage_entry_id=self.syft_blob_storage_entry_id,
@@ -171,34 +185,43 @@
         # relative
         from ...client.api import APIRegistry
 
         api = APIRegistry.api_for(
             node_uid=self.syft_node_location,
             user_verify_key=self.syft_client_verify_key,
         )
+
         if api and api.connection and isinstance(self.url, GridURL):
-            blob_url = api.connection.to_blob_route(
-                self.url.url_path, host=self.url.host_or_ip
-            )
+            if self.proxy_node_uid is None:
+                blob_url = api.connection.to_blob_route(
+                    self.url.url_path, host=self.url.host_or_ip
+                )
+            else:
+                blob_url = api.connection.stream_via(
+                    self.proxy_node_uid, self.url.url_path
+                )
+                stream = True
         else:
             blob_url = self.url
+
         try:
-            if self.type_ is BlobFileType:
-                if stream:
-                    return syft_iter_content(blob_url, chunk_size)
-                else:
-                    response = requests.get(str(blob_url), stream=False)  # nosec
-                    response.raise_for_status()
-                    return response.content
-            else:
-                response = requests.get(str(blob_url), stream=stream)  # nosec
-                response.raise_for_status()
-                return deserialize(response.content, from_bytes=True)
+            if (is_blob_file := issubclass(self.type_, BlobFileType)) and stream:
+                return syft_iter_content(blob_url, chunk_size)
+
+            response = requests.get(str(blob_url), stream=stream)  # nosec
+            resp_content = response.content
+            response.raise_for_status()
+
+            return (
+                resp_content
+                if is_blob_file
+                else deserialize(resp_content, from_bytes=True)
+            )
         except requests.RequestException as e:
-            return SyftError(message=f"Failed to retrieve with Error: {e}")
+            return SyftError(message=f"Failed to retrieve with error: {e}")
 
 
 @serializable()
 class BlobDeposit(SyftObject):
     __canonical_name__ = "BlobDeposit"
     __version__ = SYFT_OBJECT_VERSION_2
 
@@ -243,7 +266,17 @@
         raise NotImplementedError
 
 
 @serializable()
 class BlobStorageConfig(SyftBaseModel):
     client_type: type[BlobStorageClient]
     client_config: BlobStorageClientConfig
+
+
+@migrate(BlobRetrievalByURLV4, BlobRetrievalByURL)
+def upgrade_blob_retrieval_by_url() -> list[Callable]:
+    return [make_set_default("proxy_node_uid", None)]
+
+
+@migrate(BlobRetrievalByURL, BlobRetrievalByURLV4)
+def downgrade_blob_retrieval_by_url() -> list[Callable]:
+    return [drop(["proxy_node_uid"])]
```

### Comparing `syft-0.8.7b7/src/syft/store/blob_storage/on_disk.py` & `syft-0.8.7b8/src/syft/store/blob_storage/on_disk.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/store/blob_storage/seaweedfs.py` & `syft-0.8.7b8/src/syft/store/blob_storage/seaweedfs.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 from typing import Any
 
 # third party
 import boto3
 from botocore.client import BaseClient as S3BaseClient
 from botocore.client import ClientError as BotoClientError
 from botocore.client import Config
+from botocore.exceptions import ConnectionError
 import requests
+from tenacity import retry
+from tenacity import retry_if_exception_type
+from tenacity import stop_after_delay
+from tenacity import wait_fixed
 from tqdm import tqdm
 from typing_extensions import Self
 
 # relative
 from . import BlobDeposit
 from . import BlobRetrieval
 from . import BlobStorageClient
@@ -71,14 +76,15 @@
 
             # this is the total nr of chunks in all parts
             total_iterations = math.ceil(part_size / chunk_size) * len(self.urls)
 
             with tqdm(
                 total=total_iterations,
                 desc=f"Uploading progress",  # noqa
+                colour="green",
             ) as pbar:
                 for part_no, url in enumerate(
                     self.urls,
                     start=1,
                 ):
                     if api is not None and api.connection is not None:
                         blob_url = api.connection.to_blob_route(
@@ -211,20 +217,30 @@
         default_bucket_name: str,
         config: SeaweedFSClientConfig,
     ):
         self.client = client
         self.default_bucket_name = default_bucket_name
         self.config = config
 
+        self._check_connection()
+
     def __enter__(self) -> Self:
         return self
 
     def __exit__(self, *exc: Any) -> None:
         self.client.close()
 
+    @retry(
+        wait=wait_fixed(5),
+        stop=stop_after_delay(60),
+        retry=retry_if_exception_type(ConnectionError),
+    )
+    def _check_connection(self) -> dict:
+        return self.client.list_buckets()
+
     def read(
         self,
         fp: SecureFilePathLocation,
         type_: type | None,
         bucket_name: str | None = None,
     ) -> BlobRetrieval:
         if bucket_name is None:
```

### Comparing `syft-0.8.7b7/src/syft/store/dict_document_store.py` & `syft-0.8.7b8/src/syft/store/dict_document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,13 @@
             The Document type used. Default: DictDocumentStore
         `backing_store`: Type[KeyValueBackingStore]
             The backend type used. Default: DictBackingStore
         locking_config: LockingConfig
             The config used for store locking. Available options:
                 * NoLockingConfig: no locking, ideal for single-thread stores.
                 * ThreadingLockingConfig: threading-based locking, ideal for same-process in-memory stores.
-                * FileLockingConfig: file based locking, ideal for same-device different-processes/threads stores.
             Defaults to ThreadingLockingConfig.
     """
 
     store_type: type[DocumentStore] = DictDocumentStore
     backing_store: type[KeyValueBackingStore] = DictBackingStore
     locking_config: LockingConfig = Field(default_factory=ThreadingLockingConfig)
```

### Comparing `syft-0.8.7b7/src/syft/store/document_store.py` & `syft-0.8.7b8/src/syft/store/document_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -312,15 +312,19 @@
     ) -> None:
         if root_verify_key is None:
             root_verify_key = SyftSigningKey.generate().verify_key
         self.node_uid = node_uid
         self.root_verify_key = root_verify_key
         self.settings = settings
         self.store_config = store_config
-        self.init_store()
+        res = self.init_store()
+        if res.is_err():
+            raise RuntimeError(
+                f"Something went wrong initializing the store: {res.err()}"
+            )
 
         store_config.locking_config.lock_name = f"StorePartition-{settings.name}"
         self.lock = SyftLock(store_config.locking_config)
 
     def init_store(self) -> Result[Ok, Err]:
         try:
             self.unique_cks = self.settings.unique_keys.all
@@ -793,15 +797,14 @@
             Document Store type
         client_config: Optional[StoreClientConfig]
             Backend-specific config
         locking_config: LockingConfig
             The config used for store locking. Available options:
                 * NoLockingConfig: no locking, ideal for single-thread stores.
                 * ThreadingLockingConfig: threading-based locking, ideal for same-process in-memory stores.
-                * FileLockingConfig: file based locking, ideal for same-device different-processes/threads stores.
             Defaults to NoLockingConfig.
     """
 
     __canonical_name__ = "StoreConfig"
     __version__ = SYFT_OBJECT_VERSION_2
 
     store_type: type[DocumentStore]
```

### Comparing `syft-0.8.7b7/src/syft/store/kv_document_store.py` & `syft-0.8.7b8/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/store/linked_obj.py` & `syft-0.8.7b8/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/store/mongo_client.py` & `syft-0.8.7b8/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/store/mongo_codecs.py` & `syft-0.8.7b8/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/store/mongo_document_store.py` & `syft-0.8.7b8/src/syft/store/mongo_document_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -991,15 +991,14 @@
             The type of the DocumentStore. Default: MongoDocumentStore
         `db_name`: str
             Database name
         locking_config: LockingConfig
             The config used for store locking. Available options:
                 * NoLockingConfig: no locking, ideal for single-thread stores.
                 * ThreadingLockingConfig: threading-based locking, ideal for same-process in-memory stores.
-                * FileLockingConfig: file based locking, ideal for same-device different-processes/threads stores.
             Defaults to NoLockingConfig.
     """
 
     client_config: MongoStoreClientConfig
     store_type: type[DocumentStore] = MongoDocumentStore
     db_name: str = "app"
     backing_store: type[KeyValueBackingStore] = MongoBackingStore
```

### Comparing `syft-0.8.7b7/src/syft/store/sqlite_document_store.py` & `syft-0.8.7b8/src/syft/store/sqlite_document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -454,15 +454,14 @@
             Class interacting with QueueStash. Default: SQLiteDocumentStore
         `backing_store`: KeyValueBackingStore
             The Store core logic. Default: SQLiteBackingStore
         locking_config: LockingConfig
             The config used for store locking. Available options:
                 * NoLockingConfig: no locking, ideal for single-thread stores.
                 * ThreadingLockingConfig: threading-based locking, ideal for same-process in-memory stores.
-                * FileLockingConfig: file based locking, ideal for same-device different-processes/threads stores.
-            Defaults to FileLockingConfig.
+            Defaults to NoLockingConfig.
     """
 
     client_config: SQLiteStoreClientConfig
     store_type: type[DocumentStore] = SQLiteDocumentStore
     backing_store: type[KeyValueBackingStore] = SQLiteBackingStore
     locking_config: LockingConfig = Field(default_factory=NoLockingConfig)
```

### Comparing `syft-0.8.7b7/src/syft/types/blob_storage.py` & `syft-0.8.7b8/src/syft/types/blob_storage.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/types/dicttuple.py` & `syft-0.8.7b8/src/syft/types/dicttuple.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/types/grid_url.py` & `syft-0.8.7b8/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/types/identity.py` & `syft-0.8.7b8/src/syft/types/identity.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/types/syft_metaclass.py` & `syft-0.8.7b8/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/types/syft_migration.py` & `syft-0.8.7b8/src/syft/types/syft_migration.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/types/syft_object.py` & `syft-0.8.7b8/src/syft/types/syft_object.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 # stdlib
 from collections import defaultdict
 from collections.abc import Callable
 from collections.abc import Generator
 from collections.abc import Iterable
 from collections.abc import KeysView
 from collections.abc import Mapping
-from collections.abc import MutableMapping
-from collections.abc import MutableSequence
 from collections.abc import Sequence
 from collections.abc import Set
 from hashlib import sha256
 import inspect
 from inspect import Signature
-import re
-import traceback
 import types
 from types import NoneType
 from types import UnionType
 import typing
 from typing import Any
 from typing import ClassVar
 from typing import Optional
 from typing import TYPE_CHECKING
 from typing import Union
 from typing import get_args
 from typing import get_origin
 
 # third party
-import pandas as pd
 import pydantic
 from pydantic import ConfigDict
 from pydantic import EmailStr
 from pydantic import Field
 from pydantic import model_validator
 from pydantic.fields import PydanticUndefined
 from result import OkErr
@@ -40,19 +35,18 @@
 
 # relative
 from ..node.credentials import SyftVerifyKey
 from ..serde.recursive_primitives import recursive_serde_register_type
 from ..serde.serialize import _serialize as serialize
 from ..util.autoreload import autoreload_enabled
 from ..util.markdown import as_markdown_python_code
-from ..util.notebook_ui.notebook_addons import create_table_template
+from ..util.notebook_ui.components.tabulator_template import build_tabulator_table
 from ..util.util import aggressive_set_attr
 from ..util.util import full_name_with_qualname
 from ..util.util import get_qualname_for
-from .dicttuple import DictTuple
 from .syft_metaclass import Empty
 from .syft_metaclass import PartialModelMetaclass
 from .uid import UID
 
 if TYPE_CHECKING:
     # relative
     from ..service.sync.diff_state import AttrDiff
@@ -63,21 +57,23 @@
 
 
 SYFT_OBJECT_VERSION_1 = 1
 SYFT_OBJECT_VERSION_2 = 2
 SYFT_OBJECT_VERSION_3 = 3
 SYFT_OBJECT_VERSION_4 = 4
 SYFT_OBJECT_VERSION_5 = 5
+SYFT_OBJECT_VERSION_6 = 6
 
 supported_object_versions = [
     SYFT_OBJECT_VERSION_1,
     SYFT_OBJECT_VERSION_2,
     SYFT_OBJECT_VERSION_3,
     SYFT_OBJECT_VERSION_4,
     SYFT_OBJECT_VERSION_5,
+    SYFT_OBJECT_VERSION_6,
 ]
 
 HIGHEST_SYFT_OBJECT_VERSION = max(supported_object_versions)
 LOWEST_SYFT_OBJECT_VERSION = min(supported_object_versions)
 
 
 # These attributes are dynamically added based on node/client
@@ -418,14 +414,15 @@
 
     __repr_attrs__: ClassVar[list[str]] = []  # show these in html repr collections
     __attr_custom_repr__: ClassVar[list[str] | None] = (
         None  # show these in html repr of an object
     )
     __validate_private_attrs__: ClassVar[bool] = True
     __table_coll_widths__: ClassVar[list[str] | None] = None
+    __table_sort_attr__: ClassVar[str | None] = None
 
     def __syft_get_funcs__(self) -> list[tuple[str, Signature]]:
         funcs = print_type_cache[type(self)]
         if len(funcs) > 0:
             return funcs
 
         for attr in dir(type(self)):
@@ -760,204 +757,19 @@
 def short_uid(uid: UID | None) -> str | None:
     if uid is None:
         return uid
     else:
         return str(uid)[:6] + "..."
 
 
-def get_repr_values_table(
-    _self: Mapping | Iterable,
-    is_homogenous: bool,
-    extra_fields: list | None = None,
-) -> dict:
-    if extra_fields is None:
-        extra_fields = []
-
-    cols = defaultdict(list)
-    for item in iter(_self.items() if isinstance(_self, Mapping) else _self):
-        # unpack dict
-        if isinstance(_self, Mapping):
-            key, item = item
-            cols["key"].append(key)
-
-        # get id
-        id_ = getattr(item, "id", None)
-        include_id = getattr(item, "__syft_include_id_coll_repr__", True)
-        if id_ is not None and include_id:
-            cols["id"].append({"value": str(id_), "type": "clipboard"})
-
-        if type(item) == type:
-            t = full_name_with_qualname(item)
-        else:
-            try:
-                t = item.__class__.__name__
-            except Exception:
-                t = item.__repr__()
-
-        if not is_homogenous:
-            cols["type"].append(t)
-
-        # if has _coll_repr_
-
-        if hasattr(item, "_coll_repr_"):
-            ret_val = item._coll_repr_()
-            if "id" in ret_val:
-                del ret_val["id"]
-            for key in ret_val.keys():
-                cols[key].append(ret_val[key])
-        else:
-            for field in extra_fields:
-                value = item
-                try:
-                    attrs = field.split(".")
-                    for i, attr in enumerate(attrs):
-                        # find indexing like abc[1]
-                        res = re.search(r"\[[+-]?\d+\]", attr)
-                        has_index = False
-                        if res:
-                            has_index = True
-                            index_str = res.group()
-                            index = int(index_str.replace("[", "").replace("]", ""))
-                            attr = attr.replace(index_str, "")
-
-                        value = getattr(value, attr, None)
-                        if isinstance(value, list) and has_index:
-                            value = value[index]
-                        # If the object has a special representation when nested we will use that instead
-                        if (
-                            hasattr(value, "__repr_syft_nested__")
-                            and i == len(attrs) - 1
-                        ):
-                            value = value.__repr_syft_nested__()
-                        if (
-                            isinstance(value, list)
-                            and i == len(attrs) - 1
-                            and len(value) > 0
-                            and hasattr(value[0], "__repr_syft_nested__")
-                        ):
-                            value = [
-                                (
-                                    x.__repr_syft_nested__()
-                                    if hasattr(x, "__repr_syft_nested__")
-                                    else x
-                                )
-                                for x in value
-                            ]
-                    if value is None:
-                        value = "n/a"
-
-                except Exception as e:
-                    print(e)
-                    value = None
-                cols[field].append(str(value))
-
-    df = pd.DataFrame(cols)
-
-    if "created_at" in df.columns:
-        df.sort_values(by="created_at", ascending=False, inplace=True)
-
-    return df.to_dict("records")  # type: ignore
-
-
-def _get_grid_template_columns(first_value: Any) -> tuple[str | None, str | None]:
-    grid_template_cols = getattr(first_value, "__table_coll_widths__", None)
-    if isinstance(grid_template_cols, list):
-        grid_template_columns = " ".join(grid_template_cols)
-        grid_template_cell_columns = "unset"
-    else:
-        grid_template_columns = None
-        grid_template_cell_columns = None
-    return grid_template_columns, grid_template_cell_columns
-
-
-def list_dict_repr_html(self: Mapping | Set | Iterable) -> str:
-    try:
-        max_check = 1
-        items_checked = 0
-        has_syft = False
-        extra_fields: list = []
-        if isinstance(self, Mapping):
-            values: Any = list(self.values())
-        elif isinstance(self, Set):
-            values = list(self)
-        else:
-            values = self
-
-        if len(values) == 0:
-            return self.__repr__()
-
-        for item in iter(self.values() if isinstance(self, Mapping) else self):
-            items_checked += 1
-            if items_checked > max_check:
-                break
-
-            if hasattr(type(item), "mro") and type(item) != type:
-                mro: list | str = type(item).mro()
-            elif hasattr(item, "mro") and type(item) != type:
-                mro = item.mro()
-            else:
-                mro = str(self)
-
-            if "syft" in str(mro).lower():
-                has_syft = True
-                extra_fields = getattr(item, "__repr_attrs__", [])
-                break
-
-        if has_syft:
-            # if custom_repr:
-            table_icon = None
-            if hasattr(values[0], "icon"):
-                table_icon = values[0].icon
-            # this is a list of dicts
-            is_homogenous = len({type(x) for x in values}) == 1
-            # third party
-
-            try:
-                vals = get_repr_values_table(
-                    self, is_homogenous, extra_fields=extra_fields
-                )
-            except Exception:
-                return str(self)
-
-            first_value = values[0]
-            if is_homogenous:
-                cls_name = first_value.__class__.__name__
-                grid_template_columns, grid_template_cell_columns = (
-                    _get_grid_template_columns(first_value)
-                )
-            else:
-                cls_name = ""
-                grid_template_columns = None
-                grid_template_cell_columns = None
-
-            return create_table_template(
-                vals,
-                f"{cls_name} {self.__class__.__name__.capitalize()}",
-                table_icon=table_icon,
-                grid_template_columns=grid_template_columns,
-                grid_template_cell_columns=grid_template_cell_columns,
-            )
-
-    except Exception as e:
-        print(
-            f"error representing {type(self)} of objects. {e}, {traceback.format_exc()}"
-        )
-        pass
-
-    # stdlib
-    import html
-
-    return html.escape(self.__repr__())
-
-
 # give lists and dicts a _repr_html_ if they contain SyftObject's
-aggressive_set_attr(type([]), "_repr_html_", list_dict_repr_html)
-aggressive_set_attr(type({}), "_repr_html_", list_dict_repr_html)
-aggressive_set_attr(type(set()), "_repr_html_", list_dict_repr_html)
-aggressive_set_attr(tuple, "_repr_html_", list_dict_repr_html)
+aggressive_set_attr(type([]), "_repr_html_", build_tabulator_table)
+aggressive_set_attr(type({}), "_repr_html_", build_tabulator_table)
+aggressive_set_attr(type(set()), "_repr_html_", build_tabulator_table)
+aggressive_set_attr(tuple, "_repr_html_", build_tabulator_table)
 
 
 class StorableObjectType:
     def to(self, projection: type, context: Context | None = None) -> Any:
         # 🟡 TODO 19: Could we do an mro style inheritence conversion? Risky?
         transform = SyftObjectRegistry.get_transform(type(self), projection)
         return transform(self, context)
@@ -978,51 +790,28 @@
     def __iter__(self) -> TupleGenerator:
         yield from ((k, v) for k, v in super().__iter__() if v is not Empty)
 
 
 recursive_serde_register_type(PartialSyftObject)
 
 
-def attach_attribute_to_syft_object(result: Any, attr_dict: dict[str, Any]) -> Any:
-    constructor = None
-    extra_args = []
-
-    single_entity = False
-
+def attach_attribute_to_syft_object(result: Any, attr_dict: dict[str, Any]) -> None:
+    iterator: Iterable
     if isinstance(result, OkErr):
-        constructor = type(result)
-        result = result.value
-
-    if isinstance(result, MutableMapping):
-        iterable_keys: Iterable = result.keys()
-    elif isinstance(result, MutableSequence):
-        iterable_keys = range(len(result))
-    elif isinstance(result, tuple):
-        iterable_keys = range(len(result))
-        constructor = type(result)
-        if isinstance(result, DictTuple):
-            extra_args.append(result.keys())
-        result = list(result)
+        iterator = (result._value,)
+    elif isinstance(result, Mapping):
+        iterator = result.values()
+    elif isinstance(result, Sequence):
+        iterator = result
     else:
-        iterable_keys = range(1)
-        result = [result]
-        single_entity = True
+        iterator = (result,)
 
-    for key in iterable_keys:
-        _object = result[key]
+    for _object in iterator:
         # if object is SyftBaseObject,
         # then attach the value to the attribute
         # on the object
         if isinstance(_object, SyftBaseObject):
             for attr_name, attr_value in attr_dict.items():
                 setattr(_object, attr_name, attr_value)
 
-            for field_name, attr in _object.__dict__.items():
-                updated_attr = attach_attribute_to_syft_object(attr, attr_dict)
-                setattr(_object, field_name, updated_attr)
-        result[key] = _object
-
-    wrapped_result = result[0] if single_entity else result
-    if constructor is not None:
-        wrapped_result = constructor(wrapped_result, *extra_args)
-
-    return wrapped_result
+            for field in _object.model_fields.keys():
+                attach_attribute_to_syft_object(getattr(_object, field), attr_dict)
```

### Comparing `syft-0.8.7b7/src/syft/types/syncable_object.py` & `syft-0.8.7b8/src/syft/types/syncable_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/types/transforms.py` & `syft-0.8.7b8/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/types/twin_object.py` & `syft-0.8.7b8/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/types/uid.py` & `syft-0.8.7b8/src/syft/types/uid.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,22 @@
 from collections.abc import Callable
 from collections.abc import Sequence
 import hashlib
 from typing import Any
 import uuid
 from uuid import UUID as uuid_type
 
+# third party
+from typing_extensions import Self
+
 # relative
 from ..serde.serializable import serializable
 from ..util.logger import critical
 from ..util.logger import traceback_and_raise
 
-try:
-    # Python >= 3.11
-    # stdlib
-    from typing import Self
-except ImportError:
-    # Python < 3.11
-    # third party
-    from typing_extensions import Self
-
 
 @serializable(attrs=["value"])
 class UID:
     """A unique ID for every Syft object.
 
     This object creates a unique ID for every object in the Syft
     ecosystem. This ID is guaranteed to be unique for the node on
@@ -79,24 +73,24 @@
             value = uuid.UUID(bytes=value, version=4)
         elif isinstance(value, UID):
             value = value.value
 
         self.value = uuid.uuid4() if value is None else value
 
     @staticmethod
-    def from_string(value: str) -> "UID":
+    def from_string(value: str) -> UID:
         try:
             return UID(value=uuid.UUID(value))
         except ValueError as e:
             critical(f"Unable to convert {value} to UUID. {e}")
             traceback_and_raise(e)
             raise
 
     @staticmethod
-    def with_seed(value: str) -> "UID":
+    def with_seed(value: str) -> UID:
         md5 = hashlib.md5(value.encode("utf-8"), usedforsecurity=False)
         return UID(md5.hexdigest())
 
     def to_string(self) -> str:
         return self.no_dash
 
     def __str__(self) -> str:
@@ -195,15 +189,15 @@
         Return a SHORT human-readable version of the ID which
         makes it print nicer when embedded (often alongside other
         UID objects) within other object __repr__ methods."""
 
         return str(self.value)[:8]
 
     @property
-    def id(self) -> "UID":
+    def id(self) -> UID:
         return self
 
     @classmethod
     def _check_or_convert(cls, value: str | uuid.UUID | UID) -> UID:
         if isinstance(value, uuid.UUID):
             return UID(value)
         elif isinstance(value, str):
```

### Comparing `syft-0.8.7b7/src/syft/util/_std_stream_capture.py` & `syft-0.8.7b8/src/syft/util/_std_stream_capture.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/util/autoreload.py` & `syft-0.8.7b8/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/util/experimental_flags.py` & `syft-0.8.7b8/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/util/filterwarnings.py` & `syft-0.8.7b8/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/util/fonts.py` & `syft-0.8.7b8/src/syft/assets/css/fonts.css`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,93 @@
-# ruff: noqa
-FONT_CSS = """
 /* cyrillic-ext */
 @font-face {
-  font-family: 'Open Sans';
+  font-family: "Open Sans";
   font-style: normal;
   font-weight: 300 800;
   font-stretch: 100%;
-  src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTSKmu0SC55K5gw.woff2) format('woff2');
-  unicode-range: U+0460-052F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F, U+FE2E-FE2F;
+  src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTSKmu0SC55K5gw.woff2)
+    format("woff2");
+  unicode-range: U+0460-052F, U+1C80-1C88, U+20B4, U+2DE0-2DFF, U+A640-A69F,
+    U+FE2E-FE2F;
 }
+
 /* cyrillic */
 @font-face {
-  font-family: 'Open Sans';
+  font-family: "Open Sans";
   font-style: normal;
   font-weight: 300 800;
   font-stretch: 100%;
-  src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTSumu0SC55K5gw.woff2) format('woff2');
+  src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTSumu0SC55K5gw.woff2)
+    format("woff2");
   unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
 }
+
 /* greek-ext */
 @font-face {
-  font-family: 'Open Sans';
+  font-family: "Open Sans";
   font-style: normal;
   font-weight: 300 800;
   font-stretch: 100%;
-  src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTSOmu0SC55K5gw.woff2) format('woff2');
+  src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTSOmu0SC55K5gw.woff2)
+    format("woff2");
   unicode-range: U+1F00-1FFF;
 }
+
 /* greek */
 @font-face {
-  font-family: 'Open Sans';
+  font-family: "Open Sans";
   font-style: normal;
   font-weight: 300 800;
   font-stretch: 100%;
-  src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTSymu0SC55K5gw.woff2) format('woff2');
+  src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTSymu0SC55K5gw.woff2)
+    format("woff2");
   unicode-range: U+0370-03FF;
 }
+
 /* hebrew */
 @font-face {
-  font-family: 'Open Sans';
+  font-family: "Open Sans";
   font-style: normal;
   font-weight: 300 800;
   font-stretch: 100%;
-  src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTS2mu0SC55K5gw.woff2) format('woff2');
+  src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTS2mu0SC55K5gw.woff2)
+    format("woff2");
   unicode-range: U+0590-05FF, U+200C-2010, U+20AA, U+25CC, U+FB1D-FB4F;
 }
+
 /* vietnamese */
 @font-face {
-  font-family: 'Open Sans';
+  font-family: "Open Sans";
   font-style: normal;
   font-weight: 300 800;
   font-stretch: 100%;
-  src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTSCmu0SC55K5gw.woff2) format('woff2');
-  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1, U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329, U+1EA0-1EF9, U+20AB;
+  src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTSCmu0SC55K5gw.woff2)
+    format("woff2");
+  unicode-range: U+0102-0103, U+0110-0111, U+0128-0129, U+0168-0169, U+01A0-01A1,
+    U+01AF-01B0, U+0300-0301, U+0303-0304, U+0308-0309, U+0323, U+0329,
+    U+1EA0-1EF9, U+20AB;
 }
+
 /* latin-ext */
 @font-face {
-  font-family: 'Open Sans';
+  font-family: "Open Sans";
   font-style: normal;
   font-weight: 300 800;
   font-stretch: 100%;
-  src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTSGmu0SC55K5gw.woff2) format('woff2');
-  unicode-range: U+0100-02AF, U+0304, U+0308, U+0329, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF;
+  src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTSGmu0SC55K5gw.woff2)
+    format("woff2");
+  unicode-range: U+0100-02AF, U+0304, U+0308, U+0329, U+1E00-1E9F, U+1EF2-1EFF,
+    U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF;
 }
+
 /* latin */
 @font-face {
-  font-family: 'Open Sans';
+  font-family: "Open Sans";
   font-style: normal;
   font-weight: 300 800;
   font-stretch: 100%;
-  src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTS-mu0SC55I.woff2) format('woff2');
-  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
+  src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTS-mu0SC55I.woff2)
+    format("woff2");
+  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA,
+    U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+2074, U+20AC, U+2122, U+2191,
+    U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
 }
-"""
-
-ITABLES_CSS = ".itables {font-family: 'Consolas', monospace, sans-serif;}"
```

### Comparing `syft-0.8.7b7/src/syft/util/logger.py` & `syft-0.8.7b8/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/util/markdown.py` & `syft-0.8.7b8/src/syft/util/markdown.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/util/notebook_ui/components/base.py` & `syft-0.8.7b8/src/syft/util/notebook_ui/components/base.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/util/notebook_ui/components/sync.py` & `syft-0.8.7b8/src/syft/util/notebook_ui/components/sync.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,29 @@
 # stdlib
+import datetime
 from typing import Any
 
 # third party
 from pydantic import model_validator
 
 # relative
 from ....client.sync_decision import SyncDirection
 from ....service.code.user_code import UserCode
 from ....service.job.job_stash import Job
 from ....service.request.request import Request
+from ....service.response import SyftError
+from ....service.user.user import UserView
+from ....types.datetime import DateTime
+from ....types.datetime import format_timedelta_human_readable
 from ....types.syft_object import SYFT_OBJECT_VERSION_1
 from ....types.syft_object import SyftObject
-from ..notebook_addons import CSS_CODE
+from ..icons import Icon
+from ..styles import CSS_CODE
 from .base import HTMLComponentBase
 
-COPY_ICON = (
-    '<svg width="13" height="13" viewBox="0 0 13 13" fill="none" xmlns="http://www.w3.org/2000/svg">'
-    '<path d="M12 0.5H4C3.86739 0.5 3.74021 0.552679 3.64645 0.646447C3.55268 0.740215 3.5 0.867392 '
-    "3.5 1V3.5H1C0.867392 3.5 0.740215 3.55268 0.646447 3.64645C0.552679 3.74021 0.5 3.86739 0.5 "
-    "4V12C0.5 12.1326 0.552679 12.2598 0.646447 12.3536C0.740215 12.4473 0.867392 12.5 1 12.5H9C9.13261 "
-    "12.5 9.25979 12.4473 9.35355 12.3536C9.44732 12.2598 9.5 12.1326 9.5 12V9.5H12C12.1326 9.5 12.2598 "
-    "9.44732 12.3536 9.35355C12.4473 9.25979 12.5 9.13261 12.5 9V1C12.5 0.867392 12.4473 0.740215 12.3536 "
-    "0.646447C12.2598 0.552679 12.1326 0.5 12 0.5ZM8.5 11.5H1.5V4.5H8.5V11.5ZM11.5 8.5H9.5V4C9.5 3.86739 "
-    '9.44732 3.74021 9.35355 3.64645C9.25979 3.55268 9.13261 3.5 9 3.5H4.5V1.5H11.5V8.5Z" fill="#B4B0BF"/>'
-    "</svg>"
-)
-
-INFO_ICON = """<svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg">
-<path d="M7 1.3125C5.87512 1.3125 4.7755 1.64607 3.8402 2.27102C2.90489 2.89597 2.17591 3.78423 1.74544 4.82349C1.31496 5.86274 1.20233 7.00631 1.42179 8.10958C1.64124 9.21284 2.18292 10.2263 2.97833 11.0217C3.77374 11.8171 4.78716 12.3588 5.89043 12.5782C6.99369 12.7977 8.13726 12.685 9.17651 12.2546C10.2158 11.8241 11.104 11.0951 11.729 10.1598C12.3539 9.2245 12.6875 8.12488 12.6875 7C12.6859 5.49207 12.0862 4.04636 11.0199 2.98009C9.95365 1.91382 8.50793 1.31409 7 1.3125ZM7 11.8125C6.04818 11.8125 5.11773 11.5303 4.32632 11.0014C3.53491 10.4726 2.91808 9.72103 2.55383 8.84166C2.18959 7.9623 2.09428 6.99466 2.27997 6.06113C2.46566 5.12759 2.92401 4.27009 3.59705 3.59705C4.27009 2.92401 5.1276 2.46566 6.06113 2.27997C6.99466 2.09428 7.9623 2.18958 8.84167 2.55383C9.72104 2.91808 10.4726 3.53491 11.0014 4.32632C11.5303 5.11773 11.8125 6.04818 11.8125 7C11.8111 8.27591 11.3036 9.49915 10.4014 10.4014C9.49915 11.3036 8.27591 11.8111 7 11.8125ZM7.875 9.625C7.875 9.74103 7.82891 9.85231 7.74686 9.93436C7.66481 10.0164 7.55353 10.0625 7.4375 10.0625C7.20544 10.0625 6.98288 9.97031 6.81878 9.80622C6.65469 9.64212 6.5625 9.41956 6.5625 9.1875V7C6.44647 7 6.33519 6.95391 6.25314 6.87186C6.1711 6.78981 6.125 6.67853 6.125 6.5625C6.125 6.44647 6.1711 6.33519 6.25314 6.25314C6.33519 6.17109 6.44647 6.125 6.5625 6.125C6.79457 6.125 7.01713 6.21719 7.18122 6.38128C7.34531 6.54538 7.4375 6.76794 7.4375 7V9.1875C7.55353 9.1875 7.66481 9.23359 7.74686 9.31564C7.82891 9.39769 7.875 9.50897 7.875 9.625ZM6.125 4.59375C6.125 4.46396 6.16349 4.33708 6.2356 4.22916C6.30771 4.12124 6.4102 4.03712 6.53012 3.98745C6.65003 3.93778 6.78198 3.92479 6.90928 3.95011C7.03658 3.97543 7.15351 4.03793 7.24529 4.12971C7.33707 4.22149 7.39957 4.33842 7.42489 4.46572C7.45021 4.59302 7.43722 4.72497 7.38755 4.84489C7.33788 4.9648 7.25377 5.06729 7.14585 5.1394C7.03793 5.21151 6.91105 5.25 6.78125 5.25C6.6072 5.25 6.44028 5.18086 6.31721 5.05779C6.19414 4.93472 6.125 4.7678 6.125 4.59375Z" fill="#1F567A"/>
-</svg>
-"""  # noqa: E501
-
 COPY_CSS = """
 .copy-container {
   cursor: pointer;
   border-radius: 3px;
   padding: 0px 3px;
   display: inline-block;
   transition: background-color 0.3s;
@@ -60,31 +49,46 @@
   overflow: hidden;
   text-overflow: ellipsis;
   vertical-align: bottom;
 }
 """
 
 
-class CopyIDButton(HTMLComponentBase):
+class CopyButton(HTMLComponentBase):
     __canonical_name__ = "CopyButton"
     __version__ = SYFT_OBJECT_VERSION_1
     copy_text: str
     max_width: int = 50
 
+    def format_copy_text(self, copy_text: str) -> str:
+        return copy_text
+
     def to_html(self) -> str:
         copy_js = f"event.stopPropagation(); navigator.clipboard.writeText('{self.copy_text}');"
+        text_formatted = self.format_copy_text(self.copy_text)
         button_html = f"""
         <style>{COPY_CSS}</style>
         <div class="copy-container" onclick="{copy_js}">
-            <span class="copy-text-display" style="max-width: {self.max_width}px;">#{self.copy_text}</span>{COPY_ICON}
+            <span class="copy-text-display" style="max-width: {self.max_width}px;">
+                {text_formatted}
+            </span>
+            {Icon.COPY.svg}
         </div>
         """
         return button_html
 
 
+class CopyIDButton(CopyButton):
+    __canonical_name__ = "CopyIDButton"
+    __version__ = SYFT_OBJECT_VERSION_1
+
+    def format_copy_text(self, copy_text: str) -> str:
+        return f"#{copy_text}"
+
+
 class SyncTableObject(HTMLComponentBase):
     __canonical_name__ = "SyncTableObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     object: SyftObject
 
     def get_status_str(self) -> str:
@@ -98,37 +102,76 @@
             if len(statusses) != 1:
                 raise ValueError("Request code should have exactly one status")
             status_tuple = statusses[0]
             status, _ = status_tuple
             return status.value
         return ""  # type: ignore
 
+    def get_updated_by(self) -> str:
+        # TODO replace with centralized SyftObject created/updated by attribute
+        if isinstance(self.object, Request):
+            email = self.object.requesting_user_email
+            if email is not None:
+                return f"Requested by {email}"
+
+        user_view: UserView | SyftError | None = None
+        if isinstance(self.object, UserCode):
+            user_view = self.object.user
+
+        if isinstance(user_view, UserView):
+            return f"Created by {user_view.email}"
+        return ""
+
+    def get_updated_delta_str(self) -> str:
+        # TODO replace with centralized SyftObject created/updated by attribute
+        if isinstance(self.object, Job):
+            # NOTE Job is not using DateTime for creation_time, so we need to handle it separately
+            time_str = self.object.creation_time
+            if time_str is not None:
+                t = datetime.datetime.fromisoformat(time_str)
+                delta = datetime.datetime.now(datetime.timezone.utc) - t
+                return f"{format_timedelta_human_readable(delta)} ago"
+
+        dt: DateTime | None = None
+        if isinstance(self.object, Request):
+            dt = self.object.request_time
+        if isinstance(self.object, UserCode):
+            dt = self.object.submit_time
+        if dt is not None:
+            delta = DateTime.now().timedelta(dt)
+            delta_str = format_timedelta_human_readable(delta)
+            return f"{delta_str} ago"
+
+        return ""
+
     def to_html(self) -> str:
-        type_html = Badge(object=self.object).to_html()
+        type_html = TypeLabel(object=self.object).to_html()
 
-        type_html = Badge(object=self.object).to_html()
+        type_html = TypeLabel(object=self.object).to_html()
         description_html = MainDescription(object=self.object).to_html()
         copy_id_button = CopyIDButton(
             copy_text=str(self.object.id.id), max_width=60
         ).to_html()
 
-        updated_delta_str = "29m ago"
-        updated_by = "john@doe.org"
+        updated_delta_str = self.get_updated_delta_str()
+        updated_by = self.get_updated_by()
         status_str = self.get_status_str()
-        status_seperator = " • " if len(status_str) else ""
+        status_row = " • ".join(
+            s for s in [status_str, updated_by, updated_delta_str] if s
+        )
         summary_html = f"""
             <div style="display: flex; gap: 8px; justify-content: space-between; width: 100%; overflow: hidden; align-items: center;">
             <div style="display: flex; gap: 8px; justify-content: start; align-items: center;">
             {type_html} {description_html}
             </div>
             {copy_id_button}
             </div>
             <div style="display: table-row">
             <span class='syncstate-col-footer'>
-            {status_str}{status_seperator}Updated by {updated_by} {updated_delta_str}
+            {status_row}
             </span>
             </div>
         """  # noqa: E501
         summary_html = summary_html.replace("\n", "").replace("    ", "")
         return summary_html
 
 
@@ -153,49 +196,75 @@
     font-family: 'Open Sans';
 }
 """
 
 
 class Alert(HTMLComponentBase):
     __canonical_name__ = "Alert"
-    __version__ = SYFT_OBJECT_VERSION_1  # Ensure the version constant is correctly defined elsewhere
+    __version__ = SYFT_OBJECT_VERSION_1
     message: str
 
     def to_html(self) -> str:
-        full_message = f"{INFO_ICON} {self.message}"
+        full_message = f"{Icon.INFO.svg} {self.message}"
         return f"""
             <style>{ALERT_CSS}</style>
             <div class="syft-alert-container">
             <div class="syft-alert-info">
             {full_message}
             </div>
             </div>
             """
 
 
 class Badge(HTMLComponentBase):
-    __canonical_name__ = "CopyButton"
+    __canonical_name__ = "Badge"
+    __version__ = SYFT_OBJECT_VERSION_1
+    value: str
+    badge_class: str
+
+    def to_html(self) -> str:
+        value = str(self.value).upper()
+        return f'<span class="badge {self.badge_class}">{value}</span>'
+
+
+class Label(HTMLComponentBase):
+    __canonical_name__ = "Label"
+    __version__ = SYFT_OBJECT_VERSION_1
+    value: str
+    label_class: str
+
+    def to_html(self) -> str:
+        value = str(self.value).upper()
+        return f'<span class="label {self.label_class}">{value}</span>'
+
+
+class TypeLabel(Label):
+    __canonical_name__ = "TypeLabel"
     __version__ = SYFT_OBJECT_VERSION_1
     object: SyftObject
 
-    def type_badge_class(self) -> str:
-        if isinstance(self.object, UserCode):
+    @model_validator(mode="before")
+    @classmethod
+    def validate_label(cls, data: dict) -> dict:
+        obj = data["object"]
+        data["label_class"] = cls.type_label_class(obj)
+        data["value"] = type(obj).__name__.upper()
+        return data
+
+    @staticmethod
+    def type_label_class(obj: Any) -> str:
+        if isinstance(obj, UserCode):
             return "label-light-blue"
-        elif isinstance(self.object, Job):  # type: ignore
+        elif isinstance(obj, Job):  # type: ignore
             return "label-light-blue"
-        elif isinstance(self.object, Request):  # type: ignore
+        elif isinstance(obj, Request):  # type: ignore
             # TODO: handle other requests
             return "label-light-purple"
         return "label-light-blue"  # type: ignore
 
-    def to_html(self) -> str:
-        badge_class = self.type_badge_class()
-        object_type = type(self.object).__name__.upper()
-        return f'<div class="label {badge_class}">{object_type}</div>'
-
 
 class MainDescription(HTMLComponentBase):
     __canonical_name__ = "CopyButton"
     __version__ = SYFT_OBJECT_VERSION_1
     object: SyftObject
 
     def main_object_description_str(self) -> str:
@@ -231,15 +300,15 @@
 
     def to_html(self) -> str:
         # CSS Styles
         style = CSS_CODE
 
         first_line_html = "<span style='color: #B4B0BF;'>Syncing changes on</span>"
 
-        type_html = Badge(object=self.object).to_html()
+        type_html = TypeLabel(object=self.object).to_html()
         description_html = MainDescription(object=self.object).to_html()
         copy_id_button = CopyIDButton(
             copy_text=str(self.object.id.id), max_width=60
         ).to_html()
 
         second_line_html = f"""
             <div class="widget-header2">
```

### Comparing `syft-0.8.7b7/src/syft/util/schema.py` & `syft-0.8.7b8/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/util/telemetry.py` & `syft-0.8.7b8/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/util/trace_decorator.py` & `syft-0.8.7b8/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft/util/util.py` & `syft-0.8.7b8/src/syft/util/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from multiprocessing import set_start_method
 from multiprocessing.synchronize import Event as EventClass
 from multiprocessing.synchronize import Lock as LockBase
 import operator
 import os
 from pathlib import Path
 import platform
+import random
 import re
 from secrets import randbelow
 import socket
 import sys
 import threading
 import time
 import types
@@ -305,43 +306,60 @@
 
     multiprocessing.Process(
         target=print_process, args=(message, finish, success, lock)
     ).start()
     return (finish, success)
 
 
-def find_available_port(host: str, port: int, search: bool = False) -> int:
+def find_available_port(
+    host: str, port: int | None = None, search: bool = False
+) -> int:
+    if port is None:
+        port = random.randint(1500, 65000)  # nosec
     port_available = False
     while not port_available:
         try:
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             result_of_check = sock.connect_ex((host, port))
 
             if result_of_check != 0:
                 port_available = True
                 break
             else:
                 if search:
                     port += 1
                 else:
                     break
+            sock.close()
 
         except Exception as e:
             print(f"Failed to check port {port}. {e}")
     sock.close()
 
     if search is False and port_available is False:
         error = (
             f"{port} is in use, either free the port or "
             + f"try: {port}+ to auto search for a port"
         )
         raise Exception(error)
     return port
 
 
+def get_random_available_port() -> int:
+    """Retrieve a random available port number from the host OS.
+
+    Returns
+    -------
+    int: Available port number.
+    """
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as soc:
+        soc.bind(("localhost", 0))
+        return soc.getsockname()[1]
+
+
 def get_loaded_syft() -> ModuleType:
     return sys.modules[__name__.split(".")[0]]
 
 
 def get_subclasses(obj_type: type) -> list[type]:
     """Recursively generate the list of all classes within the sub-tree of an object
 
@@ -884,27 +902,14 @@
         new_module = types.ModuleType(module_name)
     else:
         new_module = sys.modules["syft"].__dict__[module_name]
     setattr(new_module, klass.__name__, klass)
     sys.modules["syft"].__dict__[module_name] = new_module
 
 
-def get_syft_src_path() -> Path:
-    return Path(__file__).parent.parent.parent.expanduser()
-
-
-def get_grid_src_path() -> Path:
-    syft_path = get_syft_src_path()
-    return syft_path.parent.parent / "grid"
-
-
-def get_syft_cpu_dockerfile() -> Path:
-    return get_grid_src_path() / "backend" / "worker_cpu.dockerfile"
-
-
 def get_queue_address(port: int) -> str:
     """Get queue address based on container host name."""
 
     container_host = os.getenv("CONTAINER_HOST", None)
     if container_host == "k8s":
         return f"tcp://backend:{port}"
     elif container_host == "docker":
```

### Comparing `syft-0.8.7b7/src/syft/util/version_compare.py` & `syft-0.8.7b8/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b7/src/syft.egg-info/PKG-INFO` & `syft-0.8.7b8/src/syft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.7b7
+Version: 0.8.7b8
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -14,15 +14,14 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
 Requires-Dist: setuptools
 Requires-Dist: bcrypt==4.1.2
 Requires-Dist: boto3==1.34.56
 Requires-Dist: forbiddenfruit==0.1.4
-Requires-Dist: gevent==23.9.1
 Requires-Dist: loguru==0.7.2
 Requires-Dist: networkx==3.2.1
 Requires-Dist: packaging>=23.0
 Requires-Dist: pyarrow==15.0.0
 Requires-Dist: pycapnp==2.0.0b2
 Requires-Dist: pydantic[email]==2.6.0
 Requires-Dist: pydantic-settings==2.2.1
@@ -35,35 +34,34 @@
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: typeguard==4.1.5
 Requires-Dist: typing_extensions==4.10.0
 Requires-Dist: sherlock[filelock]==0.4.1
 Requires-Dist: uvicorn[standard]==0.27.1
 Requires-Dist: fastapi==0.110.0
 Requires-Dist: psutil==5.9.8
-Requires-Dist: hagrid>=0.3
 Requires-Dist: itables==1.7.1
 Requires-Dist: argon2-cffi==23.1.0
 Requires-Dist: matplotlib==3.8.3
-Requires-Dist: jaxlib==0.4.20
-Requires-Dist: jax==0.4.20
 Requires-Dist: numpy<=1.24.4,>=1.23.5; python_version < "3.12"
 Requires-Dist: numpy<1.27,>=1.26.4; python_version >= "3.12"
 Requires-Dist: pandas==2.2.1
 Requires-Dist: docker==6.1.3
 Requires-Dist: kr8s==0.13.5
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: azure-storage-blob==12.19.1
 Requires-Dist: ipywidgets==8.1.2
+Requires-Dist: rich==13.7.1
+Requires-Dist: jinja2==3.1.4
+Requires-Dist: tenacity==8.3.0
 Provides-Extra: data-science
 Requires-Dist: transformers==4.39.3; extra == "data-science"
 Requires-Dist: opendp==0.9.2; extra == "data-science"
 Requires-Dist: evaluate==0.4.1; extra == "data-science"
 Requires-Dist: recordlinkage==0.16; extra == "data-science"
-Requires-Dist: dm-haiku==0.0.10; extra == "data-science"
-Requires-Dist: torch[cpu]==2.2.1; extra == "data-science"
+Requires-Dist: torch==2.3.0; extra == "data-science"
 Provides-Extra: dev
 Requires-Dist: pytest<8; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-xdist[psutil]; extra == "dev"
 Requires-Dist: pytest-parallel; extra == "dev"
 Requires-Dist: pytest-randomly; extra == "dev"
 Requires-Dist: pytest-sugar; extra == "dev"
@@ -108,62 +106,74 @@
 
 <img alt="Syft Logo" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/title_syft_light.png" width="200px" />
 
 Perform data science on `data` that remains in `someone else's` server
 
 # Quickstart
 
-✅ `Linux` ✅ `macOS` ✅ `Windows` ✅ `Docker` ✅ `Podman` ✅ `Kubernetes`
+✅ `Linux` ✅ `macOS` ✅ `Windows` ✅ `Docker` ✅ `Kubernetes`
 
 ## Install Client
 
 ```bash
 $ pip install -U syft[data_science]
 ```
 
 ## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
 sy.requires(">=0.8.6,<0.8.7")
-node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
+node = sy.orchestra.launch(
+    name="my-domain",
+    port=8080,
+    create_producer=True,
+    n_consumers=1,
+    dev_mode=True,
+    reset=True, # resets database
+)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Launch Client
 
 ```python
 import syft as sy
 sy.requires(">=0.8.6,<0.8.7")
-domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
+domain_client = sy.login(
+    port=8080,
+    email="info@openmined.org",
+    password="changethis"
+)
 ```
 
 ## PySyft in 10 minutes
 
 📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api">API Example Notebooks</a>
 
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/04-pytorch-example.ipynb">04-pytorch-example.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/08-code-version.ipynb">08-code-version.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/09-blob-storage.ipynb">09-blob-storage.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/10-container-images.ipynb">10-container-images.ipynb</a>
 - <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/11-container-images-k8s.ipynb">11-container-images-k8s.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/12-custom-api-endpoint.ipynb">12-custom-api-endpoint.ipynb</a>
 
 ## Deploy Kubernetes Helm Chart
 
 **Note**: Assuming we have a Kubernetes cluster already setup.
 
 #### 1. Add and update Helm repo for Syft
 
@@ -200,44 +210,35 @@
 
 For AWS EKS
 
 ```sh
 helm install ... --set ingress.className="alb"
 ```
 
-For Google GKE we need the [`gce` annotation](https://cloud.google.com/kubernetes-engine/docs/how-to/load-balance-ingress#create-ingress) annotation.
+For Google GKE we need the [`gce` annotation](https://cloud.google.com/kubernetes-engine/docs/how-to/load-balance-ingress#create-ingress).
 
 ```sh
 helm install ... --set ingress.class="gce"
 ```
 
-## Deploy to a Container Engine or Cloud
+## Note:
 
-1. Install our handy 🛵 cli tool which makes deploying a Domain or Gateway server to Docker or VM a one-liner:  
-   `pip install -U hagrid`
+🚨 Our old deployment tool `HAGrid` has been `deprecated`. For the updated deployment options kindly refer to:
 
-2. Then run our interactive jupyter Install 🧙🏽‍♂️ Wizard<sup>BETA</sup>:  
-   `hagrid quickstart`
-
-3. In the tutorial you will learn how to install and deploy:  
-   `PySyft` = our `numpy`-like 🐍 Python library for computing on `private data` in someone else's `Domain`
-
-   `PyGrid` = our 🐳 `docker` / 🐧 `vm` `Domain` & `Gateway` Servers where `private data` lives
+- 📚 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/tutorials/deployments">Deployments</a>
 
 ## Docs and Support
 
 - 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
 - `#support` on <a href="https://slack.openmined.org/">Slack</a>
 
 # Install Notes
 
-- HAGrid 0.3 Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
-- Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
-- PySyft 0.8.1 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
-- PyGrid Requires: 🐳 `docker`, 🦦 `podman` or ☸️ `kubernetes` - Run: `hagrid launch ...`
+- PySyft 0.8.6 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
+- PyGrid Requires: 🐳 `docker` or ☸️ `kubernetes`
 
 # Versions
 
 `0.9.0` - Coming soon...  
 `0.8.7` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
 `0.8.6` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8">API</a>
 
@@ -252,21 +253,17 @@
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
 - `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
 - `0.2.0` - `0.5.0`
 
 PySyft and PyGrid use the same `version` and its best to match them up where possible. We release weekly betas which can be used in each context:
 
-PySyft (Stable): `pip install -U syft`  
-PyGrid (Stable) `hagrid launch ... tag=latest`
-
-PySyft (Beta): `pip install -U syft --pre`  
-PyGrid (Beta): `hagrid launch ... tag=beta`
+PySyft (Stable): `pip install -U syft`
 
-HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually the best.
+PySyft (Beta): `pip install -U syft --pre`
 
 # What is Syft?
 
 <img align="right" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
 
 `Syft` is OpenMined's `open source` stack that provides `secure` and `private` Data Science in Python. Syft decouples `private data` from model training, using techniques like [Federated Learning](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and integration with `Deep Learning` frameworks, so that you as a `Data Scientist` can maintain your current workflow while using these new `privacy-enhancing techniques`.
```

### Comparing `syft-0.8.7b7/src/syft.egg-info/SOURCES.txt` & `syft-0.8.7b8/src/syft.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -5,32 +5,48 @@
 pyproject.toml
 setup.cfg
 setup.py
 src/syft/VERSION
 src/syft/__init__.py
 src/syft/__main__.py
 src/syft/abstract_node.py
-src/syft/gevent_patch.py
+src/syft/orchestra.py
 src/syft/stable_version.py
 src/syft.egg-info/PKG-INFO
 src/syft.egg-info/SOURCES.txt
 src/syft.egg-info/dependency_links.txt
 src/syft.egg-info/entry_points.txt
 src/syft.egg-info/not-zip-safe
 src/syft.egg-info/requires.txt
 src/syft.egg-info/top_level.txt
+src/syft/assets/css/fonts.css
+src/syft/assets/css/itables.css
+src/syft/assets/css/style.css
+src/syft/assets/css/tabulator_pysyft.min.css
+src/syft/assets/img/logo.png
+src/syft/assets/img/small-grid-symbol-logo.png
+src/syft/assets/jinja/table.jinja2
+src/syft/assets/js/table.js
+src/syft/assets/js/tabulator.min.js
+src/syft/assets/svg/arrow.svg
+src/syft/assets/svg/clipboard.svg
+src/syft/assets/svg/copy.svg
+src/syft/assets/svg/folder.svg
+src/syft/assets/svg/info.svg
+src/syft/assets/svg/request.svg
+src/syft/assets/svg/search.svg
+src/syft/assets/svg/table.svg
 src/syft/capnp/__init__.py
 src/syft/capnp/iterable.capnp
 src/syft/capnp/kv_iterable.capnp
 src/syft/capnp/recursive_serde.capnp
 src/syft/client/__init__.py
 src/syft/client/api.py
 src/syft/client/client.py
 src/syft/client/connection.py
-src/syft/client/deploy.py
 src/syft/client/domain_client.py
 src/syft/client/enclave_client.py
 src/syft/client/gateway_client.py
 src/syft/client/protocol.py
 src/syft/client/registry.py
 src/syft/client/search.py
 src/syft/client/sync_decision.py
@@ -44,17 +60,14 @@
 src/syft/custom_worker/config.py
 src/syft/custom_worker/k8s.py
 src/syft/custom_worker/runner_k8s.py
 src/syft/custom_worker/utils.py
 src/syft/exceptions/__init__.py
 src/syft/exceptions/exception.py
 src/syft/exceptions/user.py
-src/syft/img/base64.py
-src/syft/img/logo.png
-src/syft/img/small-grid-symbol-logo.png
 src/syft/node/__init__.py
 src/syft/node/credentials.py
 src/syft/node/domain.py
 src/syft/node/enclave.py
 src/syft/node/gateway.py
 src/syft/node/node.py
 src/syft/node/routes.py
@@ -101,14 +114,17 @@
 src/syft/service/action/numpy.py
 src/syft/service/action/pandas.py
 src/syft/service/action/plan.py
 src/syft/service/action/verification.py
 src/syft/service/api/api.py
 src/syft/service/api/api_service.py
 src/syft/service/api/api_stash.py
+src/syft/service/attestation/__init__.py
+src/syft/service/attestation/attestation_constants.py
+src/syft/service/attestation/attestation_service.py
 src/syft/service/blob_storage/__init__.py
 src/syft/service/blob_storage/remote_profile.py
 src/syft/service/blob_storage/service.py
 src/syft/service/blob_storage/stash.py
 src/syft/service/code/__init__.py
 src/syft/service/code/code_parse.py
 src/syft/service/code/status_service.py
@@ -143,14 +159,15 @@
 src/syft/service/metadata/metadata_service.py
 src/syft/service/metadata/migrations.py
 src/syft/service/metadata/node_metadata.py
 src/syft/service/network/association_request.py
 src/syft/service/network/network_service.py
 src/syft/service/network/node_peer.py
 src/syft/service/network/routes.py
+src/syft/service/network/utils.py
 src/syft/service/notification/__init__.py
 src/syft/service/notification/email_templates.py
 src/syft/service/notification/notification_service.py
 src/syft/service/notification/notification_stash.py
 src/syft/service/notification/notifications.py
 src/syft/service/notifier/notifier.py
 src/syft/service/notifier/notifier_enums.py
@@ -236,29 +253,32 @@
 src/syft/types/syft_object.py
 src/syft/types/syncable_object.py
 src/syft/types/transforms.py
 src/syft/types/twin_object.py
 src/syft/types/uid.py
 src/syft/util/__init__.py
 src/syft/util/_std_stream_capture.py
+src/syft/util/assets.py
 src/syft/util/autoreload.py
 src/syft/util/colors.py
 src/syft/util/constants.py
 src/syft/util/decorators.py
 src/syft/util/env.py
 src/syft/util/experimental_flags.py
 src/syft/util/filterwarnings.py
-src/syft/util/fonts.py
-src/syft/util/jax_settings.py
 src/syft/util/logger.py
 src/syft/util/markdown.py
 src/syft/util/options.py
 src/syft/util/schema.py
+src/syft/util/table.py
 src/syft/util/telemetry.py
 src/syft/util/trace_decorator.py
 src/syft/util/util.py
 src/syft/util/version_compare.py
 src/syft/util/notebook_ui/__init__.py
-src/syft/util/notebook_ui/notebook_addons.py
+src/syft/util/notebook_ui/icons.py
+src/syft/util/notebook_ui/styles.py
 src/syft/util/notebook_ui/components/__init__.py
 src/syft/util/notebook_ui/components/base.py
-src/syft/util/notebook_ui/components/sync.py
+src/syft/util/notebook_ui/components/sync.py
+src/syft/util/notebook_ui/components/table_template.py
+src/syft/util/notebook_ui/components/tabulator_template.py
```

### Comparing `syft-0.8.7b7/src/syft.egg-info/requires.txt` & `syft-0.8.7b8/src/syft.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 setuptools
 bcrypt==4.1.2
 boto3==1.34.56
 forbiddenfruit==0.1.4
-gevent==23.9.1
 loguru==0.7.2
 networkx==3.2.1
 packaging>=23.0
 pyarrow==15.0.0
 pycapnp==2.0.0b2
 pydantic[email]==2.6.0
 pydantic-settings==2.2.1
@@ -19,40 +18,39 @@
 tqdm==4.66.2
 typeguard==4.1.5
 typing_extensions==4.10.0
 sherlock[filelock]==0.4.1
 uvicorn[standard]==0.27.1
 fastapi==0.110.0
 psutil==5.9.8
-hagrid>=0.3
 itables==1.7.1
 argon2-cffi==23.1.0
 matplotlib==3.8.3
-jaxlib==0.4.20
-jax==0.4.20
 pandas==2.2.1
 docker==6.1.3
 kr8s==0.13.5
 PyYAML==6.0.1
 azure-storage-blob==12.19.1
 ipywidgets==8.1.2
+rich==13.7.1
+jinja2==3.1.4
+tenacity==8.3.0
 
 [:python_version < "3.12"]
 numpy<=1.24.4,>=1.23.5
 
 [:python_version >= "3.12"]
 numpy<1.27,>=1.26.4
 
 [data_science]
 transformers==4.39.3
 opendp==0.9.2
 evaluate==0.4.1
 recordlinkage==0.16
-dm-haiku==0.0.10
-torch[cpu]==2.2.1
+torch==2.3.0
 
 [dev]
 pytest<8
 pytest-cov
 pytest-xdist[psutil]
 pytest-parallel
 pytest-randomly
```

