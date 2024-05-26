# Comparing `tmp/ambient_backend_api_client-0.1.8.tar.gz` & `tmp/ambient_backend_api_client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient_backend_api_client-0.1.8.tar", last modified: Sun May 26 15:19:40 2024, max compression
+gzip compressed data, was "ambient_backend_api_client-0.1.9.tar", last modified: Sun May 26 15:58:49 2024, max compression
```

## Comparing `ambient_backend_api_client-0.1.8.tar` & `ambient_backend_api_client-0.1.9.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:19:40.083705 ambient_backend_api_client-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-26 15:19:40.083705 ambient_backend_api_client-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:19:40.063705 ambient_backend_api_client-0.1.8/ambient_backend_api_client/
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:19:40.067705 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71865 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/clusters_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10046 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    82605 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/nodes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    53254 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    19071 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/ping_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/requests_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41751 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/services_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31740 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/unimplemented_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    62218 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26521 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14468 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:19:40.075705 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/account_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/ambient_action_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/ambient_event_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/architecture_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/auth0_device_code_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/cluster_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/create_service_acct_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/creation_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/event_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/event_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/interface_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/list_results_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/models_cluster_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/models_node_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/network_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/node_architecture_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/node_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/node_role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/notification_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/notification_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/notification_severity_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/organization_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/owner_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/post_clusters_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/post_service_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/refresh_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/request_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/status_enum_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/subscription_model_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/user_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/user_role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/validation_error_loc_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:19:40.063705 ambient_backend_api_client-0.1.8/ambient_backend_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-26 15:19:39.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-26 15:19:40.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 15:19:39.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-26 15:19:39.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-26 15:19:39.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-26 15:19:40.083705 ambient_backend_api_client-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:19:40.083705 ambient_backend_api_client-0.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_account_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_ambient_action_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_ambient_event_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_architecture_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_auth0_device_code_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_cluster_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_clusters_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_create_service_acct_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_creation_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_event_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_event_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_health_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_interface_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_list_results_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_models_cluster_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_models_node_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_network_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_node_architecture_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_node_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_node_role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_nodes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_notification_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_notification_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_notification_severity_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_organization_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_owner_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_ping_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_post_clusters_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_post_service_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_request_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_requests_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_service_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_service_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_service_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_service_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_services_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_status_enum_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_subscription_model_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_unimplemented_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_user_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_user_role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_users_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_validation_error_loc_inner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:58:49.567252 ambient_backend_api_client-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-26 15:58:49.567252 ambient_backend_api_client-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:58:49.551252 ambient_backend_api_client-0.1.9/ambient_backend_api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:58:49.555252 ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71865 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/clusters_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10046 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82605 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/nodes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53254 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19071 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/requests_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41751 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/services_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31740 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/unimplemented_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62218 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26521 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14468 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:58:49.559252 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/ambient_action_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/ambient_event_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/architecture_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/auth0_device_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/cluster_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/create_service_acct_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/creation_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/event_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/event_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/interface_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/list_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/models_cluster_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/models_node_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/network_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/node_architecture_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/node_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/node_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/notification_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/notification_severity_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/organization_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/owner_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/post_clusters_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/post_service_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/refresh_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/request_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/service_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/service_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/service_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/service_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/status_enum_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/subscription_model_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/user_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/user_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/validation_error_loc_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:58:49.551252 ambient_backend_api_client-0.1.9/ambient_backend_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-26 15:58:49.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-26 15:58:49.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 15:58:49.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-26 15:58:49.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-26 15:58:49.000000 ambient_backend_api_client-0.1.9/ambient_backend_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-26 15:58:49.571252 ambient_backend_api_client-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:58:49.567252 ambient_backend_api_client-0.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_ambient_action_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_ambient_event_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_architecture_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_auth0_device_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_cluster_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_clusters_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_create_service_acct_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_creation_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_event_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_event_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_health_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_interface_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_list_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_models_cluster_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_models_node_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_network_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_node_architecture_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_node_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_node_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_nodes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_notification_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_notification_severity_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_organization_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_owner_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_post_clusters_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_post_service_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_request_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_requests_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_service_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_service_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_service_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_service_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_services_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_status_enum_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_subscription_model_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_unimplemented_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_user_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_user_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-26 15:58:39.000000 ambient_backend_api_client-0.1.9/test/test_validation_error_loc_inner.py
```

### Comparing `ambient_backend_api_client-0.1.8/README.md` & `ambient_backend_api_client-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/__init__.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/__init__.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/clusters_api.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/clusters_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/health_api.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/health_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/nodes_api.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/nodes_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/notifications_api.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/notifications_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/ping_api.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/ping_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/requests_api.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/requests_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/services_api.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/services_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from pydantic import StrictStr
+from pydantic import StrictInt
 from typing import Any, Dict
 from ambient_backend_api_client.models.post_service_response import PostServiceResponse
 from ambient_backend_api_client.models.service import Service
 from ambient_backend_api_client.models.service_create import ServiceCreate
 from ambient_backend_api_client.models.service_list import ServiceList
 
 from ambient_backend_api_client.api_client import ApiClient, RequestSerialized
@@ -314,15 +314,15 @@
 
 
 
 
     @validate_call
     async def get_service_services_service_id_get(
         self,
-        service_id: StrictStr,
+        service_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -333,15 +333,15 @@
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Service:
         """Get Service
 
         Get a service
 
         :param service_id: (required)
-        :type service_id: str
+        :type service_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -382,15 +382,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     async def get_service_services_service_id_get_with_http_info(
         self,
-        service_id: StrictStr,
+        service_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -401,15 +401,15 @@
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Service]:
         """Get Service
 
         Get a service
 
         :param service_id: (required)
-        :type service_id: str
+        :type service_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -450,15 +450,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     async def get_service_services_service_id_get_without_preload_content(
         self,
-        service_id: StrictStr,
+        service_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -469,15 +469,15 @@
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Get Service
 
         Get a service
 
         :param service_id: (required)
-        :type service_id: str
+        :type service_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -818,15 +818,15 @@
 
 
 
 
     @validate_call
     async def patch_service_services_service_id_patch(
         self,
-        service_id: StrictStr,
+        service_id: StrictInt,
         body: Dict[str, Any],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -838,15 +838,15 @@
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Service:
         """Patch Service
 
         Patch a service
 
         :param service_id: (required)
-        :type service_id: str
+        :type service_id: int
         :param body: (required)
         :type body: object
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -890,15 +890,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     async def patch_service_services_service_id_patch_with_http_info(
         self,
-        service_id: StrictStr,
+        service_id: StrictInt,
         body: Dict[str, Any],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -910,15 +910,15 @@
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Service]:
         """Patch Service
 
         Patch a service
 
         :param service_id: (required)
-        :type service_id: str
+        :type service_id: int
         :param body: (required)
         :type body: object
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -962,15 +962,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     async def patch_service_services_service_id_patch_without_preload_content(
         self,
-        service_id: StrictStr,
+        service_id: StrictInt,
         body: Dict[str, Any],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -982,15 +982,15 @@
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Patch Service
 
         Patch a service
 
         :param service_id: (required)
-        :type service_id: str
+        :type service_id: int
         :param body: (required)
         :type body: object
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
```

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/unimplemented_api.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/unimplemented_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/users_api.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/api/users_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api_client.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api_response.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/api_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/configuration.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/exceptions.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/__init__.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/account_type.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/account_type.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/ambient_action_enum.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/ambient_action_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/ambient_event_type_enum.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/ambient_event_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/architecture_enum.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/auth0_device_code_response.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/auth0_device_code_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/cluster.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     architecture: ArchitectureEnum
     nodes: List[StrictStr]
     docker_swarm_attrs: Optional[Dict[str, Any]] = None
     site: Optional[StrictStr] = ''
     manager_node: Optional[StrictStr] = None
     cluster_group: Optional[StrictStr] = 'default'
     tags: Optional[List[StrictStr]] = None
-    identifier: Optional[StrictStr] = 'dc664e78-bd5d-4360-94b7-07cc434ee02e'
+    identifier: Optional[StrictStr] = '723bb589-7266-4cfc-ba6f-d99fa1c096c3'
     status: ModelsClusterStatusEnum
     __properties: ClassVar[List[str]] = ["id", "name", "resource_type", "description", "org_id", "user_id", "role", "architecture", "nodes", "docker_swarm_attrs", "site", "manager_node", "cluster_group", "tags", "identifier", "status"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
@@ -139,13 +139,13 @@
             "architecture": obj.get("architecture"),
             "nodes": obj.get("nodes"),
             "docker_swarm_attrs": obj.get("docker_swarm_attrs"),
             "site": obj.get("site") if obj.get("site") is not None else '',
             "manager_node": obj.get("manager_node"),
             "cluster_group": obj.get("cluster_group") if obj.get("cluster_group") is not None else 'default',
             "tags": obj.get("tags"),
-            "identifier": obj.get("identifier") if obj.get("identifier") is not None else 'dc664e78-bd5d-4360-94b7-07cc434ee02e',
+            "identifier": obj.get("identifier") if obj.get("identifier") is not None else '723bb589-7266-4cfc-ba6f-d99fa1c096c3',
             "status": obj.get("status")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/cluster_create.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/cluster_create.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     architecture: ArchitectureEnum
     nodes: List[StrictStr]
     docker_swarm_attrs: Optional[Dict[str, Any]] = None
     site: Optional[StrictStr] = ''
     manager_node: Optional[StrictStr] = None
     cluster_group: Optional[StrictStr] = 'default'
     tags: Optional[List[StrictStr]] = None
-    identifier: Optional[StrictStr] = 'dc664e78-bd5d-4360-94b7-07cc434ee02e'
+    identifier: Optional[StrictStr] = '723bb589-7266-4cfc-ba6f-d99fa1c096c3'
     __properties: ClassVar[List[str]] = ["id", "name", "resource_type", "description", "org_id", "user_id", "role", "architecture", "nodes", "docker_swarm_attrs", "site", "manager_node", "cluster_group", "tags", "identifier"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -137,12 +137,12 @@
             "architecture": obj.get("architecture"),
             "nodes": obj.get("nodes"),
             "docker_swarm_attrs": obj.get("docker_swarm_attrs"),
             "site": obj.get("site") if obj.get("site") is not None else '',
             "manager_node": obj.get("manager_node"),
             "cluster_group": obj.get("cluster_group") if obj.get("cluster_group") is not None else 'default',
             "tags": obj.get("tags"),
-            "identifier": obj.get("identifier") if obj.get("identifier") is not None else 'dc664e78-bd5d-4360-94b7-07cc434ee02e'
+            "identifier": obj.get("identifier") if obj.get("identifier") is not None else '723bb589-7266-4cfc-ba6f-d99fa1c096c3'
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/create_service_acct_request.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/create_service_acct_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/creation_method.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/creation_method.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/event.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/event.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/event_label.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/event_label.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/event_template.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/event_template.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/http_validation_error.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/interface_type_enum.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/interface_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/list_results_response.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/list_results_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from typing_extensions import Self
 
 class ListResultsResponse(BaseModel):
     """
     ListResultsResponse
     """ # noqa: E501
     count: StrictInt
-    timestamp: Optional[StrictStr] = '2024-05-26T09:10:32.907072'
+    timestamp: Optional[StrictStr] = '2024-05-26T09:37:47.692461'
     results: List[Any]
     __properties: ClassVar[List[str]] = ["count", "timestamp", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
@@ -79,13 +79,13 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
-            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else '2024-05-26T09:10:32.907072',
+            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else '2024-05-26T09:37:47.692461',
             "results": obj.get("results")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/models_cluster_status_enum.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/models_cluster_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/models_node_status_enum.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/models_node_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/network_interface.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/network_interface.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/node.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/node.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/node_architecture_enum.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/node_architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/node_create.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/node_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/node_role_enum.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/node_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/notification.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/notification.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/notification_list.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/notification_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class NotificationList(BaseModel):
     """
     NotificationList
     """ # noqa: E501
     count: StrictInt
-    timestamp: Optional[StrictStr] = '2024-05-26T09:10:32.907072'
+    timestamp: Optional[StrictStr] = '2024-05-26T09:37:47.692461'
     results: List[Notification]
     __properties: ClassVar[List[str]] = ["count", "timestamp", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
@@ -87,13 +87,13 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
-            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else '2024-05-26T09:10:32.907072',
+            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else '2024-05-26T09:37:47.692461',
             "results": [Notification.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/notification_request.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/notification_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/notification_severity_enum.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/notification_severity_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/organization_create.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/organization_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/owner_type_enum.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/owner_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/post_clusters_response.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/post_clusters_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 from typing import Optional, Set
 from typing_extensions import Self
 
 class PostClustersResponse(BaseModel):
     """
     PostClustersResponse
     """ # noqa: E501
-    request_id: StrictStr
-    requested_ts: Optional[StrictStr] = '2024-05-26T09:10:32.907623'
+    request_id: StrictInt
+    requested_ts: Optional[StrictStr] = '2024-05-26T09:37:47.693032'
     location_root: Optional[StrictStr] = 'http://localhost:8001/requests/'
     refresh_interval: Optional[StrictInt] = 10
     cluster: Cluster
     __properties: ClassVar[List[str]] = ["request_id", "requested_ts", "location_root", "refresh_interval", "cluster"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -85,15 +85,15 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "request_id": obj.get("request_id"),
-            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else '2024-05-26T09:10:32.907623',
+            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else '2024-05-26T09:37:47.693032',
             "location_root": obj.get("location_root") if obj.get("location_root") is not None else 'http://localhost:8001/requests/',
             "refresh_interval": obj.get("refresh_interval") if obj.get("refresh_interval") is not None else 10,
             "cluster": Cluster.from_dict(obj["cluster"]) if obj.get("cluster") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/post_service_response.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/post_service_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 from typing import Optional, Set
 from typing_extensions import Self
 
 class PostServiceResponse(BaseModel):
     """
     PostServiceResponse
     """ # noqa: E501
-    request_id: StrictStr
-    requested_ts: Optional[StrictStr] = '2024-05-26T09:10:32.907623'
+    request_id: StrictInt
+    requested_ts: Optional[StrictStr] = '2024-05-26T09:37:47.693032'
     location_root: Optional[StrictStr] = 'http://localhost:8001/requests/'
     refresh_interval: Optional[StrictInt] = 10
     service: Service
     __properties: ClassVar[List[str]] = ["request_id", "requested_ts", "location_root", "refresh_interval", "service"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -85,15 +85,15 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "request_id": obj.get("request_id"),
-            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else '2024-05-26T09:10:32.907623',
+            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else '2024-05-26T09:37:47.693032',
             "location_root": obj.get("location_root") if obj.get("location_root") is not None else 'http://localhost:8001/requests/',
             "refresh_interval": obj.get("refresh_interval") if obj.get("refresh_interval") is not None else 10,
             "service": Service.from_dict(obj["service"]) if obj.get("service") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/refresh_token_response.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/refresh_token_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/request.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name: StrictStr
     resource_type: ResourceTypeEnum
     description: Optional[StrictStr] = None
     org_id: Optional[StrictInt] = None
     user_id: Optional[StrictInt] = None
     status: Optional[RequestStatusEnum] = None
     error: Optional[StrictStr] = None
-    requested_ts: Optional[Union[StrictFloat, StrictInt]] = 1.7167362329035609E9
+    requested_ts: Optional[Union[StrictFloat, StrictInt]] = 1.716737867688868E9
     started_ts: Optional[Union[StrictFloat, StrictInt]] = None
     failed_ts: Optional[Union[StrictFloat, StrictInt]] = None
     completed_ts: Optional[Union[StrictFloat, StrictInt]] = None
     notes: Optional[List[StrictStr]] = None
     data: Optional[Dict[str, Any]] = None
     __properties: ClassVar[List[str]] = ["id", "name", "resource_type", "description", "org_id", "user_id", "status", "error", "requested_ts", "started_ts", "failed_ts", "completed_ts", "notes", "data"]
 
@@ -134,15 +134,15 @@
             "name": obj.get("name"),
             "resource_type": obj.get("resource_type"),
             "description": obj.get("description"),
             "org_id": obj.get("org_id"),
             "user_id": obj.get("user_id"),
             "status": obj.get("status"),
             "error": obj.get("error"),
-            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 1.7167362329035609E9,
+            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 1.716737867688868E9,
             "started_ts": obj.get("started_ts"),
             "failed_ts": obj.get("failed_ts"),
             "completed_ts": obj.get("completed_ts"),
             "notes": obj.get("notes"),
             "data": obj.get("data")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/request_status_enum.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/request_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/resource_type_enum.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/role_enum.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/service.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service_create.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/service_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service_list.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/service_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class ServiceList(BaseModel):
     """
     ServiceList
     """ # noqa: E501
     count: StrictInt
-    timestamp: Optional[StrictStr] = '2024-05-26T09:10:32.907072'
+    timestamp: Optional[StrictStr] = '2024-05-26T09:37:47.692461'
     results: List[Service]
     __properties: ClassVar[List[str]] = ["count", "timestamp", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
@@ -87,13 +87,13 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
-            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else '2024-05-26T09:10:32.907072',
+            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else '2024-05-26T09:37:47.692461',
             "results": [Service.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service_state.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/service_state.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service_status_enum.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/service_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/status_enum_input.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/status_enum_input.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/subscription_model_enum.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/subscription_model_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/token_response.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/token_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/user.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/user.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/user_preferences.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/user_preferences.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/user_role_enum.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/user_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/validation_error.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/validation_error_loc_inner.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/models/validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client/rest.py` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client/rest.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/ambient_backend_api_client.egg-info/SOURCES.txt` & `ambient_backend_api_client-0.1.9/ambient_backend_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/pyproject.toml` & `ambient_backend_api_client-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/setup.py` & `ambient_backend_api_client-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "ambient_backend_api_client"
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "aiohttp >= 3.0.0",
     "aiohttp-retry >= 2.8.3",
     "pydantic >= 2",
```

### Comparing `ambient_backend_api_client-0.1.8/test/test_account_type.py` & `ambient_backend_api_client-0.1.9/test/test_account_type.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_ambient_action_enum.py` & `ambient_backend_api_client-0.1.9/test/test_ambient_action_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_ambient_event_type_enum.py` & `ambient_backend_api_client-0.1.9/test/test_ambient_event_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_architecture_enum.py` & `ambient_backend_api_client-0.1.9/test/test_architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_auth0_device_code_response.py` & `ambient_backend_api_client-0.1.9/test/test_auth0_device_code_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_cluster.py` & `ambient_backend_api_client-0.1.9/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_cluster_create.py` & `ambient_backend_api_client-0.1.9/test/test_cluster_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_clusters_api.py` & `ambient_backend_api_client-0.1.9/test/test_clusters_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_create_service_acct_request.py` & `ambient_backend_api_client-0.1.9/test/test_create_service_acct_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_creation_method.py` & `ambient_backend_api_client-0.1.9/test/test_creation_method.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_event.py` & `ambient_backend_api_client-0.1.9/test/test_event.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_event_label.py` & `ambient_backend_api_client-0.1.9/test/test_event_label.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_event_template.py` & `ambient_backend_api_client-0.1.9/test/test_event_template.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_health_api.py` & `ambient_backend_api_client-0.1.9/test/test_health_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_http_validation_error.py` & `ambient_backend_api_client-0.1.9/test/test_http_validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_interface_type_enum.py` & `ambient_backend_api_client-0.1.9/test/test_interface_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_list_results_response.py` & `ambient_backend_api_client-0.1.9/test/test_list_results_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_models_cluster_status_enum.py` & `ambient_backend_api_client-0.1.9/test/test_models_cluster_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_models_node_status_enum.py` & `ambient_backend_api_client-0.1.9/test/test_models_node_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_network_interface.py` & `ambient_backend_api_client-0.1.9/test/test_network_interface.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_node.py` & `ambient_backend_api_client-0.1.9/test/test_node.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_node_architecture_enum.py` & `ambient_backend_api_client-0.1.9/test/test_node_architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_node_create.py` & `ambient_backend_api_client-0.1.9/test/test_node_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_node_role_enum.py` & `ambient_backend_api_client-0.1.9/test/test_node_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_nodes_api.py` & `ambient_backend_api_client-0.1.9/test/test_nodes_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_notification.py` & `ambient_backend_api_client-0.1.9/test/test_notification.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_notification_list.py` & `ambient_backend_api_client-0.1.9/test/test_notification_list.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_notification_request.py` & `ambient_backend_api_client-0.1.9/test/test_notification_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_notification_severity_enum.py` & `ambient_backend_api_client-0.1.9/test/test_notification_severity_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_notifications_api.py` & `ambient_backend_api_client-0.1.9/test/test_notifications_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_organization_create.py` & `ambient_backend_api_client-0.1.9/test/test_organization_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_owner_type_enum.py` & `ambient_backend_api_client-0.1.9/test/test_owner_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_ping_api.py` & `ambient_backend_api_client-0.1.9/test/test_ping_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_post_clusters_response.py` & `ambient_backend_api_client-0.1.9/test/test_post_clusters_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_post_service_response.py` & `ambient_backend_api_client-0.1.9/test/test_post_service_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_request.py` & `ambient_backend_api_client-0.1.9/test/test_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_request_status_enum.py` & `ambient_backend_api_client-0.1.9/test/test_request_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_requests_api.py` & `ambient_backend_api_client-0.1.9/test/test_requests_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_resource_type_enum.py` & `ambient_backend_api_client-0.1.9/test/test_resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_role_enum.py` & `ambient_backend_api_client-0.1.9/test/test_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_service.py` & `ambient_backend_api_client-0.1.9/test/test_service.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_service_create.py` & `ambient_backend_api_client-0.1.9/test/test_service_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_service_list.py` & `ambient_backend_api_client-0.1.9/test/test_service_list.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_service_state.py` & `ambient_backend_api_client-0.1.9/test/test_service_state.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_service_status_enum.py` & `ambient_backend_api_client-0.1.9/test/test_service_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_services_api.py` & `ambient_backend_api_client-0.1.9/test/test_services_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_status_enum_input.py` & `ambient_backend_api_client-0.1.9/test/test_status_enum_input.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_subscription_model_enum.py` & `ambient_backend_api_client-0.1.9/test/test_subscription_model_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_token_response.py` & `ambient_backend_api_client-0.1.9/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_unimplemented_api.py` & `ambient_backend_api_client-0.1.9/test/test_unimplemented_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_user.py` & `ambient_backend_api_client-0.1.9/test/test_user.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_user_preferences.py` & `ambient_backend_api_client-0.1.9/test/test_user_preferences.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_user_role_enum.py` & `ambient_backend_api_client-0.1.9/test/test_user_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_users_api.py` & `ambient_backend_api_client-0.1.9/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_validation_error.py` & `ambient_backend_api_client-0.1.9/test/test_validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.8/test/test_validation_error_loc_inner.py` & `ambient_backend_api_client-0.1.9/test/test_validation_error_loc_inner.py`

 * *Files identical despite different names*

