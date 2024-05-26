# Comparing `tmp/aligned-0.0.98.tar.gz` & `tmp/aligned-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligned-0.0.98.tar", max compression
+gzip compressed data, was "aligned-0.0.9a0.tar", max compression
```

## Comparing `aligned-0.0.98.tar` & `aligned-0.0.9a0.tar`

### file list

```diff
@@ -1,112 +1,73 @@
--rw-r--r--   0        0        0    11358 2024-05-26 17:23:12.496008 aligned-0.0.98/LICENSE
--rw-r--r--   0        0        0     9984 2024-05-26 17:23:12.496008 aligned-0.0.98/README.md
--rw-r--r--   0        0        0     2193 2024-05-26 17:23:12.496008 aligned-0.0.98/aligned/__init__.py
--rw-r--r--   0        0        0     1174 2024-05-26 17:23:12.496008 aligned-0.0.98/aligned/active_learning/job.py
--rw-r--r--   0        0        0     1906 2024-05-26 17:23:12.496008 aligned-0.0.98/aligned/active_learning/selection.py
--rw-r--r--   0        0        0     2202 2024-05-26 17:23:12.496008 aligned-0.0.98/aligned/active_learning/write_policy.py
--rw-r--r--   0        0        0     7485 2024-05-26 17:23:12.496008 aligned-0.0.98/aligned/checks.py
--rw-r--r--   0        0        0    10831 2024-05-26 17:23:12.496008 aligned-0.0.98/aligned/cli.py
--rw-r--r--   0        0        0    12133 2024-05-26 17:23:12.496008 aligned-0.0.98/aligned/compiler/aggregation_factory.py
--rw-r--r--   0        0        0    57199 2024-05-26 17:23:12.496008 aligned-0.0.98/aligned/compiler/feature_factory.py
--rw-r--r--   0        0        0    17497 2024-05-26 17:23:12.496008 aligned-0.0.98/aligned/compiler/model.py
--rw-r--r--   0        0        0     6557 2024-05-26 17:23:12.496008 aligned-0.0.98/aligned/compiler/repo_reader.py
--rw-r--r--   0        0        0      283 2024-05-26 17:23:12.496008 aligned-0.0.98/aligned/compiler/tests/features.py
--rw-r--r--   0        0        0      540 2024-05-26 17:23:12.496008 aligned-0.0.98/aligned/compiler/tests/test_repo_reader.py
--rw-r--r--   0        0        0    24833 2024-05-26 17:23:12.496008 aligned-0.0.98/aligned/compiler/transformation_factory.py
--rw-r--r--   0        0        0      829 2024-05-26 17:23:12.496008 aligned-0.0.98/aligned/compiler/vector_index_factory.py
--rw-r--r--   0        0        0     1224 2024-05-26 17:23:12.496008 aligned-0.0.98/aligned/data_file.py
--rw-r--r--   0        0        0        0 2024-05-26 17:23:12.496008 aligned-0.0.98/aligned/data_source/__init__.py
--rw-r--r--   0        0        0    40434 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/data_source/batch_data_source.py
--rw-r--r--   0        0        0     3232 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/data_source/model_predictor.py
--rw-r--r--   0        0        0     2836 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/data_source/stream_data_source.py
--rw-r--r--   0        0        0     1794 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/data_source/tests/test_batch_source.py
--rw-r--r--   0        0        0     6383 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/enricher.py
--rw-r--r--   0        0        0      669 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/exceptions.py
--rw-r--r--   0        0        0    11593 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/exposed_model/interface.py
--rw-r--r--   0        0        0     7474 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/exposed_model/mlflow.py
--rw-r--r--   0        0        0    14148 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/exposed_model/ollama.py
--rw-r--r--   0        0        0     4259 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/exposed_model/tests/test_model.py
--rw-r--r--   0        0        0     6099 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/feature_source.py
--rw-r--r--   0        0        0    69476 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/feature_store.py
--rw-r--r--   0        0        0      235 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/feature_view/__init__.py
--rw-r--r--   0        0        0     5301 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/feature_view/combined_view.py
--rw-r--r--   0        0        0    27991 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/feature_view/feature_view.py
--rw-r--r--   0        0        0      846 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/feature_view/tests/test_brest_cancer.py
--rw-r--r--   0        0        0     2830 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/feature_view/tests/test_brest_cancer_event_timestamp.py
--rw-r--r--   0        0        0      969 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/feature_view/tests/test_check_schema.py
--rw-r--r--   0        0        0     3183 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/feature_view/tests/test_combined_view.py
--rw-r--r--   0        0        0      737 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/feature_view/tests/test_custom_source.py
--rw-r--r--   0        0        0     2242 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/feature_view/tests/test_hidden_variable.py
--rw-r--r--   0        0        0     3982 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/feature_view/tests/test_joined_source.py
--rw-r--r--   0        0        0     1079 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/jobs/tests/test_combined_job.py
--rw-r--r--   0        0        0     4983 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/jobs/tests/test_derived_job.py
--rw-r--r--   0        0        0        0 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/local/__init__.py
--rw-r--r--   0        0        0    20557 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/local/job.py
--rw-r--r--   0        0        0      817 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/local/tests/test_directory_interfaces.py
--rw-r--r--   0        0        0     1626 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/local/tests/test_jobs.py
--rw-r--r--   0        0        0        0 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/psql/__init__.py
--rw-r--r--   0        0        0    25143 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/psql/jobs.py
--rw-r--r--   0        0        0        0 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/redis/__init__.py
--rw-r--r--   0        0        0     4185 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/redis/job.py
--rw-r--r--   0        0        0     5232 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/redis/tests/test_redis_job.py
--rw-r--r--   0        0        0        0 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/redshift/__init__.py
--rw-r--r--   0        0        0    18626 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/redshift/jobs.py
--rw-r--r--   0        0        0     4749 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/redshift/sql_job.py
--rw-r--r--   0        0        0    18952 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/request/retrival_request.py
--rw-r--r--   0        0        0     1916 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/request/tests/test_feature_request_generation.py
--rw-r--r--   0        0        0    92197 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/retrival_job.py
--rw-r--r--   0        0        0        0 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/s3/__init__.py
--rw-r--r--   0        0        0     2018 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/s3/storage.py
--rw-r--r--   0        0        0      251 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/schemas/codable.py
--rw-r--r--   0        0        0      312 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/schemas/constraint_types.py
--rw-r--r--   0        0        0     3730 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/schemas/constraints.py
--rw-r--r--   0        0        0     3720 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/schemas/date_formatter.py
--rw-r--r--   0        0        0     3558 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/schemas/derivied_feature.py
--rw-r--r--   0        0        0     2745 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/schemas/event_trigger.py
--rw-r--r--   0        0        0    12057 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/schemas/feature.py
--rw-r--r--   0        0        0    16861 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/schemas/feature_view.py
--rw-r--r--   0        0        0    10179 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/schemas/folder.py
--rw-r--r--   0        0        0     3197 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/schemas/literal_value.py
--rw-r--r--   0        0        0     9445 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/schemas/model.py
--rw-r--r--   0        0        0     2207 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/schemas/record_coders.py
--rw-r--r--   0        0        0     7594 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/schemas/repo_definition.py
--rw-r--r--   0        0        0     1686 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/schemas/target.py
--rw-r--r--   0        0        0     8976 2024-05-26 17:23:12.500008 aligned-0.0.98/aligned/schemas/text_vectoriser.py
--rw-r--r--   0        0        0    70372 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/schemas/transformation.py
--rw-r--r--   0        0        0     2330 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/schemas/vector_storage.py
--rw-r--r--   0        0        0     9963 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/server.py
--rw-r--r--   0        0        0     1047 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/source_validation.py
--rw-r--r--   0        0        0        0 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/sources/__init__.py
--rw-r--r--   0        0        0    29061 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/sources/azure_blob_storage.py
--rw-r--r--   0        0        0     1125 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/sources/kafka.py
--rw-r--r--   0        0        0    32235 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/sources/local.py
--rw-r--r--   0        0        0     7407 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/sources/psql.py
--rw-r--r--   0        0        0    10451 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/sources/redis.py
--rw-r--r--   0        0        0     5021 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/sources/redshift.py
--rw-r--r--   0        0        0     8642 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/sources/s3.py
--rw-r--r--   0        0        0     8698 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/sources/tests/test_parquet.py
--rw-r--r--   0        0        0     4464 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/sources/tests/test_psql.py
--rw-r--r--   0        0        0     9894 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/split_strategy.py
--rw-r--r--   0        0        0      196 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/storage.py
--rw-r--r--   0        0        0        0 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/streams/__init__.py
--rw-r--r--   0        0        0     1037 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/streams/interface.py
--rw-r--r--   0        0        0      617 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/streams/kafka.py
--rw-r--r--   0        0        0     1641 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/streams/redis.py
--rw-r--r--   0        0        0      682 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/tests/test_cache_enricher.py
--rw-r--r--   0        0        0      623 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/tests/test_cached_parquet.py
--rw-r--r--   0        0        0     1628 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/tests/test_date_timezone_converter.py
--rw-r--r--   0        0        0     1767 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/tests/test_feature_view_wrapper.py
--rw-r--r--   0        0        0     2246 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/tests/test_filter_job_request.py
--rw-r--r--   0        0        0     6722 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/tests/test_model_target.py
--rw-r--r--   0        0        0     3355 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/tests/test_models_as_feature.py
--rw-r--r--   0        0        0     1506 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/tests/test_source_validation.py
--rw-r--r--   0        0        0     2057 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/tests/test_statistic_enricher.py
--rw-r--r--   0        0        0     3178 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/tests/test_timestamp_decoding.py
--rw-r--r--   0        0        0     3734 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/tests/test_train_test_validate_set.py
--rw-r--r--   0        0        0     5286 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/tests/test_transformations.py
--rw-r--r--   0        0        0      935 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/validation/interface.py
--rw-r--r--   0        0        0     2882 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/validation/pandera.py
--rw-r--r--   0        0        0     1464 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/validation/tests/test_pandera_validator.py
--rw-r--r--   0        0        0    12497 2024-05-26 17:23:12.504008 aligned-0.0.98/aligned/worker.py
--rw-r--r--   0        0        0     3227 2024-05-26 17:23:12.504008 aligned-0.0.98/pyproject.toml
--rw-r--r--   0        0        0    13042 1970-01-01 00:00:00.000000 aligned-0.0.98/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-01-03 20:34:00.544967 aligned-0.0.9a0/LICENSE
+-rw-r--r--   0        0        0     8521 2023-01-03 20:34:00.544967 aligned-0.0.9a0/README.md
+-rw-r--r--   0        0        0     1189 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/__init__.py
+-rw-r--r--   0        0        0    14066 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/cli.py
+-rw-r--r--   0        0        0      441 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/compiler/constraint_factory.py
+-rw-r--r--   0        0        0    19110 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/compiler/feature_factory.py
+-rw-r--r--   0        0        0     5784 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/compiler/repo_reader.py
+-rw-r--r--   0        0        0    18324 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/compiler/transformation_factory.py
+-rw-r--r--   0        0        0      822 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/data_file.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/data_source/__init__.py
+-rw-r--r--   0        0        0     3467 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/data_source/batch_data_source.py
+-rw-r--r--   0        0        0     1973 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/data_source/stream_data_source.py
+-rw-r--r--   0        0        0     8108 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/enricher.py
+-rw-r--r--   0        0        0      278 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/entity_data_source.py
+-rw-r--r--   0        0        0      341 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/exceptions.py
+-rw-r--r--   0        0        0     7657 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_source.py
+-rw-r--r--   0        0        0    17949 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_store.py
+-rw-r--r--   0        0        0      298 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/__init__.py
+-rw-r--r--   0        0        0     4969 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/combined_view.py
+-rw-r--r--   0        0        0    10029 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/feature_view.py
+-rw-r--r--   0        0        0      944 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/tests/test_brest_cancer.py
+-rw-r--r--   0        0        0     3135 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/tests/test_brest_cancer_event_timestamp.py
+-rw-r--r--   0        0        0     1239 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/tests/test_combined_view.py
+-rw-r--r--   0        0        0     1692 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/tests/test_hidden_variable.py
+-rw-r--r--   0        0        0     1074 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/jobs/tests/test_combined_job.py
+-rw-r--r--   0        0        0     1981 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/jobs/tests/test_derived_job.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/local/__init__.py
+-rw-r--r--   0        0        0     6962 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/local/job.py
+-rw-r--r--   0        0        0     8899 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/local/source.py
+-rw-r--r--   0        0        0     1105 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/local/tests/test_jobs.py
+-rw-r--r--   0        0        0     3006 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/model.py
+-rw-r--r--   0        0        0     2967 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/online_source.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/psql/__init__.py
+-rw-r--r--   0        0        0     4431 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/psql/data_source.py
+-rw-r--r--   0        0        0    10601 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/psql/jobs.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/__init__.py
+-rw-r--r--   0        0        0     4348 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/config.py
+-rw-r--r--   0        0        0     3288 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/job.py
+-rw-r--r--   0        0        0     2275 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/stream.py
+-rw-r--r--   0        0        0     4402 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/tests/test_redis_job.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redshift/__init__.py
+-rw-r--r--   0        0        0     2660 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redshift/data_source.py
+-rw-r--r--   0        0        0     1172 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redshift/factory.py
+-rw-r--r--   0        0        0     8250 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/request/retrival_request.py
+-rw-r--r--   0        0        0     1817 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/request/tests/test_feature_request_generation.py
+-rw-r--r--   0        0        0    15322 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/retrival_job.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/s3/__init__.py
+-rw-r--r--   0        0        0     5715 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/s3/config.py
+-rw-r--r--   0        0        0     1447 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/s3/factory.py
+-rw-r--r--   0        0        0     1846 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/s3/storage.py
+-rw-r--r--   0        0        0      251 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/codable.py
+-rw-r--r--   0        0        0     2356 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/constraints.py
+-rw-r--r--   0        0        0     1379 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/derivied_feature.py
+-rw-r--r--   0        0        0     3663 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/feature.py
+-rw-r--r--   0        0        0     8217 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/feature_view.py
+-rw-r--r--   0        0        0      409 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/model.py
+-rw-r--r--   0        0        0     4478 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/repo_definition.py
+-rw-r--r--   0        0        0    37245 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/transformation.py
+-rw-r--r--   0        0        0     8663 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/server.py
+-rw-r--r--   0        0        0     5086 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/split_strategy.py
+-rw-r--r--   0        0        0      196 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/storage.py
+-rw-r--r--   0        0        0      682 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_cache_enricher.py
+-rw-r--r--   0        0        0      549 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_cached_parquet.py
+-rw-r--r--   0        0        0     2056 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_statistic_enricher.py
+-rw-r--r--   0        0        0     2371 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_train_test_validate_set.py
+-rw-r--r--   0        0        0      905 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_transformations.py
+-rw-r--r--   0        0        0      193 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/validation/interface.py
+-rw-r--r--   0        0        0     2392 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/validation/pandera.py
+-rw-r--r--   0        0        0      848 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/validation/tests/test_pandera_validator.py
+-rw-r--r--   0        0        0     3846 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/worker.py
+-rw-r--r--   0        0        0     2553 2023-01-03 20:34:00.552967 aligned-0.0.9a0/pyproject.toml
+-rw-r--r--   0        0        0    10667 1970-01-01 00:00:00.000000 aligned-0.0.9a0/setup.py
+-rw-r--r--   0        0        0    10982 1970-01-01 00:00:00.000000 aligned-0.0.9a0/PKG-INFO
```

### Comparing `aligned-0.0.98/LICENSE` & `aligned-0.0.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aligned-0.0.98/aligned/cli.py` & `aligned-0.0.9a0/aligned/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,234 +1,127 @@
 import asyncio
 import logging
 import os
 import sys
-from contextlib import suppress
-from functools import wraps
+from dataclasses import dataclass
+from datetime import datetime
 from pathlib import Path
-from typing import Any
+from typing import Any, Coroutine
 
 import click
-import json
 from pytz import utc  # type: ignore
 
-from aligned.compiler.repo_reader import RepoReader, RepoReference
-from aligned.feature_store import ContractStore
-from aligned.worker import StreamWorker
-from collections.abc import Callable
-from datetime import datetime
-
+from aligned.compiler.repo_reader import RepoReader
+from aligned.feature_source import WritableFeatureSource
+from aligned.schemas.codable import Codable
+from aligned.schemas.feature import Feature
+from aligned.schemas.repo_definition import RepoDefinition
 
-def coro(func: Callable) -> Callable:
-    @wraps(func)
-    def wrapper(*args, **kwargs: Any) -> Any:
-        return asyncio.run(func(*args, **kwargs))
 
-    return wrapper
+def sync(method: Coroutine) -> Any:
+    return asyncio.get_event_loop().run_until_complete(method)
 
 
 def make_tzaware(t: datetime) -> datetime:
     """We assume tz-naive datetimes are UTC"""
     if t.tzinfo is None:
         return t.replace(tzinfo=utc)
     else:
         return t
 
 
 def load_envs(path: Path) -> None:
-    from dotenv import load_dotenv
-
-    if not load_dotenv(path):
-        click.echo(f'No env file found at {path}')
-
-
-def setup_logger():
-    from importlib.util import find_spec
-    from logging.config import dictConfig
-
-    handler = 'console'
-    log_format = '%(levelname)s:\t\b%(asctime)s %(name)s:%(lineno)d %(message)s'
-    configs = {
-        'version': 1,
-        'disable_existing_loggers': False,
-        'filters': {},
-        'formatters': {
-            'console': {'class': 'logging.Formatter', 'datefmt': '%H:%M:%S', 'format': log_format}
-        },
-        'handlers': {
-            'console': {
-                'class': 'logging.StreamHandler',
-                'filters': [],
-                'formatter': 'console',
-            }
-        },
-        'loggers': {
-            # project
-            '': {'handlers': [handler], 'level': 'INFO', 'propagate': True},
-        },
-    }
-
-    if find_spec('asgi_correlation_id'):
-        log_format = '%(levelname)s:\t\b%(asctime)s %(name)s:%(lineno)d [%(correlation_id)s] %(message)s'
-        configs['filters']['correlation_id'] = {
-            '()': 'asgi_correlation_id.CorrelationIdFilter',
-            'uuid_length': 16,
-        }
-        configs['handlers']['console']['filters'].append('correlation_id')
-        configs['formatters']['console']['format'] = log_format
-
-    dictConfig(configs)
-
+    if path.is_file():
+        import os
 
-async def store_from_reference(reference_file: str, dir: Path | None = None) -> ContractStore:
-    from aligned import FileSource
-
-    if dir is None:
-        dir = Path.cwd()
-
-    if ':' in reference_file:
-        path, obj = reference_file.split(':')
-        reference_file_path = Path(path).absolute()
-        repo_ref = RepoReference.reference_object(dir, reference_file_path, obj)
+        with path.open() as file:
+            for line in file:
+                if len(line) < 3:
+                    continue
+                key, value = line.strip().split('=')
+                os.environ[key] = value
     else:
-        repo_ref = RepoReference('const', {'const': FileSource.json_at(reference_file)})
-
-    if file := repo_ref.selected_file:
-        return await file.as_contract_store()
-    else:
-        raise ValueError(f'No repo file found at {dir}')
+        click.echo(f'No env file found at {path}')
 
 
 @click.group()
 def cli() -> None:
     pass
 
 
-@cli.command('compile')
-@coro
+@cli.command('apply')
 @click.option(
     '--repo-path',
     default='.',
     help='The path to the repo',
 )
 @click.option(
     '--reference-file',
-    default='contract_store.json',
-    help='The path to a contract store reference file. Defining where to read and write the feature store',
+    default='feature_store_location.py',
+    help='The path to a feature store reference file. Defining where to read and write the feature store',
 )
 @click.option(
     '--env-file',
     default='.env',
     help='The path to env variables',
 )
-@click.option('--ignore-file', default='.alignedignore', help='The files Aligned should ignore')
-async def compile(repo_path: str, reference_file: str, env_file: str, ignore_file: str) -> None:
+def apply_command(repo_path: str, reference_file: str, env_file: str) -> None:
     """
     Create or update a feature store deployment
     """
-    from aligned import FileSource
-
-    setup_logger()
 
     dir = Path.cwd() if repo_path == '.' else Path(repo_path).absolute()
-    ignore_path = dir / ignore_file
-
+    reference_file_path = Path(reference_file).absolute()
     load_envs(dir / env_file)
     sys.path.append(str(dir))
+    repo_ref = RepoReader.reference_from_path(dir, reference_file_path)
 
-    excludes = []
+    click.echo(f'Updating file at: {repo_ref.selected}')
 
-    if ignore_path.is_file():
-        excludes = ignore_path.read_text().split('\n')
+    # old_def = sync(repo_ref.selected_file.feature_store())
 
-    if ':' in reference_file:
-        path, obj = reference_file.split(':')
-        reference_file_path = Path(path).absolute()
-        repo_ref = RepoReference.reference_object(dir, reference_file_path, obj)
-    else:
-        repo_ref = RepoReference('const', {'const': FileSource.json_at(reference_file)})
+    repo_def = sync(RepoReader.definition_from_path(dir))
 
     if file := repo_ref.selected_file:
-        click.echo(f'Updating file at: {file}')
-
-        repo_def = await RepoReader.definition_from_path(dir, excludes)
-
-        await file.write(repo_def.to_json(omit_none=True).encode('utf-8'))
+        sync(file.write(repo_def.to_json(omit_none=True).encode('utf-8')))
     else:
         click.echo(f'No repo file found at {dir}')
 
 
-@cli.command('check-updates')
-@coro
-@click.option('--updated-contract')
-@click.option('--reference-contract')
-@click.option('--output-format', default='markdown', help='The output format')
-@click.option('--output-file', default=None, help='The output format')
-async def check_updates(
-    updated_contract: str,
-    reference_contract: str,
-    output_format: str,
-    output_file: str | None,
-):
+@cli.command('plan')
+@click.option(
+    '--repo-path',
+    default='.',
+    help='The path to the repo',
+)
+@click.option(
+    '--env-file',
+    default='.env',
+    help='The path to env variables',
+)
+def plan_command(repo_path: str, env_file: str) -> None:
     """
-    Check if the current changes conflicts with an existing contract store.
-
-    This will check if:
-
-    1. Exposed models have the needed features.
-    2. If any transformations that a model depend on have changed.
+    Prints the plan for updating the feature store file
     """
-    from aligned.checks import (
-        check_exposed_models_have_needed_features,
-        impacted_models_from_transformation_diffs,
-        check_exposed_models_for_potential_distribution_shift,
-        ContractStoreUpdateCheckReport,
-    )
-
-    as_markdown = output_format == 'markdown' or output_format == 'md'
 
-    new_contract_store = await store_from_reference(updated_contract)
-    old_contract_store = await store_from_reference(reference_contract)
-
-    checks = await check_exposed_models_have_needed_features(new_contract_store)
-    potential_drifts = await check_exposed_models_for_potential_distribution_shift(
-        old_contract_store, new_contract_store
-    )
-    transformation_changes = impacted_models_from_transformation_diffs(
-        new_store=new_contract_store, old_store=old_contract_store
-    )
-    not_ok_checks = [check for check in checks if not check.is_ok]
-
-    report = ContractStoreUpdateCheckReport(
-        needed_model_input=not_ok_checks,
-        potential_distribution_shifts=potential_drifts,
-        model_transformation_changes=transformation_changes,
-    )
-
-    if as_markdown:
-        output = report.as_markdown()
-    else:
-        output = json.dumps(report)
-
-    if output_file:
-        path = Path(output_file)
-        path.write_text(output)
-    else:
-        click.echo(output)
+    dir = Path.cwd() if repo_path == '.' else Path(repo_path).absolute()
+    sys.path.append(str(dir))
+    load_envs(dir / env_file)
+    click.echo(RepoReader.definition_from_path(dir))
 
 
 @cli.command('serve')
 @click.option(
     '--repo-path',
     default='.',
     help='The path to the repo',
 )
 @click.option(
     '--host',
-    default=None,
+    default='127.0.0.1',
     help='The host to serve on',
 )
 @click.option(
     '--port',
     '-p',
     default=8000,
     help='The port to serve on',
@@ -248,29 +141,55 @@
     '--reload',
     '-r',
     default=False,
     help='If the server should reload on dir changes',
 )
 @click.option(
     '--server-path',
-    default='server:server',
+    default='feature_store_location:feature_server',
     help='The path to the feature store server',
 )
 def serve_command(
-    repo_path: str, port: int, workers: int, env_file: str, reload: bool, server_path: str, host: str | None
+    repo_path: str, host: str, port: int, workers: int, env_file: str, reload: bool, server_path: str
 ) -> None:
     """
-    Starts an API serving data based on a contract store.
+    Starts a API serving the feature store
     """
-    import uvicorn
-
-    setup_logger()
+    from logging.config import dictConfig
 
-    host = host or os.getenv('HOST', '127.0.0.1')
+    import uvicorn
 
+    handler = 'console'
+    log_format = '%(levelname)s:\t\b%(asctime)s %(name)s:%(lineno)d [%(correlation_id)s] %(message)s'
+    dictConfig(
+        {
+            'version': 1,
+            'disable_existing_loggers': False,
+            'filters': {
+                'correlation_id': {
+                    '()': 'asgi_correlation_id.CorrelationIdFilter',
+                    'uuid_length': 16,
+                },
+            },
+            'formatters': {
+                'console': {'class': 'logging.Formatter', 'datefmt': '%H:%M:%S', 'format': log_format}
+            },
+            'handlers': {
+                'console': {
+                    'class': 'logging.StreamHandler',
+                    'filters': ['correlation_id'],
+                    'formatter': 'console',
+                }
+            },
+            'loggers': {
+                # project
+                '': {'handlers': [handler], 'level': 'INFO', 'propagate': True},
+            },
+        }
+    )
     os.environ['ALADDIN_ENABLE_SERVER'] = 'True'
     # Needed in order to find the feature_store_location file
     dir = Path.cwd() if repo_path == '.' else Path(repo_path).absolute()
     sys.path.append(str(dir))
     env_file_path = dir / env_file
     load_envs(env_file_path)
     uvicorn.run(
@@ -280,103 +199,262 @@
         workers=workers or workers,
         reload=reload,
         env_file=env_file_path,
     )
 
 
 @cli.command('serve-worker')
-@coro
 @click.option(
     '--repo-path',
     default='.',
     help='The path to the repo',
 )
 @click.option(
-    '--worker-path',
-    default='worker.py:worker',
-    help='The path to the `StreamWorker`',
+    '--reference-file',
+    default='feature_store_location.py',
+    help='The path to a feature store reference file. Defining where to read and write the feature store',
+)
+@click.option(
+    '--workers',
+    '-w',
+    default=1,
+    help='The number of workers',
 )
+@click.option('--views', '-v', help='The views to run in a worker', multiple=True)
 @click.option(
     '--env-file',
     default='.env',
     help='The path to env variables',
 )
-async def serve_worker_command(repo_path: str, worker_path: str, env_file: str) -> None:
+def serve_worker_command(
+    repo_path: str, reference_file: str, views: list[str], workers: int, env_file: str
+) -> None:
     """
-    Starts a worker that process the contract store streams and store them in an online source.
+    Starts a API serving the feature store
     """
-    setup_logger()
+    from logging.config import dictConfig
+
+    from aligned.worker import start
 
+    handler = 'console'
+    log_format = '%(levelname)s:\t\b%(asctime)s %(name)s:%(lineno)d [%(correlation_id)s] %(message)s'
+    dictConfig(
+        {
+            'version': 1,
+            'disable_existing_loggers': False,
+            'filters': {
+                'correlation_id': {
+                    '()': 'asgi_correlation_id.CorrelationIdFilter',
+                    'uuid_length': 16,
+                },
+            },
+            'formatters': {
+                'console': {'class': 'logging.Formatter', 'datefmt': '%H:%M:%S', 'format': log_format}
+            },
+            'handlers': {
+                'console': {
+                    'class': 'logging.StreamHandler',
+                    'filters': ['correlation_id'],
+                    'formatter': 'console',
+                }
+            },
+            'loggers': {
+                # project
+                '': {'handlers': [handler], 'level': 'INFO', 'propagate': True},
+            },
+        }
+    )
     # Needed in order to find the feature_store_location file
-    path, obj = worker_path.split(':')
     dir = Path.cwd() if repo_path == '.' else Path(repo_path).absolute()
-    reference_file_path = Path(path).absolute()
+    reference_file_path = Path(reference_file).absolute()
     sys.path.append(str(dir))
     env_file_path = dir / env_file
     load_envs(env_file_path)
 
-    worker = StreamWorker.from_object(dir, reference_file_path, obj)
+    repo_ref = RepoReader.reference_from_path(dir, reference_file_path)
 
-    await worker.start()
+    if not repo_ref.selected_file:
+        raise ValueError('No selected feature store in the repo reference. Make sure the env var is set')
+
+    feature_store = sync(repo_ref.selected_file.feature_store())
+
+    sync(start(store=feature_store, feature_views_to_process=set(views)))
+
+
+@cli.command('materialize')
+@click.option(
+    '--repo-path',
+    default='.',
+    help='The path to the repo',
+)
+@click.option(
+    '--env-file',
+    default='.env',
+    help='The path to env variables',
+)
+@click.option(
+    '--days',
+    help='The number of days to materialize',
+)
+@click.option(
+    '--view',
+    help='The feature view to materialize',
+)
+def materialize_command(repo_path: str, env_file: str, days: str, view: str) -> None:
+    """
+    Materializes the feature store
+    """
+    from aligned.feature_store import FeatureStore
 
+    dir = Path.cwd() if repo_path == '.' else Path(repo_path).absolute()
+    load_envs(dir / env_file)
 
-@cli.command('create-indexes')
-@coro
+    sys.path.append(str(dir))
+    repo_def = sync(RepoDefinition.from_path(repo_path))
+    store = FeatureStore.from_definition(repo_def)
+    batch_store = store.offline_store()
+
+    if not isinstance(store.feature_source, WritableFeatureSource):
+        raise ValueError('Batch feature sources are not supported for materialization')
+
+    number_of_days = int(days)
+    views = [view] if view else list(store.feature_views.keys())
+
+    click.echo(f'Materializing the last {number_of_days} days')
+    for feature_view in views:
+        fv_store = batch_store.feature_view(feature_view)
+        click.echo(f'Materializing {feature_view}')
+        sync(
+            store.feature_source.write(
+                fv_store.previous(days=number_of_days), fv_store.view.request_all.needed_requests
+            )
+        )
+
+
+@dataclass
+class CategoricalFeatureSummary(Codable):
+    missing_percentage: float
+    unique_values: int
+    values: list[str]
+    value_count: list[int]
+
+
+@dataclass
+class NumericFeatureSummary(Codable):
+    missing_percentage: float
+    mean: float | None
+    median: float | None
+    std: float | None
+    lowest: float | None
+    highests: float | None
+    histogram_count: list[int]
+    histogram_splits: list[float]
+
+
+@dataclass
+class ProfilingResult(Codable):
+    numeric_features: dict[str, NumericFeatureSummary]
+    categorical_features: dict[str, CategoricalFeatureSummary]
+
+
+# Should add some way of profiling models, not feature views.
+# Or maybe both
+@cli.command('profile')
 @click.option(
     '--repo-path',
     default='.',
     help='The path to the repo',
 )
 @click.option(
     '--reference-file',
-    default='feature_store_location.py:source',
-    help='The path to a feature store reference file. Defining where to read and write the feature store',
+    default='feature_store_location.py',
+    help='The file defining where to read the feature store from',
 )
+@click.option('--output', default='profiling-result.json')
+@click.option('--dataset-size', default=10000)
 @click.option(
     '--env-file',
     default='.env',
     help='The path to env variables',
 )
-async def create_indexes(repo_path: str, reference_file: str, env_file: str) -> None:
-    """
-    Creates a set of vector indexes for the contract store.
-    """
-    from aligned import ContractStore, FileSource
+def profile(repo_path: str, reference_file: str, env_file: str, output: str, dataset_size: int) -> None:
+    import numpy as np
+    from pandas import DataFrame
 
-    setup_logger()
+    from aligned import FeatureStore
 
     # Make sure modules can be read, and that the env is set
-    path, obj = reference_file.split(':')
     dir = Path.cwd() if repo_path == '.' else Path(repo_path).absolute()
-    reference_file_path = Path(path)
-
     sys.path.append(str(dir))
     env_file_path = dir / env_file
     load_envs(env_file_path)
 
-    repo_ref = RepoReference('const', {'const': FileSource.json_at('./feature-store.json')})
-    with suppress(ValueError):
-        repo_ref = RepoReference.reference_object(dir, reference_file_path, obj)
-
-    if file := repo_ref.selected_file:
-        click.echo(f'Updating file at: {file}')
-
-        repo_def = await RepoReader.definition_from_path(dir)
-    else:
-        click.echo(f'No repo file found at {dir}. Returning without creating indexes')
-        return
+    online_store: FeatureStore = sync(FeatureStore.from_reference_at_path(repo_path, reference_file))
+    feature_store = online_store.offline_store()
 
-    feature_store = ContractStore.from_definition(repo_def)
+    results = ProfilingResult(numeric_features={}, categorical_features={})
 
     for feature_view_name in sorted(feature_store.feature_views.keys()):
-        view = feature_store.feature_views[feature_view_name]
-        if view.indexes is None:
-            continue
-
-        for index in view.indexes:
-            click.echo(f'Creating indexes for: {feature_view_name}')
-            await index.storage.create_index(index)
+        click.echo(f'Profiling: {feature_view_name}')
+        feature_view = feature_store.feature_view(feature_view_name)
+        data_set: DataFrame = sync(feature_view.all(limit=dataset_size).to_pandas())
+
+        all_features: list[Feature] = list(feature_view.view.features) + list(
+            feature_view.view.derived_features
+        )
+        for feature in all_features:
+
+            data_slice = data_set[feature.name]
+
+            reference = f'{feature_view_name}:{feature.name}'
+
+            if (not feature.dtype.is_numeric) or feature.dtype.name == 'bool':
+                unique_values = data_slice.unique()
+                filter_unique_nan_values = [
+                    value
+                    for value in unique_values
+                    if not (
+                        str(value).lower() == 'nan' or str(value).lower() == 'nat' or str(value) == '<NA>'
+                    )
+                ]
+
+                results.categorical_features[reference] = CategoricalFeatureSummary(
+                    missing_percentage=(data_slice.isna() | data_slice.isnull()).sum() / data_slice.shape[0],
+                    unique_values=unique_values.shape[0],
+                    values=[str(value) for value in filter_unique_nan_values],
+                    value_count=data_slice.value_counts()[filter_unique_nan_values].tolist(),
+                )
+            else:
+                description = data_slice.describe()
+                n_bins = np.min([50, len(data_slice.unique())])
+                max_value = description['max']
+                min_value = description['min']
+
+                if np.isnan(max_value):
+                    continue
+
+                width = (max_value - min_value) / n_bins
+
+                if width <= 0:
+                    histogram = [description['count']]
+                    cuts = []
+                else:
+                    cuts = np.arange(start=min_value, stop=max_value + width, step=width)
+                    histogram, _ = np.histogram(data_slice.loc[~data_slice.isna()].values, cuts)
+
+                results.numeric_features[reference] = NumericFeatureSummary(
+                    missing_percentage=(data_slice.isna() | data_slice.isnull()).sum() / data_slice.shape[0],
+                    mean=description['mean'] if not np.isnan(description['mean']) else None,
+                    median=description['50%'] if not np.isnan(description['50%']) else None,
+                    std=description['std'] if not np.isnan(description['std']) else None,
+                    lowest=description['min'] if not np.isnan(description['min']) else None,
+                    highests=description['max'] if not np.isnan(description['max']) else None,
+                    histogram_count=list(histogram),
+                    histogram_splits=list(cuts),
+                )
+
+    Path(output).write_bytes(results.to_json().encode('utf-8'))
 
 
 if __name__ == '__main__':
     logging.basicConfig(level=logging.INFO, format='{asctime} {message}', style='{')
     cli()
```

### Comparing `aligned-0.0.98/aligned/compiler/repo_reader.py` & `aligned-0.0.9a0/aligned/compiler/repo_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import logging
-from datetime import datetime
 from importlib import import_module
 from inspect import getmro, isclass
+from pathlib import Path
 from typing import Any
-from aligned.compiler.model import ModelContractWrapper
 
 from aligned.enricher import Enricher
-from aligned.feature_view.combined_view import CombinedFeatureViewWrapper
-from aligned.feature_view.feature_view import FeatureViewWrapper
-from aligned.schemas.repo_definition import EnricherReference, RepoDefinition, RepoMetadata, RepoReference
-from pathlib import Path
-
+from aligned.model import Model
+from aligned.online_source import BatchOnlineSource, OnlineSource
+from aligned.schemas.repo_definition import EnricherReference, RepoDefinition, RepoReference
 
 logger = logging.getLogger(__name__)
 
 
 def imports_for(file_path: Path) -> set[str]:
     try:
         with open(file_path) as file:
@@ -49,108 +46,98 @@
     # Remove the class name. Only store the superclasses
     # Otherwise it might init a abstract class and crash
     s = str(obj).replace("'", '').replace('>', '')
     super_class_names.remove(s.split('.')[-1])
     return super_class_names
 
 
-def find_files(repo_path: Path, ignore_path: Path | None = None, file_extension: str = 'py') -> list[Path]:
+def python_files(repo_path: Path, ignore_path: Path | None = None) -> list[Path]:
     files = {
         path.resolve()
-        for path in repo_path.resolve().glob(f'**/*.{file_extension}')
-        if path.is_file()
-        and '__init__.py' != path.name
-        and not any(part.startswith('.') for part in path.parts)
+        for path in repo_path.resolve().glob('**/*.py')
+        if path.is_file() and '__init__.py' != path.name
     }
     if ignore_path:
         ignore_files = {
             path.resolve()
-            for path in ignore_path.glob(f'**/*.{file_extension}')
-            if path.is_file()
-            and '__init__.py' != path.name
-            and not any(part.startswith('.') for part in path.parts)
+            for path in ignore_path.glob('**/*.py')
+            if path.is_file() and '__init__.py' != path.name
         }
         files -= ignore_files
     return sorted(files)
 
 
 def path_to_py_module(path: Path, repo_root: Path) -> str:
-    return str(path.relative_to(repo_root.resolve()))[: -len('.py')].replace('./', '').replace('/', '.')
+    return str(path.relative_to(repo_root))[: -len('.py')].replace('./', '').replace('/', '.')
 
 
 class RepoReader:
     """
     A class reading a repo, and generates a repo config
     """
 
     @staticmethod
-    async def definition_from_path(repo_path: Path, excludes: list[str] | None = None) -> RepoDefinition:
-
-        excluded_files: list[Path] = []
-        for exclude in excludes or []:
-            excluded_files.extend(repo_path.resolve().glob(exclude))
-
-        metadata = RepoMetadata(created_at=datetime.now(), name=repo_path.name, github_url=None)
+    async def definition_from_path(repo_path: Path) -> RepoDefinition:
         repo = RepoDefinition(
-            metadata=metadata,
             feature_views=set(),
             combined_feature_views=set(),
             models=set(),
+            online_source=BatchOnlineSource(),
             enrichers=[],
         )
 
         feature_view_names: dict[str, str] = {}
 
-        for py_file in find_files(repo_path):
-            if py_file in excluded_files:
-                continue
-
+        for py_file in python_files(repo_path):
             imports = imports_for(py_file)
 
             module_path = path_to_py_module(py_file, repo_path)
-
-            if module_path.startswith('aladdin') or module_path.startswith('.') or module_path.endswith('__'):
-                # Skip no feature defintion modules
+            if (
+                module_path.startswith('aladdin')
+                or module_path.startswith('.')
+                or module_path.startswith('heroku')
+                or module_path.endswith('__')
+            ):
+                # Skip aladdin modules
                 continue
 
             module = import_module(module_path)
 
             for attribute in dir(module):
                 if attribute in imports:
                     continue
 
                 obj = getattr(module, attribute)
 
-                if isinstance(obj, Enricher):
+                if isinstance(obj, Model):
+                    if not obj.name:
+                        obj.name = attribute
+                    repo.models.add(obj.schema())
+
+                elif isinstance(obj, Enricher):
                     repo.enrichers.append(
                         EnricherReference(module=module_path, attribute_name=attribute, enricher=obj)
                     )
-                elif isinstance(obj, FeatureViewWrapper):
-                    repo.feature_views.add(obj.compile())
-                elif isinstance(obj, CombinedFeatureViewWrapper):
-                    repo.combined_feature_views.add(obj.compile())
-                elif isinstance(obj, ModelContractWrapper):
-                    repo.models.add(obj.compile())
+                elif isinstance(obj, OnlineSource):
+                    repo.online_source = obj
                 else:
                     classes = super_classes_in(obj)
-                    if 'ModelContract' in classes:
-                        repo.models.add(obj.compile())
-                    elif 'FeatureView' in classes:
-                        fv = obj.compile()
+                    if 'FeatureView' in classes:
+                        fv = await obj.compile()
                         if fv.name in feature_view_names:
                             raise Exception(
                                 (
                                     f'Duplicate feature view names: {fv.name},',
                                     f' in {py_file}, and {feature_view_names[fv.name]}',
                                 )
                             )
                         feature_view_names[fv.name] = py_file.as_posix()
                         repo.feature_views.add(fv)
                     elif 'CombinedFeatureView' in classes:
-                        fv = obj.compile()
+                        fv = await obj.compile()
                         if fv.name in feature_view_names:
                             raise Exception(
                                 (
                                     f'Duplicate feature view names: {fv.name},',
                                     f' in {py_file}, and {feature_view_names[fv.name]}',
                                 )
                             )
```

### Comparing `aligned-0.0.98/aligned/data_source/stream_data_source.py` & `aligned-0.0.9a0/aligned/data_source/batch_data_source.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,101 @@
-from __future__ import annotations
-
-from abc import ABC
-from dataclasses import dataclass, field
-from typing import TYPE_CHECKING
+from abc import ABC, abstractmethod
+from datetime import datetime
+from typing import Optional, TypeVar
 
 from mashumaro.types import SerializableType
 
+from aligned.request.retrival_request import RetrivalRequest
+from aligned.retrival_job import DateRangeJob, FullExtractJob, RetrivalJob
 from aligned.schemas.codable import Codable
-
-if TYPE_CHECKING:
-    from aligned.retrival_job import RetrivalJob
-    from aligned.streams.interface import ReadableStream
+from aligned.schemas.feature import Feature
 
 
-class StreamDataSourceFactory:
+class BatchDataSourceFactory:
 
-    supported_data_sources: dict[str, type[StreamDataSource]]
+    supported_data_sources: dict[str, type['BatchDataSource']]
 
-    _shared: StreamDataSourceFactory | None = None
+    _shared: Optional['BatchDataSourceFactory'] = None
 
     def __init__(self) -> None:
-        from aligned.sources.kafka import KafkaTopicConfig
-        from aligned.sources.redis import RedisStreamSource
+        from aligned.local.source import CsvFileSource
+        from aligned.psql.data_source import PostgreSQLDataSource
+        from aligned.redshift.data_source import RedshiftSQLDataSource
+        from aligned.s3.config import AwsS3CsvDataSource, AwsS3ParquetDataSource
 
         self.supported_data_sources = {
-            HttpStreamSource.name: HttpStreamSource,
-            RedisStreamSource.name: RedisStreamSource,
-            KafkaTopicConfig.name: KafkaTopicConfig,
+            PostgreSQLDataSource.type_name: PostgreSQLDataSource,
+            CsvFileSource.type_name: CsvFileSource,
+            AwsS3CsvDataSource.type_name: AwsS3CsvDataSource,
+            AwsS3ParquetDataSource.type_name: AwsS3ParquetDataSource,
+            RedshiftSQLDataSource.type_name: RedshiftSQLDataSource,
         }
 
     @classmethod
-    def shared(cls) -> StreamDataSourceFactory:
+    def shared(cls) -> 'BatchDataSourceFactory':
         if cls._shared:
             return cls._shared
-        cls._shared = StreamDataSourceFactory()
+        cls._shared = BatchDataSourceFactory()
         return cls._shared
 
 
-class StreamDataSource(ABC, Codable, SerializableType):
+T = TypeVar('T')
+
+
+class BatchDataSource(ABC, Codable, SerializableType):
     """
-    Used to determend if an API call should be created, or if we should listen to a stream.
+    A definition to where a specific pice of data can be found.
+    E.g: A database table, a file, a web service, etc.
+
+    Ths can thereafter be combined with other BatchDataSources in order to create a rich dataset.
     """
 
-    name: str
-    topic_name: str
+    type_name: str
+
+    @abstractmethod
+    def job_group_key(self) -> str:
+        pass
 
     def _serialize(self) -> dict:
-        assert self.name in StreamDataSourceFactory.shared().supported_data_sources
         return self.to_dict()
 
+    def __hash__(self) -> int:
+        return hash(self.job_group_key())
+
     @classmethod
-    def _deserialize(cls, value: dict) -> StreamDataSource:
-        name = value['name']
-        if name not in StreamDataSourceFactory.shared().supported_data_sources:
+    def _deserialize(cls, value: dict) -> 'BatchDataSource':
+        name_type = value['type_name']
+        if name_type not in BatchDataSourceFactory.shared().supported_data_sources:
             raise ValueError(
-                f"Unknown stream data source id: '{name}'.\nRemember to add the"
-                ' data source to the StreamDataSourceFactory.supported_data_sources if'
+                f"Unknown batch data source id: '{name_type}'.\nRemember to add the"
+                ' data source to the BatchDataSourceFactory.supported_data_sources if'
                 ' it is a custom type.'
             )
-        del value['name']
-        data_class = StreamDataSourceFactory.shared().supported_data_sources[name]
+        del value['type_name']
+        data_class = BatchDataSourceFactory.shared().supported_data_sources[name_type]
         return data_class.from_dict(value)
 
-    def consumer(self, from_timestamp: str | None = None) -> ReadableStream:
-        """Returns a consumer that actually can load data
-
-        E.g:
-        ```python
-        redis_config = RedisConfig(env_var="REDIS_URL")
-
-        consumer = redis_config.consumer()
-        ```
-
-        Returns:
-            ReadableStream: A stream you can read records from
-        """
+    def all_data(self, request: RetrivalRequest, limit: int | None) -> FullExtractJob:
         raise NotImplementedError()
 
+    def all_between_dates(
+        self,
+        request: RetrivalRequest,
+        start_date: datetime,
+        end_date: datetime,
+    ) -> DateRangeJob:
+        raise NotImplementedError()
 
-@dataclass
-class HttpStreamSource(StreamDataSource):
-
-    topic_name: str
-    mappings: dict[str, str] = field(default_factory=dict)
+    @classmethod
+    def feature_for(cls: type[T], facts: dict[str, list], requests: dict[T, RetrivalRequest]) -> RetrivalJob:
+        raise NotImplementedError()
 
-    name: str = 'http'
 
-    def map_values(self, mappings: dict[str, str]) -> HttpStreamSource:
-        return HttpStreamSource(topic_name=self.topic_name, mappings=self.mappings | mappings)
+class ColumnFeatureMappable:
+    mapping_keys: dict[str, str]
 
+    def columns_for(self, features: list[Feature]) -> list[str]:
+        return [self.mapping_keys.get(feature.name, feature.name) for feature in features]
 
-class SinkableDataSource:
-    async def write_to_stream(self, job: RetrivalJob) -> None:
-        pass
+    def feature_identifier_for(self, columns: list[str]) -> list[str]:
+        reverse_map = {v: k for k, v in self.mapping_keys.items()}
+        return [reverse_map.get(column, column) for column in columns]
```

### Comparing `aligned-0.0.98/aligned/enricher.py` & `aligned-0.0.9a0/aligned/enricher.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
+from contextlib import suppress
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from pathlib import Path
 
 import pandas as pd
 from mashumaro.types import SerializableType
 
+from aligned.redis.config import RedisConfig
 from aligned.schemas.codable import Codable
-from aligned.sources.redis import RedisConfig
+
+with suppress(ModuleNotFoundError):
+    import dask.dataframe as dd
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class TimespanSelector(Codable):
     timespand: timedelta
@@ -53,14 +57,18 @@
     def cache(self, ttl: timedelta, cache_key: str) -> Enricher:
         return FileCacheEnricher(ttl, cache_key, self)
 
     @abstractmethod
     async def as_df(self) -> pd.DataFrame:
         pass
 
+    @abstractmethod
+    async def as_dask(self) -> dd.DataFrame:
+        pass
+
 
 class SupportedEnrichers:
 
     types: dict[str, type[Enricher]]
 
     _shared: SupportedEnrichers | None = None
 
@@ -98,14 +106,19 @@
         self.timeout = timeout
 
     async def as_df(self) -> pd.DataFrame:
         redis = self.config.redis()
         async with redis.lock(self.lock_name, timeout=self.timeout) as _:
             return await self.enricher.as_df()
 
+    async def as_dask(self) -> dd.DataFrame:
+        redis = self.config.redis()
+        async with redis.lock(self.lock_name, timeout=self.timeout) as _:
+            return await self.enricher.as_dask()
+
 
 @dataclass
 class CsvFileSelectedEnricher(Enricher):
     file: str
     time: TimespanSelector | None = field(default=None)
     limit: int | None = field(default=None)
     name: str = 'selective_file'
@@ -128,14 +141,17 @@
         if not self.time:
             return file
 
         date = datetime.now() - self.time.timespand
         selector = file[self.time.time_column] >= date
         return file.loc[selector]
 
+    async def as_dask(self) -> dd.DataFrame:
+        return dd.read_csv(self.file)
+
 
 @dataclass
 class CsvFileEnricher(Enricher):
 
     file: str
     name: str = 'file'
 
@@ -143,14 +159,17 @@
         self, time: TimespanSelector | None = None, limit: int | None = None
     ) -> CsvFileSelectedEnricher:
         return CsvFileSelectedEnricher(self.file, time=time, limit=limit)
 
     async def as_df(self) -> pd.DataFrame:
         return pd.read_csv(self.file)
 
+    async def as_dask(self) -> dd.DataFrame:
+        return dd.read_csv(self.file)
+
 
 @dataclass
 class LoadedStatEnricher(Enricher):
 
     stat: str
     columns: list[str]
     enricher: Enricher
@@ -162,14 +181,24 @@
         if self.stat == 'mean':
             return renamed[self.columns].mean()
         elif self.stat == 'std':
             return renamed[self.columns].std()
         else:
             raise ValueError(f'Not supporting stat: {self.stat}')
 
+    async def as_dask(self) -> dd.DataFrame:
+        data = await self.enricher.as_dask()
+        renamed = data.rename(columns=self.mapping_keys)
+        if self.stat == 'mean':
+            return renamed[self.columns].mean()
+        elif self.stat == 'std':
+            return renamed[self.columns].std()
+        else:
+            raise ValueError(f'Not supporting stat: {self.stat}')
+
 
 @dataclass
 class FileCacheEnricher(Enricher):
 
     ttl: timedelta
     file_path: str
     enricher: Enricher
@@ -195,14 +224,28 @@
             logger.info(f'Storing cache at file {file_uri.as_uri()}')
             data.to_parquet(file_uri)
         else:
             logger.info('Loading cache')
             data = pd.read_parquet(file_uri)
         return data
 
+    async def as_dask(self) -> dd.DataFrame:
+        file_uri = Path(self.file_path).absolute()
+
+        if self.is_out_of_date_cache():
+            logger.info('Fetching from source')
+            data: dd.DataFrame = await self.enricher.as_dask()
+            file_uri.parent.mkdir(exist_ok=True, parents=True)
+            logger.info(f'Storing cache at file {file_uri.as_uri()}')
+            data.to_parquet(file_uri)
+        else:
+            logger.info('Loading cache')
+            data = dd.read_parquet(file_uri)
+        return data
+
 
 @dataclass
 class SqlDatabaseEnricher(Enricher):
 
     query: str
     values: dict | None
     url_env: str
@@ -212,16 +255,20 @@
         self.query = query
         self.values = values
         self.url_env = url_env
 
     async def as_df(self) -> pd.DataFrame:
         import os
 
-        import connectorx as cx
-
-        df = cx.read_sql(os.environ[self.url_env], self.query, return_type='pandas')
+        from databases import Database
 
+        async with Database(os.environ[self.url_env]) as db:
+            records = await db.fetch_all(self.query, values=self.values)
+        df = pd.DataFrame.from_records([dict(record) for record in records])
         for name, dtype in df.dtypes.iteritems():
             if dtype == 'object':  # Need to convert the databases UUID type
                 df[name] = df[name].astype('str')
-
         return df
+
+    async def as_dask(self) -> dd.DataFrame:
+        pdf = await self.as_df()
+        return dd.from_pandas(pdf)
```

### Comparing `aligned-0.0.98/aligned/feature_view/combined_view.py` & `aligned-0.0.9a0/aligned/feature_view/combined_view.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,159 +1,120 @@
 import logging
 from abc import ABC, abstractproperty
 from dataclasses import dataclass
-from typing import Generic, TypeVar, Any, Type, Callable, TYPE_CHECKING
+from typing import Callable
 
 from aligned.compiler.feature_factory import FeatureFactory
-from aligned.feature_view.feature_view import FeatureView
+from aligned.feature_view.feature_view import FeatureSelectable, FeatureView, FVType
 from aligned.request.retrival_request import RetrivalRequest
 from aligned.schemas.derivied_feature import DerivedFeature
-from aligned.schemas.feature import FeatureLocation
 from aligned.schemas.feature_view import CompiledCombinedFeatureView, CompiledFeatureView
 
-if TYPE_CHECKING:
-    from aligned.feature_store import FeatureViewStore
-
 logger = logging.getLogger(__name__)
 
-T = TypeVar('T')
-
 
 @dataclass
 class CombinedFeatureViewMetadata:
     name: str
     description: str | None = None
     tags: dict[str, str] | None = None
     owner: str | None = None
 
 
-@dataclass
-class CombinedFeatureViewWrapper(Generic[T]):
-
-    metadata: CombinedFeatureViewMetadata
-    view: Type[T]
-
-    def __call__(self) -> T:
-        # Needed to make sure that the `location` is set in the view's features
-        _ = self.compile()
-        return self.view()
-
-    def compile(self) -> CompiledCombinedFeatureView:
-        return CombinedFeatureView.compile_with_metadata(self.view(), self.metadata)
-
-    def query(self) -> 'FeatureViewStore':
-        """Makes it possible to query the feature view for features
-
-        ```python
-        @feature_view(...)
-        class SomeView:
-
-            id = Int32().as_entity()
-
-            a = Int32()
-            b = Int32()
-
-        data = await SomeView.query().features_for({
-            "id": [1, 2, 3],
-        }).to_pandas()
-        ```
-
-        Returns:
-            FeatureViewStore: Returns a queryable `FeatureViewStore` containing the feature view
-        """
-        from aligned import ContractStore
-
-        store = ContractStore.experimental()
-        store.add_combined_view(self.compile())
-        return store.feature_view(self.metadata.name)
-
-    async def process(self, data: dict[str, list[Any]]) -> list[dict]:
-        df = await self.query().process_input(data).to_lazy_polars()
-        return df.collect().to_dicts()
-
-
-def combined_feature_view(
-    name: str, description: str, tags: dict[str, str] | None = None, owner: str | None = None
-) -> Callable[[Type[T]], CombinedFeatureViewWrapper[T]]:
-    """
-    Wraps a view as a combined view
-
-    ```python
-    @combined_feature_view(
-        name="my_combined_view",
-        description="some description"
-    )
-    class MyView:
-
-        other = OtherView()
-        another = AnotherView()
-
-        y = other.x * another.y
-    ```
-    """
-
-    def decorator(cls: Type[T]) -> CombinedFeatureViewWrapper[T]:
-        return CombinedFeatureViewWrapper(
-            CombinedFeatureViewMetadata(name, description, tags=tags, owner=owner), cls
-        )
-
-    return decorator
-
-
-class CombinedFeatureView(ABC):
+class CombinedFeatureView(ABC, FeatureSelectable):
     @abstractproperty
     def metadata(self) -> CombinedFeatureViewMetadata:
-        raise NotImplementedError(f'Need to add a metadata field to in {self}')
+        pass
 
     @staticmethod
     def _needed_features(
-        depending_on: list[FeatureFactory], feature_views: dict[FeatureLocation, CompiledFeatureView]
+        depending_on: list[FeatureFactory], feature_views: dict[str, CompiledFeatureView]
     ) -> list[RetrivalRequest]:
 
         feature_refs: dict[CompiledFeatureView, set[str]] = {}
 
         for feature_dep in depending_on:
-            view = feature_views[feature_dep._location]
+            view = feature_views[feature_dep._feature_view]
             feature_refs.setdefault(view, set()).add(feature_dep.name)
 
         return [
             feature_view.request_for(features).needed_requests[0]
             for feature_view, features in feature_refs.items()
         ]
 
     @classmethod
-    def compile(cls) -> CompiledCombinedFeatureView:
-        instance = cls()
-        return CombinedFeatureView.compile_with_metadata(instance, instance.metadata)
+    async def compile(cls) -> CompiledCombinedFeatureView:
+        transformations: set[DerivedFeature] = set()
+        metadata = cls().metadata
+        var_names = [name for name in cls().__dir__() if not name.startswith('_')]
 
-    @staticmethod
-    def compile_with_metadata(
-        view: Any, metadata: CombinedFeatureViewMetadata
-    ) -> CompiledCombinedFeatureView:
+        requests: dict[str, list[RetrivalRequest]] = {}
+        feature_view_deps: dict[str, CompiledFeatureView] = {}
+
+        for var_name in var_names:
+            feature = getattr(cls, var_name)
+            if isinstance(feature, FeatureView):
+                # Needs to compile the view one more time. unfortunally..
+                # not optimal as the view will be duplicated in the definition file
+                feature_view_deps[feature.metadata.name] = await feature.compile()
+            if isinstance(feature, FeatureFactory):
+                feature._feature_view = metadata.name
+                feature._name = var_name  # Needed in some cases for later inferance and features
+                if not feature.transformation:
+                    logger.info('Feature had no transformation, which do not make sense in a CombinedView')
+                    continue
+                requests[var_name] = CombinedFeatureView._needed_features(
+                    feature.transformation.using_features, feature_view_deps
+                )
+
+                transformations.add(await feature.compile(list(feature_view_deps.values())))
+
+        return CompiledCombinedFeatureView(
+            name=metadata.name,
+            features=transformations,
+            feature_referances=requests,
+        )
+
+    @classmethod
+    def compile_only_graph(cls) -> CompiledCombinedFeatureView:
         transformations: set[DerivedFeature] = set()
-        var_names = [name for name in view.__dir__() if not name.startswith('_')]
+        metadata = cls().metadata
+        var_names = [name for name in cls().__dir__() if not name.startswith('_')]
 
         requests: dict[str, list[RetrivalRequest]] = {}
-        feature_view_deps: dict[FeatureLocation, CompiledFeatureView] = {}
+        feature_view_deps: dict[str, CompiledFeatureView] = {}
 
         for var_name in var_names:
-            feature = getattr(view, var_name)
+            feature = getattr(cls, var_name)
             if isinstance(feature, FeatureView):
                 # Needs to compile the view one more time. unfortunally..
                 # not optimal as the view will be duplicated in the definition file
-                feature_view_deps[FeatureLocation.feature_view(feature.metadata.name)] = feature.compile()
+                feature_view_deps[feature.metadata.name] = feature.compile_graph_only()
             if isinstance(feature, FeatureFactory):
-                feature._location = FeatureLocation.combined_view(var_name)
+                feature._feature_view = metadata.name
+                feature._name = var_name  # Needed in some cases for later inferance and features
                 if not feature.transformation:
                     logger.info('Feature had no transformation, which do not make sense in a CombinedView')
                     continue
                 requests[var_name] = CombinedFeatureView._needed_features(
                     feature.transformation.using_features, feature_view_deps
                 )
 
-                transformations.add(feature.compile())
+                transformations.add(feature.compile_graph_only())
 
         return CompiledCombinedFeatureView(
             name=metadata.name,
             features=transformations,
             feature_referances=requests,
         )
+
+    @classmethod
+    def select(
+        cls: type[FVType], features: Callable[[type[FVType]], list[FeatureFactory]]
+    ) -> RetrivalRequest:
+        view: CompiledCombinedFeatureView = cls.compile_only_graph()  # type: ignore[attr-defined]
+        names = features(cls)
+        return view.requests_for({feat.name for feat in names})
+
+    @classmethod
+    def select_all(cls: type[FVType]) -> RetrivalRequest:
+        return cls.compile_only_graph().request_all  # type: ignore[attr-defined]
```

### Comparing `aligned-0.0.98/aligned/feature_view/tests/test_brest_cancer.py` & `aligned-0.0.9a0/aligned/feature_view/tests/test_brest_cancer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import pytest
 
-from aligned import ContractStore
-from aligned.feature_view.feature_view import FeatureView
+from aligned import FeatureStore, FeatureView
 
 
 @pytest.mark.asyncio
 async def test_all_features(
-    breast_scan_without_timestamp_feature_store: ContractStore,
+    breast_scan_without_timestamp_feature_store: FeatureStore,
     breast_scan_feature_viewout_with_datetime: FeatureView,
 ) -> None:
     store = breast_scan_without_timestamp_feature_store
     feature_view = breast_scan_feature_viewout_with_datetime
 
     features = await store.feature_view(feature_view.metadata.name).all().to_pandas()
 
+    for feature in type(breast_scan_feature_viewout_with_datetime).select_all().features_to_include:
+        assert feature in features.columns
+
     assert 'is_malignant' in features.columns
     assert not features['is_malignant'].isna().any()
     assert 'diagnosis' in features.columns
     assert 'scan_id' in features.columns
 
     limit = 10
     limit_features = await store.feature_view(feature_view.metadata.name).all(limit=limit).to_pandas()
```

### Comparing `aligned-0.0.98/aligned/feature_view/tests/test_brest_cancer_event_timestamp.py` & `aligned-0.0.9a0/aligned/feature_view/tests/test_brest_cancer_event_timestamp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,93 @@
 from datetime import datetime
 
 import pytest
 
-from aligned import ContractStore
-from aligned.feature_view.feature_view import FeatureView
+from aligned import FeatureStore, FeatureView
 
 
 @pytest.mark.asyncio
 async def test_between_datetime_features(
     breast_scan_feature_view_with_datetime: FeatureView,
-    breast_scan_with_timestamp_feature_store: ContractStore,
+    breast_scan_with_timestamp_feature_store: FeatureStore,
 ) -> None:
     feature_view = breast_scan_feature_view_with_datetime
     store = breast_scan_with_timestamp_feature_store
     features = await store.feature_view(feature_view.metadata.name).all().to_pandas()
 
+    for feature in type(feature_view).select_all().features_to_include:
+        assert feature in features.columns
+
     assert 'created_at' in features.columns
     assert 'is_malignant' in features.columns
     assert 'diagnosis' in features.columns
     assert 'scan_id' in features.columns
 
     limit_features = (
         await store.feature_view(feature_view.metadata.name)
-        .between_dates(
+        .between(
             start_date=datetime(2020, 1, 5),
             end_date=datetime(2020, 1, 11),
         )
         .to_pandas()
     )
     assert limit_features.shape[0] == 6
 
 
 @pytest.mark.asyncio
 async def test_between_datetime_features_with_aggregation(
     breast_scan_feature_view_with_datetime_and_aggregation: FeatureView,
-    breast_scan_with_timestamp_and_aggregation_feature_store: ContractStore,
+    breast_scan_with_timestamp_and_aggregation_feature_store: FeatureStore,
 ) -> None:
     feature_view = breast_scan_feature_view_with_datetime_and_aggregation
     store = breast_scan_with_timestamp_and_aggregation_feature_store
     features = await store.feature_view(feature_view.metadata.name).all().to_pandas()
 
+    for feature in type(feature_view).select_all().features_to_include:
+        assert feature in features.columns
+
     assert 'created_at' in features.columns
     assert 'is_malignant' in features.columns
     assert 'diagnosis' in features.columns
     assert 'scan_id' in features.columns
 
     limit_features = (
         await store.feature_view(feature_view.metadata.name)
-        .between_dates(
+        .between(
             start_date=datetime(2020, 1, 5),
             end_date=datetime(2020, 1, 11),
         )
         .to_pandas()
     )
 
     assert limit_features.shape[0] == 6
+    assert features['mean_fd_worst_for_group'].isna().count() != 0
+
+
+@pytest.mark.asyncio
+async def test_between_datetime_features_polars(
+    breast_scan_feature_view_with_datetime: FeatureView,
+    breast_scan_with_timestamp_feature_store: FeatureStore,
+) -> None:
+    feature_view = breast_scan_feature_view_with_datetime
+    store = breast_scan_with_timestamp_feature_store
+    job = store.feature_view(feature_view.metadata.name).all()
+    features = (await job.to_polars()).collect()
+
+    for feature in type(feature_view).select_all().features_to_include:
+        assert feature in features.columns
 
+    assert 'created_at' in features.columns
+    assert 'is_malignant' in features.columns
+    assert 'diagnosis' in features.columns
+    assert 'scan_id' in features.columns
 
-# @pytest.mark.asyncio
-# async def test_between_datetime_features_polars(
-#     breast_scan_feature_view_with_datetime: FeatureView,
-#     breast_scan_with_timestamp_feature_store: FeatureStore,
-# ) -> None:
-#     feature_view = breast_scan_feature_view_with_datetime
-#     store = breast_scan_with_timestamp_feature_store
-#     job = store.feature_view(feature_view.metadata.name).all()
-#     features = (await job.to_polars()).collect()
-
-#     assert 'created_at' in features.columns
-#     assert 'is_malignant' in features.columns
-#     assert 'diagnosis' in features.columns
-#     assert 'scan_id' in features.columns
-
-#     limit_features = (
-#         await store.feature_view(feature_view.metadata.name)
-#         .between_dates(
-#             start_date=datetime(2020, 1, 5),
-#             end_date=datetime(2020, 1, 11),
-#         )
-#         .to_polars()
-#     ).collect()
+    limit_features = (
+        await store.feature_view(feature_view.metadata.name)
+        .between(
+            start_date=datetime(2020, 1, 5),
+            end_date=datetime(2020, 1, 11),
+        )
+        .to_polars()
+    ).collect()
 
-#     assert limit_features.shape[0] == 6
+    assert limit_features.shape[0] == 6
```

### Comparing `aligned-0.0.98/aligned/jobs/tests/test_combined_job.py` & `aligned-0.0.9a0/aligned/jobs/tests/test_combined_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,11 +23,11 @@
     retrival_job: RetrivalJob,
     retrival_job_with_timestamp: RetrivalJob,
     combined_retrival_request: RetrivalRequest,
 ) -> None:
     job = CombineFactualJob(
         jobs=[retrival_job, retrival_job_with_timestamp], combined_requests=[combined_retrival_request]
     )
-    data = (await job.to_lazy_polars()).collect()
+    data = (await job.to_polars()).collect()
 
     assert set(data.columns) == {'id', 'a', 'b', 'c', 'd', 'created_at', 'c+d', 'a+c+d'}
     assert data.shape[0] == 5
```

### Comparing `aligned-0.0.98/aligned/request/tests/test_feature_request_generation.py` & `aligned-0.0.9a0/aligned/request/tests/test_feature_request_generation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 
-from aligned.feature_view.feature_view import FeatureView
+from aligned import FeatureView
 
 
 @pytest.mark.asyncio
 async def test_fetch_all_request(titanic_feature_view: FeatureView) -> None:
 
-    compiled_view = type(titanic_feature_view).compile()
+    compiled_view = await type(titanic_feature_view).compile()
     request = compiled_view.request_all
 
     expected_features = {
         'age',
         'name',
         'sex',
         'survived',
@@ -33,23 +33,21 @@
     assert len(request.request_result.entities) == 1
     assert len(request.request_result.features) == len(expected_features)
 
 
 @pytest.mark.asyncio
 async def test_fetch_features_request(titanic_feature_view: FeatureView) -> None:
 
-    compiled_view = type(titanic_feature_view).compile()
+    compiled_view = await type(titanic_feature_view).compile()
     wanted_features = {'cabin', 'is_male'}
     request = compiled_view.request_for(wanted_features)
     expected_features = {'sex', 'cabin', 'is_male'}
     assert not request.needs_event_timestamp
     assert len(request.needed_requests) == 1
 
     retrival_request = request.needed_requests[0]
     missing_features = expected_features - retrival_request.all_feature_names
-    # All the features to retrive and computed
     assert retrival_request.all_feature_names == expected_features, f'Missing features {missing_features}'
     assert retrival_request.entity_names == {'passenger_id'}
 
-    # All the features that is returned
     assert len(request.request_result.entities) == 1
-    assert len(request.request_result.features) == len(wanted_features)
+    assert len(request.request_result.features) == len(expected_features)
```

### Comparing `aligned-0.0.98/aligned/schemas/constraints.py` & `aligned-0.0.9a0/aligned/schemas/constraints.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from dataclasses import dataclass
-from typing import Optional as OptionalType
+from typing import Optional
 
 from mashumaro.types import SerializableType
 
 from aligned.schemas.codable import Codable
 
 
 class Constraint(Codable, SerializableType):
     name: str
 
     def __hash__(self) -> int:
         return hash(self.name)
 
     def _serialize(self) -> dict:
-        assert self.name in SupportedConstraints.shared().types, f'Constraint {self.name} is not supported'
         return self.to_dict()
 
     @classmethod
     def _deserialize(cls, value: dict) -> 'Constraint':
         name_type = value['name']
         del value['name']
         data_class = SupportedConstraints.shared().types[name_type]
@@ -25,38 +24,26 @@
         return data_class.from_dict(value)
 
 
 class SupportedConstraints:
 
     types: dict[str, type[Constraint]]
 
-    _shared: OptionalType['SupportedConstraints'] = None
+    _shared: Optional['SupportedConstraints'] = None
 
     def __init__(self) -> None:
-        from aligned.schemas.constraint_types import (
-            ReferencingColumn,
-        )
-
         self.types = {}
 
         for tran_type in [
             LowerBound,
             LowerBoundInclusive,
             UpperBound,
             UpperBoundInclusive,
             Required,
-            Optional,
             InDomain,
-            MaxLength,
-            MinLength,
-            StartsWith,
-            EndsWith,
-            Unique,
-            Regex,
-            ReferencingColumn,
         ]:
             self.add(tran_type)
 
     def add(self, constraint: type[Constraint]) -> None:
         self.types[constraint.name] = constraint
 
     @classmethod
@@ -104,72 +91,14 @@
     name = 'upper_bound_inc'
 
     def __hash__(self) -> int:
         return hash(self.name)
 
 
 @dataclass
-class Unique(Constraint):
-    name = 'unique'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
-class MinLength(Constraint):
-    value: int
-
-    name = 'min_length'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
-class Regex(Constraint):
-    value: str
-
-    name = 'regex'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
-class EndsWith(Constraint):
-    value: str
-
-    name = 'ends_with'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
-class StartsWith(Constraint):
-    value: str
-
-    name = 'starts_with'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
-class MaxLength(Constraint):
-    value: int
-
-    name = 'max_length'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
 class And(Constraint):
 
     left: Constraint
     right: Constraint
     name = 'and'
 
     def __hash__(self) -> int:
@@ -182,23 +111,14 @@
     name = 'requierd'
 
     def __hash__(self) -> int:
         return hash(self.name)
 
 
 @dataclass
-class Optional(Constraint):
-
-    name = 'optional'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
 class InDomain(Constraint):
 
     values: list[str]
     name = 'in_domain'
 
     def __hash__(self) -> int:
         return hash(self.name)
```

### Comparing `aligned-0.0.98/aligned/server.py` & `aligned-0.0.9a0/aligned/server.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-from __future__ import annotations
-
 import asyncio
 import logging
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any
 
 from fastapi import FastAPI, HTTPException, Response
-from fastapi.responses import RedirectResponse
 from numpy import nan
 from pydantic import BaseModel
 
 from aligned.data_source.stream_data_source import HttpStreamSource
 from aligned.feature_source import WritableFeatureSource
-from aligned.feature_store import ContractStore
+from aligned.feature_store import FeatureStore
 from aligned.schemas.feature import Feature
 from aligned.schemas.feature_view import CompiledFeatureView
-from aligned.sources.local import StorageFileReference
 
 logger = logging.getLogger(__name__)
 
 
 class APIFeatureRequest(BaseModel):
     entities: dict[str, list]
     features: list[str]
@@ -31,15 +27,15 @@
     name: str
     views: list[CompiledFeatureView]
     mappings: dict[str, str]
 
 
 class FastAPIServer:
     @staticmethod
-    def write_to_topic_path(topic: TopicInfo, feature_store: ContractStore, app: FastAPI) -> None:
+    def write_to_topic_path(topic: TopicInfo, feature_store: FeatureStore, app: FastAPI) -> None:
 
         required_features: set[Feature] = set()
         for view in topic.views:
             required_features.update(view.entities.union(view.features))
 
         view_names = [view.name for view in topic.views]
         mappings: dict[str, list[str]] = {
@@ -91,28 +87,25 @@
                     feature_values[output_name] = [value if value != {} else None for value in values]
 
             await asyncio.gather(
                 *[feature_store.feature_view(view_name).write(feature_values) for view_name in view_names]
             )
 
     @staticmethod
-    def feature_view_path(name: str, feature_store: ContractStore, app: FastAPI) -> None:
+    def feature_view_path(name: str, feature_store: FeatureStore, app: FastAPI) -> None:
         @app.post(f'/feature-views/{name}/all')
         async def all(limit: int | None = None) -> dict:
             df = await feature_store.feature_view(name).all(limit=limit).to_pandas()
             df.replace(nan, value=None, inplace=True)
             return df.to_dict('list')
 
     @staticmethod
-    def model_path(name: str, feature_store: ContractStore, app: FastAPI) -> None:
-        from aligned.feature_store import RawStringFeatureRequest
-
-        model = feature_store.models[name]
-        features = {f'{feature.location.identifier}:{feature.name}' for feature in model.features}
-        feature_request = feature_store.requests_for(RawStringFeatureRequest(features))
+    def model_path(name: str, feature_store: FeatureStore, app: FastAPI) -> None:
+        model = feature_store.model_requests[name]
+        feature_request = feature_store.requests_for_model(model)
 
         entities: set[Feature] = set()
         for request in feature_request.needed_requests:
             entities.update(request.entities)
 
         required_features = entities.copy()
         for request in feature_request.needed_requests:
@@ -155,43 +148,28 @@
                 entity_values['event_timestamp'] = [
                     datetime.fromtimestamp(value)
                     if isinstance(value, (float, int))
                     else datetime.fromisoformat(value)
                     for value in entity_values['event_timestamp']
                 ]
 
-            df = await feature_store.model(name).features_for(entity_values).to_lazy_polars()
-            pandas_df = df.collect().to_pandas()
+            df = await feature_store.model(name).features_for(entity_values).to_pandas()
             orient = 'values'
-            body = ','.join(
-                [f'"{column}":{pandas_df[column].to_json(orient=orient)}' for column in pandas_df.columns]
-            )
+            body = ','.join([f'"{column}":{df[column].to_json(orient=orient)}' for column in df.columns])
             return Response(content=f'{{{body}}}', media_type='application/json')
 
     @staticmethod
-    def app(feature_store: ContractStore, auth_tokens: list[str] | None = None) -> FastAPI:
+    def app(feature_store: FeatureStore) -> FastAPI:
         from asgi_correlation_id import CorrelationIdMiddleware
         from fastapi import FastAPI
         from fastapi.middleware import Middleware
-        from prometheus_fastapi_instrumentator import Instrumentator
-        from starlette.status import HTTP_200_OK
 
         app = FastAPI(middleware=[Middleware(CorrelationIdMiddleware)])
         app.docs_url = '/docs'
 
-        prom_instrument = Instrumentator().instrument(app)
-
-        @app.on_event('startup')
-        async def startup():
-            prom_instrument.expose(app)
-
-        @app.get('health', status_code=HTTP_200_OK)
-        def health() -> None:
-            return
-
         for model in feature_store.all_models:
             FastAPIServer.model_path(model, feature_store, app)
 
         can_write_to_store = isinstance(feature_store.feature_source, WritableFeatureSource)
 
         topics: dict[str, TopicInfo] = {}
 
@@ -221,49 +199,31 @@
             logger.info(
                 (
                     'Warning! The server is not using a WritableFeatureSource, ',
                     'and can therefore not setup stream sources',
                 )
             )
 
-        @app.get('/')
-        async def root() -> RedirectResponse:
-            return RedirectResponse('/docs')
-
         @app.post('/features')
         async def features(payload: APIFeatureRequest) -> dict:
-            import json
-
             df = await feature_store.features_for(
-                payload.entities, features=payload.features
-            ).to_lazy_polars()
-            json_data = json.dumps(df.collect().to_dict(as_series=False))
-            return Response(content=json_data, media_type='application/json')
+                payload.entities,
+                features=payload.features,
+            ).to_pandas()
+            orient = 'values'
+            body = ','.join([f'"{column}":{df[column].to_json(orient=orient)}' for column in df.columns])
+            return Response(content=f'{{{body}}}', media_type='application/json')
 
         return app
 
     @staticmethod
     def run(
-        feature_store: ContractStore,
+        feature_store: FeatureStore,
         host: str | None = None,
         port: int | None = None,
         workers: int | None = None,
     ) -> None:
         import uvicorn
 
         app = FastAPIServer.app(feature_store)
 
         uvicorn.run(app, host=host or '127.0.0.1', port=port or 8000, workers=workers or workers)
-
-
-class FeatureServer:
-
-    definition_reference: StorageFileReference
-    auth_keys: list[str] | None = None
-
-    @staticmethod
-    def from_reference(source: StorageFileReference) -> FeatureServer:
-        return FeatureServer(source)
-
-    async def build_app(self) -> FastAPI:
-        definitions = await self.definition_reference.feature_store()
-        return FastAPIServer.app(definitions)
```

### Comparing `aligned-0.0.98/aligned/sources/s3.py` & `aligned-0.0.9a0/aligned/s3/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,21 @@
 from dataclasses import dataclass
 from datetime import datetime
 from io import BytesIO
 
 import pandas as pd
-import polars as pl
 from httpx import HTTPStatusError
 
 from aligned.data_source.batch_data_source import BatchDataSource, ColumnFeatureMappable
 from aligned.exceptions import UnableToFindFileException
 from aligned.local.job import FileDateJob, FileFullJob
-from aligned.retrival_job import RetrivalRequest, RetrivalJob
+from aligned.local.source import CsvConfig, DataFileReference, ParquetConfig, StorageFileReference
+from aligned.retrival_job import DateRangeJob, FullExtractJob, RetrivalRequest
 from aligned.s3.storage import AwsS3Storage
 from aligned.schemas.codable import Codable
-from aligned.sources.local import (
-    CsvConfig,
-    DataFileReference,
-    ParquetConfig,
-    PartitionedParquetFileSource,
-    StorageFileReference,
-    Directory,
-    DeltaFileConfig,
-    DateFormatter,
-)
 from aligned.storage import Storage
 
 try:
     from aioaws.s3 import S3Config
 except ModuleNotFoundError:
 
     class S3Config:  # type: ignore[no-redef]
@@ -55,15 +45,15 @@
     def url(self) -> str:
         import os
 
         region = os.environ[self.bucket_env]
         bucket = os.environ[self.bucket_env]
         return f'https://{region}.amazoneaws.com/{bucket}/'
 
-    def json_at(self, path: str, mapping_keys: dict[str, str] | None = None) -> 'AwsS3DataSource':
+    def file_at(self, path: str, mapping_keys: dict[str, str] | None = None) -> 'AwsS3DataSource':
         return AwsS3DataSource(config=self, path=path)
 
     def csv_at(
         self, path: str, mapping_keys: dict[str, str] | None = None, csv_config: CsvConfig | None = None
     ) -> 'AwsS3CsvDataSource':
         return AwsS3CsvDataSource(
             config=self, path=path, mapping_keys=mapping_keys or {}, csv_config=csv_config or CsvConfig()
@@ -72,77 +62,20 @@
     def parquet_at(
         self, path: str, mapping_keys: dict[str, str] | None = None, config: ParquetConfig | None = None
     ) -> 'AwsS3ParquetDataSource':
         return AwsS3ParquetDataSource(
             config=self, path=path, mapping_keys=mapping_keys or {}, parquet_config=config or ParquetConfig()
         )
 
-    def sub_directory(self, path: str) -> 'AwsS3Directory':
-        return AwsS3Directory(config=self, path=path)
-
-    def directory(self, path: str) -> 'AwsS3Directory':
-        return self.sub_directory(path)
-
     @property
     def storage(self) -> Storage:
         return AwsS3Storage(self)
 
 
 @dataclass
-class AwsS3Directory(Directory):
-
-    config: AwsS3Config
-    path: str
-
-    def json_at(self, path: str) -> 'AwsS3DataSource':
-        return AwsS3DataSource(config=self.config, path=f'{self.path}/{path}')
-
-    def csv_at(
-        self, path: str, mapping_keys: dict[str, str] | None = None, csv_config: CsvConfig | None = None
-    ) -> 'AwsS3CsvDataSource':
-        return AwsS3CsvDataSource(
-            config=self.config,
-            path=f'{self.path}/{path}',
-            mapping_keys=mapping_keys or {},
-            csv_config=csv_config or CsvConfig(),
-        )
-
-    def parquet_at(
-        self, path: str, mapping_keys: dict[str, str] | None = None, config: ParquetConfig | None = None
-    ) -> 'AwsS3ParquetDataSource':
-        return AwsS3ParquetDataSource(
-            config=self.config,
-            path=f'{self.path}/{path}',
-            mapping_keys=mapping_keys or {},
-            parquet_config=config or ParquetConfig(),
-        )
-
-    def partitioned_parquet_at(
-        self,
-        directory: str,
-        partition_keys: list[str],
-        mapping_keys: dict[str, str] | None = None,
-        config: ParquetConfig | None = None,
-        date_formatter: DateFormatter | None = None,
-    ) -> PartitionedParquetFileSource:
-        raise NotImplementedError(type(self))
-
-    def delta_at(
-        self, path: str, mapping_keys: dict[str, str] | None = None, config: DeltaFileConfig | None = None
-    ) -> BatchDataSource:
-        raise NotImplementedError(type(self))
-
-    def sub_directory(self, path: str) -> 'AwsS3Directory':
-        return AwsS3Directory(config=self.config, path=f'{self.path}/{path}')
-
-    def directory(self, path: str) -> 'AwsS3Directory':
-        return self.sub_directory(path)
-
-
-@dataclass
 class AwsS3DataSource(StorageFileReference, ColumnFeatureMappable):
 
     config: AwsS3Config
     path: str
 
     type_name: str = 'aws_s3'
 
@@ -202,41 +135,32 @@
             sep=self.csv_config.seperator,
             index=self.csv_config.should_write_index,
             compression=self.csv_config.compression,
         )
         buffer.seek(0)
         await self.storage.write(self.path, buffer.read())
 
-    async def write_polars(self, df: pl.LazyFrame) -> None:
-        buffer = BytesIO()
-        df.collect().write_csv(
-            buffer,
-            sep=self.csv_config.seperator,
-        )
-        buffer.seek(0)
-        await self.storage.write(self.path, buffer.read())
-
-    def all_data(self, request: RetrivalRequest, limit: int | None) -> RetrivalJob:
+    def all_data(self, request: RetrivalRequest, limit: int | None) -> FullExtractJob:
         return FileFullJob(self, request=request, limit=limit)
 
     def all_between_dates(
         self, request: RetrivalRequest, start_date: datetime, end_date: datetime
-    ) -> RetrivalJob:
+    ) -> DateRangeJob:
         return FileDateJob(self, request, start_date, end_date)
 
 
 @dataclass
 class AwsS3ParquetDataSource(BatchDataSource, DataFileReference, ColumnFeatureMappable):
 
     config: AwsS3Config
     path: str
-    mapping_keys: dict[str, str]
+    mapping_keys: dict[str, str]  # = field(default_factory=dict)
 
-    parquet_config: ParquetConfig
-    type_name: str = 'aws_s3_parquet'
+    parquet_config: ParquetConfig  # = field(default_factory=ParquetConfig)
+    type_name: str = 'aws_s3_parquet'  # = field(default='aws_s3_parquet')
 
     def job_group_key(self) -> str:
         return f'{self.type_name}/{self.path}'
 
     @property
     def storage(self) -> Storage:
         return self.config.storage
@@ -251,28 +175,12 @@
             buffer = BytesIO(data)
             return pd.read_parquet(buffer)
         except FileNotFoundError:
             raise UnableToFindFileException()
         except HTTPStatusError:
             raise UnableToFindFileException()
 
-    async def to_lazy_polars(self) -> pl.LazyFrame:
-        try:
-            data = await self.storage.read(self.path)
-            buffer = BytesIO(data)
-            return pl.read_parquet(buffer).lazy()
-        except FileNotFoundError:
-            raise UnableToFindFileException()
-        except HTTPStatusError:
-            raise UnableToFindFileException()
-
     async def write_pandas(self, df: pd.DataFrame) -> None:
         buffer = BytesIO()
-        df.to_parquet(buffer, compression=self.parquet_config.compression, engine=self.parquet_config.engine)
-        buffer.seek(0)
-        await self.storage.write(self.path, buffer.read())
-
-    async def write_polars(self, df: pl.LazyFrame) -> None:
-        buffer = BytesIO()
-        df.collect().write_parquet(buffer, compression=self.parquet_config.compression)
+        df.to_parquet(buffer)
         buffer.seek(0)
         await self.storage.write(self.path, buffer.read())
```

### Comparing `aligned-0.0.98/aligned/tests/test_cache_enricher.py` & `aligned-0.0.9a0/aligned/tests/test_cache_enricher.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.98/aligned/tests/test_cached_parquet.py` & `aligned-0.0.9a0/aligned/tests/test_cached_parquet.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import pytest
 
-from aligned import ContractStore, FileSource
+from aligned import FeatureStore, FileSource
 
 
 @pytest.mark.asyncio
-async def test_cached_at(titanic_feature_store: ContractStore) -> None:
-    """
-    Checks that we load all rows form the cached file.
-    """
+async def test_cached_at(titanic_feature_store: FeatureStore) -> None:
     file_source = FileSource.parquet_at('test_data/titanic.parquet')
-
-    cached = await file_source.read_pandas()
     data_set = (
         await titanic_feature_store.feature_view('titanic_parquet').all().cached_at(file_source).to_pandas()
     )
+    cached = await file_source.read_pandas()
 
     assert cached.shape[0] == data_set.shape[0]
     assert (set(cached.columns).intersection(set(data_set.columns)) - set(cached.columns)) == set()
```

### Comparing `aligned-0.0.98/aligned/tests/test_statistic_enricher.py` & `aligned-0.0.9a0/aligned/tests/test_statistic_enricher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import timedelta
 
 import pandas as pd
 import pytest
 from freezegun import freeze_time
 
 from aligned.enricher import TimespanSelector
-from aligned.sources.local import CsvFileSource
+from aligned.local.source import CsvFileSource
 
 
 @pytest.mark.asyncio
 async def test_statistic_enricher(scan_with_datetime: CsvFileSource) -> None:
     columns = {'fractal_dimension_worst', 'symmetry_worst'}
     file = await scan_with_datetime.mean(columns=columns).as_df()
     limit_file = await scan_with_datetime.mean(columns=columns, limit=3).as_df()
```

### Comparing `aligned-0.0.98/pyproject.toml` & `aligned-0.0.9a0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 [tool.poetry]
 name = "aligned"
-version = "0.0.98"
-description = "A data managment and lineage tool for ML applications."
+version = "0.0.9a"
+description = "A scalable feature store that makes it easy to align offline and online ML systems"
 authors = ["Mats E. Mollestad <mats@mollestad.no>"]
 license = "Apache-2.0"
 readme = "README.md"
-homepage = "https://github.com/MatsMoll/aligned"
-repository = "https://github.com/MatsMoll/aligned"
+homepage = "https://github.com/otovo/aladdin"
+repository = "https://github.com/otovo/aladdin"
 keywords = [
     'python',
     'typed',
     'ml',
     'prediction',
     'feature',
     'store',
     'feature-store',
-    'mlops',
     'feast',
     'tecton',
-    'dbt',
-    'data',
-    'lineage'
 ]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Operating System :: OS Independent',
@@ -40,65 +36,46 @@
 ]
 packages = [
     { include = "aligned" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-python-dotenv = "^0.21.0"
 click = "^8.1.3"
-pandas = "^2.0.0"
-fastapi = { version = "^0.100.0", optional = true }
+pandas = "^1.3.1"
+fastapi = { version = "^0.77.1", optional = true }
 uvicorn = { version = "^0.17.6", optional = true }
 redis = { version = "^4.3.1", optional = true }
 mashumaro = "^3.0.1"
 dill = "^0.3.4"
 aioaws = { version = "^0.12", optional = true }
+databases = { version = "^0.5.5", optional = true }
+asyncpg = { version = "^0.25.0", optional = true }
+pyarrow = "^8.0.0"
 Jinja2 = "^3.1.2"
 nest-asyncio = "^1.5.5"
-pydantic = "^2.0.0"
-prometheus_client = "^0.16.0"
 asgi-correlation-id = { version = "^3.0.0", optional = true }
-pandera = { version = "^0.17.0", optional = true}
-polars = { version = "^0.20.0", extras = ["pyarrow"] }
-pillow = { version = "^9.4.0", optional = true }
-prometheus-fastapi-instrumentator = { version="^5.9.1", optional = true }
-kafka-python = { version= "^2.0.2", optional = true }
-connectorx = { version = "^0.3.2", optional = true }
-asyncpg = { version = "^0.29.0", optional = true }
-sqlglot = { version = "^22.5.0", optional = true }
-ollama = { version = "^0.1.8", optional = true }
-httpx = "^0.27.0"
-mlflow = { version = "^2.11.3", optional = true }
-adlfs = { version = "^2024.4.1", optional = true }
+dask = {version = "^2022.7.0", extras = ["dataframe"], optional = true}
+pandera = {version = "^0.13.3", optional = true}
+httpx = "^0.23.0"
+polars = { version = "^0.15.6", extras = ["all"] }
 
 [tool.poetry.extras]
-aws = ["aioaws", "connectorx"]
-psql = ["connectorx", "asyncpg"]
+aws = ["aioaws", "databases"]
+psql = ["databases", "asyncpg"]
 redis = ["redis"]
-server = ["asgi-correlation-id", "fastapi", "uvicorn", "prometheus-fastapi-instrumentator"]
+server = ["asgi-correlation-id", "fastapi", "uvicorn"]
+dask = ["dask"]
 pandera = ["pandera"]
-image = ["pillow"]
-kafka = ["kafka-python"]
-ollama = ["ollama"]
-sql = ["sqlglot"]
-mlflow = ["mlflow"]
-azure = ["adlfs"]
 
 [tool.poetry.group.dev.dependencies]
 types-redis = "^4.2.6"
 pytest-mock = "^3.8.1"
 freezegun = "^1.2.2"
 pytest-asyncio = "^0.20.1"
-fakeredis = "^2.10.0"
-sqlalchemy = "^2.0.19"
-printf-log-formatter = "^0.3.0"
-isort = "^5.12.0"
-black = "^23.7.0"
-psycopg2 = "^2.9.6"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 aligned = 'aligned.cli:cli'
```

