# Comparing `tmp/spaceone-api-2.0.dev78.tar.gz` & `tmp/spaceone-api-2.0.dev89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceone-api-2.0.dev78.tar", last modified: Tue Dec 26 10:34:04 2023, max compression
+gzip compressed data, was "spaceone-api-2.0.dev89.tar", last modified: Thu Jan  4 17:50:06 2024, max compression
```

## Comparing `spaceone-api-2.0.dev78.tar` & `spaceone-api-2.0.dev89.tar`

### file list

```diff
@@ -1,290 +1,290 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.210587 spaceone-api-2.0.dev78/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-12-26 10:34:04.210587 spaceone-api-2.0.dev78/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-26 10:34:04.210587 spaceone-api-2.0.dev78/setup.cfg
--rwxrwxrwx   0 runner    (1001) docker     (127)     1009 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.174587 spaceone-api-2.0.dev78/spaceone/
--rwxrwxrwx   0 runner    (1001) docker     (127)       64 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.174587 spaceone-api-2.0.dev78/spaceone/api/
--rwxrwxrwx   0 runner    (1001) docker     (127)       13 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.174587 spaceone-api-2.0.dev78/spaceone/api/board/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/board/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.174587 spaceone-api-2.0.dev78/spaceone/api/board/v1/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/board/v1/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     7444 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/board/v1/post_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    13279 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/board/v1/post_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.174587 spaceone-api-2.0.dev78/spaceone/api/config/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.174587 spaceone-api-2.0.dev78/spaceone/api/config/v1/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/config/v1/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6151 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/config/v1/domain_config_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    13548 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/config/v1/domain_config_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6024 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/config/v1/user_config_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    13344 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/config/v1/user_config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.174587 spaceone-api-2.0.dev78/spaceone/api/core/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.174587 spaceone-api-2.0.dev78/spaceone/api/core/v1/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/core/v1/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     3351 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/core/v1/handler_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)      159 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/core/v1/handler_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11552 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/core/v1/query_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)      159 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/core/v1/query_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     1622 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/core/v1/server_info_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2768 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/core/v1/server_info_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.178587 spaceone-api-2.0.dev78/spaceone/api/core/v2/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/core/v2/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     1996 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/core/v2/handler_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)      159 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/core/v2/handler_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2658 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/core/v2/plugin_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)      159 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/core/v2/plugin_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11013 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/core/v2/query_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)      159 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/core/v2/query_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.178587 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.178587 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/plugin/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/plugin/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2856 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/plugin/cost_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2800 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/plugin/cost_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2561 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/plugin/data_source_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     4686 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/plugin/data_source_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2690 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/plugin/job_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2792 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/plugin/job_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.182587 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11174 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/budget_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    13961 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/budget_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     5837 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/budget_usage_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6469 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/budget_usage_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     7424 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/cost_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    12237 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/cost_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6661 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/cost_query_set_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    12538 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/cost_query_set_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    15135 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/data_source_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    21972 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/data_source_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11508 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/data_source_rule_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    15344 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/data_source_rule_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6074 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/job_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     7976 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/job_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     5687 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/job_task_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6598 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/job_task_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.182587 spaceone-api-2.0.dev78/spaceone/api/dashboard/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.182587 spaceone-api-2.0.dev78/spaceone/api/dashboard/v1/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/dashboard/v1/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11109 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/dashboard/v1/private_dashboard_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    19927 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/dashboard/v1/private_dashboard_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11908 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/dashboard/v1/public_dashboard_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    19798 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/dashboard/v1/public_dashboard_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.182587 spaceone-api-2.0.dev78/spaceone/api/file_manager/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/file_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.182587 spaceone-api-2.0.dev78/spaceone/api/file_manager/v1/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/file_manager/v1/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     8181 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/file_manager/v1/file_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    13163 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/file_manager/v1/file_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.182587 spaceone-api-2.0.dev78/spaceone/api/identity/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/identity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.182587 spaceone-api-2.0.dev78/spaceone/api/identity/plugin/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/identity/plugin/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     4443 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/identity/plugin/auth_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     7868 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/identity/plugin/auth_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.186587 spaceone-api-2.0.dev78/spaceone/api/identity/v1/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6694 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/api_key_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    13106 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/api_key_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     1672 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/authorization_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2786 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/authorization_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     4249 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/domain_owner_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     8183 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/domain_owner_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     9302 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/domain_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    21983 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/domain_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     3058 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/endpoint_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2732 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/endpoint_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6184 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/policy_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11326 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/policy_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    13125 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/project_group_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    21293 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/project_group_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11066 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/project_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    18640 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/project_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6955 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/provider_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11481 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/provider_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     7734 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/role_binding_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11781 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/role_binding_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     7996 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/role_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11165 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/role_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     7878 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/service_account_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    12018 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/service_account_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2962 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/token_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     4330 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/token_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    15591 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/user_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    30262 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v1/user_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.194587 spaceone-api-2.0.dev78/spaceone/api/identity/v2/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     9992 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/app_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    17945 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/app_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     8828 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/domain_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    18453 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/domain_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     3012 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/endpoint_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2710 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/endpoint_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     3951 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/external_auth_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6438 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/external_auth_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6992 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/project_group_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    13790 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/project_group_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    10483 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/project_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    22361 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/project_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6642 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/provider_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11490 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/provider_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     8281 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/role_binding_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11825 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/role_binding_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6345 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/role_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11174 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/role_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     7069 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/schema_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11332 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/schema_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     8548 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/service_account_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    15917 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/service_account_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2329 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/system_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2705 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/system_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     4866 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/token_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     4342 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/token_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     8763 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/trusted_account_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    13990 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/trusted_account_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     7001 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/user_group_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    15271 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/user_group_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11290 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/user_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    19973 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/user_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     7457 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/user_profile_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    17347 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/user_profile_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     7345 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/workspace_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    16780 2023-12-26 10:33:45.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/workspace_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     9057 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/workspace_user_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    10137 2023-12-26 10:33:46.000000 spaceone-api-2.0.dev78/spaceone/api/identity/v2/workspace_user_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.194587 spaceone-api-2.0.dev78/spaceone/api/inventory/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.194587 spaceone-api-2.0.dev78/spaceone/api/inventory/plugin/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/plugin/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     3996 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/plugin/collector_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6616 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/plugin/collector_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2686 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/plugin/job_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2738 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/plugin/job_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.198587 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     4696 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/change_history_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     4653 2023-12-26 10:33:44.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/change_history_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    10849 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    15980 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11713 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_query_set_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    20293 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_query_set_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    10859 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_report_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    14182 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_report_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     5222 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_stats_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6632 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_stats_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     7893 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_type_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    12802 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_type_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    12578 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/collector_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    17496 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/collector_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    10662 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/collector_rule_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    14772 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/collector_rule_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6362 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/job_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     9505 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/job_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6471 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/job_task_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     8142 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/job_task_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     5753 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/note_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11201 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/note_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6072 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/region_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11848 2023-12-26 10:33:43.000000 spaceone-api-2.0.dev78/spaceone/api/inventory/v1/region_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.198587 spaceone-api-2.0.dev78/spaceone/api/monitoring/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.198587 spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2462 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/data_source_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     4867 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/data_source_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2996 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/event_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2919 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/event_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2449 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/log_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2714 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/log_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     3417 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/metric_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     4834 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/metric_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2422 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/webhook_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     4831 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/webhook_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.202587 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     9415 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/alert_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    15380 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/alert_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    10313 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/data_source_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    19714 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/data_source_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11114 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/escalation_policy_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    14945 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/escalation_policy_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     5675 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/event_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     8178 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/event_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11095 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/event_rule_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    13987 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/event_rule_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2473 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/log_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2664 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/log_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     3895 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/metric_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     4686 2023-12-26 10:33:48.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/metric_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     5697 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/note_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11463 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/note_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     7745 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/project_alert_config_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    13470 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/project_alert_config_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     9971 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/webhook_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    19152 2023-12-26 10:33:47.000000 spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/webhook_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.202587 spaceone-api-2.0.dev78/spaceone/api/notification/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/notification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.202587 spaceone-api-2.0.dev78/spaceone/api/notification/plugin/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/notification/plugin/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2579 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/notification/plugin/notification_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     3176 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/notification/plugin/notification_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2425 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/notification/plugin/protocol_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     4758 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/notification/plugin/protocol_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.206587 spaceone-api-2.0.dev78/spaceone/api/notification/v1/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/notification/v1/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     9925 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/notification/v1/notification_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    14247 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/notification/v1/notification_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    12206 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/notification/v1/project_channel_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    21477 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/notification/v1/project_channel_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    10506 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/notification/v1/protocol_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    17648 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/notification/v1/protocol_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11057 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/notification/v1/user_channel_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    21131 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/notification/v1/user_channel_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.206587 spaceone-api-2.0.dev78/spaceone/api/plugin/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.206587 spaceone-api-2.0.dev78/spaceone/api/plugin/v1/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/plugin/v1/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     4284 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/plugin/v1/plugin_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     6674 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/plugin/v1/plugin_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    11186 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/plugin/v1/supervisor_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    21525 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/plugin/v1/supervisor_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.206587 spaceone-api-2.0.dev78/spaceone/api/repository/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/repository/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.206587 spaceone-api-2.0.dev78/spaceone/api/repository/v1/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/repository/v1/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     9815 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/repository/v1/plugin_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    17751 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/repository/v1/plugin_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2786 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/repository/v1/repository_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2867 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/repository/v1/repository_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.206587 spaceone-api-2.0.dev78/spaceone/api/sample/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/sample/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.206587 spaceone-api-2.0.dev78/spaceone/api/sample/v1/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/sample/v1/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     1679 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/sample/v1/helloworld_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2675 2023-12-26 10:33:50.000000 spaceone-api-2.0.dev78/spaceone/api/sample/v1/helloworld_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.206587 spaceone-api-2.0.dev78/spaceone/api/secret/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.206587 spaceone-api-2.0.dev78/spaceone/api/secret/v1/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/secret/v1/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     8531 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/secret/v1/secret_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    15007 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/secret/v1/secret_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     8092 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/secret/v1/trusted_secret_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    13938 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/secret/v1/trusted_secret_pb2_grpc.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     7986 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/secret/v1/user_secret_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)    15515 2023-12-26 10:33:49.000000 spaceone-api-2.0.dev78/spaceone/api/secret/v1/user_secret_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.206587 spaceone-api-2.0.dev78/spaceone/api/statistics/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/statistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.210587 spaceone-api-2.0.dev78/spaceone/api/statistics/v1/
--rwxrwxrwx   0 runner    (1001) docker     (127)        0 2023-12-26 10:33:51.000000 spaceone-api-2.0.dev78/spaceone/api/statistics/v1/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     5223 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/statistics/v1/resource_pb2.py
--rwxrwxrwx   0 runner    (1001) docker     (127)     2968 2023-12-26 10:33:42.000000 spaceone-api-2.0.dev78/spaceone/api/statistics/v1/resource_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 10:34:04.210587 spaceone-api-2.0.dev78/spaceone_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-12-26 10:34:03.000000 spaceone-api-2.0.dev78/spaceone_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2023-12-26 10:34:04.000000 spaceone-api-2.0.dev78/spaceone_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-26 10:34:03.000000 spaceone-api-2.0.dev78/spaceone_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-26 10:34:03.000000 spaceone-api-2.0.dev78/spaceone_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-26 10:34:03.000000 spaceone-api-2.0.dev78/spaceone_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.751173 spaceone-api-2.0.dev89/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-04 17:50:06.747173 spaceone-api-2.0.dev89/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-04 17:50:06.751173 spaceone-api-2.0.dev89/setup.cfg
+-rwxrwxrwx   0 runner    (1001) docker     (127)     1009 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.711173 spaceone-api-2.0.dev89/spaceone/
+-rwxrwxrwx   0 runner    (1001) docker     (127)       64 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.711173 spaceone-api-2.0.dev89/spaceone/api/
+-rwxrwxrwx   0 runner    (1001) docker     (127)       13 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.711173 spaceone-api-2.0.dev89/spaceone/api/board/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/board/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.711173 spaceone-api-2.0.dev89/spaceone/api/board/v1/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/board/v1/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     7444 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/board/v1/post_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    13279 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/board/v1/post_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.711173 spaceone-api-2.0.dev89/spaceone/api/config/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.711173 spaceone-api-2.0.dev89/spaceone/api/config/v1/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/config/v1/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6151 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/config/v1/domain_config_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    13548 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/config/v1/domain_config_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6024 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/config/v1/user_config_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    13344 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/config/v1/user_config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.711173 spaceone-api-2.0.dev89/spaceone/api/core/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.711173 spaceone-api-2.0.dev89/spaceone/api/core/v1/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/core/v1/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     3351 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/core/v1/handler_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)      159 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/core/v1/handler_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11552 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/core/v1/query_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)      159 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/core/v1/query_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     1622 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/core/v1/server_info_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2768 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/core/v1/server_info_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.715174 spaceone-api-2.0.dev89/spaceone/api/core/v2/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/core/v2/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     1996 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/core/v2/handler_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)      159 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/core/v2/handler_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2658 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/core/v2/plugin_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)      159 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/core/v2/plugin_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11013 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/core/v2/query_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)      159 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/core/v2/query_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.715174 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.715174 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/plugin/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/plugin/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2856 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/plugin/cost_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2800 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/plugin/cost_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2561 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/plugin/data_source_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     4686 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/plugin/data_source_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2690 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/plugin/job_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2792 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/plugin/job_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.719174 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11174 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/budget_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    13961 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/budget_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     5837 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/budget_usage_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6469 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/budget_usage_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     7424 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/cost_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    12237 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/cost_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6703 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/cost_query_set_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    12538 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/cost_query_set_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    15135 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/data_source_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    21972 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/data_source_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11508 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/data_source_rule_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    15344 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/data_source_rule_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6074 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/job_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     7976 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/job_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     5687 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/job_task_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6598 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/job_task_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.719174 spaceone-api-2.0.dev89/spaceone/api/dashboard/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.719174 spaceone-api-2.0.dev89/spaceone/api/dashboard/v1/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/dashboard/v1/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11109 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/dashboard/v1/private_dashboard_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    19927 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/dashboard/v1/private_dashboard_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11908 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/dashboard/v1/public_dashboard_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    19798 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/dashboard/v1/public_dashboard_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.719174 spaceone-api-2.0.dev89/spaceone/api/file_manager/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/file_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.719174 spaceone-api-2.0.dev89/spaceone/api/file_manager/v1/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/file_manager/v1/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     8181 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/file_manager/v1/file_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    13163 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/file_manager/v1/file_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.719174 spaceone-api-2.0.dev89/spaceone/api/identity/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/identity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.719174 spaceone-api-2.0.dev89/spaceone/api/identity/plugin/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/identity/plugin/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     3301 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/plugin/external_auth_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     4671 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/plugin/external_auth_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.723173 spaceone-api-2.0.dev89/spaceone/api/identity/v1/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6694 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/api_key_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    13106 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/api_key_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     1672 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/authorization_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2786 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/authorization_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     4249 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/domain_owner_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     8183 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/domain_owner_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     9302 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/domain_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    21983 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/domain_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     3058 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/endpoint_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2732 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/endpoint_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6184 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/policy_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11326 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/policy_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    13125 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/project_group_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    21293 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/project_group_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11066 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/project_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    18640 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/project_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6955 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/provider_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11481 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/provider_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     7734 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/role_binding_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11781 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/role_binding_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     7996 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/role_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11165 2024-01-04 17:49:48.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/role_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     7878 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/service_account_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    12018 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/service_account_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2962 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/token_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     4330 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/token_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    15591 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/user_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    30262 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v1/user_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.731173 spaceone-api-2.0.dev89/spaceone/api/identity/v2/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    10065 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/app_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    17987 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/app_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     8828 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/domain_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    18453 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/domain_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     3012 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/endpoint_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2710 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/endpoint_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     3951 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/external_auth_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6438 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/external_auth_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6992 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/project_group_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    13790 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/project_group_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    10483 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/project_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    22361 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/project_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6642 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/provider_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11490 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/provider_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     8281 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/role_binding_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11825 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/role_binding_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6345 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/role_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11174 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/role_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     7069 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/schema_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11332 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/schema_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     8548 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/service_account_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    15917 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/service_account_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2329 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/system_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2705 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/system_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     4866 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/token_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     4342 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/token_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     8763 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/trusted_account_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    13990 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/trusted_account_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     7001 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/user_group_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    15271 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/user_group_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11284 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/user_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    19973 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/user_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     7457 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/user_profile_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    17347 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/user_profile_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     7345 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/workspace_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    16780 2024-01-04 17:49:49.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/workspace_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     9140 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/workspace_user_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    10137 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/identity/v2/workspace_user_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.731173 spaceone-api-2.0.dev89/spaceone/api/inventory/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.731173 spaceone-api-2.0.dev89/spaceone/api/inventory/plugin/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/plugin/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     3996 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/plugin/collector_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6616 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/plugin/collector_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2686 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/plugin/job_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2738 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/plugin/job_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.735173 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     4696 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/change_history_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     4653 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/change_history_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    10849 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    15980 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11713 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_query_set_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    20293 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_query_set_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    10859 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_report_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    14182 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_report_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     5222 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_stats_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6632 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_stats_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     7893 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_type_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    12802 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_type_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    12578 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/collector_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    17496 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/collector_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    10662 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/collector_rule_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    14772 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/collector_rule_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6362 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/job_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     9505 2024-01-04 17:49:47.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/job_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6471 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/job_task_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     8142 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/job_task_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     5753 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/note_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11201 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/note_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6072 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/region_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11848 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/inventory/v1/region_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.735173 spaceone-api-2.0.dev89/spaceone/api/monitoring/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.739173 spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2462 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/data_source_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     4867 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/data_source_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2996 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/event_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2919 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/event_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2449 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/log_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2714 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/log_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     3417 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/metric_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     4834 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/metric_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2422 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/webhook_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     4831 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/webhook_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.743173 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     9415 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/alert_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    15380 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/alert_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    10313 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/data_source_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    19714 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/data_source_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11114 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/escalation_policy_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    14945 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/escalation_policy_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     5675 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/event_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     8178 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/event_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11095 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/event_rule_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    13987 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/event_rule_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2473 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/log_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2664 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/log_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     3895 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/metric_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     4686 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/metric_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     5697 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/note_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11463 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/note_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     7745 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/project_alert_config_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    13470 2024-01-04 17:49:51.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/project_alert_config_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     9971 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/webhook_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    19152 2024-01-04 17:49:50.000000 spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/webhook_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.743173 spaceone-api-2.0.dev89/spaceone/api/notification/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/notification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.743173 spaceone-api-2.0.dev89/spaceone/api/notification/plugin/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/notification/plugin/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2579 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/notification/plugin/notification_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     3176 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/notification/plugin/notification_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2425 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/notification/plugin/protocol_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     4758 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/notification/plugin/protocol_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.743173 spaceone-api-2.0.dev89/spaceone/api/notification/v1/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/notification/v1/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     9925 2024-01-04 17:49:45.000000 spaceone-api-2.0.dev89/spaceone/api/notification/v1/notification_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    14247 2024-01-04 17:49:45.000000 spaceone-api-2.0.dev89/spaceone/api/notification/v1/notification_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    12206 2024-01-04 17:49:45.000000 spaceone-api-2.0.dev89/spaceone/api/notification/v1/project_channel_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    21477 2024-01-04 17:49:45.000000 spaceone-api-2.0.dev89/spaceone/api/notification/v1/project_channel_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    10506 2024-01-04 17:49:45.000000 spaceone-api-2.0.dev89/spaceone/api/notification/v1/protocol_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    17648 2024-01-04 17:49:45.000000 spaceone-api-2.0.dev89/spaceone/api/notification/v1/protocol_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11071 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/notification/v1/user_channel_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    21131 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/notification/v1/user_channel_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.743173 spaceone-api-2.0.dev89/spaceone/api/plugin/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.743173 spaceone-api-2.0.dev89/spaceone/api/plugin/v1/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/plugin/v1/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     4284 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/plugin/v1/plugin_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6674 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/plugin/v1/plugin_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    11186 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/plugin/v1/supervisor_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    21525 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/plugin/v1/supervisor_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.743173 spaceone-api-2.0.dev89/spaceone/api/repository/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/repository/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.747173 spaceone-api-2.0.dev89/spaceone/api/repository/v1/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/repository/v1/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     9815 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/repository/v1/plugin_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    17751 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/repository/v1/plugin_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2786 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/repository/v1/repository_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2867 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/repository/v1/repository_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.747173 spaceone-api-2.0.dev89/spaceone/api/sample/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/sample/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.747173 spaceone-api-2.0.dev89/spaceone/api/sample/v1/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/sample/v1/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     1679 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/sample/v1/helloworld_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2675 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/sample/v1/helloworld_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.747173 spaceone-api-2.0.dev89/spaceone/api/secret/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.747173 spaceone-api-2.0.dev89/spaceone/api/secret/v1/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/secret/v1/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     8531 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/secret/v1/secret_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    15007 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/secret/v1/secret_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     8092 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/secret/v1/trusted_secret_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    13938 2024-01-04 17:49:53.000000 spaceone-api-2.0.dev89/spaceone/api/secret/v1/trusted_secret_pb2_grpc.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     7986 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/secret/v1/user_secret_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)    15515 2024-01-04 17:49:52.000000 spaceone-api-2.0.dev89/spaceone/api/secret/v1/user_secret_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.747173 spaceone-api-2.0.dev89/spaceone/api/statistics/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/statistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.747173 spaceone-api-2.0.dev89/spaceone/api/statistics/v1/
+-rwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-01-04 17:49:54.000000 spaceone-api-2.0.dev89/spaceone/api/statistics/v1/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     5223 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/statistics/v1/resource_pb2.py
+-rwxrwxrwx   0 runner    (1001) docker     (127)     2968 2024-01-04 17:49:46.000000 spaceone-api-2.0.dev89/spaceone/api/statistics/v1/resource_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 17:50:06.747173 spaceone-api-2.0.dev89/spaceone_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-04 17:50:06.000000 spaceone-api-2.0.dev89/spaceone_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-01-04 17:50:06.000000 spaceone-api-2.0.dev89/spaceone_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-04 17:50:06.000000 spaceone-api-2.0.dev89/spaceone_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-04 17:50:06.000000 spaceone-api-2.0.dev89/spaceone_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-04 17:50:06.000000 spaceone-api-2.0.dev89/spaceone_api.egg-info/top_level.txt
```

### Comparing `spaceone-api-2.0.dev78/setup.py` & `spaceone-api-2.0.dev89/setup.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/board/v1/post_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/board/v1/post_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/board/v1/post_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/board/v1/post_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/config/v1/domain_config_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/config/v1/domain_config_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/config/v1/domain_config_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/config/v1/domain_config_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/config/v1/user_config_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/config/v1/user_config_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/config/v1/user_config_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/config/v1/user_config_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/core/v1/handler_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/core/v1/handler_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/core/v1/query_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/core/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/core/v1/server_info_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/core/v1/server_info_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/core/v1/server_info_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/core/v1/server_info_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/core/v2/handler_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/core/v2/handler_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/core/v2/plugin_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/core/v2/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/core/v2/query_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/core/v2/query_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/plugin/cost_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/plugin/cost_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/plugin/cost_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/plugin/cost_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/plugin/data_source_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/plugin/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/plugin/data_source_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/plugin/data_source_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/plugin/job_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/plugin/job_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/plugin/job_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/plugin/job_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/budget_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/budget_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/budget_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/budget_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/budget_usage_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/budget_usage_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/budget_usage_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/budget_usage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/cost_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/cost_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/cost_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/cost_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/cost_query_set_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/cost_query_set_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from spaceone.api.core.v2 import query_pb2 as spaceone_dot_api_dot_core_dot_v2_dot_query__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2spaceone/api/cost_analysis/v1/cost_query_set.proto\x12\x1dspaceone.api.cost_analysis.v1\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\x1a spaceone/api/core/v2/query.proto\"\x92\x01\n\x19\x43reateCostQuerySetRequest\x12\x16\n\x0e\x64\x61ta_source_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12(\n\x07options\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12%\n\x04tags\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x95\x01\n\x19UpdateCostQuerySetRequest\x12\x19\n\x11\x63ost_query_set_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12(\n\x07options\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12%\n\x04tags\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\"0\n\x13\x43ostQuerySetRequest\x12\x19\n\x11\x63ost_query_set_id\x18\x01 \x01(\t\"e\n\x11\x43ostQuerySetQuery\x12*\n\x05query\x18\x01 \x01(\x0b\x32\x1b.spaceone.api.core.v2.Query\x12\x16\n\x0e\x64\x61ta_source_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\"\xf0\x01\n\x10\x43ostQuerySetInfo\x12\x19\n\x11\x63ost_query_set_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12(\n\x07options\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12%\n\x04tags\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x11\n\tdomain_id\x18\x15 \x01(\t\x12\x0f\n\x07user_id\x18\x16 \x01(\t\x12\x16\n\x0e\x64\x61ta_source_id\x18\x17 \x01(\t\x12\x12\n\ncreated_at\x18\x1f \x01(\t\x12\x12\n\nupdated_at\x18  \x01(\t\"j\n\x11\x43ostQuerySetsInfo\x12@\n\x07results\x18\x01 \x03(\x0b\x32/.spaceone.api.cost_analysis.v1.CostQuerySetInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05\"e\n\x15\x43ostQuerySetStatQuery\x12\x34\n\x05query\x18\x01 \x01(\x0b\x32%.spaceone.api.core.v2.StatisticsQuery\x12\x16\n\x0e\x64\x61ta_source_id\x18\x02 \x01(\t2\xb4\x07\n\x0c\x43ostQuerySet\x12\xa7\x01\n\x06\x63reate\x12\x38.spaceone.api.cost_analysis.v1.CreateCostQuerySetRequest\x1a/.spaceone.api.cost_analysis.v1.CostQuerySetInfo\"2\x82\xd3\xe4\x93\x02,\"\'/cost-analysis/v1/cost-query-set/create:\x01*\x12\xa7\x01\n\x06update\x12\x38.spaceone.api.cost_analysis.v1.UpdateCostQuerySetRequest\x1a/.spaceone.api.cost_analysis.v1.CostQuerySetInfo\"2\x82\xd3\xe4\x93\x02,\"\'/cost-analysis/v1/cost-query-set/update:\x01*\x12\x88\x01\n\x06\x64\x65lete\x12\x32.spaceone.api.cost_analysis.v1.CostQuerySetRequest\x1a\x16.google.protobuf.Empty\"2\x82\xd3\xe4\x93\x02,\"\'/cost-analysis/v1/cost-query-set/delete:\x01*\x12\x9b\x01\n\x03get\x12\x32.spaceone.api.cost_analysis.v1.CostQuerySetRequest\x1a/.spaceone.api.cost_analysis.v1.CostQuerySetInfo\"/\x82\xd3\xe4\x93\x02)\"$/cost-analysis/v1/cost-query-set/get:\x01*\x12\x9c\x01\n\x04list\x12\x30.spaceone.api.cost_analysis.v1.CostQuerySetQuery\x1a\x30.spaceone.api.cost_analysis.v1.CostQuerySetsInfo\"0\x82\xd3\xe4\x93\x02*\"%/cost-analysis/v1/cost-query-set/list:\x01*\x12\x87\x01\n\x04stat\x12\x34.spaceone.api.cost_analysis.v1.CostQuerySetStatQuery\x1a\x17.google.protobuf.Struct\"0\x82\xd3\xe4\x93\x02*\"%/cost-analysis/v1/cost-query-set/stat:\x01*BDZBgithub.com/cloudforet-io/api/dist/go/spaceone/api/cost_analysis/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2spaceone/api/cost_analysis/v1/cost_query_set.proto\x12\x1dspaceone.api.cost_analysis.v1\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\x1a spaceone/api/core/v2/query.proto\"\x92\x01\n\x19\x43reateCostQuerySetRequest\x12\x16\n\x0e\x64\x61ta_source_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12(\n\x07options\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12%\n\x04tags\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x95\x01\n\x19UpdateCostQuerySetRequest\x12\x19\n\x11\x63ost_query_set_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12(\n\x07options\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12%\n\x04tags\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\"0\n\x13\x43ostQuerySetRequest\x12\x19\n\x11\x63ost_query_set_id\x18\x01 \x01(\t\"e\n\x11\x43ostQuerySetQuery\x12*\n\x05query\x18\x01 \x01(\x0b\x32\x1b.spaceone.api.core.v2.Query\x12\x16\n\x0e\x64\x61ta_source_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\"\x86\x02\n\x10\x43ostQuerySetInfo\x12\x19\n\x11\x63ost_query_set_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12(\n\x07options\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12%\n\x04tags\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x11\n\tdomain_id\x18\x15 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x16 \x01(\t\x12\x0f\n\x07user_id\x18\x17 \x01(\t\x12\x16\n\x0e\x64\x61ta_source_id\x18\x18 \x01(\t\x12\x12\n\ncreated_at\x18\x1f \x01(\t\x12\x12\n\nupdated_at\x18  \x01(\t\"j\n\x11\x43ostQuerySetsInfo\x12@\n\x07results\x18\x01 \x03(\x0b\x32/.spaceone.api.cost_analysis.v1.CostQuerySetInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05\"e\n\x15\x43ostQuerySetStatQuery\x12\x34\n\x05query\x18\x01 \x01(\x0b\x32%.spaceone.api.core.v2.StatisticsQuery\x12\x16\n\x0e\x64\x61ta_source_id\x18\x02 \x01(\t2\xb4\x07\n\x0c\x43ostQuerySet\x12\xa7\x01\n\x06\x63reate\x12\x38.spaceone.api.cost_analysis.v1.CreateCostQuerySetRequest\x1a/.spaceone.api.cost_analysis.v1.CostQuerySetInfo\"2\x82\xd3\xe4\x93\x02,\"\'/cost-analysis/v1/cost-query-set/create:\x01*\x12\xa7\x01\n\x06update\x12\x38.spaceone.api.cost_analysis.v1.UpdateCostQuerySetRequest\x1a/.spaceone.api.cost_analysis.v1.CostQuerySetInfo\"2\x82\xd3\xe4\x93\x02,\"\'/cost-analysis/v1/cost-query-set/update:\x01*\x12\x88\x01\n\x06\x64\x65lete\x12\x32.spaceone.api.cost_analysis.v1.CostQuerySetRequest\x1a\x16.google.protobuf.Empty\"2\x82\xd3\xe4\x93\x02,\"\'/cost-analysis/v1/cost-query-set/delete:\x01*\x12\x9b\x01\n\x03get\x12\x32.spaceone.api.cost_analysis.v1.CostQuerySetRequest\x1a/.spaceone.api.cost_analysis.v1.CostQuerySetInfo\"/\x82\xd3\xe4\x93\x02)\"$/cost-analysis/v1/cost-query-set/get:\x01*\x12\x9c\x01\n\x04list\x12\x30.spaceone.api.cost_analysis.v1.CostQuerySetQuery\x1a\x30.spaceone.api.cost_analysis.v1.CostQuerySetsInfo\"0\x82\xd3\xe4\x93\x02*\"%/cost-analysis/v1/cost-query-set/list:\x01*\x12\x87\x01\n\x04stat\x12\x34.spaceone.api.cost_analysis.v1.CostQuerySetStatQuery\x1a\x17.google.protobuf.Struct\"0\x82\xd3\xe4\x93\x02*\"%/cost-analysis/v1/cost-query-set/stat:\x01*BDZBgithub.com/cloudforet-io/api/dist/go/spaceone/api/cost_analysis/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'spaceone.api.cost_analysis.v1.cost_query_set_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'ZBgithub.com/cloudforet-io/api/dist/go/spaceone/api/cost_analysis/v1'
@@ -43,15 +43,15 @@
   _globals['_UPDATECOSTQUERYSETREQUEST']._serialized_start=358
   _globals['_UPDATECOSTQUERYSETREQUEST']._serialized_end=507
   _globals['_COSTQUERYSETREQUEST']._serialized_start=509
   _globals['_COSTQUERYSETREQUEST']._serialized_end=557
   _globals['_COSTQUERYSETQUERY']._serialized_start=559
   _globals['_COSTQUERYSETQUERY']._serialized_end=660
   _globals['_COSTQUERYSETINFO']._serialized_start=663
-  _globals['_COSTQUERYSETINFO']._serialized_end=903
-  _globals['_COSTQUERYSETSINFO']._serialized_start=905
-  _globals['_COSTQUERYSETSINFO']._serialized_end=1011
-  _globals['_COSTQUERYSETSTATQUERY']._serialized_start=1013
-  _globals['_COSTQUERYSETSTATQUERY']._serialized_end=1114
-  _globals['_COSTQUERYSET']._serialized_start=1117
-  _globals['_COSTQUERYSET']._serialized_end=2065
+  _globals['_COSTQUERYSETINFO']._serialized_end=925
+  _globals['_COSTQUERYSETSINFO']._serialized_start=927
+  _globals['_COSTQUERYSETSINFO']._serialized_end=1033
+  _globals['_COSTQUERYSETSTATQUERY']._serialized_start=1035
+  _globals['_COSTQUERYSETSTATQUERY']._serialized_end=1136
+  _globals['_COSTQUERYSET']._serialized_start=1139
+  _globals['_COSTQUERYSET']._serialized_end=2087
 # @@protoc_insertion_point(module_scope)
```

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/cost_query_set_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/cost_query_set_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/data_source_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/data_source_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/data_source_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/data_source_rule_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/data_source_rule_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/data_source_rule_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/data_source_rule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/job_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/job_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/job_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/job_task_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/job_task_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/cost_analysis/v1/job_task_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/cost_analysis/v1/job_task_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/dashboard/v1/private_dashboard_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/dashboard/v1/private_dashboard_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/dashboard/v1/private_dashboard_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/dashboard/v1/private_dashboard_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/dashboard/v1/public_dashboard_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/dashboard/v1/public_dashboard_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/dashboard/v1/public_dashboard_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/dashboard/v1/public_dashboard_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/file_manager/v1/file_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/file_manager/v1/file_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/file_manager/v1/file_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/file_manager/v1/file_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/plugin/auth_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/plugin/collector_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: spaceone/api/identity/plugin/auth.proto
+# source: spaceone/api/inventory/plugin/collector.proto
 # Protobuf Python Version: 4.25.0
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
@@ -12,36 +12,32 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'spaceone/api/identity/plugin/auth.proto\x12\x1cspaceone.api.identity.plugin\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\"7\n\x0bInitRequest\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"w\n\rVerifyRequest\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\x0bsecret_data\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0e\n\x06schema\x18\x03 \x01(\t\"\x97\x01\n\x0b\x46indRequest\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\x0bsecret_data\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07user_id\x18\x03 \x01(\t\x12\x0f\n\x07keyword\x18\x04 \x01(\t\x12\x0e\n\x06schema\x18\x05 \x01(\t\"\xa9\x01\n\x0cLoginRequest\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\x0bsecret_data\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x31\n\x10user_credentials\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0e\n\x06schema\x18\x04 \x01(\t\"\xd4\x01\n\x08UserInfo\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\x12\x0e\n\x06mobile\x18\x04 \x01(\t\x12\r\n\x05group\x18\x05 \x01(\t\x12;\n\x05state\x18\x06 \x01(\x0e\x32,.spaceone.api.identity.plugin.UserInfo.State\">\n\x05State\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x10\n\x0cUNIDENTIFIED\x10\x03\"g\n\tUsersInfo\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.spaceone.api.identity.plugin.UserInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05\x12\x0c\n\x04more\x18\x03 \x01(\x08\":\n\x0e\x41uthVerifyInfo\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"7\n\nPluginInfo\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct2\xf3\x02\n\x04\x41uth\x12]\n\x04init\x12).spaceone.api.identity.plugin.InitRequest\x1a(.spaceone.api.identity.plugin.PluginInfo\"\x00\x12O\n\x06verify\x12+.spaceone.api.identity.plugin.VerifyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\\\n\x04\x66ind\x12).spaceone.api.identity.plugin.FindRequest\x1a\'.spaceone.api.identity.plugin.UsersInfo\"\x00\x12]\n\x05login\x12*.spaceone.api.identity.plugin.LoginRequest\x1a&.spaceone.api.identity.plugin.UserInfo\"\x00\x42\x43ZAgithub.com/cloudforet-io/api/dist/go/spaceone/api/identity/pluginb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-spaceone/api/inventory/plugin/collector.proto\x12\x1dspaceone.api.inventory.plugin\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\"7\n\x0bInitRequest\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"g\n\rVerifyRequest\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\x0bsecret_data\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xc0\x01\n\x0e\x43ollectRequest\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\x0bsecret_data\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\'\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12-\n\x0ctask_options\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xe9\x02\n\x0cResourceInfo\x12@\n\x05state\x18\x01 \x01(\x0e\x32\x31.spaceone.api.inventory.plugin.ResourceInfo.State\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x15\n\rresource_type\x18\x03 \x01(\t\x12,\n\x0bmatch_rules\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12)\n\x08resource\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12(\n\x07options\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\"l\n\x05State\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x43REATED\x10\x01\x12\x0b\n\x07PENDING\x10\x02\x12\x0e\n\nINPROGRESS\x10\x03\x12\x0b\n\x07SUCCESS\x10\x04\x12\x0b\n\x07\x46\x41ILURE\x10\x05\x12\x0b\n\x07TIMEOUT\x10\x06\x12\x08\n\x04IDLE\x10\x07\"?\n\x13\x43ollectorVerifyInfo\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"7\n\nPluginInfo\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct2\xa9\x02\n\tCollector\x12_\n\x04init\x12*.spaceone.api.inventory.plugin.InitRequest\x1a).spaceone.api.inventory.plugin.PluginInfo\"\x00\x12P\n\x06verify\x12,.spaceone.api.inventory.plugin.VerifyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12i\n\x07\x63ollect\x12-.spaceone.api.inventory.plugin.CollectRequest\x1a+.spaceone.api.inventory.plugin.ResourceInfo\"\x00\x30\x01\x42\x44ZBgithub.com/cloudforet-io/api/dist/go/spaceone/api/inventory/pluginb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'spaceone.api.identity.plugin.auth_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'spaceone.api.inventory.plugin.collector_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
-  _globals['DESCRIPTOR']._serialized_options = b'ZAgithub.com/cloudforet-io/api/dist/go/spaceone/api/identity/plugin'
-  _globals['_INITREQUEST']._serialized_start=132
-  _globals['_INITREQUEST']._serialized_end=187
-  _globals['_VERIFYREQUEST']._serialized_start=189
-  _globals['_VERIFYREQUEST']._serialized_end=308
-  _globals['_FINDREQUEST']._serialized_start=311
-  _globals['_FINDREQUEST']._serialized_end=462
-  _globals['_LOGINREQUEST']._serialized_start=465
-  _globals['_LOGINREQUEST']._serialized_end=634
-  _globals['_USERINFO']._serialized_start=637
-  _globals['_USERINFO']._serialized_end=849
-  _globals['_USERINFO_STATE']._serialized_start=787
-  _globals['_USERINFO_STATE']._serialized_end=849
-  _globals['_USERSINFO']._serialized_start=851
-  _globals['_USERSINFO']._serialized_end=954
-  _globals['_AUTHVERIFYINFO']._serialized_start=956
-  _globals['_AUTHVERIFYINFO']._serialized_end=1014
-  _globals['_PLUGININFO']._serialized_start=1016
-  _globals['_PLUGININFO']._serialized_end=1071
-  _globals['_AUTH']._serialized_start=1074
-  _globals['_AUTH']._serialized_end=1445
+  _globals['DESCRIPTOR']._serialized_options = b'ZBgithub.com/cloudforet-io/api/dist/go/spaceone/api/inventory/plugin'
+  _globals['_INITREQUEST']._serialized_start=139
+  _globals['_INITREQUEST']._serialized_end=194
+  _globals['_VERIFYREQUEST']._serialized_start=196
+  _globals['_VERIFYREQUEST']._serialized_end=299
+  _globals['_COLLECTREQUEST']._serialized_start=302
+  _globals['_COLLECTREQUEST']._serialized_end=494
+  _globals['_RESOURCEINFO']._serialized_start=497
+  _globals['_RESOURCEINFO']._serialized_end=858
+  _globals['_RESOURCEINFO_STATE']._serialized_start=750
+  _globals['_RESOURCEINFO_STATE']._serialized_end=858
+  _globals['_COLLECTORVERIFYINFO']._serialized_start=860
+  _globals['_COLLECTORVERIFYINFO']._serialized_end=923
+  _globals['_PLUGININFO']._serialized_start=925
+  _globals['_PLUGININFO']._serialized_end=980
+  _globals['_COLLECTOR']._serialized_start=983
+  _globals['_COLLECTOR']._serialized_end=1280
 # @@protoc_insertion_point(module_scope)
```

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/plugin/auth_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/plugin/v1/plugin_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,166 +1,134 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from spaceone.api.identity.plugin import auth_pb2 as spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2
+from spaceone.api.plugin.v1 import plugin_pb2 as spaceone_dot_api_dot_plugin_dot_v1_dot_plugin__pb2
 
 
-class AuthStub(object):
+class PluginStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.init = channel.unary_unary(
-                '/spaceone.api.identity.plugin.Auth/init',
-                request_serializer=spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.InitRequest.SerializeToString,
-                response_deserializer=spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.PluginInfo.FromString,
+        self.get_plugin_endpoint = channel.unary_unary(
+                '/spaceone.api.plugin.v1.Plugin/get_plugin_endpoint',
+                request_serializer=spaceone_dot_api_dot_plugin_dot_v1_dot_plugin__pb2.PluginEndpointRequest.SerializeToString,
+                response_deserializer=spaceone_dot_api_dot_plugin_dot_v1_dot_plugin__pb2.PluginEndpoint.FromString,
                 )
-        self.verify = channel.unary_unary(
-                '/spaceone.api.identity.plugin.Auth/verify',
-                request_serializer=spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.VerifyRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
-        self.find = channel.unary_unary(
-                '/spaceone.api.identity.plugin.Auth/find',
-                request_serializer=spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.FindRequest.SerializeToString,
-                response_deserializer=spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.UsersInfo.FromString,
+        self.get_plugin_metadata = channel.unary_unary(
+                '/spaceone.api.plugin.v1.Plugin/get_plugin_metadata',
+                request_serializer=spaceone_dot_api_dot_plugin_dot_v1_dot_plugin__pb2.PluginMetadataRequest.SerializeToString,
+                response_deserializer=spaceone_dot_api_dot_plugin_dot_v1_dot_plugin__pb2.PluginMetadata.FromString,
                 )
-        self.login = channel.unary_unary(
-                '/spaceone.api.identity.plugin.Auth/login',
-                request_serializer=spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.LoginRequest.SerializeToString,
-                response_deserializer=spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.UserInfo.FromString,
+        self.notify_failure = channel.unary_unary(
+                '/spaceone.api.plugin.v1.Plugin/notify_failure',
+                request_serializer=spaceone_dot_api_dot_plugin_dot_v1_dot_plugin__pb2.PluginFailureRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
 
 
-class AuthServicer(object):
+class PluginServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def init(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def verify(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def get_plugin_endpoint(self, request, context):
+        """Gets the `endpoint` of a specific plugin instance. A Plugin returns only a single `endpoint` by determining `labels` and `priority`. If the requested plugin instance is already deployed, the `endpoint` is returned. If not, the `endpoint` is returned after deploying the plugin instance.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def find(self, request, context):
+    def get_plugin_metadata(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def login(self, request, context):
+    def notify_failure(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_AuthServicer_to_server(servicer, server):
+def add_PluginServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'init': grpc.unary_unary_rpc_method_handler(
-                    servicer.init,
-                    request_deserializer=spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.InitRequest.FromString,
-                    response_serializer=spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.PluginInfo.SerializeToString,
+            'get_plugin_endpoint': grpc.unary_unary_rpc_method_handler(
+                    servicer.get_plugin_endpoint,
+                    request_deserializer=spaceone_dot_api_dot_plugin_dot_v1_dot_plugin__pb2.PluginEndpointRequest.FromString,
+                    response_serializer=spaceone_dot_api_dot_plugin_dot_v1_dot_plugin__pb2.PluginEndpoint.SerializeToString,
             ),
-            'verify': grpc.unary_unary_rpc_method_handler(
-                    servicer.verify,
-                    request_deserializer=spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.VerifyRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            'get_plugin_metadata': grpc.unary_unary_rpc_method_handler(
+                    servicer.get_plugin_metadata,
+                    request_deserializer=spaceone_dot_api_dot_plugin_dot_v1_dot_plugin__pb2.PluginMetadataRequest.FromString,
+                    response_serializer=spaceone_dot_api_dot_plugin_dot_v1_dot_plugin__pb2.PluginMetadata.SerializeToString,
             ),
-            'find': grpc.unary_unary_rpc_method_handler(
-                    servicer.find,
-                    request_deserializer=spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.FindRequest.FromString,
-                    response_serializer=spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.UsersInfo.SerializeToString,
-            ),
-            'login': grpc.unary_unary_rpc_method_handler(
-                    servicer.login,
-                    request_deserializer=spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.LoginRequest.FromString,
-                    response_serializer=spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.UserInfo.SerializeToString,
+            'notify_failure': grpc.unary_unary_rpc_method_handler(
+                    servicer.notify_failure,
+                    request_deserializer=spaceone_dot_api_dot_plugin_dot_v1_dot_plugin__pb2.PluginFailureRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'spaceone.api.identity.plugin.Auth', rpc_method_handlers)
+            'spaceone.api.plugin.v1.Plugin', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class Auth(object):
+class Plugin(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def init(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/spaceone.api.identity.plugin.Auth/init',
-            spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.InitRequest.SerializeToString,
-            spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.PluginInfo.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def verify(request,
+    def get_plugin_endpoint(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/spaceone.api.identity.plugin.Auth/verify',
-            spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.VerifyRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        return grpc.experimental.unary_unary(request, target, '/spaceone.api.plugin.v1.Plugin/get_plugin_endpoint',
+            spaceone_dot_api_dot_plugin_dot_v1_dot_plugin__pb2.PluginEndpointRequest.SerializeToString,
+            spaceone_dot_api_dot_plugin_dot_v1_dot_plugin__pb2.PluginEndpoint.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def find(request,
+    def get_plugin_metadata(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/spaceone.api.identity.plugin.Auth/find',
-            spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.FindRequest.SerializeToString,
-            spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.UsersInfo.FromString,
+        return grpc.experimental.unary_unary(request, target, '/spaceone.api.plugin.v1.Plugin/get_plugin_metadata',
+            spaceone_dot_api_dot_plugin_dot_v1_dot_plugin__pb2.PluginMetadataRequest.SerializeToString,
+            spaceone_dot_api_dot_plugin_dot_v1_dot_plugin__pb2.PluginMetadata.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def login(request,
+    def notify_failure(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/spaceone.api.identity.plugin.Auth/login',
-            spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.LoginRequest.SerializeToString,
-            spaceone_dot_api_dot_identity_dot_plugin_dot_auth__pb2.UserInfo.FromString,
+        return grpc.experimental.unary_unary(request, target, '/spaceone.api.plugin.v1.Plugin/notify_failure',
+            spaceone_dot_api_dot_plugin_dot_v1_dot_plugin__pb2.PluginFailureRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/api_key_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/api_key_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/api_key_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/authorization_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/authorization_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/authorization_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/authorization_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/domain_owner_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/domain_owner_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/domain_owner_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/domain_owner_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/domain_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/domain_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/domain_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/domain_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/endpoint_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/endpoint_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/endpoint_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/policy_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/policy_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/policy_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/policy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/project_group_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/project_group_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/project_group_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/project_group_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/project_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/project_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/project_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/project_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/provider_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/provider_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/provider_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/provider_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/role_binding_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/role_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/role_binding_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/role_binding_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/role_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/role_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/role_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/role_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/service_account_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/service_account_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/service_account_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/service_account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/token_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/token_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/token_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/token_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/user_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v1/user_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v1/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/app_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/app_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from spaceone.api.core.v2 import query_pb2 as spaceone_dot_api_dot_core_dot_v2_dot_query__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"spaceone/api/identity/v2/app.proto\x12\x18spaceone.api.identity.v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\x1a spaceone/api/core/v2/query.proto\"\x8a\x02\n\x10\x43reateAppRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07role_id\x18\x02 \x01(\t\x12%\n\x04tags\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x12\n\nexpired_at\x18\x04 \x01(\t\x12P\n\x0eresource_group\x18\x14 \x01(\x0e\x32\x38.spaceone.api.identity.v2.CreateAppRequest.ResourceGroup\x12\x14\n\x0cworkspace_id\x18\x15 \x01(\t\"4\n\rResourceGroup\x12\x08\n\x04NONE\x10\x00\x12\n\n\x06\x44OMAIN\x10\x01\x12\r\n\tWORKSPACE\x10\x02\"W\n\x10UpdateAppRequest\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12%\n\x04tags\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\">\n\x18GenerateAPIKeyAppRequest\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\x12\x12\n\nexpired_at\x18\x02 \x01(\t\"\x1c\n\nAppRequest\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\"8\n\x0f\x41ppCheckRequest\x12\x12\n\napi_key_id\x18\x01 \x01(\t\x12\x11\n\tdomain_id\x18\x02 \x01(\t\"#\n\x0c\x43heckAppInfo\x12\x13\n\x0bpermissions\x18\x01 \x03(\t\"\xd9\x04\n\x07\x41ppInfo\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\x12\x0f\n\x07\x61pi_key\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x36\n\x05state\x18\x04 \x01(\x0e\x32\'.spaceone.api.identity.v2.AppInfo.State\x12%\n\x04tags\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12=\n\trole_type\x18\x06 \x01(\x0e\x32*.spaceone.api.identity.v2.AppInfo.RoleType\x12G\n\x0eresource_group\x18\x14 \x01(\x0e\x32/.spaceone.api.identity.v2.AppInfo.ResourceGroup\x12\x11\n\tdomain_id\x18\x15 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x16 \x01(\t\x12\x0f\n\x07role_id\x18\x17 \x01(\t\x12\x12\n\napi_key_id\x18\x18 \x01(\t\x12\x12\n\ncreated_at\x18\x1f \x01(\t\x12\x12\n\nexpired_at\x18  \x01(\t\"?\n\x05State\x12\x0e\n\nSTATE_NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07\x45XPIRED\x10\x03\"E\n\x08RoleType\x12\x12\n\x0eROLE_TYPE_NONE\x10\x00\x12\x10\n\x0c\x44OMAIN_ADMIN\x10\x01\x12\x13\n\x0fWORKSPACE_OWNER\x10\x02\":\n\rResourceGroup\x12\x0e\n\nGROUP_NONE\x10\x00\x12\n\n\x06\x44OMAIN\x10\x01\x12\r\n\tWORKSPACE\x10\x02\"\xde\x03\n\x0e\x41ppSearchQuery\x12*\n\x05query\x18\x01 \x01(\x0b\x32\x1b.spaceone.api.core.v2.Query\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12=\n\x05state\x18\x04 \x01(\x0e\x32..spaceone.api.identity.v2.AppSearchQuery.State\x12\x44\n\trole_type\x18\x05 \x01(\x0e\x32\x31.spaceone.api.identity.v2.AppSearchQuery.RoleType\x12\x14\n\x0cworkspace_id\x18\x15 \x01(\t\x12\x0f\n\x07role_id\x18\x16 \x01(\t\x12\x12\n\napi_key_id\x18\x17 \x01(\t\"?\n\x05State\x12\x0e\n\nSTATE_NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07\x45XPIRED\x10\x03\"E\n\x08RoleType\x12\x12\n\x0eROLE_TYPE_NONE\x10\x00\x12\x10\n\x0c\x44OMAIN_ADMIN\x10\x01\x12\x13\n\x0fWORKSPACE_OWNER\x10\x02\":\n\rResourceGroup\x12\x0e\n\nGROUP_NONE\x10\x00\x12\n\n\x06\x44OMAIN\x10\x01\x12\r\n\tWORKSPACE\x10\x02\"S\n\x08\x41ppsInfo\x12\x32\n\x07results\x18\x01 \x03(\x0b\x32!.spaceone.api.identity.v2.AppInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05\"D\n\x0c\x41ppStatQuery\x12\x34\n\x05query\x18\x01 \x01(\x0b\x32%.spaceone.api.core.v2.StatisticsQuery2\xa7\t\n\x03\x41pp\x12{\n\x06\x63reate\x12*.spaceone.api.identity.v2.CreateAppRequest\x1a!.spaceone.api.identity.v2.AppInfo\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/identity/v2/app/create:\x01*\x12{\n\x06update\x12*.spaceone.api.identity.v2.UpdateAppRequest\x1a!.spaceone.api.identity.v2.AppInfo\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/identity/v2/app/update:\x01*\x12\x97\x01\n\x10generate_api_key\x12\x32.spaceone.api.identity.v2.GenerateAPIKeyAppRequest\x1a!.spaceone.api.identity.v2.AppInfo\",\x82\xd3\xe4\x93\x02&\"!/identity/v2/app/generate-api-key:\x01*\x12u\n\x06\x65nable\x12$.spaceone.api.identity.v2.AppRequest\x1a!.spaceone.api.identity.v2.AppInfo\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/identity/v2/app/enable:\x01*\x12w\n\x07\x64isable\x12$.spaceone.api.identity.v2.AppRequest\x1a!.spaceone.api.identity.v2.AppInfo\"#\x82\xd3\xe4\x93\x02\x1d\"\x18/identity/v2/app/disable:\x01*\x12j\n\x06\x64\x65lete\x12$.spaceone.api.identity.v2.AppRequest\x1a\x16.google.protobuf.Empty\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/identity/v2/app/delete:\x01*\x12o\n\x03get\x12$.spaceone.api.identity.v2.AppRequest\x1a!.spaceone.api.identity.v2.AppInfo\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x14/identity/v2/app/get:\x01*\x12\\\n\x05\x63heck\x12).spaceone.api.identity.v2.AppCheckRequest\x1a&.spaceone.api.identity.v2.CheckAppInfo\"\x00\x12v\n\x04list\x12(.spaceone.api.identity.v2.AppSearchQuery\x1a\".spaceone.api.identity.v2.AppsInfo\" \x82\xd3\xe4\x93\x02\x1a\"\x15/identity/v2/app/list:\x01*\x12i\n\x04stat\x12&.spaceone.api.identity.v2.AppStatQuery\x1a\x17.google.protobuf.Struct\" \x82\xd3\xe4\x93\x02\x1a\"\x15/identity/v2/app/stat:\x01*B?Z=github.com/cloudforet-io/api/dist/go/spaceone/api/identity/v2b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"spaceone/api/identity/v2/app.proto\x12\x18spaceone.api.identity.v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\x1a spaceone/api/core/v2/query.proto\"\x8a\x02\n\x10\x43reateAppRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07role_id\x18\x02 \x01(\t\x12%\n\x04tags\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x12\n\nexpired_at\x18\x04 \x01(\t\x12P\n\x0eresource_group\x18\x14 \x01(\x0e\x32\x38.spaceone.api.identity.v2.CreateAppRequest.ResourceGroup\x12\x14\n\x0cworkspace_id\x18\x15 \x01(\t\"4\n\rResourceGroup\x12\x08\n\x04NONE\x10\x00\x12\n\n\x06\x44OMAIN\x10\x01\x12\r\n\tWORKSPACE\x10\x02\"W\n\x10UpdateAppRequest\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12%\n\x04tags\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\">\n\x18GenerateAPIKeyAppRequest\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\x12\x12\n\nexpired_at\x18\x02 \x01(\t\"\x1c\n\nAppRequest\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\"7\n\x0f\x41ppCheckRequest\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x11\n\tdomain_id\x18\x02 \x01(\t\"#\n\x0c\x43heckAppInfo\x12\x13\n\x0bpermissions\x18\x01 \x03(\t\"\xf8\x04\n\x07\x41ppInfo\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\x12\x15\n\rclient_secret\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x36\n\x05state\x18\x04 \x01(\x0e\x32\'.spaceone.api.identity.v2.AppInfo.State\x12%\n\x04tags\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12=\n\trole_type\x18\x06 \x01(\x0e\x32*.spaceone.api.identity.v2.AppInfo.RoleType\x12G\n\x0eresource_group\x18\x14 \x01(\x0e\x32/.spaceone.api.identity.v2.AppInfo.ResourceGroup\x12\x11\n\tdomain_id\x18\x15 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x16 \x01(\t\x12\x0f\n\x07role_id\x18\x17 \x01(\t\x12\x11\n\tclient_id\x18\x18 \x01(\t\x12\x12\n\ncreated_at\x18\x1f \x01(\t\x12\x12\n\nexpired_at\x18  \x01(\t\x12\x18\n\x10last_accessed_at\x18! \x01(\t\"?\n\x05State\x12\x0e\n\nSTATE_NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07\x45XPIRED\x10\x03\"E\n\x08RoleType\x12\x12\n\x0eROLE_TYPE_NONE\x10\x00\x12\x10\n\x0c\x44OMAIN_ADMIN\x10\x01\x12\x13\n\x0fWORKSPACE_OWNER\x10\x02\":\n\rResourceGroup\x12\x0e\n\nGROUP_NONE\x10\x00\x12\n\n\x06\x44OMAIN\x10\x01\x12\r\n\tWORKSPACE\x10\x02\"\xdd\x03\n\x0e\x41ppSearchQuery\x12*\n\x05query\x18\x01 \x01(\x0b\x32\x1b.spaceone.api.core.v2.Query\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12=\n\x05state\x18\x04 \x01(\x0e\x32..spaceone.api.identity.v2.AppSearchQuery.State\x12\x44\n\trole_type\x18\x05 \x01(\x0e\x32\x31.spaceone.api.identity.v2.AppSearchQuery.RoleType\x12\x14\n\x0cworkspace_id\x18\x15 \x01(\t\x12\x0f\n\x07role_id\x18\x16 \x01(\t\x12\x11\n\tclient_id\x18\x17 \x01(\t\"?\n\x05State\x12\x0e\n\nSTATE_NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07\x45XPIRED\x10\x03\"E\n\x08RoleType\x12\x12\n\x0eROLE_TYPE_NONE\x10\x00\x12\x10\n\x0c\x44OMAIN_ADMIN\x10\x01\x12\x13\n\x0fWORKSPACE_OWNER\x10\x02\":\n\rResourceGroup\x12\x0e\n\nGROUP_NONE\x10\x00\x12\n\n\x06\x44OMAIN\x10\x01\x12\r\n\tWORKSPACE\x10\x02\"S\n\x08\x41ppsInfo\x12\x32\n\x07results\x18\x01 \x03(\x0b\x32!.spaceone.api.identity.v2.AppInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05\"D\n\x0c\x41ppStatQuery\x12\x34\n\x05query\x18\x01 \x01(\x0b\x32%.spaceone.api.core.v2.StatisticsQuery2\xb3\t\n\x03\x41pp\x12{\n\x06\x63reate\x12*.spaceone.api.identity.v2.CreateAppRequest\x1a!.spaceone.api.identity.v2.AppInfo\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/identity/v2/app/create:\x01*\x12{\n\x06update\x12*.spaceone.api.identity.v2.UpdateAppRequest\x1a!.spaceone.api.identity.v2.AppInfo\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/identity/v2/app/update:\x01*\x12\xa3\x01\n\x16generate_client_secret\x12\x32.spaceone.api.identity.v2.GenerateAPIKeyAppRequest\x1a!.spaceone.api.identity.v2.AppInfo\"2\x82\xd3\xe4\x93\x02,\"\'/identity/v2/app/generate-client-secret:\x01*\x12u\n\x06\x65nable\x12$.spaceone.api.identity.v2.AppRequest\x1a!.spaceone.api.identity.v2.AppInfo\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/identity/v2/app/enable:\x01*\x12w\n\x07\x64isable\x12$.spaceone.api.identity.v2.AppRequest\x1a!.spaceone.api.identity.v2.AppInfo\"#\x82\xd3\xe4\x93\x02\x1d\"\x18/identity/v2/app/disable:\x01*\x12j\n\x06\x64\x65lete\x12$.spaceone.api.identity.v2.AppRequest\x1a\x16.google.protobuf.Empty\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/identity/v2/app/delete:\x01*\x12o\n\x03get\x12$.spaceone.api.identity.v2.AppRequest\x1a!.spaceone.api.identity.v2.AppInfo\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x14/identity/v2/app/get:\x01*\x12\\\n\x05\x63heck\x12).spaceone.api.identity.v2.AppCheckRequest\x1a&.spaceone.api.identity.v2.CheckAppInfo\"\x00\x12v\n\x04list\x12(.spaceone.api.identity.v2.AppSearchQuery\x1a\".spaceone.api.identity.v2.AppsInfo\" \x82\xd3\xe4\x93\x02\x1a\"\x15/identity/v2/app/list:\x01*\x12i\n\x04stat\x12&.spaceone.api.identity.v2.AppStatQuery\x1a\x17.google.protobuf.Struct\" \x82\xd3\xe4\x93\x02\x1a\"\x15/identity/v2/app/stat:\x01*B?Z=github.com/cloudforet-io/api/dist/go/spaceone/api/identity/v2b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'spaceone.api.identity.v2.app_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z=github.com/cloudforet-io/api/dist/go/spaceone/api/identity/v2'
   _globals['_APP'].methods_by_name['create']._options = None
   _globals['_APP'].methods_by_name['create']._serialized_options = b'\202\323\344\223\002\034\"\027/identity/v2/app/create:\001*'
   _globals['_APP'].methods_by_name['update']._options = None
   _globals['_APP'].methods_by_name['update']._serialized_options = b'\202\323\344\223\002\034\"\027/identity/v2/app/update:\001*'
-  _globals['_APP'].methods_by_name['generate_api_key']._options = None
-  _globals['_APP'].methods_by_name['generate_api_key']._serialized_options = b'\202\323\344\223\002&\"!/identity/v2/app/generate-api-key:\001*'
+  _globals['_APP'].methods_by_name['generate_client_secret']._options = None
+  _globals['_APP'].methods_by_name['generate_client_secret']._serialized_options = b'\202\323\344\223\002,\"\'/identity/v2/app/generate-client-secret:\001*'
   _globals['_APP'].methods_by_name['enable']._options = None
   _globals['_APP'].methods_by_name['enable']._serialized_options = b'\202\323\344\223\002\034\"\027/identity/v2/app/enable:\001*'
   _globals['_APP'].methods_by_name['disable']._options = None
   _globals['_APP'].methods_by_name['disable']._serialized_options = b'\202\323\344\223\002\035\"\030/identity/v2/app/disable:\001*'
   _globals['_APP'].methods_by_name['delete']._options = None
   _globals['_APP'].methods_by_name['delete']._serialized_options = b'\202\323\344\223\002\034\"\027/identity/v2/app/delete:\001*'
   _globals['_APP'].methods_by_name['get']._options = None
@@ -51,33 +51,33 @@
   _globals['_UPDATEAPPREQUEST']._serialized_start=456
   _globals['_UPDATEAPPREQUEST']._serialized_end=543
   _globals['_GENERATEAPIKEYAPPREQUEST']._serialized_start=545
   _globals['_GENERATEAPIKEYAPPREQUEST']._serialized_end=607
   _globals['_APPREQUEST']._serialized_start=609
   _globals['_APPREQUEST']._serialized_end=637
   _globals['_APPCHECKREQUEST']._serialized_start=639
-  _globals['_APPCHECKREQUEST']._serialized_end=695
-  _globals['_CHECKAPPINFO']._serialized_start=697
-  _globals['_CHECKAPPINFO']._serialized_end=732
-  _globals['_APPINFO']._serialized_start=735
-  _globals['_APPINFO']._serialized_end=1336
-  _globals['_APPINFO_STATE']._serialized_start=1142
-  _globals['_APPINFO_STATE']._serialized_end=1205
-  _globals['_APPINFO_ROLETYPE']._serialized_start=1207
-  _globals['_APPINFO_ROLETYPE']._serialized_end=1276
-  _globals['_APPINFO_RESOURCEGROUP']._serialized_start=1278
-  _globals['_APPINFO_RESOURCEGROUP']._serialized_end=1336
-  _globals['_APPSEARCHQUERY']._serialized_start=1339
-  _globals['_APPSEARCHQUERY']._serialized_end=1817
-  _globals['_APPSEARCHQUERY_STATE']._serialized_start=1142
-  _globals['_APPSEARCHQUERY_STATE']._serialized_end=1205
-  _globals['_APPSEARCHQUERY_ROLETYPE']._serialized_start=1207
-  _globals['_APPSEARCHQUERY_ROLETYPE']._serialized_end=1276
-  _globals['_APPSEARCHQUERY_RESOURCEGROUP']._serialized_start=1278
-  _globals['_APPSEARCHQUERY_RESOURCEGROUP']._serialized_end=1336
-  _globals['_APPSINFO']._serialized_start=1819
-  _globals['_APPSINFO']._serialized_end=1902
-  _globals['_APPSTATQUERY']._serialized_start=1904
-  _globals['_APPSTATQUERY']._serialized_end=1972
-  _globals['_APP']._serialized_start=1975
-  _globals['_APP']._serialized_end=3166
+  _globals['_APPCHECKREQUEST']._serialized_end=694
+  _globals['_CHECKAPPINFO']._serialized_start=696
+  _globals['_CHECKAPPINFO']._serialized_end=731
+  _globals['_APPINFO']._serialized_start=734
+  _globals['_APPINFO']._serialized_end=1366
+  _globals['_APPINFO_STATE']._serialized_start=1172
+  _globals['_APPINFO_STATE']._serialized_end=1235
+  _globals['_APPINFO_ROLETYPE']._serialized_start=1237
+  _globals['_APPINFO_ROLETYPE']._serialized_end=1306
+  _globals['_APPINFO_RESOURCEGROUP']._serialized_start=1308
+  _globals['_APPINFO_RESOURCEGROUP']._serialized_end=1366
+  _globals['_APPSEARCHQUERY']._serialized_start=1369
+  _globals['_APPSEARCHQUERY']._serialized_end=1846
+  _globals['_APPSEARCHQUERY_STATE']._serialized_start=1172
+  _globals['_APPSEARCHQUERY_STATE']._serialized_end=1235
+  _globals['_APPSEARCHQUERY_ROLETYPE']._serialized_start=1237
+  _globals['_APPSEARCHQUERY_ROLETYPE']._serialized_end=1306
+  _globals['_APPSEARCHQUERY_RESOURCEGROUP']._serialized_start=1308
+  _globals['_APPSEARCHQUERY_RESOURCEGROUP']._serialized_end=1366
+  _globals['_APPSINFO']._serialized_start=1848
+  _globals['_APPSINFO']._serialized_end=1931
+  _globals['_APPSTATQUERY']._serialized_start=1933
+  _globals['_APPSTATQUERY']._serialized_end=2001
+  _globals['_APP']._serialized_start=2004
+  _globals['_APP']._serialized_end=3207
 # @@protoc_insertion_point(module_scope)
```

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/app_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/app_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
                 response_deserializer=spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.AppInfo.FromString,
                 )
         self.update = channel.unary_unary(
                 '/spaceone.api.identity.v2.App/update',
                 request_serializer=spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.UpdateAppRequest.SerializeToString,
                 response_deserializer=spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.AppInfo.FromString,
                 )
-        self.generate_api_key = channel.unary_unary(
-                '/spaceone.api.identity.v2.App/generate_api_key',
+        self.generate_client_secret = channel.unary_unary(
+                '/spaceone.api.identity.v2.App/generate_client_secret',
                 request_serializer=spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.GenerateAPIKeyAppRequest.SerializeToString,
                 response_deserializer=spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.AppInfo.FromString,
                 )
         self.enable = channel.unary_unary(
                 '/spaceone.api.identity.v2.App/enable',
                 request_serializer=spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.AppRequest.SerializeToString,
                 response_deserializer=spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.AppInfo.FromString,
@@ -79,15 +79,15 @@
 
     def update(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def generate_api_key(self, request, context):
+    def generate_client_secret(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def enable(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -140,16 +140,16 @@
                     response_serializer=spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.AppInfo.SerializeToString,
             ),
             'update': grpc.unary_unary_rpc_method_handler(
                     servicer.update,
                     request_deserializer=spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.UpdateAppRequest.FromString,
                     response_serializer=spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.AppInfo.SerializeToString,
             ),
-            'generate_api_key': grpc.unary_unary_rpc_method_handler(
-                    servicer.generate_api_key,
+            'generate_client_secret': grpc.unary_unary_rpc_method_handler(
+                    servicer.generate_client_secret,
                     request_deserializer=spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.GenerateAPIKeyAppRequest.FromString,
                     response_serializer=spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.AppInfo.SerializeToString,
             ),
             'enable': grpc.unary_unary_rpc_method_handler(
                     servicer.enable,
                     request_deserializer=spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.AppRequest.FromString,
                     response_serializer=spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.AppInfo.SerializeToString,
@@ -225,25 +225,25 @@
         return grpc.experimental.unary_unary(request, target, '/spaceone.api.identity.v2.App/update',
             spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.UpdateAppRequest.SerializeToString,
             spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.AppInfo.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def generate_api_key(request,
+    def generate_client_secret(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/spaceone.api.identity.v2.App/generate_api_key',
+        return grpc.experimental.unary_unary(request, target, '/spaceone.api.identity.v2.App/generate_client_secret',
             spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.GenerateAPIKeyAppRequest.SerializeToString,
             spaceone_dot_api_dot_identity_dot_v2_dot_app__pb2.AppInfo.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def enable(request,
```

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/domain_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/domain_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/domain_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/domain_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/endpoint_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/endpoint_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/endpoint_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/external_auth_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/external_auth_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/external_auth_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/external_auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/project_group_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/project_group_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/project_group_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/project_group_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/project_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/project_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/project_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/project_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/provider_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/provider_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/provider_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/provider_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/role_binding_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/role_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/role_binding_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/role_binding_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/role_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/role_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/role_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/role_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/schema_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/schema_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/schema_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/service_account_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/service_account_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/service_account_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/service_account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/system_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/system_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/system_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/system_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/token_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/token_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/token_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/token_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/trusted_account_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/trusted_account_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/trusted_account_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/trusted_account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/user_group_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/user_group_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/user_group_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/user_group_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/user_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/user_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from spaceone.api.core.v2 import query_pb2 as spaceone_dot_api_dot_core_dot_v2_dot_query__pb2
 from spaceone.api.identity.v2 import workspace_pb2 as spaceone_dot_api_dot_identity_dot_v2_dot_workspace__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#spaceone/api/identity/v2/user.proto\x12\x18spaceone.api.identity.v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\x1a spaceone/api/core/v2/query.proto\x1a(spaceone/api/identity/v2/workspace.proto\"\xa3\x01\n\x03MFA\x12\x32\n\x05state\x18\x01 \x01(\x0e\x32#.spaceone.api.identity.v2.MFA.State\x12\x10\n\x08mfa_type\x18\x02 \x01(\t\x12(\n\x07options\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\",\n\x05State\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\"\xed\x01\n\x11\x43reateUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x35\n\tauth_type\x18\x05 \x01(\x0e\x32\".spaceone.api.identity.v2.AuthType\x12\x10\n\x08language\x18\x06 \x01(\t\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12%\n\x04tags\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x16\n\x0ereset_password\x18\t \x01(\x08\"\xb6\x01\n\x11UpdateUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x10\n\x08language\x18\x05 \x01(\t\x12\x10\n\x08timezone\x18\x06 \x01(\t\x12%\n\x04tags\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x16\n\x0ereset_password\x18\x08 \x01(\x08\"8\n\x16VerifyUserEmailRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\r\n\x05\x65mail\x18\x02 \x01(\t\"(\n\x15\x44isableUserMFARequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\"t\n\x19SetRequiredActionsRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x46\n\x10required_actions\x18\x02 \x03(\x0e\x32,.spaceone.api.identity.v2.UserRequiredAction\"\x1e\n\x0bUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\"\x9d\x02\n\x0fUserSearchQuery\x12*\n\x05query\x18\x01 \x01(\x0b\x32\x1b.spaceone.api.core.v2.Query\x12\x0f\n\x07user_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12>\n\x05state\x18\x04 \x01(\x0e\x32/.spaceone.api.identity.v2.UserSearchQuery.State\x12\r\n\x05\x65mail\x18\x05 \x01(\t\x12\x35\n\tauth_type\x18\x06 \x01(\x0e\x32\".spaceone.api.identity.v2.AuthType\"9\n\x05State\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07PENDING\x10\x03\"\x94\x05\n\x08UserInfo\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x37\n\x05state\x18\x03 \x01(\x0e\x32(.spaceone.api.identity.v2.UserInfo.State\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x16\n\x0e\x65mail_verified\x18\x05 \x01(\x08\x12\x35\n\tauth_type\x18\x06 \x01(\x0e\x32\".spaceone.api.identity.v2.AuthType\x12>\n\trole_type\x18\x07 \x01(\x0e\x32+.spaceone.api.identity.v2.UserInfo.RoleType\x12*\n\x03mfa\x18\x08 \x01(\x0b\x32\x1d.spaceone.api.identity.v2.MFA\x12\x10\n\x08language\x18\n \x01(\t\x12\x10\n\x08timezone\x18\x0b \x01(\t\x12\x15\n\rapi_key_count\x18\x0c \x01(\x05\x12\x46\n\x10required_actions\x18\r \x03(\x0e\x32,.spaceone.api.identity.v2.UserRequiredAction\x12%\n\x04tags\x18\x0e \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x11\n\tdomain_id\x18\x15 \x01(\t\x12\x12\n\ncreated_at\x18\x1f \x01(\t\x12\x18\n\x10last_accessed_at\x18  \x01(\t\"?\n\x05State\x12\x0e\n\nSTATE_NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07PENDING\x10\x03\":\n\x08RoleType\x12\x12\n\x0eROLE_TYPE_NONE\x10\x00\x12\x10\n\x0c\x44OMAIN_ADMIN\x10\x01\x12\x08\n\x04USER\x10\x02\"U\n\tUsersInfo\x12\x33\n\x07results\x18\x01 \x03(\x0b\x32\".spaceone.api.identity.v2.UserInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05\"E\n\rUserStatQuery\x12\x34\n\x05query\x18\x01 \x01(\x0b\x32%.spaceone.api.core.v2.StatisticsQuery*5\n\x08\x41uthType\x12\x10\n\x0cNONE_BACKEND\x10\x00\x12\t\n\x05LOCAL\x10\x01\x12\x0c\n\x08\x45XTERNAL\x10\x02*)\n\x12UserRequiredAction\x12\x13\n\x0fUPDATE_PASSWORD\x10\x00\x32\x80\x0b\n\x04User\x12~\n\x06\x63reate\x12+.spaceone.api.identity.v2.CreateUserRequest\x1a\".spaceone.api.identity.v2.UserInfo\"#\x82\xd3\xe4\x93\x02\x1d\"\x18/identity/v2/user/create:\x01*\x12~\n\x06update\x12+.spaceone.api.identity.v2.UpdateUserRequest\x1a\".spaceone.api.identity.v2.UserInfo\"#\x82\xd3\xe4\x93\x02\x1d\"\x18/identity/v2/user/update:\x01*\x12\x83\x01\n\x0cverify_email\x12\x30.spaceone.api.identity.v2.VerifyUserEmailRequest\x1a\x16.google.protobuf.Empty\")\x82\xd3\xe4\x93\x02#\"\x1e/identity/v2/user/verify-email:\x01*\x12\x8c\x01\n\x0b\x64isable_mfa\x12/.spaceone.api.identity.v2.DisableUserMFARequest\x1a\".spaceone.api.identity.v2.UserInfo\"(\x82\xd3\xe4\x93\x02\"\"\x1d/identity/v2/user/disable-mfa:\x01*\x12\xa2\x01\n\x14set_required_actions\x12\x33.spaceone.api.identity.v2.SetRequiredActionsRequest\x1a\".spaceone.api.identity.v2.UserInfo\"1\x82\xd3\xe4\x93\x02+\"&/identity/v2/user/set-required-actions:\x01*\x12x\n\x06\x65nable\x12%.spaceone.api.identity.v2.UserRequest\x1a\".spaceone.api.identity.v2.UserInfo\"#\x82\xd3\xe4\x93\x02\x1d\"\x18/identity/v2/user/enable:\x01*\x12z\n\x07\x64isable\x12%.spaceone.api.identity.v2.UserRequest\x1a\".spaceone.api.identity.v2.UserInfo\"$\x82\xd3\xe4\x93\x02\x1e\"\x19/identity/v2/user/disable:\x01*\x12l\n\x06\x64\x65lete\x12%.spaceone.api.identity.v2.UserRequest\x1a\x16.google.protobuf.Empty\"#\x82\xd3\xe4\x93\x02\x1d\"\x18/identity/v2/user/delete:\x01*\x12r\n\x03get\x12%.spaceone.api.identity.v2.UserRequest\x1a\".spaceone.api.identity.v2.UserInfo\" \x82\xd3\xe4\x93\x02\x1a\"\x15/identity/v2/user/get:\x01*\x12y\n\x04list\x12).spaceone.api.identity.v2.UserSearchQuery\x1a#.spaceone.api.identity.v2.UsersInfo\"!\x82\xd3\xe4\x93\x02\x1b\"\x16/identity/v2/user/list:\x01*\x12k\n\x04stat\x12\'.spaceone.api.identity.v2.UserStatQuery\x1a\x17.google.protobuf.Struct\"!\x82\xd3\xe4\x93\x02\x1b\"\x16/identity/v1/user/stat:\x01*B?Z=github.com/cloudforet-io/api/dist/go/spaceone/api/identity/v2b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#spaceone/api/identity/v2/user.proto\x12\x18spaceone.api.identity.v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\x1a spaceone/api/core/v2/query.proto\x1a(spaceone/api/identity/v2/workspace.proto\"\xa3\x01\n\x03MFA\x12\x32\n\x05state\x18\x01 \x01(\x0e\x32#.spaceone.api.identity.v2.MFA.State\x12\x10\n\x08mfa_type\x18\x02 \x01(\t\x12(\n\x07options\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\",\n\x05State\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\"\xed\x01\n\x11\x43reateUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x35\n\tauth_type\x18\x05 \x01(\x0e\x32\".spaceone.api.identity.v2.AuthType\x12\x10\n\x08language\x18\x06 \x01(\t\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12%\n\x04tags\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x16\n\x0ereset_password\x18\t \x01(\x08\"\xb6\x01\n\x11UpdateUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x10\n\x08language\x18\x05 \x01(\t\x12\x10\n\x08timezone\x18\x06 \x01(\t\x12%\n\x04tags\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x16\n\x0ereset_password\x18\x08 \x01(\x08\"8\n\x16VerifyUserEmailRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\r\n\x05\x65mail\x18\x02 \x01(\t\"(\n\x15\x44isableUserMFARequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\"t\n\x19SetRequiredActionsRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x46\n\x10required_actions\x18\x02 \x03(\x0e\x32,.spaceone.api.identity.v2.UserRequiredAction\"\x1e\n\x0bUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\"\x9d\x02\n\x0fUserSearchQuery\x12*\n\x05query\x18\x01 \x01(\x0b\x32\x1b.spaceone.api.core.v2.Query\x12\x0f\n\x07user_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12>\n\x05state\x18\x04 \x01(\x0e\x32/.spaceone.api.identity.v2.UserSearchQuery.State\x12\r\n\x05\x65mail\x18\x05 \x01(\t\x12\x35\n\tauth_type\x18\x06 \x01(\x0e\x32\".spaceone.api.identity.v2.AuthType\"9\n\x05State\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07PENDING\x10\x03\"\x8e\x05\n\x08UserInfo\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x37\n\x05state\x18\x03 \x01(\x0e\x32(.spaceone.api.identity.v2.UserInfo.State\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x16\n\x0e\x65mail_verified\x18\x05 \x01(\x08\x12\x35\n\tauth_type\x18\x06 \x01(\x0e\x32\".spaceone.api.identity.v2.AuthType\x12\x0f\n\x07role_id\x18\x07 \x01(\t\x12>\n\trole_type\x18\x08 \x01(\x0e\x32+.spaceone.api.identity.v2.UserInfo.RoleType\x12*\n\x03mfa\x18\t \x01(\x0b\x32\x1d.spaceone.api.identity.v2.MFA\x12\x10\n\x08language\x18\x0b \x01(\t\x12\x10\n\x08timezone\x18\x0c \x01(\t\x12\x46\n\x10required_actions\x18\r \x03(\x0e\x32,.spaceone.api.identity.v2.UserRequiredAction\x12%\n\x04tags\x18\x0e \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x11\n\tdomain_id\x18\x15 \x01(\t\x12\x12\n\ncreated_at\x18\x1f \x01(\t\x12\x18\n\x10last_accessed_at\x18  \x01(\t\"?\n\x05State\x12\x0e\n\nSTATE_NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07PENDING\x10\x03\":\n\x08RoleType\x12\x12\n\x0eROLE_TYPE_NONE\x10\x00\x12\x10\n\x0c\x44OMAIN_ADMIN\x10\x01\x12\x08\n\x04USER\x10\x02\"U\n\tUsersInfo\x12\x33\n\x07results\x18\x01 \x03(\x0b\x32\".spaceone.api.identity.v2.UserInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05\"E\n\rUserStatQuery\x12\x34\n\x05query\x18\x01 \x01(\x0b\x32%.spaceone.api.core.v2.StatisticsQuery*5\n\x08\x41uthType\x12\x10\n\x0cNONE_BACKEND\x10\x00\x12\t\n\x05LOCAL\x10\x01\x12\x0c\n\x08\x45XTERNAL\x10\x02*)\n\x12UserRequiredAction\x12\x13\n\x0fUPDATE_PASSWORD\x10\x00\x32\x80\x0b\n\x04User\x12~\n\x06\x63reate\x12+.spaceone.api.identity.v2.CreateUserRequest\x1a\".spaceone.api.identity.v2.UserInfo\"#\x82\xd3\xe4\x93\x02\x1d\"\x18/identity/v2/user/create:\x01*\x12~\n\x06update\x12+.spaceone.api.identity.v2.UpdateUserRequest\x1a\".spaceone.api.identity.v2.UserInfo\"#\x82\xd3\xe4\x93\x02\x1d\"\x18/identity/v2/user/update:\x01*\x12\x83\x01\n\x0cverify_email\x12\x30.spaceone.api.identity.v2.VerifyUserEmailRequest\x1a\x16.google.protobuf.Empty\")\x82\xd3\xe4\x93\x02#\"\x1e/identity/v2/user/verify-email:\x01*\x12\x8c\x01\n\x0b\x64isable_mfa\x12/.spaceone.api.identity.v2.DisableUserMFARequest\x1a\".spaceone.api.identity.v2.UserInfo\"(\x82\xd3\xe4\x93\x02\"\"\x1d/identity/v2/user/disable-mfa:\x01*\x12\xa2\x01\n\x14set_required_actions\x12\x33.spaceone.api.identity.v2.SetRequiredActionsRequest\x1a\".spaceone.api.identity.v2.UserInfo\"1\x82\xd3\xe4\x93\x02+\"&/identity/v2/user/set-required-actions:\x01*\x12x\n\x06\x65nable\x12%.spaceone.api.identity.v2.UserRequest\x1a\".spaceone.api.identity.v2.UserInfo\"#\x82\xd3\xe4\x93\x02\x1d\"\x18/identity/v2/user/enable:\x01*\x12z\n\x07\x64isable\x12%.spaceone.api.identity.v2.UserRequest\x1a\".spaceone.api.identity.v2.UserInfo\"$\x82\xd3\xe4\x93\x02\x1e\"\x19/identity/v2/user/disable:\x01*\x12l\n\x06\x64\x65lete\x12%.spaceone.api.identity.v2.UserRequest\x1a\x16.google.protobuf.Empty\"#\x82\xd3\xe4\x93\x02\x1d\"\x18/identity/v2/user/delete:\x01*\x12r\n\x03get\x12%.spaceone.api.identity.v2.UserRequest\x1a\".spaceone.api.identity.v2.UserInfo\" \x82\xd3\xe4\x93\x02\x1a\"\x15/identity/v2/user/get:\x01*\x12y\n\x04list\x12).spaceone.api.identity.v2.UserSearchQuery\x1a#.spaceone.api.identity.v2.UsersInfo\"!\x82\xd3\xe4\x93\x02\x1b\"\x16/identity/v2/user/list:\x01*\x12k\n\x04stat\x12\'.spaceone.api.identity.v2.UserStatQuery\x1a\x17.google.protobuf.Struct\"!\x82\xd3\xe4\x93\x02\x1b\"\x16/identity/v1/user/stat:\x01*B?Z=github.com/cloudforet-io/api/dist/go/spaceone/api/identity/v2b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'spaceone.api.identity.v2.user_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z=github.com/cloudforet-io/api/dist/go/spaceone/api/identity/v2'
@@ -45,18 +45,18 @@
   _globals['_USER'].methods_by_name['delete']._serialized_options = b'\202\323\344\223\002\035\"\030/identity/v2/user/delete:\001*'
   _globals['_USER'].methods_by_name['get']._options = None
   _globals['_USER'].methods_by_name['get']._serialized_options = b'\202\323\344\223\002\032\"\025/identity/v2/user/get:\001*'
   _globals['_USER'].methods_by_name['list']._options = None
   _globals['_USER'].methods_by_name['list']._serialized_options = b'\202\323\344\223\002\033\"\026/identity/v2/user/list:\001*'
   _globals['_USER'].methods_by_name['stat']._options = None
   _globals['_USER'].methods_by_name['stat']._serialized_options = b'\202\323\344\223\002\033\"\026/identity/v1/user/stat:\001*'
-  _globals['_AUTHTYPE']._serialized_start=2180
-  _globals['_AUTHTYPE']._serialized_end=2233
-  _globals['_USERREQUIREDACTION']._serialized_start=2235
-  _globals['_USERREQUIREDACTION']._serialized_end=2276
+  _globals['_AUTHTYPE']._serialized_start=2174
+  _globals['_AUTHTYPE']._serialized_end=2227
+  _globals['_USERREQUIREDACTION']._serialized_start=2229
+  _globals['_USERREQUIREDACTION']._serialized_end=2270
   _globals['_MFA']._serialized_start=231
   _globals['_MFA']._serialized_end=394
   _globals['_MFA_STATE']._serialized_start=350
   _globals['_MFA_STATE']._serialized_end=394
   _globals['_CREATEUSERREQUEST']._serialized_start=397
   _globals['_CREATEUSERREQUEST']._serialized_end=634
   _globals['_UPDATEUSERREQUEST']._serialized_start=637
@@ -70,19 +70,19 @@
   _globals['_USERREQUEST']._serialized_start=1039
   _globals['_USERREQUEST']._serialized_end=1069
   _globals['_USERSEARCHQUERY']._serialized_start=1072
   _globals['_USERSEARCHQUERY']._serialized_end=1357
   _globals['_USERSEARCHQUERY_STATE']._serialized_start=1300
   _globals['_USERSEARCHQUERY_STATE']._serialized_end=1357
   _globals['_USERINFO']._serialized_start=1360
-  _globals['_USERINFO']._serialized_end=2020
-  _globals['_USERINFO_STATE']._serialized_start=1897
-  _globals['_USERINFO_STATE']._serialized_end=1960
-  _globals['_USERINFO_ROLETYPE']._serialized_start=1962
-  _globals['_USERINFO_ROLETYPE']._serialized_end=2020
-  _globals['_USERSINFO']._serialized_start=2022
-  _globals['_USERSINFO']._serialized_end=2107
-  _globals['_USERSTATQUERY']._serialized_start=2109
-  _globals['_USERSTATQUERY']._serialized_end=2178
-  _globals['_USER']._serialized_start=2279
-  _globals['_USER']._serialized_end=3687
+  _globals['_USERINFO']._serialized_end=2014
+  _globals['_USERINFO_STATE']._serialized_start=1891
+  _globals['_USERINFO_STATE']._serialized_end=1954
+  _globals['_USERINFO_ROLETYPE']._serialized_start=1956
+  _globals['_USERINFO_ROLETYPE']._serialized_end=2014
+  _globals['_USERSINFO']._serialized_start=2016
+  _globals['_USERSINFO']._serialized_end=2101
+  _globals['_USERSTATQUERY']._serialized_start=2103
+  _globals['_USERSTATQUERY']._serialized_end=2172
+  _globals['_USER']._serialized_start=2273
+  _globals['_USER']._serialized_end=3681
 # @@protoc_insertion_point(module_scope)
```

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/user_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/user_profile_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/user_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/user_profile_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/user_profile_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/workspace_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/workspace_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/workspace_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/workspace_user_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/workspace_user_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from spaceone.api.core.v2 import query_pb2 as spaceone_dot_api_dot_core_dot_v2_dot_query__pb2
 from spaceone.api.identity.v2 import user_pb2 as spaceone_dot_api_dot_identity_dot_v2_dot_user__pb2
 from spaceone.api.identity.v2 import role_binding_pb2 as spaceone_dot_api_dot_identity_dot_v2_dot_role__binding__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-spaceone/api/identity/v2/workspace_user.proto\x12\x18spaceone.api.identity.v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\x1a spaceone/api/core/v2/query.proto\x1a#spaceone/api/identity/v2/user.proto\x1a+spaceone/api/identity/v2/role_binding.proto\"\x87\x02\n\x1a\x43reateWorkspaceUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x35\n\tauth_type\x18\x05 \x01(\x0e\x32\".spaceone.api.identity.v2.AuthType\x12\x10\n\x08language\x18\x06 \x01(\t\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12%\n\x04tags\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x16\n\x0ereset_password\x18\t \x01(\x08\x12\x0f\n\x07role_id\x18\n \x01(\t\"\'\n\x14WorkspaceUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\"\xd9\x01\n\x18WorkspaceUserFindRequest\x12\x0f\n\x07keyword\x18\x01 \x01(\t\x12G\n\x05state\x18\x02 \x01(\x0e\x32\x38.spaceone.api.identity.v2.WorkspaceUserFindRequest.State\x12(\n\x04page\x18\x03 \x01(\x0b\x32\x1a.spaceone.api.core.v2.Page\"9\n\x05State\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07PENDING\x10\x03\"\xe9\x04\n\x11WorkspaceUserInfo\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12@\n\x05state\x18\x03 \x01(\x0e\x32\x31.spaceone.api.identity.v2.WorkspaceUserInfo.State\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x35\n\tauth_type\x18\x05 \x01(\x0e\x32\".spaceone.api.identity.v2.AuthType\x12G\n\trole_type\x18\x06 \x01(\x0e\x32\x34.spaceone.api.identity.v2.WorkspaceUserInfo.RoleType\x12\x10\n\x08language\x18\x07 \x01(\t\x12\x10\n\x08timezone\x18\x08 \x01(\t\x12\x15\n\rapi_key_count\x18\t \x01(\x05\x12%\n\x04tags\x18\n \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x44\n\x11role_binding_info\x18\x0b \x01(\x0b\x32).spaceone.api.identity.v2.RoleBindingInfo\x12\x11\n\tdomain_id\x18\x15 \x01(\t\x12\x12\n\ncreated_at\x18\x1f \x01(\t\x12\x18\n\x10last_accessed_at\x18  \x01(\t\"?\n\x05State\x12\x0e\n\nSTATE_NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07PENDING\x10\x03\":\n\x08RoleType\x12\x12\n\x0eROLE_TYPE_NONE\x10\x00\x12\x10\n\x0c\x44OMAIN_ADMIN\x10\x01\x12\x08\n\x04USER\x10\x02\"\xc5\x02\n\x18WorkspaceUserSearchQuery\x12*\n\x05query\x18\x01 \x01(\x0b\x32\x1b.spaceone.api.core.v2.Query\x12\x0f\n\x07user_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12G\n\x05state\x18\x04 \x01(\x0e\x32\x38.spaceone.api.identity.v2.WorkspaceUserSearchQuery.State\x12\r\n\x05\x65mail\x18\x05 \x01(\t\x12\x35\n\tauth_type\x18\x06 \x01(\x0e\x32\".spaceone.api.identity.v2.AuthType\x12\x14\n\x0cworkspace_id\x18\x15 \x01(\t\"9\n\x05State\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07PENDING\x10\x03\"g\n\x12WorkspaceUsersInfo\x12<\n\x07results\x18\x01 \x03(\x0b\x32+.spaceone.api.identity.v2.WorkspaceUserInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05\"\xb1\x01\n\x0fUserSummaryInfo\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12>\n\x05state\x18\x03 \x01(\x0e\x32/.spaceone.api.identity.v2.UserSummaryInfo.State\"?\n\x05State\x12\x0e\n\nSTATE_NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07PENDING\x10\x03\"c\n\x10UsersSummaryInfo\x12:\n\x07results\x18\x01 \x03(\x0b\x32).spaceone.api.identity.v2.UserSummaryInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05\"N\n\x16WorkspaceUserStatQuery\x12\x34\n\x05query\x18\x01 \x01(\x0b\x32%.spaceone.api.core.v2.StatisticsQuery2\xeb\x05\n\rWorkspaceUser\x12\x9a\x01\n\x06\x63reate\x12\x34.spaceone.api.identity.v2.CreateWorkspaceUserRequest\x1a+.spaceone.api.identity.v2.WorkspaceUserInfo\"-\x82\xd3\xe4\x93\x02\'\"\"/identity/v2/workspace-user/create:\x01*\x12\x8e\x01\n\x03get\x12..spaceone.api.identity.v2.WorkspaceUserRequest\x1a+.spaceone.api.identity.v2.WorkspaceUserInfo\"*\x82\xd3\xe4\x93\x02$\"\x1f/identity/v2/workspace-user/get:\x01*\x12\x93\x01\n\x04\x66ind\x12\x32.spaceone.api.identity.v2.WorkspaceUserFindRequest\x1a*.spaceone.api.identity.v2.UsersSummaryInfo\"+\x82\xd3\xe4\x93\x02%\" /identity/v2/workspace-user/find:\x01*\x12\x95\x01\n\x04list\x12\x32.spaceone.api.identity.v2.WorkspaceUserSearchQuery\x1a,.spaceone.api.identity.v2.WorkspaceUsersInfo\"+\x82\xd3\xe4\x93\x02%\" /identity/v2/workspace-user/list:\x01*\x12~\n\x04stat\x12\x30.spaceone.api.identity.v2.WorkspaceUserStatQuery\x1a\x17.google.protobuf.Struct\"+\x82\xd3\xe4\x93\x02%\" /identity/v1/workspace-user/stat:\x01*B?Z=github.com/cloudforet-io/api/dist/go/spaceone/api/identity/v2b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-spaceone/api/identity/v2/workspace_user.proto\x12\x18spaceone.api.identity.v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\x1a spaceone/api/core/v2/query.proto\x1a#spaceone/api/identity/v2/user.proto\x1a+spaceone/api/identity/v2/role_binding.proto\"\x87\x02\n\x1a\x43reateWorkspaceUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x35\n\tauth_type\x18\x05 \x01(\x0e\x32\".spaceone.api.identity.v2.AuthType\x12\x10\n\x08language\x18\x06 \x01(\t\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12%\n\x04tags\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x16\n\x0ereset_password\x18\t \x01(\x08\x12\x0f\n\x07role_id\x18\n \x01(\t\"\xd9\x01\n\x18WorkspaceUserFindRequest\x12\x0f\n\x07keyword\x18\x01 \x01(\t\x12G\n\x05state\x18\x02 \x01(\x0e\x32\x38.spaceone.api.identity.v2.WorkspaceUserFindRequest.State\x12(\n\x04page\x18\x03 \x01(\x0b\x32\x1a.spaceone.api.core.v2.Page\"9\n\x05State\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07PENDING\x10\x03\"=\n\x14WorkspaceUserRequest\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x15 \x01(\t\"\xe9\x04\n\x11WorkspaceUserInfo\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12@\n\x05state\x18\x03 \x01(\x0e\x32\x31.spaceone.api.identity.v2.WorkspaceUserInfo.State\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x35\n\tauth_type\x18\x05 \x01(\x0e\x32\".spaceone.api.identity.v2.AuthType\x12G\n\trole_type\x18\x06 \x01(\x0e\x32\x34.spaceone.api.identity.v2.WorkspaceUserInfo.RoleType\x12\x10\n\x08language\x18\x07 \x01(\t\x12\x10\n\x08timezone\x18\x08 \x01(\t\x12\x15\n\rapi_key_count\x18\t \x01(\x05\x12%\n\x04tags\x18\n \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x44\n\x11role_binding_info\x18\x0b \x01(\x0b\x32).spaceone.api.identity.v2.RoleBindingInfo\x12\x11\n\tdomain_id\x18\x15 \x01(\t\x12\x12\n\ncreated_at\x18\x1f \x01(\t\x12\x18\n\x10last_accessed_at\x18  \x01(\t\"?\n\x05State\x12\x0e\n\nSTATE_NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07PENDING\x10\x03\":\n\x08RoleType\x12\x12\n\x0eROLE_TYPE_NONE\x10\x00\x12\x10\n\x0c\x44OMAIN_ADMIN\x10\x01\x12\x08\n\x04USER\x10\x02\"\xc5\x02\n\x18WorkspaceUserSearchQuery\x12*\n\x05query\x18\x01 \x01(\x0b\x32\x1b.spaceone.api.core.v2.Query\x12\x0f\n\x07user_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12G\n\x05state\x18\x04 \x01(\x0e\x32\x38.spaceone.api.identity.v2.WorkspaceUserSearchQuery.State\x12\r\n\x05\x65mail\x18\x05 \x01(\t\x12\x35\n\tauth_type\x18\x06 \x01(\x0e\x32\".spaceone.api.identity.v2.AuthType\x12\x14\n\x0cworkspace_id\x18\x15 \x01(\t\"9\n\x05State\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07PENDING\x10\x03\"g\n\x12WorkspaceUsersInfo\x12<\n\x07results\x18\x01 \x03(\x0b\x32+.spaceone.api.identity.v2.WorkspaceUserInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05\"\xb1\x01\n\x0fUserSummaryInfo\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12>\n\x05state\x18\x03 \x01(\x0e\x32/.spaceone.api.identity.v2.UserSummaryInfo.State\"?\n\x05State\x12\x0e\n\nSTATE_NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07PENDING\x10\x03\"c\n\x10UsersSummaryInfo\x12:\n\x07results\x18\x01 \x03(\x0b\x32).spaceone.api.identity.v2.UserSummaryInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05\"d\n\x16WorkspaceUserStatQuery\x12\x34\n\x05query\x18\x01 \x01(\x0b\x32%.spaceone.api.core.v2.StatisticsQuery\x12\x14\n\x0cworkspace_id\x18\x15 \x01(\t2\xeb\x05\n\rWorkspaceUser\x12\x9a\x01\n\x06\x63reate\x12\x34.spaceone.api.identity.v2.CreateWorkspaceUserRequest\x1a+.spaceone.api.identity.v2.WorkspaceUserInfo\"-\x82\xd3\xe4\x93\x02\'\"\"/identity/v2/workspace-user/create:\x01*\x12\x8e\x01\n\x03get\x12..spaceone.api.identity.v2.WorkspaceUserRequest\x1a+.spaceone.api.identity.v2.WorkspaceUserInfo\"*\x82\xd3\xe4\x93\x02$\"\x1f/identity/v2/workspace-user/get:\x01*\x12\x93\x01\n\x04\x66ind\x12\x32.spaceone.api.identity.v2.WorkspaceUserFindRequest\x1a*.spaceone.api.identity.v2.UsersSummaryInfo\"+\x82\xd3\xe4\x93\x02%\" /identity/v2/workspace-user/find:\x01*\x12\x95\x01\n\x04list\x12\x32.spaceone.api.identity.v2.WorkspaceUserSearchQuery\x1a,.spaceone.api.identity.v2.WorkspaceUsersInfo\"+\x82\xd3\xe4\x93\x02%\" /identity/v2/workspace-user/list:\x01*\x12~\n\x04stat\x12\x30.spaceone.api.identity.v2.WorkspaceUserStatQuery\x1a\x17.google.protobuf.Struct\"+\x82\xd3\xe4\x93\x02%\" /identity/v1/workspace-user/stat:\x01*B?Z=github.com/cloudforet-io/api/dist/go/spaceone/api/identity/v2b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'spaceone.api.identity.v2.workspace_user_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z=github.com/cloudforet-io/api/dist/go/spaceone/api/identity/v2'
@@ -36,36 +36,36 @@
   _globals['_WORKSPACEUSER'].methods_by_name['find']._serialized_options = b'\202\323\344\223\002%\" /identity/v2/workspace-user/find:\001*'
   _globals['_WORKSPACEUSER'].methods_by_name['list']._options = None
   _globals['_WORKSPACEUSER'].methods_by_name['list']._serialized_options = b'\202\323\344\223\002%\" /identity/v2/workspace-user/list:\001*'
   _globals['_WORKSPACEUSER'].methods_by_name['stat']._options = None
   _globals['_WORKSPACEUSER'].methods_by_name['stat']._serialized_options = b'\202\323\344\223\002%\" /identity/v1/workspace-user/stat:\001*'
   _globals['_CREATEWORKSPACEUSERREQUEST']._serialized_start=281
   _globals['_CREATEWORKSPACEUSERREQUEST']._serialized_end=544
-  _globals['_WORKSPACEUSERREQUEST']._serialized_start=546
-  _globals['_WORKSPACEUSERREQUEST']._serialized_end=585
-  _globals['_WORKSPACEUSERFINDREQUEST']._serialized_start=588
-  _globals['_WORKSPACEUSERFINDREQUEST']._serialized_end=805
-  _globals['_WORKSPACEUSERFINDREQUEST_STATE']._serialized_start=748
-  _globals['_WORKSPACEUSERFINDREQUEST_STATE']._serialized_end=805
-  _globals['_WORKSPACEUSERINFO']._serialized_start=808
-  _globals['_WORKSPACEUSERINFO']._serialized_end=1425
-  _globals['_WORKSPACEUSERINFO_STATE']._serialized_start=1302
-  _globals['_WORKSPACEUSERINFO_STATE']._serialized_end=1365
-  _globals['_WORKSPACEUSERINFO_ROLETYPE']._serialized_start=1367
-  _globals['_WORKSPACEUSERINFO_ROLETYPE']._serialized_end=1425
-  _globals['_WORKSPACEUSERSEARCHQUERY']._serialized_start=1428
-  _globals['_WORKSPACEUSERSEARCHQUERY']._serialized_end=1753
-  _globals['_WORKSPACEUSERSEARCHQUERY_STATE']._serialized_start=748
-  _globals['_WORKSPACEUSERSEARCHQUERY_STATE']._serialized_end=805
-  _globals['_WORKSPACEUSERSINFO']._serialized_start=1755
-  _globals['_WORKSPACEUSERSINFO']._serialized_end=1858
-  _globals['_USERSUMMARYINFO']._serialized_start=1861
-  _globals['_USERSUMMARYINFO']._serialized_end=2038
-  _globals['_USERSUMMARYINFO_STATE']._serialized_start=1302
-  _globals['_USERSUMMARYINFO_STATE']._serialized_end=1365
-  _globals['_USERSSUMMARYINFO']._serialized_start=2040
-  _globals['_USERSSUMMARYINFO']._serialized_end=2139
-  _globals['_WORKSPACEUSERSTATQUERY']._serialized_start=2141
-  _globals['_WORKSPACEUSERSTATQUERY']._serialized_end=2219
-  _globals['_WORKSPACEUSER']._serialized_start=2222
-  _globals['_WORKSPACEUSER']._serialized_end=2969
+  _globals['_WORKSPACEUSERFINDREQUEST']._serialized_start=547
+  _globals['_WORKSPACEUSERFINDREQUEST']._serialized_end=764
+  _globals['_WORKSPACEUSERFINDREQUEST_STATE']._serialized_start=707
+  _globals['_WORKSPACEUSERFINDREQUEST_STATE']._serialized_end=764
+  _globals['_WORKSPACEUSERREQUEST']._serialized_start=766
+  _globals['_WORKSPACEUSERREQUEST']._serialized_end=827
+  _globals['_WORKSPACEUSERINFO']._serialized_start=830
+  _globals['_WORKSPACEUSERINFO']._serialized_end=1447
+  _globals['_WORKSPACEUSERINFO_STATE']._serialized_start=1324
+  _globals['_WORKSPACEUSERINFO_STATE']._serialized_end=1387
+  _globals['_WORKSPACEUSERINFO_ROLETYPE']._serialized_start=1389
+  _globals['_WORKSPACEUSERINFO_ROLETYPE']._serialized_end=1447
+  _globals['_WORKSPACEUSERSEARCHQUERY']._serialized_start=1450
+  _globals['_WORKSPACEUSERSEARCHQUERY']._serialized_end=1775
+  _globals['_WORKSPACEUSERSEARCHQUERY_STATE']._serialized_start=707
+  _globals['_WORKSPACEUSERSEARCHQUERY_STATE']._serialized_end=764
+  _globals['_WORKSPACEUSERSINFO']._serialized_start=1777
+  _globals['_WORKSPACEUSERSINFO']._serialized_end=1880
+  _globals['_USERSUMMARYINFO']._serialized_start=1883
+  _globals['_USERSUMMARYINFO']._serialized_end=2060
+  _globals['_USERSUMMARYINFO_STATE']._serialized_start=1324
+  _globals['_USERSUMMARYINFO_STATE']._serialized_end=1387
+  _globals['_USERSSUMMARYINFO']._serialized_start=2062
+  _globals['_USERSSUMMARYINFO']._serialized_end=2161
+  _globals['_WORKSPACEUSERSTATQUERY']._serialized_start=2163
+  _globals['_WORKSPACEUSERSTATQUERY']._serialized_end=2263
+  _globals['_WORKSPACEUSER']._serialized_start=2266
+  _globals['_WORKSPACEUSER']._serialized_end=3013
 # @@protoc_insertion_point(module_scope)
```

### Comparing `spaceone-api-2.0.dev78/spaceone/api/identity/v2/workspace_user_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/v2/workspace_user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/plugin/collector_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/log_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: spaceone/api/inventory/plugin/collector.proto
+# source: spaceone/api/monitoring/plugin/log.proto
 # Protobuf Python Version: 4.25.0
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-spaceone/api/inventory/plugin/collector.proto\x12\x1dspaceone.api.inventory.plugin\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\"7\n\x0bInitRequest\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"g\n\rVerifyRequest\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\x0bsecret_data\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xc0\x01\n\x0e\x43ollectRequest\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\x0bsecret_data\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\'\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12-\n\x0ctask_options\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xe9\x02\n\x0cResourceInfo\x12@\n\x05state\x18\x01 \x01(\x0e\x32\x31.spaceone.api.inventory.plugin.ResourceInfo.State\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x15\n\rresource_type\x18\x03 \x01(\t\x12,\n\x0bmatch_rules\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12)\n\x08resource\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12(\n\x07options\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\"l\n\x05State\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x43REATED\x10\x01\x12\x0b\n\x07PENDING\x10\x02\x12\x0e\n\nINPROGRESS\x10\x03\x12\x0b\n\x07SUCCESS\x10\x04\x12\x0b\n\x07\x46\x41ILURE\x10\x05\x12\x0b\n\x07TIMEOUT\x10\x06\x12\x08\n\x04IDLE\x10\x07\"?\n\x13\x43ollectorVerifyInfo\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"7\n\nPluginInfo\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct2\xa9\x02\n\tCollector\x12_\n\x04init\x12*.spaceone.api.inventory.plugin.InitRequest\x1a).spaceone.api.inventory.plugin.PluginInfo\"\x00\x12P\n\x06verify\x12,.spaceone.api.inventory.plugin.VerifyRequest\x1a\x16.google.protobuf.Empty\"\x00\x12i\n\x07\x63ollect\x12-.spaceone.api.inventory.plugin.CollectRequest\x1a+.spaceone.api.inventory.plugin.ResourceInfo\"\x00\x30\x01\x42\x44ZBgithub.com/cloudforet-io/api/dist/go/spaceone/api/inventory/pluginb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(spaceone/api/monitoring/plugin/log.proto\x12\x1espaceone.api.monitoring.plugin\x1a\x1cgoogle/protobuf/struct.proto\"!\n\x04Sort\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\x08\"\x8c\x02\n\nLogRequest\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\x0bsecret_data\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12&\n\x05query\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07keyword\x18\x05 \x01(\t\x12\r\n\x05start\x18\n \x01(\t\x12\x0b\n\x03\x65nd\x18\x0b \x01(\t\x12\x32\n\x04sort\x18\x0c \x01(\x0b\x32$.spaceone.api.monitoring.plugin.Sort\x12\r\n\x05limit\x18\r \x01(\x05\"8\n\x0cLogsDataInfo\x12(\n\x07results\x18\x01 \x03(\x0b\x32\x17.google.protobuf.Struct2k\n\x03Log\x12\x64\n\x04list\x12*.spaceone.api.monitoring.plugin.LogRequest\x1a,.spaceone.api.monitoring.plugin.LogsDataInfo\"\x00\x30\x01\x42\x45ZCgithub.com/cloudforet-io/api/dist/go/spaceone/api/monitoring/pluginb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'spaceone.api.inventory.plugin.collector_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'spaceone.api.monitoring.plugin.log_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
-  _globals['DESCRIPTOR']._serialized_options = b'ZBgithub.com/cloudforet-io/api/dist/go/spaceone/api/inventory/plugin'
-  _globals['_INITREQUEST']._serialized_start=139
-  _globals['_INITREQUEST']._serialized_end=194
-  _globals['_VERIFYREQUEST']._serialized_start=196
-  _globals['_VERIFYREQUEST']._serialized_end=299
-  _globals['_COLLECTREQUEST']._serialized_start=302
-  _globals['_COLLECTREQUEST']._serialized_end=494
-  _globals['_RESOURCEINFO']._serialized_start=497
-  _globals['_RESOURCEINFO']._serialized_end=858
-  _globals['_RESOURCEINFO_STATE']._serialized_start=750
-  _globals['_RESOURCEINFO_STATE']._serialized_end=858
-  _globals['_COLLECTORVERIFYINFO']._serialized_start=860
-  _globals['_COLLECTORVERIFYINFO']._serialized_end=923
-  _globals['_PLUGININFO']._serialized_start=925
-  _globals['_PLUGININFO']._serialized_end=980
-  _globals['_COLLECTOR']._serialized_start=983
-  _globals['_COLLECTOR']._serialized_end=1280
+  _globals['DESCRIPTOR']._serialized_options = b'ZCgithub.com/cloudforet-io/api/dist/go/spaceone/api/monitoring/plugin'
+  _globals['_SORT']._serialized_start=106
+  _globals['_SORT']._serialized_end=139
+  _globals['_LOGREQUEST']._serialized_start=142
+  _globals['_LOGREQUEST']._serialized_end=410
+  _globals['_LOGSDATAINFO']._serialized_start=412
+  _globals['_LOGSDATAINFO']._serialized_end=468
+  _globals['_LOG']._serialized_start=470
+  _globals['_LOG']._serialized_end=577
 # @@protoc_insertion_point(module_scope)
```

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/plugin/collector_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/plugin/collector_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/plugin/job_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/plugin/job_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/plugin/job_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/plugin/job_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/change_history_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/change_history_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/change_history_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/change_history_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_query_set_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_query_set_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_query_set_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_query_set_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_report_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_report_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_report_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_report_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_stats_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_stats_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_stats_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_type_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_type_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/cloud_service_type_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/cloud_service_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/collector_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/collector_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/collector_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/collector_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/collector_rule_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/collector_rule_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/collector_rule_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/collector_rule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/job_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/job_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/job_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/job_task_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/job_task_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/job_task_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/job_task_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/note_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/note_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/note_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/note_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/region_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/region_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/inventory/v1/region_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/inventory/v1/region_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/data_source_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/data_source_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/data_source_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/event_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/event_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/event_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/event_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/log_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/identity/plugin/external_auth_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: spaceone/api/monitoring/plugin/log.proto
+# source: spaceone/api/identity/plugin/external_auth.proto
 # Protobuf Python Version: 4.25.0
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(spaceone/api/monitoring/plugin/log.proto\x12\x1espaceone.api.monitoring.plugin\x1a\x1cgoogle/protobuf/struct.proto\"!\n\x04Sort\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\x08\"\x8c\x02\n\nLogRequest\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\x0bsecret_data\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12&\n\x05query\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07keyword\x18\x05 \x01(\t\x12\r\n\x05start\x18\n \x01(\t\x12\x0b\n\x03\x65nd\x18\x0b \x01(\t\x12\x32\n\x04sort\x18\x0c \x01(\x0b\x32$.spaceone.api.monitoring.plugin.Sort\x12\r\n\x05limit\x18\r \x01(\x05\"8\n\x0cLogsDataInfo\x12(\n\x07results\x18\x01 \x03(\x0b\x32\x17.google.protobuf.Struct2k\n\x03Log\x12\x64\n\x04list\x12*.spaceone.api.monitoring.plugin.LogRequest\x1a,.spaceone.api.monitoring.plugin.LogsDataInfo\"\x00\x30\x01\x42\x45ZCgithub.com/cloudforet-io/api/dist/go/spaceone/api/monitoring/pluginb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0spaceone/api/identity/plugin/external_auth.proto\x12\x1cspaceone.api.identity.plugin\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\"J\n\x0bInitRequest\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x11\n\tdomain_id\x18\x15 \x01(\t\"\xe9\x01\n\x10\x41uthorizeRequest\x12(\n\x07options\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x11\n\tschema_id\x18\x02 \x01(\t\x12,\n\x0bsecret_data\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\x0b\x63redentials\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x11\n\tdomain_id\x18\x15 \x01(\t\"\xd4\x01\n\x08UserInfo\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\x12\x0e\n\x06mobile\x18\x04 \x01(\t\x12\r\n\x05group\x18\x05 \x01(\t\x12;\n\x05state\x18\x06 \x01(\x0e\x32,.spaceone.api.identity.plugin.UserInfo.State\">\n\x05State\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x10\n\x0cUNIDENTIFIED\x10\x03\"7\n\nPluginInfo\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct2\xd4\x01\n\x0c\x45xternalAuth\x12]\n\x04init\x12).spaceone.api.identity.plugin.InitRequest\x1a(.spaceone.api.identity.plugin.PluginInfo\"\x00\x12\x65\n\tauthorize\x12..spaceone.api.identity.plugin.AuthorizeRequest\x1a&.spaceone.api.identity.plugin.UserInfo\"\x00\x42\x43ZAgithub.com/cloudforet-io/api/dist/go/spaceone/api/identity/pluginb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'spaceone.api.monitoring.plugin.log_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'spaceone.api.identity.plugin.external_auth_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
-  _globals['DESCRIPTOR']._serialized_options = b'ZCgithub.com/cloudforet-io/api/dist/go/spaceone/api/monitoring/plugin'
-  _globals['_SORT']._serialized_start=106
-  _globals['_SORT']._serialized_end=139
-  _globals['_LOGREQUEST']._serialized_start=142
-  _globals['_LOGREQUEST']._serialized_end=410
-  _globals['_LOGSDATAINFO']._serialized_start=412
-  _globals['_LOGSDATAINFO']._serialized_end=468
-  _globals['_LOG']._serialized_start=470
-  _globals['_LOG']._serialized_end=577
+  _globals['DESCRIPTOR']._serialized_options = b'ZAgithub.com/cloudforet-io/api/dist/go/spaceone/api/identity/plugin'
+  _globals['_INITREQUEST']._serialized_start=141
+  _globals['_INITREQUEST']._serialized_end=215
+  _globals['_AUTHORIZEREQUEST']._serialized_start=218
+  _globals['_AUTHORIZEREQUEST']._serialized_end=451
+  _globals['_USERINFO']._serialized_start=454
+  _globals['_USERINFO']._serialized_end=666
+  _globals['_USERINFO_STATE']._serialized_start=604
+  _globals['_USERINFO_STATE']._serialized_end=666
+  _globals['_PLUGININFO']._serialized_start=668
+  _globals['_PLUGININFO']._serialized_end=723
+  _globals['_EXTERNALAUTH']._serialized_start=726
+  _globals['_EXTERNALAUTH']._serialized_end=938
 # @@protoc_insertion_point(module_scope)
```

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/log_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/log_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/metric_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/metric_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/metric_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/webhook_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/webhook_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/plugin/webhook_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/plugin/webhook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/alert_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/alert_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/alert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/data_source_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/data_source_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/data_source_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/escalation_policy_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/escalation_policy_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/escalation_policy_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/escalation_policy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/event_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/event_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/event_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/event_rule_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/event_rule_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/event_rule_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/event_rule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/log_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/log_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/log_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/log_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/metric_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/metric_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/metric_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/note_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/note_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/note_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/note_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/project_alert_config_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/project_alert_config_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/project_alert_config_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/project_alert_config_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/webhook_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/webhook_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/monitoring/v1/webhook_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/monitoring/v1/webhook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/notification/plugin/notification_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/notification/plugin/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/notification/plugin/notification_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/notification/plugin/notification_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/notification/plugin/protocol_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/notification/plugin/protocol_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/notification/plugin/protocol_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/notification/plugin/protocol_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/notification/v1/notification_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/notification/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/notification/v1/notification_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/notification/v1/notification_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/notification/v1/project_channel_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/notification/v1/project_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/notification/v1/project_channel_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/notification/v1/project_channel_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/notification/v1/protocol_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/notification/v1/protocol_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/notification/v1/protocol_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/notification/v1/protocol_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/notification/v1/user_channel_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/notification/v1/user_channel_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from spaceone.api.core.v2 import query_pb2 as spaceone_dot_api_dot_core_dot_v2_dot_query__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/spaceone/api/notification/v1/user_channel.proto\x12\x1cspaceone.api.notification.v1\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\x1a spaceone/api/core/v2/query.proto\"\xe3\x01\n\x13UserChannelSchedule\x12P\n\x0b\x64\x61y_of_week\x18\x01 \x03(\x0e\x32;.spaceone.api.notification.v1.UserChannelSchedule.DayOfWeek\x12\x12\n\nstart_hour\x18\x02 \x01(\x05\x12\x10\n\x08\x65nd_hour\x18\x03 \x01(\x05\"T\n\tDayOfWeek\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03MON\x10\x01\x12\x07\n\x03TUE\x10\x02\x12\x07\n\x03WED\x10\x03\x12\x07\n\x03THU\x10\x04\x12\x07\n\x03\x46RI\x10\x05\x12\x07\n\x03SAT\x10\x06\x12\x07\n\x03SUN\x10\x07\"\x93\x02\n\x18\x43reateUserChannelRequest\x12\x13\n\x0bprotocol_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12%\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cis_subscribe\x18\x04 \x01(\x08\x12\x15\n\rsubscriptions\x18\x05 \x03(\t\x12\x14\n\x0cis_scheduled\x18\x06 \x01(\x08\x12\x43\n\x08schedule\x18\x07 \x01(\x0b\x32\x31.spaceone.api.notification.v1.UserChannelSchedule\x12%\n\x04tags\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xd4\x01\n\x18UpdateUserChannelRequest\x12\x17\n\x0fuser_channel_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12%\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x43\n\x08schedule\x18\x04 \x01(\x0b\x32\x31.spaceone.api.notification.v1.UserChannelSchedule\x12%\n\x04tags\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x96\x01\n UpdateUserChannelScheduleRequest\x12\x17\n\x0fuser_channel_id\x18\x01 \x01(\t\x12\x14\n\x0cis_scheduled\x18\x02 \x01(\x08\x12\x43\n\x08schedule\x18\x03 \x01(\x0b\x32\x31.spaceone.api.notification.v1.UserChannelSchedule\"l\n$UpdateUserChannelSubscriptionRequest\x12\x17\n\x0fuser_channel_id\x18\x01 \x01(\t\x12\x14\n\x0cis_subscribe\x18\x02 \x01(\x08\x12\x15\n\rsubscriptions\x18\x03 \x03(\t\"-\n\x12UserChannelRequest\x12\x17\n\x0fuser_channel_id\x18\x01 \x01(\t\"\xc2\x02\n\x10UserChannelQuery\x12*\n\x05query\x18\x01 \x01(\x0b\x32\x1b.spaceone.api.core.v2.Query\x12\x17\n\x0fuser_channel_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12N\n\x05state\x18\x04 \x01(\x0e\x32?.spaceone.api.notification.v1.UserChannelQuery.UserChannelState\x12\x14\n\x0cis_subscribe\x18\x05 \x01(\x08\x12\x14\n\x0cis_scheduled\x18\x06 \x01(\x08\x12\x13\n\x0bprotocol_id\x18\x15 \x01(\t\x12\x11\n\tsecret_id\x18\x16 \x01(\t\"7\n\x10UserChannelState\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\"\xf6\x03\n\x0fUserChannelInfo\x12\x17\n\x0fuser_channel_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12M\n\x05state\x18\x03 \x01(\x0e\x32>.spaceone.api.notification.v1.UserChannelInfo.UserChannelState\x12%\n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cis_subscribe\x18\x05 \x01(\x08\x12\x15\n\rsubscriptions\x18\x06 \x03(\t\x12\x14\n\x0cis_scheduled\x18\x07 \x01(\x08\x12\x43\n\x08schedule\x18\x08 \x01(\x0b\x32\x31.spaceone.api.notification.v1.UserChannelSchedule\x12%\n\x04tags\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x11\n\tdomain_id\x18\x15 \x01(\t\x12\x0f\n\x07user_id\x18\x16 \x01(\t\x12\x13\n\x0bprotocol_id\x18\x17 \x01(\t\x12\x11\n\tsecret_id\x18\x18 \x01(\t\x12\x12\n\ncreated_at\x18\x1f \x01(\t\"7\n\x10UserChannelState\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\"g\n\x10UserChannelsInfo\x12>\n\x07results\x18\x01 \x03(\x0b\x32-.spaceone.api.notification.v1.UserChannelInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05\"L\n\x14UserChannelStatQuery\x12\x34\n\x05query\x18\x01 \x01(\x0b\x32%.spaceone.api.core.v2.StatisticsQuery2\xc3\x0c\n\x0bUserChannel\x12\xa0\x01\n\x06\x63reate\x12\x36.spaceone.api.notification.v1.CreateUserChannelRequest\x1a-.spaceone.api.notification.v1.UserChannelInfo\"/\x82\xd3\xe4\x93\x02)\"$/notification/v1/user-channel/create:\x01*\x12\xa0\x01\n\x06update\x12\x36.spaceone.api.notification.v1.UpdateUserChannelRequest\x1a-.spaceone.api.notification.v1.UserChannelInfo\"/\x82\xd3\xe4\x93\x02)\"$/notification/v1/user-channel/update:\x01*\x12\xb4\x01\n\x0cset_schedule\x12>.spaceone.api.notification.v1.UpdateUserChannelScheduleRequest\x1a-.spaceone.api.notification.v1.UserChannelInfo\"5\x82\xd3\xe4\x93\x02/\"*/notification/v1/user-channel/set-schedule:\x01*\x12\xc0\x01\n\x10set_subscription\x12\x42.spaceone.api.notification.v1.UpdateUserChannelSubscriptionRequest\x1a-.spaceone.api.notification.v1.UserChannelInfo\"9\x82\xd3\xe4\x93\x02\x33\"./notification/v1/user-channel/set-subscription:\x01*\x12\x9a\x01\n\x06\x65nable\x12\x30.spaceone.api.notification.v1.UserChannelRequest\x1a-.spaceone.api.notification.v1.UserChannelInfo\"/\x82\xd3\xe4\x93\x02)\"$/notification/v1/user-channel/enable:\x01*\x12\x9c\x01\n\x07\x64isable\x12\x30.spaceone.api.notification.v1.UserChannelRequest\x1a-.spaceone.api.notification.v1.UserChannelInfo\"0\x82\xd3\xe4\x93\x02*\"%/notification/v1/user-channel/disable:\x01*\x12\x83\x01\n\x06\x64\x65lete\x12\x30.spaceone.api.notification.v1.UserChannelRequest\x1a\x16.google.protobuf.Empty\"/\x82\xd3\xe4\x93\x02)\"$/notification/v1/user-channel/delete:\x01*\x12\x94\x01\n\x03get\x12\x30.spaceone.api.notification.v1.UserChannelRequest\x1a-.spaceone.api.notification.v1.UserChannelInfo\",\x82\xd3\xe4\x93\x02&\"!/notification/v1/user-channel/get:\x01*\x12\x95\x01\n\x04list\x12..spaceone.api.notification.v1.UserChannelQuery\x1a..spaceone.api.notification.v1.UserChannelsInfo\"-\x82\xd3\xe4\x93\x02\'\"\"/notification/v1/user-channel/list:\x01*\x12\x82\x01\n\x04stat\x12\x32.spaceone.api.notification.v1.UserChannelStatQuery\x1a\x17.google.protobuf.Struct\"-\x82\xd3\xe4\x93\x02\'\"\"/notification/v1/user-channel/stat:\x01*BCZAgithub.com/cloudforet-io/api/dist/go/spaceone/api/notification/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/spaceone/api/notification/v1/user_channel.proto\x12\x1cspaceone.api.notification.v1\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\x1a spaceone/api/core/v2/query.proto\"\xe3\x01\n\x13UserChannelSchedule\x12P\n\x0b\x64\x61y_of_week\x18\x01 \x03(\x0e\x32;.spaceone.api.notification.v1.UserChannelSchedule.DayOfWeek\x12\x12\n\nstart_hour\x18\x02 \x01(\x05\x12\x10\n\x08\x65nd_hour\x18\x03 \x01(\x05\"T\n\tDayOfWeek\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03MON\x10\x01\x12\x07\n\x03TUE\x10\x02\x12\x07\n\x03WED\x10\x03\x12\x07\n\x03THU\x10\x04\x12\x07\n\x03\x46RI\x10\x05\x12\x07\n\x03SAT\x10\x06\x12\x07\n\x03SUN\x10\x07\"\x93\x02\n\x18\x43reateUserChannelRequest\x12\x13\n\x0bprotocol_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12%\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cis_subscribe\x18\x04 \x01(\x08\x12\x15\n\rsubscriptions\x18\x05 \x03(\t\x12\x14\n\x0cis_scheduled\x18\x06 \x01(\x08\x12\x43\n\x08schedule\x18\x07 \x01(\x0b\x32\x31.spaceone.api.notification.v1.UserChannelSchedule\x12%\n\x04tags\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xd4\x01\n\x18UpdateUserChannelRequest\x12\x17\n\x0fuser_channel_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12%\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x43\n\x08schedule\x18\x04 \x01(\x0b\x32\x31.spaceone.api.notification.v1.UserChannelSchedule\x12%\n\x04tags\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x96\x01\n UpdateUserChannelScheduleRequest\x12\x17\n\x0fuser_channel_id\x18\x01 \x01(\t\x12\x14\n\x0cis_scheduled\x18\x02 \x01(\x08\x12\x43\n\x08schedule\x18\x03 \x01(\x0b\x32\x31.spaceone.api.notification.v1.UserChannelSchedule\"l\n$UpdateUserChannelSubscriptionRequest\x12\x17\n\x0fuser_channel_id\x18\x01 \x01(\t\x12\x14\n\x0cis_subscribe\x18\x02 \x01(\x08\x12\x15\n\rsubscriptions\x18\x03 \x03(\t\"-\n\x12UserChannelRequest\x12\x17\n\x0fuser_channel_id\x18\x01 \x01(\t\"\xc7\x02\n\x10UserChannelQuery\x12*\n\x05query\x18\x01 \x01(\x0b\x32\x1b.spaceone.api.core.v2.Query\x12\x17\n\x0fuser_channel_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12N\n\x05state\x18\x04 \x01(\x0e\x32?.spaceone.api.notification.v1.UserChannelQuery.UserChannelState\x12\x14\n\x0cis_subscribe\x18\x05 \x01(\x08\x12\x14\n\x0cis_scheduled\x18\x06 \x01(\x08\x12\x13\n\x0bprotocol_id\x18\x15 \x01(\t\x12\x16\n\x0euser_secret_id\x18\x16 \x01(\t\"7\n\x10UserChannelState\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\"\xfb\x03\n\x0fUserChannelInfo\x12\x17\n\x0fuser_channel_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12M\n\x05state\x18\x03 \x01(\x0e\x32>.spaceone.api.notification.v1.UserChannelInfo.UserChannelState\x12%\n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cis_subscribe\x18\x05 \x01(\x08\x12\x15\n\rsubscriptions\x18\x06 \x03(\t\x12\x14\n\x0cis_scheduled\x18\x07 \x01(\x08\x12\x43\n\x08schedule\x18\x08 \x01(\x0b\x32\x31.spaceone.api.notification.v1.UserChannelSchedule\x12%\n\x04tags\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x11\n\tdomain_id\x18\x15 \x01(\t\x12\x0f\n\x07user_id\x18\x16 \x01(\t\x12\x13\n\x0bprotocol_id\x18\x17 \x01(\t\x12\x16\n\x0euser_secret_id\x18\x18 \x01(\t\x12\x12\n\ncreated_at\x18\x1f \x01(\t\"7\n\x10UserChannelState\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07\x45NABLED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\"g\n\x10UserChannelsInfo\x12>\n\x07results\x18\x01 \x03(\x0b\x32-.spaceone.api.notification.v1.UserChannelInfo\x12\x13\n\x0btotal_count\x18\x02 \x01(\x05\"L\n\x14UserChannelStatQuery\x12\x34\n\x05query\x18\x01 \x01(\x0b\x32%.spaceone.api.core.v2.StatisticsQuery2\xc3\x0c\n\x0bUserChannel\x12\xa0\x01\n\x06\x63reate\x12\x36.spaceone.api.notification.v1.CreateUserChannelRequest\x1a-.spaceone.api.notification.v1.UserChannelInfo\"/\x82\xd3\xe4\x93\x02)\"$/notification/v1/user-channel/create:\x01*\x12\xa0\x01\n\x06update\x12\x36.spaceone.api.notification.v1.UpdateUserChannelRequest\x1a-.spaceone.api.notification.v1.UserChannelInfo\"/\x82\xd3\xe4\x93\x02)\"$/notification/v1/user-channel/update:\x01*\x12\xb4\x01\n\x0cset_schedule\x12>.spaceone.api.notification.v1.UpdateUserChannelScheduleRequest\x1a-.spaceone.api.notification.v1.UserChannelInfo\"5\x82\xd3\xe4\x93\x02/\"*/notification/v1/user-channel/set-schedule:\x01*\x12\xc0\x01\n\x10set_subscription\x12\x42.spaceone.api.notification.v1.UpdateUserChannelSubscriptionRequest\x1a-.spaceone.api.notification.v1.UserChannelInfo\"9\x82\xd3\xe4\x93\x02\x33\"./notification/v1/user-channel/set-subscription:\x01*\x12\x9a\x01\n\x06\x65nable\x12\x30.spaceone.api.notification.v1.UserChannelRequest\x1a-.spaceone.api.notification.v1.UserChannelInfo\"/\x82\xd3\xe4\x93\x02)\"$/notification/v1/user-channel/enable:\x01*\x12\x9c\x01\n\x07\x64isable\x12\x30.spaceone.api.notification.v1.UserChannelRequest\x1a-.spaceone.api.notification.v1.UserChannelInfo\"0\x82\xd3\xe4\x93\x02*\"%/notification/v1/user-channel/disable:\x01*\x12\x83\x01\n\x06\x64\x65lete\x12\x30.spaceone.api.notification.v1.UserChannelRequest\x1a\x16.google.protobuf.Empty\"/\x82\xd3\xe4\x93\x02)\"$/notification/v1/user-channel/delete:\x01*\x12\x94\x01\n\x03get\x12\x30.spaceone.api.notification.v1.UserChannelRequest\x1a-.spaceone.api.notification.v1.UserChannelInfo\",\x82\xd3\xe4\x93\x02&\"!/notification/v1/user-channel/get:\x01*\x12\x95\x01\n\x04list\x12..spaceone.api.notification.v1.UserChannelQuery\x1a..spaceone.api.notification.v1.UserChannelsInfo\"-\x82\xd3\xe4\x93\x02\'\"\"/notification/v1/user-channel/list:\x01*\x12\x82\x01\n\x04stat\x12\x32.spaceone.api.notification.v1.UserChannelStatQuery\x1a\x17.google.protobuf.Struct\"-\x82\xd3\xe4\x93\x02\'\"\"/notification/v1/user-channel/stat:\x01*BCZAgithub.com/cloudforet-io/api/dist/go/spaceone/api/notification/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'spaceone.api.notification.v1.user_channel_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'ZAgithub.com/cloudforet-io/api/dist/go/spaceone/api/notification/v1'
@@ -57,21 +57,21 @@
   _globals['_UPDATEUSERCHANNELSCHEDULEREQUEST']._serialized_start=928
   _globals['_UPDATEUSERCHANNELSCHEDULEREQUEST']._serialized_end=1078
   _globals['_UPDATEUSERCHANNELSUBSCRIPTIONREQUEST']._serialized_start=1080
   _globals['_UPDATEUSERCHANNELSUBSCRIPTIONREQUEST']._serialized_end=1188
   _globals['_USERCHANNELREQUEST']._serialized_start=1190
   _globals['_USERCHANNELREQUEST']._serialized_end=1235
   _globals['_USERCHANNELQUERY']._serialized_start=1238
-  _globals['_USERCHANNELQUERY']._serialized_end=1560
-  _globals['_USERCHANNELQUERY_USERCHANNELSTATE']._serialized_start=1505
-  _globals['_USERCHANNELQUERY_USERCHANNELSTATE']._serialized_end=1560
-  _globals['_USERCHANNELINFO']._serialized_start=1563
-  _globals['_USERCHANNELINFO']._serialized_end=2065
-  _globals['_USERCHANNELINFO_USERCHANNELSTATE']._serialized_start=1505
-  _globals['_USERCHANNELINFO_USERCHANNELSTATE']._serialized_end=1560
-  _globals['_USERCHANNELSINFO']._serialized_start=2067
-  _globals['_USERCHANNELSINFO']._serialized_end=2170
-  _globals['_USERCHANNELSTATQUERY']._serialized_start=2172
-  _globals['_USERCHANNELSTATQUERY']._serialized_end=2248
-  _globals['_USERCHANNEL']._serialized_start=2251
-  _globals['_USERCHANNEL']._serialized_end=3854
+  _globals['_USERCHANNELQUERY']._serialized_end=1565
+  _globals['_USERCHANNELQUERY_USERCHANNELSTATE']._serialized_start=1510
+  _globals['_USERCHANNELQUERY_USERCHANNELSTATE']._serialized_end=1565
+  _globals['_USERCHANNELINFO']._serialized_start=1568
+  _globals['_USERCHANNELINFO']._serialized_end=2075
+  _globals['_USERCHANNELINFO_USERCHANNELSTATE']._serialized_start=1510
+  _globals['_USERCHANNELINFO_USERCHANNELSTATE']._serialized_end=1565
+  _globals['_USERCHANNELSINFO']._serialized_start=2077
+  _globals['_USERCHANNELSINFO']._serialized_end=2180
+  _globals['_USERCHANNELSTATQUERY']._serialized_start=2182
+  _globals['_USERCHANNELSTATQUERY']._serialized_end=2258
+  _globals['_USERCHANNEL']._serialized_start=2261
+  _globals['_USERCHANNEL']._serialized_end=3864
 # @@protoc_insertion_point(module_scope)
```

### Comparing `spaceone-api-2.0.dev78/spaceone/api/notification/v1/user_channel_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/notification/v1/user_channel_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/plugin/v1/plugin_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/plugin/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/plugin/v1/supervisor_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/plugin/v1/supervisor_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/plugin/v1/supervisor_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/plugin/v1/supervisor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/repository/v1/plugin_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/repository/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/repository/v1/plugin_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/repository/v1/plugin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/repository/v1/repository_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/repository/v1/repository_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/repository/v1/repository_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/repository/v1/repository_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/sample/v1/helloworld_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/sample/v1/helloworld_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/sample/v1/helloworld_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/sample/v1/helloworld_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/secret/v1/secret_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/secret/v1/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/secret/v1/secret_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/secret/v1/secret_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/secret/v1/trusted_secret_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/secret/v1/trusted_secret_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/secret/v1/trusted_secret_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/secret/v1/trusted_secret_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/secret/v1/user_secret_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/secret/v1/user_secret_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/secret/v1/user_secret_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/secret/v1/user_secret_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/statistics/v1/resource_pb2.py` & `spaceone-api-2.0.dev89/spaceone/api/statistics/v1/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone/api/statistics/v1/resource_pb2_grpc.py` & `spaceone-api-2.0.dev89/spaceone/api/statistics/v1/resource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spaceone-api-2.0.dev78/spaceone_api.egg-info/SOURCES.txt` & `spaceone-api-2.0.dev89/spaceone_api.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -59,16 +59,16 @@
 spaceone/api/dashboard/v1/public_dashboard_pb2_grpc.py
 spaceone/api/file_manager/__init__.py
 spaceone/api/file_manager/v1/__init__.py
 spaceone/api/file_manager/v1/file_pb2.py
 spaceone/api/file_manager/v1/file_pb2_grpc.py
 spaceone/api/identity/__init__.py
 spaceone/api/identity/plugin/__init__.py
-spaceone/api/identity/plugin/auth_pb2.py
-spaceone/api/identity/plugin/auth_pb2_grpc.py
+spaceone/api/identity/plugin/external_auth_pb2.py
+spaceone/api/identity/plugin/external_auth_pb2_grpc.py
 spaceone/api/identity/v1/__init__.py
 spaceone/api/identity/v1/api_key_pb2.py
 spaceone/api/identity/v1/api_key_pb2_grpc.py
 spaceone/api/identity/v1/authorization_pb2.py
 spaceone/api/identity/v1/authorization_pb2_grpc.py
 spaceone/api/identity/v1/domain_owner_pb2.py
 spaceone/api/identity/v1/domain_owner_pb2_grpc.py
```

