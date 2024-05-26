# Comparing `tmp/ambient_backend_api_client-0.1.7.tar.gz` & `tmp/ambient_backend_api_client-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient_backend_api_client-0.1.7.tar", last modified: Fri May 24 23:37:03 2024, max compression
+gzip compressed data, was "ambient_backend_api_client-0.1.8.tar", last modified: Sun May 26 15:19:40 2024, max compression
```

## Comparing `ambient_backend_api_client-0.1.7.tar` & `ambient_backend_api_client-0.1.8.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:37:03.207522 ambient_backend_api_client-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-24 23:37:03.207522 ambient_backend_api_client-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:37:03.191522 ambient_backend_api_client-0.1.7/ambient_backend_api_client/
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:37:03.195522 ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71865 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/clusters_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10046 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    82605 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/nodes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    53254 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    19071 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/ping_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/requests_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    42278 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/services_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31740 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/unimplemented_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    62218 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26521 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14468 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:37:03.199522 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/account_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/ambient_action_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/ambient_event_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/architecture_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/auth0_device_code_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/cluster_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/create_service_acct_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/creation_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/event_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/event_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/interface_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/list_results_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/models_cluster_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/models_node_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/network_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/node_architecture_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/node_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/node_role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/notification_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/notification_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/notification_severity_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/organization_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/owner_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/post_clusters_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/post_service_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/refresh_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/request_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/service_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/service_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/service_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/service_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/status_enum_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/subscription_model_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/user_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/user_role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/validation_error_loc_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:37:03.191522 ambient_backend_api_client-0.1.7/ambient_backend_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-24 23:37:03.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-24 23:37:03.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 23:37:03.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-24 23:37:03.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-24 23:37:03.000000 ambient_backend_api_client-0.1.7/ambient_backend_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 23:37:03.207522 ambient_backend_api_client-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:37:03.207522 ambient_backend_api_client-0.1.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_account_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_ambient_action_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_ambient_event_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_architecture_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_auth0_device_code_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_cluster_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_clusters_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_create_service_acct_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_creation_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_event_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_event_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_health_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_interface_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_list_results_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_models_cluster_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_models_node_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_network_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_node_architecture_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_node_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_node_role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_nodes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_notification_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_notification_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_notification_severity_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_organization_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_owner_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_ping_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_post_clusters_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_post_service_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_request_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_requests_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_service_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_service_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_service_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_service_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_services_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_status_enum_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_subscription_model_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_unimplemented_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_user_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_user_role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_users_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-24 23:36:55.000000 ambient_backend_api_client-0.1.7/test/test_validation_error_loc_inner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:19:40.083705 ambient_backend_api_client-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-26 15:19:40.083705 ambient_backend_api_client-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:19:40.063705 ambient_backend_api_client-0.1.8/ambient_backend_api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:19:40.067705 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71865 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/clusters_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10046 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82605 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/nodes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53254 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19071 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/requests_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41751 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/services_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31740 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/unimplemented_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62218 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26521 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14468 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:19:40.075705 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/ambient_action_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/ambient_event_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/architecture_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/auth0_device_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/cluster_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/create_service_acct_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/creation_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/event_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/event_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/interface_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/list_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/models_cluster_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/models_node_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/network_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/node_architecture_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/node_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/node_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/notification_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/notification_severity_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/organization_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/owner_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/post_clusters_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/post_service_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/refresh_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/request_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/status_enum_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/subscription_model_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/user_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/user_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/validation_error_loc_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:19:40.063705 ambient_backend_api_client-0.1.8/ambient_backend_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-26 15:19:39.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-26 15:19:40.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 15:19:39.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-26 15:19:39.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-26 15:19:39.000000 ambient_backend_api_client-0.1.8/ambient_backend_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-26 15:19:40.083705 ambient_backend_api_client-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:19:40.083705 ambient_backend_api_client-0.1.8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_ambient_action_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_ambient_event_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_architecture_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_auth0_device_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_cluster_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_clusters_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_create_service_acct_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_creation_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_event_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_event_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_health_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_interface_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_list_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_models_cluster_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_models_node_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_network_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_node_architecture_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_node_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_node_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_nodes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_notification_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_notification_severity_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_organization_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_owner_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_post_clusters_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_post_service_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_request_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_requests_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_service_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_service_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_service_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_service_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_services_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_status_enum_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_subscription_model_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_unimplemented_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_user_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_user_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-26 15:19:32.000000 ambient_backend_api_client-0.1.8/test/test_validation_error_loc_inner.py
```

### Comparing `ambient_backend_api_client-0.1.7/README.md` & `ambient_backend_api_client-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/__init__.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/__init__.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/clusters_api.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/clusters_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/health_api.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/health_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/nodes_api.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/nodes_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/notifications_api.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/notifications_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/ping_api.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/ping_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/requests_api.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/requests_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/services_api.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/services_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import StrictStr
-from typing import Any, Dict, Optional
+from typing import Any, Dict
 from ambient_backend_api_client.models.post_service_response import PostServiceResponse
 from ambient_backend_api_client.models.service import Service
 from ambient_backend_api_client.models.service_create import ServiceCreate
 from ambient_backend_api_client.models.service_list import ServiceList
 
 from ambient_backend_api_client.api_client import ApiClient, RequestSerialized
 from ambient_backend_api_client.api_response import ApiResponse
@@ -575,15 +575,14 @@
 
 
 
 
     @validate_call
     async def get_services_services_get(
         self,
-        q: Optional[StrictStr] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -593,16 +592,14 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ServiceList:
         """Get Services
 
         Get all services
 
-        :param q:
-        :type q: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -618,24 +615,22 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._get_services_services_get_serialize(
-            q=q,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "ServiceList",
-            '422': "HTTPValidationError",
         }
         response_data = await self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         await response_data.read()
         return self.api_client.response_deserialize(
@@ -643,15 +638,14 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     async def get_services_services_get_with_http_info(
         self,
-        q: Optional[StrictStr] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -661,16 +655,14 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[ServiceList]:
         """Get Services
 
         Get all services
 
-        :param q:
-        :type q: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -686,24 +678,22 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._get_services_services_get_serialize(
-            q=q,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "ServiceList",
-            '422': "HTTPValidationError",
         }
         response_data = await self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         await response_data.read()
         return self.api_client.response_deserialize(
@@ -711,15 +701,14 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     async def get_services_services_get_without_preload_content(
         self,
-        q: Optional[StrictStr] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -729,16 +718,14 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Get Services
 
         Get all services
 
-        :param q:
-        :type q: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -754,35 +741,32 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._get_services_services_get_serialize(
-            q=q,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "ServiceList",
-            '422': "HTTPValidationError",
         }
         response_data = await self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _get_services_services_get_serialize(
         self,
-        q,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -795,18 +779,14 @@
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
-        if q is not None:
-            
-            _query_params.append(('q', q))
-            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/unimplemented_api.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/unimplemented_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/api/users_api.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api/users_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/api_client.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/api_response.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/api_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/configuration.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/exceptions.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/__init__.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/account_type.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/account_type.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/ambient_action_enum.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/ambient_action_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/ambient_event_type_enum.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/ambient_event_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/architecture_enum.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/auth0_device_code_response.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/auth0_device_code_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/cluster.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     architecture: ArchitectureEnum
     nodes: List[StrictStr]
     docker_swarm_attrs: Optional[Dict[str, Any]] = None
     site: Optional[StrictStr] = ''
     manager_node: Optional[StrictStr] = None
     cluster_group: Optional[StrictStr] = 'default'
     tags: Optional[List[StrictStr]] = None
-    identifier: Optional[StrictStr] = 'c52ec791-530e-48d1-8cc7-7ed4fb8395e2'
+    identifier: Optional[StrictStr] = 'dc664e78-bd5d-4360-94b7-07cc434ee02e'
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
-            "identifier": obj.get("identifier") if obj.get("identifier") is not None else 'c52ec791-530e-48d1-8cc7-7ed4fb8395e2',
+            "identifier": obj.get("identifier") if obj.get("identifier") is not None else 'dc664e78-bd5d-4360-94b7-07cc434ee02e',
             "status": obj.get("status")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/cluster_create.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/cluster_create.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     architecture: ArchitectureEnum
     nodes: List[StrictStr]
     docker_swarm_attrs: Optional[Dict[str, Any]] = None
     site: Optional[StrictStr] = ''
     manager_node: Optional[StrictStr] = None
     cluster_group: Optional[StrictStr] = 'default'
     tags: Optional[List[StrictStr]] = None
-    identifier: Optional[StrictStr] = 'c52ec791-530e-48d1-8cc7-7ed4fb8395e2'
+    identifier: Optional[StrictStr] = 'dc664e78-bd5d-4360-94b7-07cc434ee02e'
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
-            "identifier": obj.get("identifier") if obj.get("identifier") is not None else 'c52ec791-530e-48d1-8cc7-7ed4fb8395e2'
+            "identifier": obj.get("identifier") if obj.get("identifier") is not None else 'dc664e78-bd5d-4360-94b7-07cc434ee02e'
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/create_service_acct_request.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/create_service_acct_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/creation_method.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/creation_method.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/event.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
     """
     Event
     """ # noqa: E501
     root: StrictStr
     event_label: EventLabel
     event_type: AmbientEventTypeEnum
     resource_type: ResourceTypeEnum
-    resource_id: StrictStr
+    resource_id: StrictInt
     action: Optional[AmbientActionEnum] = None
     timestamp: Union[StrictFloat, StrictInt]
     event_data: Dict[str, Any]
-    request_id: Optional[StrictStr] = None
+    request_id: Optional[StrictInt] = None
     __properties: ClassVar[List[str]] = ["root", "event_label", "event_type", "resource_type", "resource_id", "action", "timestamp", "event_data", "request_id"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
```

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/event_label.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/event_label.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/event_template.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/event_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from ambient_backend_api_client.models.ambient_action_enum import AmbientActionEnum
 from ambient_backend_api_client.models.ambient_event_type_enum import AmbientEventTypeEnum
 from ambient_backend_api_client.models.event_label import EventLabel
 from ambient_backend_api_client.models.resource_type_enum import ResourceTypeEnum
 from typing import Optional, Set
 from typing_extensions import Self
@@ -30,15 +30,15 @@
     """
     EventTemplate
     """ # noqa: E501
     root: StrictStr
     event_label: EventLabel
     event_type: AmbientEventTypeEnum
     resource_type: ResourceTypeEnum
-    resource_id: Optional[StrictStr] = None
+    resource_id: Optional[StrictInt] = None
     action: Optional[AmbientActionEnum] = None
     __properties: ClassVar[List[str]] = ["root", "event_label", "event_type", "resource_type", "resource_id", "action"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
```

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/http_validation_error.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/interface_type_enum.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/interface_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/list_results_response.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/list_results_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from typing_extensions import Self
 
 class ListResultsResponse(BaseModel):
     """
     ListResultsResponse
     """ # noqa: E501
     count: StrictInt
-    timestamp: Optional[StrictStr] = '2024-05-24T17:31:42.444659'
+    timestamp: Optional[StrictStr] = '2024-05-26T09:10:32.907072'
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
-            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else '2024-05-24T17:31:42.444659',
+            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else '2024-05-26T09:10:32.907072',
             "results": obj.get("results")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/models_cluster_status_enum.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/models_cluster_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/models_node_status_enum.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/models_node_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/network_interface.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/network_interface.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/node.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/node.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/node_architecture_enum.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/node_architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/node_create.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/node_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/node_role_enum.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/node_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/notification.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/notification.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/notification_list.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/notification_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class NotificationList(BaseModel):
     """
     NotificationList
     """ # noqa: E501
     count: StrictInt
-    timestamp: Optional[StrictStr] = '2024-05-24T17:31:42.444659'
+    timestamp: Optional[StrictStr] = '2024-05-26T09:10:32.907072'
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
-            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else '2024-05-24T17:31:42.444659',
+            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else '2024-05-26T09:10:32.907072',
             "results": [Notification.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/notification_request.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/notification_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/notification_severity_enum.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/notification_severity_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/organization_create.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/organization_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/owner_type_enum.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/owner_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/post_clusters_response.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/post_clusters_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class PostClustersResponse(BaseModel):
     """
     PostClustersResponse
     """ # noqa: E501
     request_id: StrictStr
-    requested_ts: Optional[StrictStr] = '2024-05-24T17:31:42.445217'
+    requested_ts: Optional[StrictStr] = '2024-05-26T09:10:32.907623'
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
-            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else '2024-05-24T17:31:42.445217',
+            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else '2024-05-26T09:10:32.907623',
             "location_root": obj.get("location_root") if obj.get("location_root") is not None else 'http://localhost:8001/requests/',
             "refresh_interval": obj.get("refresh_interval") if obj.get("refresh_interval") is not None else 10,
             "cluster": Cluster.from_dict(obj["cluster"]) if obj.get("cluster") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/post_service_response.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/post_service_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class PostServiceResponse(BaseModel):
     """
     PostServiceResponse
     """ # noqa: E501
     request_id: StrictStr
-    requested_ts: Optional[StrictStr] = '2024-05-24T17:31:42.445217'
+    requested_ts: Optional[StrictStr] = '2024-05-26T09:10:32.907623'
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
-            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else '2024-05-24T17:31:42.445217',
+            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else '2024-05-26T09:10:32.907623',
             "location_root": obj.get("location_root") if obj.get("location_root") is not None else 'http://localhost:8001/requests/',
             "refresh_interval": obj.get("refresh_interval") if obj.get("refresh_interval") is not None else 10,
             "service": Service.from_dict(obj["service"]) if obj.get("service") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/refresh_token_response.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/refresh_token_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/request.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 
 class Request(BaseModel):
     """
     Request
     """ # noqa: E501
     id: StrictInt
     name: StrictStr
-    resource_type: Optional[ResourceTypeEnum] = None
+    resource_type: ResourceTypeEnum
     description: Optional[StrictStr] = None
     org_id: Optional[StrictInt] = None
     user_id: Optional[StrictInt] = None
     status: Optional[RequestStatusEnum] = None
     error: Optional[StrictStr] = None
-    requested_ts: Optional[Union[StrictFloat, StrictInt]] = 1.7165935024421928E9
+    requested_ts: Optional[Union[StrictFloat, StrictInt]] = 1.7167362329035609E9
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
-            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 1.7165935024421928E9,
+            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 1.7167362329035609E9,
             "started_ts": obj.get("started_ts"),
             "failed_ts": obj.get("failed_ts"),
             "completed_ts": obj.get("completed_ts"),
             "notes": obj.get("notes"),
             "data": obj.get("data")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/request_status_enum.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/request_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/resource_type_enum.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/role_enum.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/service.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/service_create.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/service_list.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class ServiceList(BaseModel):
     """
     ServiceList
     """ # noqa: E501
     count: StrictInt
-    timestamp: Optional[StrictStr] = '2024-05-24T17:31:42.444659'
+    timestamp: Optional[StrictStr] = '2024-05-26T09:10:32.907072'
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
-            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else '2024-05-24T17:31:42.444659',
+            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else '2024-05-26T09:10:32.907072',
             "results": [Service.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/service_status_enum.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/service_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/status_enum_input.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/status_enum_input.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/subscription_model_enum.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/subscription_model_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/token_response.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/token_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/user.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/user.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/user_preferences.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/user_preferences.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/user_role_enum.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/user_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/validation_error.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/models/validation_error_loc_inner.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/models/validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client/rest.py` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client/rest.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/ambient_backend_api_client.egg-info/SOURCES.txt` & `ambient_backend_api_client-0.1.8/ambient_backend_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/pyproject.toml` & `ambient_backend_api_client-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/setup.py` & `ambient_backend_api_client-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "ambient_backend_api_client"
-VERSION = "0.1.7"
+VERSION = "0.1.8"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "aiohttp >= 3.0.0",
     "aiohttp-retry >= 2.8.3",
     "pydantic >= 2",
```

### Comparing `ambient_backend_api_client-0.1.7/test/test_account_type.py` & `ambient_backend_api_client-0.1.8/test/test_account_type.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_ambient_action_enum.py` & `ambient_backend_api_client-0.1.8/test/test_ambient_action_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_ambient_event_type_enum.py` & `ambient_backend_api_client-0.1.8/test/test_ambient_event_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_architecture_enum.py` & `ambient_backend_api_client-0.1.8/test/test_architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_auth0_device_code_response.py` & `ambient_backend_api_client-0.1.8/test/test_auth0_device_code_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_cluster.py` & `ambient_backend_api_client-0.1.8/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_cluster_create.py` & `ambient_backend_api_client-0.1.8/test/test_cluster_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_clusters_api.py` & `ambient_backend_api_client-0.1.8/test/test_clusters_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_create_service_acct_request.py` & `ambient_backend_api_client-0.1.8/test/test_create_service_acct_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_creation_method.py` & `ambient_backend_api_client-0.1.8/test/test_creation_method.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_event.py` & `ambient_backend_api_client-0.1.8/test/test_event.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_event_label.py` & `ambient_backend_api_client-0.1.8/test/test_event_label.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_event_template.py` & `ambient_backend_api_client-0.1.8/test/test_event_template.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_health_api.py` & `ambient_backend_api_client-0.1.8/test/test_health_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_http_validation_error.py` & `ambient_backend_api_client-0.1.8/test/test_http_validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_interface_type_enum.py` & `ambient_backend_api_client-0.1.8/test/test_interface_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_list_results_response.py` & `ambient_backend_api_client-0.1.8/test/test_list_results_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_models_cluster_status_enum.py` & `ambient_backend_api_client-0.1.8/test/test_models_cluster_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_models_node_status_enum.py` & `ambient_backend_api_client-0.1.8/test/test_models_node_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_network_interface.py` & `ambient_backend_api_client-0.1.8/test/test_network_interface.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_node.py` & `ambient_backend_api_client-0.1.8/test/test_node.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_node_architecture_enum.py` & `ambient_backend_api_client-0.1.8/test/test_node_architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_node_create.py` & `ambient_backend_api_client-0.1.8/test/test_node_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_node_role_enum.py` & `ambient_backend_api_client-0.1.8/test/test_node_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_nodes_api.py` & `ambient_backend_api_client-0.1.8/test/test_nodes_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_notification.py` & `ambient_backend_api_client-0.1.8/test/test_notification.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_notification_list.py` & `ambient_backend_api_client-0.1.8/test/test_notification_list.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_notification_request.py` & `ambient_backend_api_client-0.1.8/test/test_notification_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_notification_severity_enum.py` & `ambient_backend_api_client-0.1.8/test/test_notification_severity_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_notifications_api.py` & `ambient_backend_api_client-0.1.8/test/test_notifications_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_organization_create.py` & `ambient_backend_api_client-0.1.8/test/test_organization_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_owner_type_enum.py` & `ambient_backend_api_client-0.1.8/test/test_owner_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_ping_api.py` & `ambient_backend_api_client-0.1.8/test/test_ping_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_post_clusters_response.py` & `ambient_backend_api_client-0.1.8/test/test_post_clusters_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_post_service_response.py` & `ambient_backend_api_client-0.1.8/test/test_post_service_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_request.py` & `ambient_backend_api_client-0.1.8/test/test_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_request_status_enum.py` & `ambient_backend_api_client-0.1.8/test/test_request_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_requests_api.py` & `ambient_backend_api_client-0.1.8/test/test_requests_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_resource_type_enum.py` & `ambient_backend_api_client-0.1.8/test/test_resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_role_enum.py` & `ambient_backend_api_client-0.1.8/test/test_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_service.py` & `ambient_backend_api_client-0.1.8/test/test_service.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_service_create.py` & `ambient_backend_api_client-0.1.8/test/test_service_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_service_list.py` & `ambient_backend_api_client-0.1.8/test/test_service_list.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_service_state.py` & `ambient_backend_api_client-0.1.8/test/test_service_state.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_service_status_enum.py` & `ambient_backend_api_client-0.1.8/test/test_service_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_services_api.py` & `ambient_backend_api_client-0.1.8/test/test_services_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_status_enum_input.py` & `ambient_backend_api_client-0.1.8/test/test_status_enum_input.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_subscription_model_enum.py` & `ambient_backend_api_client-0.1.8/test/test_subscription_model_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_token_response.py` & `ambient_backend_api_client-0.1.8/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_unimplemented_api.py` & `ambient_backend_api_client-0.1.8/test/test_unimplemented_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_user.py` & `ambient_backend_api_client-0.1.8/test/test_user.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_user_preferences.py` & `ambient_backend_api_client-0.1.8/test/test_user_preferences.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_user_role_enum.py` & `ambient_backend_api_client-0.1.8/test/test_user_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_users_api.py` & `ambient_backend_api_client-0.1.8/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_validation_error.py` & `ambient_backend_api_client-0.1.8/test/test_validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.7/test/test_validation_error_loc_inner.py` & `ambient_backend_api_client-0.1.8/test/test_validation_error_loc_inner.py`

 * *Files identical despite different names*

