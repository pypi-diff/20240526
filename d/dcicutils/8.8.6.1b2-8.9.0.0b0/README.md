# Comparing `tmp/dcicutils-8.8.6.1b2.tar.gz` & `tmp/dcicutils-8.9.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-8.8.6.1b2.tar", max compression
+gzip compressed data, was "dcicutils-8.9.0.0b0.tar", max compression
```

## Comparing `dcicutils-8.8.6.1b2.tar` & `dcicutils-8.9.0.0b0.tar`

### file list

```diff
@@ -1,79 +1,78 @@
--rw-r--r--   0        0        0     1102 2024-05-26 12:38:56.415778 dcicutils-8.8.6.1b2/LICENSE.txt
--rw-r--r--   0        0        0     1166 2024-05-26 12:38:56.415778 dcicutils-8.8.6.1b2/README.rst
--rw-r--r--   0        0        0        0 2024-05-26 12:38:56.415778 dcicutils-8.8.6.1b2/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2024-05-26 12:38:56.415778 dcicutils-8.8.6.1b2/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2024-05-26 12:38:56.415778 dcicutils-8.8.6.1b2/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    34669 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/bundle_utils.py
--rw-r--r--   0        0        0     3295 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/captured_output.py
--rw-r--r--   0        0        0    13786 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3955 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    25653 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11127 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     7626 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/data_readers.py
--rw-r--r--   0        0        0     3098 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/data_utils.py
--rw-r--r--   0        0        0    13499 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/datetime_utils.py
--rw-r--r--   0        0        0    69908 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    73123 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10916 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/file_utils.py
--rw-r--r--   0        0        0    10026 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    34149 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0     1583 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/http_utils.py
--rw-r--r--   0        0        0    11502 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    28151 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/lang_utils.py
--rw-r--r--   0        0        0      278 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/license_policies/c4-infrastructure.jsonc
--rw-r--r--   0        0        0      296 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/license_policies/c4-python-infrastructure.jsonc
--rw-r--r--   0        0        0     5790 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/license_policies/park-lab-common-server.jsonc
--rw-r--r--   0        0        0    18864 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/license_policies/park-lab-common.jsonc
--rw-r--r--   0        0        0     3260 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
--rw-r--r--   0        0        0      283 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/license_policies/park-lab-pipeline.jsonc
--rw-r--r--   0        0        0    46978 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/log_utils.py
--rw-r--r--   0        0        0   107690 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    15422 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/portal_object_utils.py
--rw-r--r--   0        0        0    33402 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/portal_utils.py
--rw-r--r--   0        0        0    19468 2024-05-26 12:38:56.419778 dcicutils-8.8.6.1b2/dcicutils/progress_bar.py
--rw-r--r--   0        0        0    31250 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20534 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   160208 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     7055 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28868 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    10095 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/schema_utils.py
--rw-r--r--   0        0        0    13889 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0     4184 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/scripts/run_license_checker.py
--rw-r--r--   0        0        0    29777 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/scripts/view_portal_object.py
--rw-r--r--   0        0        0    19745 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    33629 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/sheet_utils.py
--rw-r--r--   0        0        0    22961 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0    64493 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/structured_data.py
--rw-r--r--   0        0        0     2895 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/submitr/progress_constants.py
--rw-r--r--   0        0        0     3467 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/submitr/ref_lookup_strategy.py
--rw-r--r--   0        0        0     8082 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/task_utils.py
--rw-r--r--   0        0        0     2997 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/tmpfile_utils.py
--rw-r--r--   0        0        0     1769 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/trace_utils.py
--rw-r--r--   0        0        0    14797 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/validation_utils.py
--rw-r--r--   0        0        0     4343 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/variant_utils.py
--rw-r--r--   0        0        0     3265 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/dcicutils/zip_utils.py
--rw-r--r--   0        0        0     4730 2024-05-26 12:38:56.423778 dcicutils-8.8.6.1b2/pyproject.toml
--rw-r--r--   0        0        0     3439 1970-01-01 00:00:00.000000 dcicutils-8.8.6.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/README.rst
+-rw-r--r--   0        0        0        0 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    34669 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/bundle_utils.py
+-rw-r--r--   0        0        0     3295 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/captured_output.py
+-rw-r--r--   0        0        0    13786 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3955 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    25653 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     7626 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/data_readers.py
+-rw-r--r--   0        0        0     3098 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    13499 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/datetime_utils.py
+-rw-r--r--   0        0        0    69908 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    72972 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0     2663 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/file_utils.py
+-rw-r--r--   0        0        0    10026 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    34149 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    28151 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0      278 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/license_policies/c4-infrastructure.jsonc
+-rw-r--r--   0        0        0      296 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/license_policies/c4-python-infrastructure.jsonc
+-rw-r--r--   0        0        0     5790 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/license_policies/park-lab-common-server.jsonc
+-rw-r--r--   0        0        0    18864 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/license_policies/park-lab-common.jsonc
+-rw-r--r--   0        0        0     3260 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
+-rw-r--r--   0        0        0      283 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/license_policies/park-lab-pipeline.jsonc
+-rw-r--r--   0        0        0    46978 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/log_utils.py
+-rw-r--r--   0        0        0   104610 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    15422 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/portal_object_utils.py
+-rw-r--r--   0        0        0    30779 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/portal_utils.py
+-rw-r--r--   0        0        0    19468 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/progress_bar.py
+-rw-r--r--   0        0        0    31250 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20534 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   160208 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     7055 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28868 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    10605 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/schema_utils.py
+-rw-r--r--   0        0        0    13889 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0     4184 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/scripts/run_license_checker.py
+-rw-r--r--   0        0        0    26262 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/scripts/view_portal_object.py
+-rw-r--r--   0        0        0    19745 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    33629 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/sheet_utils.py
+-rw-r--r--   0        0        0    22961 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0    61238 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/structured_data.py
+-rw-r--r--   0        0        0     2895 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/submitr/progress_constants.py
+-rw-r--r--   0        0        0     3467 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/submitr/ref_lookup_strategy.py
+-rw-r--r--   0        0        0     8082 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1403 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/tmpfile_utils.py
+-rw-r--r--   0        0        0     1769 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0    14797 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/validation_utils.py
+-rw-r--r--   0        0        0     4343 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/variant_utils.py
+-rw-r--r--   0        0        0     2027 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/zip_utils.py
+-rw-r--r--   0        0        0     4689 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.9.0.0b0/PKG-INFO
```

### Comparing `dcicutils-8.8.6.1b2/LICENSE.txt` & `dcicutils-8.9.0.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/README.rst` & `dcicutils-8.9.0.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/base.py` & `dcicutils-8.9.0.0b0/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/beanstalk_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/bundle_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/captured_output.py` & `dcicutils-8.9.0.0b0/dcicutils/captured_output.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/cloudformation_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/codebuild_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/command_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/common.py` & `dcicutils-8.9.0.0b0/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/contribution_scripts.py` & `dcicutils-8.9.0.0b0/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/contribution_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/contribution_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/creds_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/creds_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         """
         def _register_class(key_manager_class):
             assert issubclass(key_manager_class, KeyManager)
             if name in _KEY_MANAGERS:
                 raise ValueError(f"A KeyManager named {name!r} has already been defined.")
             key_manager_class._init_class_variables()
             key_manager_class._REGISTERED = True
-            _KEY_MANAGERS[name] = key_manager_class
+            _KEY_MANAGERS[name] = cls
             return key_manager_class
         return _register_class
 
     @classmethod
     def _init_class_variables(cls):
         class_name = cls.__name__
         # print(f"cls={cls!r}, name={class_name!r}")
```

### Comparing `dcicutils-8.8.6.1b2/dcicutils/data_readers.py` & `dcicutils-8.9.0.0b0/dcicutils/data_readers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/data_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/datetime_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/deployment_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/diff_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/docker_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/ecr_scripts.py` & `dcicutils-8.9.0.0b0/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/ecr_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/ecs_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/env_base.py` & `dcicutils-8.9.0.0b0/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/env_manager.py` & `dcicutils-8.9.0.0b0/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/env_scripts.py` & `dcicutils-8.9.0.0b0/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/env_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/env_utils_legacy.py` & `dcicutils-8.9.0.0b0/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/es_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/exceptions.py` & `dcicutils-8.9.0.0b0/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/ff_mocks.py` & `dcicutils-8.9.0.0b0/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/ff_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/ff_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -891,20 +891,17 @@
 
 def _get_es_metadata(uuids, es_client, filters, sources, chunk_size, auth):
     """
     Internal function needed because there are multiple levels of iteration
     used to create the generator.
     Should NOT be used directly
     """
-    def get_es_host_local() -> Optional[str]:
-        return os.environ.get("ES_HOST_LOCAL", None)
     health = get_health_page(key=auth)
     if es_client is None:
-        if not (es_url := get_es_host_local()):
-            es_url = health['elasticsearch']
+        es_url = health['elasticsearch']
         es_client = es_utils.create_es_client(es_url, use_aws_auth=True)
     namespace_star = health.get('namespace', '') + '*'
     # match all given uuids to _id fields
     # sending in too many uuids in the terms query can crash es; break them up
     # into groups of max size 100
     for i in range(0, len(uuids), chunk_size):
         query_uuids = uuids[i:i + chunk_size]
```

### Comparing `dcicutils-8.8.6.1b2/dcicutils/function_cache_decorator.py` & `dcicutils-8.9.0.0b0/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/glacier_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/jh_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/kibana/dashboards.json` & `dcicutils-8.9.0.0b0/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/kibana/readme.md` & `dcicutils-8.9.0.0b0/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/lang_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/license_policies/park-lab-common-server.jsonc` & `dcicutils-8.9.0.0b0/dcicutils/license_policies/park-lab-common-server.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/license_policies/park-lab-common.jsonc` & `dcicutils-8.9.0.0b0/dcicutils/license_policies/park-lab-common.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc` & `dcicutils-8.9.0.0b0/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/license_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/license_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/log_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/misc_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/misc_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 """
 This file contains functions that might be generally useful.
 """
 
 from collections import namedtuple
-import appdirs
 import contextlib
 import datetime
 import functools
 import hashlib
 import inspect
 import io
 import json
 import logging
 import math
 import os
-import platform
 import pytz
 import re
 import rfc3986.validators
 import rfc3986.exceptions
-import shortuuid
 import time
 import uuid
 import warnings
 import webtest  # importing the library makes it easier to mock testing
 
 from collections import defaultdict
 from datetime import datetime as datetime_type
@@ -1151,39 +1148,27 @@
         else:
             return text
     return text[:len(text)-len(suffix)]
 
 
 def remove_empty_properties(data: Optional[Union[list, dict]],
                             isempty: Optional[Callable] = None,
-                            isempty_array_element: Optional[Callable] = None,
-                            raise_exception_on_nonempty_array_element_after_empty: bool = False) -> None:
+                            isempty_array_element: Optional[Callable] = None) -> None:
     def _isempty(value: Any) -> bool:  # noqa
         return isempty(value) if callable(isempty) else value in [None, "", {}, []]
     if isinstance(data, dict):
         for key in list(data.keys()):
             if _isempty(value := data[key]):
                 del data[key]
             else:
-                remove_empty_properties(value, isempty=isempty, isempty_array_element=isempty_array_element,
-                                        raise_exception_on_nonempty_array_element_after_empty=  # noqa
-                                        raise_exception_on_nonempty_array_element_after_empty)
+                remove_empty_properties(value, isempty=isempty, isempty_array_element=isempty_array_element)
     elif isinstance(data, list):
         for item in data:
-            remove_empty_properties(item, isempty=isempty, isempty_array_element=isempty_array_element,
-                                    raise_exception_on_nonempty_array_element_after_empty=  # noqa
-                                    raise_exception_on_nonempty_array_element_after_empty)
+            remove_empty_properties(item, isempty=isempty, isempty_array_element=isempty_array_element)
         if callable(isempty_array_element):
-            if raise_exception_on_nonempty_array_element_after_empty is True:
-                empty_element_seen = False
-                for item in data:
-                    if not empty_element_seen and isempty_array_element(item):
-                        empty_element_seen = True
-                    elif empty_element_seen and not isempty_array_element(item):
-                        raise Exception("Non-empty element found after empty element.")
             data[:] = [item for item in data if not isempty_array_element(item)]
 
 
 class ObsoleteError(Exception):
     pass
 
 
@@ -1533,15 +1518,15 @@
         i -= 1
     return list_or_tuple[:i + 1]
 
 
 def create_dict(**kwargs) -> dict:
     result = {}
     for name in kwargs:
-        if not (kwargs[name] is None):
+        if kwargs[name]:
             result[name] = kwargs[name]
     return result
 
 
 def create_readonly_object(**kwargs):
     """
     Returns a new/unique object instance with readonly properties equal to the give kwargs.
@@ -2559,27 +2544,14 @@
     """
     Returns the given string with multiple consecutive occurrences of whitespace
     converted to a single space, and left and right trimmed of spaces.
     """
     return re.sub(r"\s+", " ", value).strip()
 
 
-def normalize_string(value: Optional[str]) -> Optional[str]:
-    """
-    Strips leading/trailing spaces, and converts multiple consecutive spaces to a single space
-    in the given string value and returns the result. If the given value is None returns an
-    empty string. If the given value is not actually even a string then return None.
-    """
-    if value is None:
-        return ""
-    elif isinstance(value, str):
-        return re.sub(r"\s+", " ", value).strip()
-    return None
-
-
 def find_nth_from_end(string: str, substring: str, nth: int) -> int:
     """
     Returns the index of the nth occurrence of the given substring within
     the given string from the END of the given string; or -1 if not found.
     """
     index = -1
     string = string[::-1]
@@ -2614,19 +2586,15 @@
     while abs(nbytes) >= ONE_K and index < MAX_UNITS_INDEX:
         nbytes /= ONE_K
         index += 1
     if index == 0:
         nbytes = int(nbytes)
         return f"{nbytes} byte{'s' if nbytes != 1 else ''}"
     unit = (UNITS_TERSE if terse else UNITS)[index]
-    size = f"{nbytes:.{precision}f}"
-    if size.endswith(f".{'0' * precision}"):
-        # Tidy up extraneous zeros.
-        size = size[:-(precision - 1)]
-    return f"{size}{'' if nospace else ' '}{unit}"
+    return f"{nbytes:.{precision}f}{'' if nospace else ' '}{unit}"
 
 
 def format_duration(seconds: Union[int, float]) -> str:
     seconds_actual = seconds
     seconds = round(max(seconds, 0))
     durations = [("year", 31536000), ("day", 86400), ("hour", 3600), ("minute", 60), ("second", 1)]
     parts = []
@@ -2698,52 +2666,7 @@
                 if self.padded and len(line) < n_headers:
                     line = pad_to(n_headers, line, padding=self.padding)
                 yield dict(zip(self.headers, line))
             elif isinstance(line, dict):
                 yield line
             else:
                 raise Exception(f"If the first line is not a list, all lines must be dictionaries: {line!r}")
-
-
-def get_app_specific_directory() -> str:
-    """
-    Returns the standard system application specific directory:
-    - On MacOS this directory: is: ~/Library/Application Support
-    - On Linux this directory is: ~/.local/share
-    - On Windows this directory is: %USERPROFILE%\\AppData\\Local  # noqa
-    N.B. This is has been tested on MacOS and Linux but not on Windows.
-    """
-    return appdirs.user_data_dir()
-
-
-def get_os_name() -> str:
-    if os_name := platform.system():
-        if os_name == "Darwin": return "osx"  # noqa
-        elif os_name == "Linux": return "linux"  # noqa
-        elif os_name == "Windows": return "windows"  # noqa
-    return ""
-
-
-def get_cpu_architecture_name() -> str:
-    if os_architecture_name := platform.machine():
-        if os_architecture_name == "x86_64": return "amd64"  # noqa
-        return os_architecture_name
-    return ""
-
-
-def create_uuid(nodash: bool = False, upper: bool = False) -> str:
-    value = str(uuid.uuid4())
-    if nodash is True:
-        value = value.replace("-", "")
-    if upper is True:
-        value = value.upper()
-    return value
-
-
-def create_short_uuid(length: Optional[int] = None, upper: bool = False):
-    # Not really techincally a uuid of course.
-    if (length is None) or (not isinstance(length, int)) or (length < 1):
-        length = 16
-    value = shortuuid.ShortUUID().random(length=length)
-    if upper is True:
-        value = value.upper()
-    return value
```

### Comparing `dcicutils-8.8.6.1b2/dcicutils/obfuscation_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/opensearch_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/portal_object_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/portal_object_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/portal_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/portal_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from collections import deque
 from functools import lru_cache
-from dcicutils.function_cache_decorator import function_cache
 import io
 import json
 from pyramid.config import Configurator as PyramidConfigurator
 from pyramid.paster import get_app as pyramid_get_app
 from pyramid.response import Response as PyramidResponse
 from pyramid.router import Router as PyramidRouter
 import os
@@ -15,15 +14,14 @@
 from typing import Callable, Dict, List, Optional, Tuple, Type, Union
 from uuid import uuid4 as uuid
 from webtest.app import TestApp, TestResponse
 from wsgiref.simple_server import make_server as wsgi_make_server
 from dcicutils.common import APP_SMAHT, OrchestratedApp, ORCHESTRATED_APPS
 from dcicutils.ff_utils import get_metadata, get_schema, patch_metadata, post_metadata
 from dcicutils.misc_utils import to_camel_case, VirtualApp
-from dcicutils.schema_utils import get_identifying_properties
 from dcicutils.tmpfile_utils import temporary_file
 
 Portal = Type["Portal"]  # Forward type reference for type hints.
 OptionalResponse = Optional[Union[Response, TestResponse]]
 
 
 class Portal:
@@ -414,62 +412,14 @@
 
     @lru_cache(maxsize=100)
     def get_schema_subtype_names(self, type_name: str) -> List[str]:
         if not (schemas_super_type_map := self.get_schemas_super_type_map()):
             return []
         return schemas_super_type_map.get(type_name, [])
 
-    @function_cache(maxsize=100, serialize_key=True)
-    def get_identifying_paths(self, portal_object: dict, portal_type: Optional[str] = None) -> List[str]:
-        """
-        Returns the list of the identifying Portal (URL) paths for the given Portal object. Favors any
-        uuid based path and defavors aliases based paths (ala self.get_identifying_property_names);
-        no other ordering defined. Returns empty list of none or otherwise not found.
-        """
-        results = []
-        if not isinstance(portal_object, dict):
-            return results
-        if not isinstance(portal_type, str) or not portal_type:
-            if not (portal_type := self.get_schema_type(portal_object)):
-                return results
-        for identifying_property in self.get_identifying_property_names(portal_type):
-            if identifying_value := portal_object.get(identifying_property):
-                if isinstance(identifying_value, list):
-                    for identifying_value_item in identifying_value:
-                        results.append(f"/{portal_type}/{identifying_value_item}")
-                elif identifying_property == "uuid":
-                    results.append(f"/{identifying_value}")
-                else:
-                    results.append(f"/{portal_type}/{identifying_value}")
-        return results
-
-    @function_cache(maxsize=100, serialize_key=True)
-    def get_identifying_property_names(self, schema: Union[str, dict]) -> List[str]:
-        """
-        Returns the list of identifying property names for the given Portal schema, which may
-        be either a schema name or a schema object; empty list of none or otherwise not found.
-        """
-        results = []
-        if isinstance(schema, str):
-            try:
-                if not (schema := self.get_schema(schema)):
-                    return results
-            except Exception:
-                return results
-        elif not isinstance(schema, dict):
-            return results
-        if not (identifying_properties := get_identifying_properties(schema)):
-            return results
-        identifying_properties = [*identifying_properties]
-        for favored_identifying_property in reversed(["uuid", "identifier"]):
-            if favored_identifying_property in identifying_properties:
-                identifying_properties.remove(favored_identifying_property)
-                identifying_properties.insert(0, favored_identifying_property)
-        return identifying_properties
-
     def url(self, url: str, raw: bool = False, database: bool = False) -> str:
         if not isinstance(url, str) or not url:
             return "/"
         elif (lowercase_url := url.lower()).startswith("http://") or lowercase_url.startswith("https://"):
             return url
         elif not (url := re.sub(r"/+", "/", url)).startswith("/"):
             url = "/"
@@ -563,30 +513,14 @@
                 def raise_for_status(self):  # noqa
                     if self.status_code < 200 or self.status_code > 399:
                         raise requests.exceptions.HTTPError(f"HTTP Error: {self.status_code}", response=self)
             response = TestResponseWrapper(response)
         return response
 
     @staticmethod
-    def _create_vapp(arg: Union[TestApp, VirtualApp, PyramidRouter, str] = None) -> TestApp:
-        if isinstance(arg, TestApp):
-            return arg
-        elif isinstance(arg, VirtualApp):
-            if not isinstance(arg.wrapped_app, TestApp):
-                raise Exception("Portal._create_vapp VirtualApp argument error.")
-            return arg.wrapped_app
-        if isinstance(arg, PyramidRouter):
-            router = arg
-        elif isinstance(arg, str) or not arg:
-            router = pyramid_get_app(arg or "development.ini", "app")
-        else:
-            raise Exception("Portal._create_vapp argument error.")
-        return TestApp(router, {"HTTP_ACCEPT": Portal.MIME_TYPE_JSON, "REMOTE_USER": "TEST"})
-
-    @staticmethod
     def create_for_testing(arg: Optional[Union[str, bool, List[dict], dict, Callable]] = None) -> Portal:
         if isinstance(arg, list) or isinstance(arg, dict) or isinstance(arg, Callable):
             return Portal(Portal._create_router_for_testing(arg))
         elif isinstance(arg, str) and arg.endswith(".ini"):
             return Portal(arg)
         elif arg == "local" or arg is True:
             minimal_ini_for_testing = "\n".join([
@@ -610,14 +544,30 @@
             ])
         else:
             minimal_ini_for_testing = "[app:app]\nuse = egg:encoded\nsqlalchemy.url = postgresql://dummy\n"
         with temporary_file(content=minimal_ini_for_testing, suffix=".ini") as ini_file:
             return Portal(ini_file)
 
     @staticmethod
+    def _create_vapp(arg: Union[TestApp, VirtualApp, PyramidRouter, str] = None) -> TestApp:
+        if isinstance(arg, TestApp):
+            return arg
+        elif isinstance(arg, VirtualApp):
+            if not isinstance(arg.wrapped_app, TestApp):
+                raise Exception("Portal._create_vapp VirtualApp argument error.")
+            return arg.wrapped_app
+        if isinstance(arg, PyramidRouter):
+            router = arg
+        elif isinstance(arg, str) or not arg:
+            router = pyramid_get_app(arg or "development.ini", "app")
+        else:
+            raise Exception("Portal._create_vapp argument error.")
+        return TestApp(router, {"HTTP_ACCEPT": Portal.MIME_TYPE_JSON, "REMOTE_USER": "TEST"})
+
+    @staticmethod
     def _create_router_for_testing(endpoints: Optional[List[Dict[str, Union[str, Callable]]]] = None) -> PyramidRouter:
         if isinstance(endpoints, dict):
             endpoints = [endpoints]
         elif isinstance(endpoints, Callable):
             endpoints = [{"path": "/", "method": "GET", "function": endpoints}]
         if not isinstance(endpoints, list) or not endpoints:
             endpoints = [{"path": "/", "method": "GET", "function": lambda request: {"status": "OK"}}]
```

### Comparing `dcicutils-8.8.6.1b2/dcicutils/progress_bar.py` & `dcicutils-8.9.0.0b0/dcicutils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/project_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/qa_checkers.py` & `dcicutils-8.9.0.0b0/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/qa_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/redis_tools.py` & `dcicutils-8.9.0.0b0/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/redis_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/s3_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/schema_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/schema_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     REF = "$ref"
     REQUIRED = "required"
     STRING = "string"
     TYPE = "type"
 
 
 class EncodedSchemaConstants:
+    DESCRIPTION = "description"
     IDENTIFYING_PROPERTIES = "identifyingProperties"
     LINK_TO = "linkTo"
     MERGE_REF = "$merge"
     MIXIN_PROPERTIES = "mixinProperties"
     UNIQUE_KEY = "uniqueKey"
 
 
@@ -183,14 +184,29 @@
     return [
         get_format(one_of_schema)
         for one_of_schema in get_one_of(schema)
         if get_format(one_of_schema)
     ]
 
 
+def is_link(property_schema: Dict[str, Any]) -> bool:
+    """Is property schema a link?"""
+    return property_schema.get(SchemaConstants.LINK_TO, False)
+
+
+def get_enum(property_schema: Dict[str, Any]) -> List[str]:
+    """Return the enum of a property schema."""
+    return property_schema.get(SchemaConstants.ENUM, [])
+
+
+def get_description(schema: Dict[str, Any]) -> str:
+    """Return the description of a schema."""
+    return schema.get(SchemaConstants.DESCRIPTION, "")
+
+
 class Schema:
 
     def __init__(self, schema: dict, type: Optional[str] = None) -> None:
         self._data = schema if isinstance(schema, dict) else (schema.data if isinstance(schema, Schema) else {})
         self._type = ((type if isinstance(type, str) else "") or
                       Schema.type_name(self._data.get("title", "")) or
                       Schema.type_name(self._data.get("$id", "")))
```

### Comparing `dcicutils-8.8.6.1b2/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-8.9.0.0b0/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/scripts/run_license_checker.py` & `dcicutils-8.9.0.0b0/dcicutils/scripts/run_license_checker.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/scripts/view_portal_object.py` & `dcicutils-8.9.0.0b0/dcicutils/scripts/view_portal_object.py`

 * *Files 13% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 # Note that instead of a uuid you can also actually use a path, for example:
 #   view-local-object /file-formats/vcf_gz_tbi
 #
 # --------------------------------------------------------------------------------------------------
 
 import argparse
 from functools import lru_cache
-import io
 import json
 import pyperclip
 import os
 import sys
 from typing import Callable, List, Optional, Tuple
 import yaml
 from dcicutils.captured_output import captured_output, uncaptured_output
@@ -94,26 +93,19 @@
                         help=f"Application name (one of: smaht, cgap, fourfront).")
     parser.add_argument("--schema", action="store_true", required=False, default=False,
                         help="View named schema rather than object.")
     parser.add_argument("--all", action="store_true", required=False, default=False,
                         help="Include all properties for schema usage.")
     parser.add_argument("--raw", action="store_true", required=False, default=False, help="Raw output.")
     parser.add_argument("--tree", action="store_true", required=False, default=False, help="Tree output for schemas.")
-    parser.add_argument("--post", type=str, required=False, default=None,
-                        help="POST data of the main arg type with data from file specified with this option.")
-    parser.add_argument("--patch", type=str, required=False, default=None,
-                        help="PATCH data of the main arg type with data from file specified with this option.")
     parser.add_argument("--database", action="store_true", required=False, default=False,
                         help="Read from database output.")
-    parser.add_argument("--bool", action="store_true", required=False,
-                        default=False, help="Only return whether found or not.")
     parser.add_argument("--yaml", action="store_true", required=False, default=False, help="YAML output.")
     parser.add_argument("--copy", "-c", action="store_true", required=False, default=False,
                         help="Copy object data to clipboard.")
-    parser.add_argument("--indent", required=False, default=False, help="Indent output.", type=int)
     parser.add_argument("--details", action="store_true", required=False, default=False, help="Detailed output.")
     parser.add_argument("--more-details", action="store_true", required=False, default=False,
                         help="More detailed output.")
     parser.add_argument("--verbose", action="store_true", required=False, default=False, help="Verbose output.")
     parser.add_argument("--debug", action="store_true", required=False, default=False, help="Debugging output.")
     args = parser.parse_args()
 
@@ -155,26 +147,14 @@
             _print("Known File Formats: None")
         return
 
     if _is_maybe_schema_name(args.uuid):
         args.schema = True
 
     if args.schema:
-        if args.post:
-            if post_data := _read_json_from_file(args.post):
-                if args.verbose:
-                    _print(f"POSTing data from file ({args.post}) as type: {args.uuid}")
-                if isinstance(post_data, dict):
-                    post_data = [post_data]
-                elif not isinstance(post_data, list):
-                    _print(f"POST data neither list nor dictionary: {args.post}")
-                for item in post_data:
-                    portal.post_metadata(args.uuid, item)
-                if args.verbose:
-                    _print(f"Done POSTing data from file ({args.post}) as type: {args.uuid}")
         schema, schema_name = _get_schema(portal, args.uuid)
         if schema:
             if args.copy:
                 pyperclip.copy(json.dumps(schema, indent=4))
             if not args.raw:
                 if parent_schema_name := _get_parent_schema_name(schema):
                     if schema.get("isAbstract") is True:
@@ -182,58 +162,22 @@
                     else:
                         _print(f"{schema_name} | parent: {parent_schema_name}")
                 else:
                     _print(schema_name)
             _print_schema(schema, details=args.details, more_details=args.details,
                           all=args.all, raw=args.raw, raw_yaml=args.yaml)
             return
-    elif args.patch:
-        if patch_data := _read_json_from_file(args.patch):
-            if args.verbose:
-                _print(f"PATCHing data from file ({args.patch}) for object: {args.uuid}")
-            if isinstance(patch_data, dict):
-                patch_data = [patch_data]
-            elif not isinstance(patch_data, list):
-                _print(f"PATCH data neither list nor dictionary: {args.patch}")
-            for item in patch_data:
-                portal.patch_metadata(args.uuid, item)
-            if args.verbose:
-                _print(f"Done PATCHing data from file ({args.patch}) as type: {args.uuid}")
-            return
-        else:
-            _print(f"No PATCH data found in file: {args.patch}")
-            exit(1)
 
-    data = _get_portal_object(portal=portal, uuid=args.uuid, raw=args.raw,
-                              database=args.database, check=args.bool, verbose=args.verbose)
-    if args.bool:
-        if data:
-            _print(f"{args.uuid}: found")
-            exit(0)
-        else:
-            _print(f"{args.uuid}: not found")
-            exit(1)
+    data = _get_portal_object(portal=portal, uuid=args.uuid, raw=args.raw, database=args.database, verbose=args.verbose)
     if args.copy:
         pyperclip.copy(json.dumps(data, indent=4))
     if args.yaml:
         _print(yaml.dump(data))
     else:
-        if args.indent > 0:
-            _print(_format_json_with_indent(data, indent=args.indent))
-        else:
-            _print(json.dumps(data, default=str, indent=4))
-
-
-def _format_json_with_indent(value: dict, indent: int = 0) -> Optional[str]:
-    if isinstance(value, dict):
-        result = json.dumps(value, indent=4)
-        if indent > 0:
-            result = f"{indent * ' '}{result}"
-            result = result.replace("\n", f"\n{indent * ' '}")
-        return result
+        _print(json.dumps(data, default=str, indent=4))
 
 
 def _create_portal(ini: str, env: Optional[str] = None,
                    server: Optional[str] = None, app: Optional[str] = None,
                    verbose: bool = False, debug: bool = False) -> Portal:
     portal = None
     with captured_output(not debug):
@@ -250,41 +194,35 @@
                 _print(f"Portal ini file: {portal.ini_file}")
             if portal.server:
                 _print(f"Portal server: {portal.server}")
         return portal
 
 
 def _get_portal_object(portal: Portal, uuid: str,
-                       raw: bool = False, database: bool = False,
-                       check: bool = False, verbose: bool = False) -> dict:
+                       raw: bool = False, database: bool = False, verbose: bool = False) -> dict:
     response = None
     try:
         if not uuid.startswith("/"):
             path = f"/{uuid}"
         else:
             path = uuid
         response = portal.get(path, raw=raw, database=database)
     except Exception as e:
         if "404" in str(e) and "not found" in str(e).lower():
             _print(f"Portal object not found at {portal.server}: {uuid}")
             _exit()
         _exit(f"Exception getting Portal object from {portal.server}: {uuid}\n{get_error_message(e)}")
     if not response:
-        if check:
-            return None
         _exit(f"Null response getting Portal object from {portal.server}: {uuid}")
     if response.status_code not in [200, 307]:
         # TODO: Understand why the /me endpoint returns HTTP status code 307, which is only why we mention it above.
         _exit(f"Invalid status code ({response.status_code}) getting Portal object from {portal.server}: {uuid}")
     if not response.json:
         _exit(f"Invalid JSON getting Portal object: {uuid}")
-    response = response.json()
-    if raw:
-        response.pop("schema_version", None)
-    return response
+    return response.json()
 
 
 @lru_cache(maxsize=1)
 def _get_schemas(portal: Portal) -> Optional[dict]:
     return portal.get_schemas()
 
 
@@ -315,15 +253,14 @@
 
 
 def _print_schema_info(schema: dict, level: int = 0,
                        details: bool = False, more_details: bool = False, all: bool = False,
                        required: Optional[List[str]] = None) -> None:
     if not schema or not isinstance(schema, dict):
         return
-    identifying_properties = schema.get("identifyingProperties")
     if level == 0:
         if required_properties := schema.get("required"):
             _print("- required properties:")
             for required_property in sorted(list(set(required_properties))):
                 if not all and required_property in _SCHEMAS_IGNORE_PROPERTIES:
                     continue
                 if property_type := (info := schema.get("properties", {}).get(required_property, {})).get("type"):
@@ -442,16 +379,14 @@
                     if isinstance(property_type, list):
                         property_type = " or ".join(sorted(property_type))
                     suffix = ""
                     if (enumeration := property.get("enum")) is not None:
                         suffix += f" | enum"
                     if property_required:
                         suffix += f" | required"
-                    if property_name in (identifying_properties or []):
-                        suffix += f" | identifying"
                     if property.get("uniqueKey"):
                         suffix += f" | unique"
                     if pattern := property.get("pattern"):
                         suffix += f" | pattern: {pattern}"
                     if (format := property.get("format")) and (format != "uuid"):
                         suffix += f" | format: {format}"
                     if isinstance(any_of := property.get("anyOf"), list):
@@ -590,31 +525,14 @@
                 extension = branch if pointer == tee else space
                 yield from tree_generator(path, prefix=prefix+extension)
     print(first + ((name_of(root_name) if callable(name_of) else root_name) or "root"))
     for line in tree_generator(root_name, prefix="   "):
         print(line)
 
 
-def _read_json_from_file(file: str) -> Optional[dict]:
-    if not os.path.exists(file):
-        _print(f"Cannot find file: {file}")
-        exit(1)
-    try:
-        with io.open(file, "r") as f:
-            try:
-                return json.load(f)
-            except Exception:
-                _print(f"Cannot parse JSON in file: {file}")
-                exit(1)
-    except Exception as e:
-        print(e)
-        _print(f"Cannot open file: {file}")
-        exit(1)
-
-
 def _print(*args, **kwargs):
     with uncaptured_output():
         PRINT(*args, **kwargs)
     sys.stdout.flush()
 
 
 def _exit(message: Optional[str] = None) -> None:
```

### Comparing `dcicutils-8.8.6.1b2/dcicutils/secrets_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/sheet_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/sheet_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/snapshot_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/ssl_certificate_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/structured_data.py` & `dcicutils-8.9.0.0b0/dcicutils/structured_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,37 +49,34 @@
 
 
 class StructuredDataSet:
 
     def __init__(self, file: Optional[str] = None, portal: Optional[Union[VirtualApp, TestApp, Portal]] = None,
                  schemas: Optional[List[dict]] = None, autoadd: Optional[dict] = None,
                  order: Optional[List[str]] = None, prune: bool = True,
-                 remove_empty_objects_from_lists: bool = True,
                  ref_lookup_strategy: Optional[Callable] = None,
                  ref_lookup_nocache: bool = False,
-                 norefs: bool = False, merge: bool = False,
+                 norefs: bool = False,
                  progress: Optional[Callable] = None,
                  debug_sleep: Optional[str] = None) -> None:
         self._progress = progress if callable(progress) else None
         self._data = {}
         self._portal = Portal(portal, data=self._data, schemas=schemas,
                               ref_lookup_strategy=ref_lookup_strategy,
                               ref_lookup_nocache=ref_lookup_nocache) if portal else None
         self._ref_lookup_strategy = ref_lookup_strategy
         self._order = order
-        self._prune = prune is True
-        self._remove_empty_objects_from_lists = remove_empty_objects_from_lists is True
+        self._prune = prune
         self._warnings = {}
         self._errors = {}
         self._resolved_refs = set()
         self._validated = False
         self._nrows = 0
         self._autoadd_properties = autoadd if isinstance(autoadd, dict) and autoadd else None
         self._norefs = True if norefs is True else False
-        self._merge = True if merge is True else False
         self._debug_sleep = None
         if debug_sleep:
             try:
                 self._debug_sleep = float(debug_sleep)
             except Exception:
                 self._debug_sleep = None
         self.load_file(file) if file else None
@@ -92,24 +89,22 @@
     def portal(self) -> Optional[Portal]:
         return self._portal
 
     @staticmethod
     def load(file: str, portal: Optional[Union[VirtualApp, TestApp, Portal]] = None,
              schemas: Optional[List[dict]] = None, autoadd: Optional[dict] = None,
              order: Optional[List[str]] = None, prune: bool = True,
-             remove_empty_objects_from_lists: bool = True,
              ref_lookup_strategy: Optional[Callable] = None,
              ref_lookup_nocache: bool = False,
-             norefs: bool = False, merge: bool = False,
+             norefs: bool = False,
              progress: Optional[Callable] = None,
              debug_sleep: Optional[str] = None) -> StructuredDataSet:
         return StructuredDataSet(file=file, portal=portal, schemas=schemas, autoadd=autoadd, order=order, prune=prune,
-                                 remove_empty_objects_from_lists=remove_empty_objects_from_lists,
                                  ref_lookup_strategy=ref_lookup_strategy, ref_lookup_nocache=ref_lookup_nocache,
-                                 norefs=norefs, merge=merge, progress=progress, debug_sleep=debug_sleep)
+                                 norefs=norefs, progress=progress, debug_sleep=debug_sleep)
 
     def validate(self, force: bool = False) -> None:
         def data_without_deleted_properties(data: dict) -> dict:
             nonlocal self
             def isempty(value: Any) -> bool:  # noqa
                 if value == RowReader.CELL_DELETION_SENTINEL:
                     return True
@@ -347,31 +342,15 @@
                 PROGRESS.LOAD_COUNT_REFS_LOOKUP_CACHE_HIT: self.ref_lookup_cache_hit_count,
                 PROGRESS.LOAD_COUNT_REFS_EXISTS_CACHE_HIT: self.ref_exists_cache_hit_count,
                 PROGRESS.LOAD_COUNT_REFS_INVALID: self.ref_invalid_identifying_property_count
             })
 
     def _load_json_file(self, file: str) -> None:
         with open(file) as f:
-            item = json.load(f)
-            if ((schema_name_inferred_from_file_name := Schema.type_name(file)) and
-                (self._portal.get_schema(schema_name_inferred_from_file_name) is not None)):  # noqa
-                # If the JSON file name looks like a schema name then assume it
-                # contains an object or an array of object of that schema type.
-                if self._merge:
-                    item = self._merge_with_existing_portal_object(item, schema_name_inferred_from_file_name)
-                self._add(Schema.type_name(file), item)
-            elif isinstance(item, dict):
-                # Otherwise if the JSON file name does not look like a schema name then
-                # assume it a dictionary where each property is the name of a schema, and
-                # which (each property) contains a list of object of that schema type.
-                for schema_name in item:
-                    item = item[schema_name]
-                    if self._merge:
-                        item = self._merge_with_existing_portal_object(item, schema_name)
-                    self._add(schema_name, item)
+            self._add(Schema.type_name(file), json.load(f))
 
     def _load_reader(self, reader: RowReader, type_name: str) -> None:
         schema = None
         noschema = False
         structured_row_template = None
         for row in reader:
             self._nrows += 1
@@ -385,22 +364,15 @@
                     type_name = schema_name
                 structured_row_template = _StructuredRowTemplate(reader.header, schema)
             structured_row = structured_row_template.create_row()
             for column_name, value in row.items():
                 structured_row_template.set_value(structured_row, column_name, value, reader.file, reader.row_number)
                 if self._autoadd_properties:
                     self._add_properties(structured_row, self._autoadd_properties, schema)
-            # New merge functionality (2024-05-25).
-            if self._merge:
-                structured_row = self._merge_with_existing_portal_object(structured_row, schema_name)
-            if (prune_error := self._prune_structured_row(structured_row)) is not None:
-                self._note_error({"src": create_dict(type=schema_name, row=reader.row_number),
-                                  "error": prune_error}, "validation")
-            else:
-                self._add(type_name, structured_row)  # TODO: why type_name and not schema_name?
+            self._add(type_name, structured_row)
             if self._progress:
                 self._progress({
                     PROGRESS.LOAD_ITEM: self._nrows,
                     PROGRESS.LOAD_COUNT_REFS: self.ref_total_count,
                     PROGRESS.LOAD_COUNT_REFS_FOUND: self.ref_total_found_count,
                     PROGRESS.LOAD_COUNT_REFS_NOT_FOUND: self.ref_total_notfound_count,
                     PROGRESS.LOAD_COUNT_REFS_LOOKUP: self.ref_lookup_count,
@@ -409,50 +381,27 @@
                     PROGRESS.LOAD_COUNT_REFS_INVALID: self.ref_invalid_identifying_property_count
                 })
         self._note_warning(reader.warnings, "reader")
         if schema:
             self._note_error(schema._unresolved_refs, "ref")
             self._resolved_refs.update(schema._resolved_refs)
 
-    def _prune_structured_row(self, data: dict) -> Optional[str]:
-        if not self._prune:
-            return None
-        if not self._remove_empty_objects_from_lists:
-            remove_empty_properties(data)
-            return None
-        try:
-            remove_empty_properties(data, isempty_array_element=lambda element: element == {},
-                                    raise_exception_on_nonempty_array_element_after_empty=True)
-        except Exception as e:
-            return str(e)
-        return None
-
     def _add(self, type_name: str, data: Union[dict, List[dict]]) -> None:
+        if self._prune:
+            remove_empty_properties(data)
         if type_name in self._data:
             self._data[type_name].extend([data] if isinstance(data, dict) else data)
         else:
             self._data[type_name] = [data] if isinstance(data, dict) else data
 
     def _add_properties(self, structured_row: dict, properties: dict, schema: Optional[dict] = None) -> None:
         for name in properties:
             if name not in structured_row and (not schema or schema.data.get("properties", {}).get(name)):
                 structured_row[name] = properties[name]
 
-    def _merge_with_existing_portal_object(self, portal_object: dict, portal_type: str) -> dict:
-        """
-        Given a Portal object (presumably/in-practice from the given metadata), if there is
-        an existing Portal item, identified by the identifying properties for the given object,
-        then merges the given object into the existing one and returns the result; otherwise
-        just returns the given object. Note that the given object may be CHANGED in place.
-        """
-        for identifying_path in self._portal.get_identifying_paths(portal_object, portal_type):
-            if existing_portal_object := self._portal.get_metadata(identifying_path, raw=True):
-                return merge_objects(existing_portal_object, portal_object)
-        return portal_object
-
     def _is_ref_lookup_specified_type(ref_lookup_flags: int) -> bool:
         return (ref_lookup_flags &
                 Portal.LOOKUP_SPECIFIED_TYPE) == Portal.LOOKUP_SPECIFIED_TYPE
 
     def _is_ref_lookup_root(ref_lookup_flags: int) -> bool:
         return (ref_lookup_flags & Portal.LOOKUP_ROOT) == Portal.LOOKUP_ROOT
```

### Comparing `dcicutils-8.8.6.1b2/dcicutils/submitr/progress_constants.py` & `dcicutils-8.9.0.0b0/dcicutils/submitr/progress_constants.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/submitr/ref_lookup_strategy.py` & `dcicutils-8.9.0.0b0/dcicutils/submitr/ref_lookup_strategy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/task_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/trace_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/validation_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/variant_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/variant_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.6.1b2/dcicutils/zip_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/zip_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from contextlib import contextmanager
 from dcicutils.tmpfile_utils import temporary_directory, temporary_file
 import gzip
 import os
-import shutil
 import tarfile
-import tempfile
 from typing import List, Optional
 import zipfile
 
 
 @contextmanager
 def unpack_zip_file_to_temporary_directory(file: str) -> str:
     with temporary_directory() as tmp_directory_name:
@@ -43,32 +41,7 @@
     if (gz := file.endswith(".gz")) or file.endswith(".tgz"):  # The .tgz suffix is simply short for .tar.gz.
         with temporary_file(name=os.path.basename(file[:-3] if gz else file[:-4] + ".tar")) as tmp_file_name:
             with open(tmp_file_name, "wb") as outputf:
                 with gzip.open(file, "rb") as inputf:
                     outputf.write(inputf.read())
                     outputf.close()
                     yield tmp_file_name
-
-
-def extract_file_from_zip(zip_file: str, file_to_extract: str,
-                          destination_file: str, raise_exception: bool = True) -> bool:
-    """
-    Extracts from the given zip file, the given file to extract, writing it to the
-    given destination file. Returns True if all is well, otherwise False, or if the
-    raise_exception argument is True (the default), then raises and exception on error.
-    """
-    try:
-        if not (destination_directory := os.path.dirname(destination_file)):
-            destination_directory = os.getcwd()
-            destination_file = os.path.join(destination_directory, destination_file)
-        with tempfile.TemporaryDirectory() as tmp_directory_name:
-            with zipfile.ZipFile(zip_file, "r") as zipf:
-                if file_to_extract not in zipf.namelist():
-                    return False
-                zipf.extract(file_to_extract, path=tmp_directory_name)
-                os.makedirs(destination_directory, exist_ok=True)
-                shutil.move(os.path.join(tmp_directory_name, file_to_extract), destination_file)
-            return True
-    except Exception as e:
-        if raise_exception:
-            raise e
-    return False
```

### Comparing `dcicutils-8.8.6.1b2/pyproject.toml` & `dcicutils-8.9.0.0b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "8.8.6.1b2"
+version = "8.9.0.0b0"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
@@ -33,21 +33,20 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11'
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.13"
-boto3 = "^1.34.93"
-botocore = "^1.34.93"
+python = ">=3.8,<3.12"
+boto3 = "^1.28.57"
+botocore = "^1.31.57"
 # The DCIC portals (cgap-portal and fourfront) are very particular about which ElasticSearch version.
 # This value is intentionally pinned and must not be changed casually.
 elasticsearch = "7.13.4"
-appdirs = "^1.4.4"
 aws-requests-auth = ">=0.4.2,<1"
 chardet = "^5.2.0"
 docker = "^4.4.4"
 gitpython = "^3.1.2"
 jsonc-parser = "^1.1.5"
 jsonschema = "^4.19.0"
 openpyxl = "^3.1.2"
@@ -57,26 +56,25 @@
 pyramid = "1.10.4"
 pytz = ">=2020.4"
 redis = "^4.5.1"
 pyperclip = "^1.8.2"
 PyYAML = "^6.0.1"
 requests = "^2.21.0"
 rfc3986 = "^1.4.0"
-shortuuid = "^1.0.13"
 structlog = "^19.2.0"
 toml = ">=0.10.1,<1"
 tqdm = "^4.66.2"
 typing-extensions = ">=3.8"  # Fourfront uses 3.8
 urllib3 = "^1.26.6"
 webtest = "^2.0.34"
 
 
 [tool.poetry.dev-dependencies]
-boto3-stubs = "^1.34.93"
-botocore-stubs = "^1.34.93"
+boto3-stubs = "^1.28.57"
+botocore-stubs = "^1.31.57"
 coverage = ">=7.2.3"
 # Loaded manually in GA workflow for coverage because a dependency on 2to3
 # in its docopts dependency makes a problem for laoding it here in poetry. -kmp 7-Apr-2023
 # coveralls = ">=3.3.1"
 flake8 = ">=3.9.2"
 flaky = ">=3.7.0"
 pip-licenses = "^4.3.3"
```

### Comparing `dcicutils-8.8.6.1b2/PKG-INFO` & `dcicutils-8.9.0.0b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 8.8.6.1b2
+Version: 8.9.0.0b0
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
-Requires-Python: >=3.8,<3.13
+Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,18 +20,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database :: Database Engines/Servers
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
-Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: aws-requests-auth (>=0.4.2,<1)
-Requires-Dist: boto3 (>=1.34.93,<2.0.0)
-Requires-Dist: botocore (>=1.34.93,<2.0.0)
+Requires-Dist: boto3 (>=1.28.57,<2.0.0)
+Requires-Dist: botocore (>=1.31.57,<2.0.0)
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
 Requires-Dist: docker (>=4.4.4,<5.0.0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: jsonc-parser (>=1.1.5,<2.0.0)
 Requires-Dist: jsonschema (>=4.19.0,<5.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
@@ -39,15 +38,14 @@
 Requires-Dist: pyOpenSSL (>=23.1.1,<24.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: pyramid (==1.10.4)
 Requires-Dist: pytz (>=2020.4)
 Requires-Dist: redis (>=4.5.1,<5.0.0)
 Requires-Dist: requests (>=2.21.0,<3.0.0)
 Requires-Dist: rfc3986 (>=1.4.0,<2.0.0)
-Requires-Dist: shortuuid (>=1.0.13,<2.0.0)
 Requires-Dist: structlog (>=19.2.0,<20.0.0)
 Requires-Dist: toml (>=0.10.1,<1)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: typing-extensions (>=3.8)
 Requires-Dist: urllib3 (>=1.26.6,<2.0.0)
 Requires-Dist: webtest (>=2.0.34,<3.0.0)
 Project-URL: Repository, https://github.com/4dn-dcic/utils
```

