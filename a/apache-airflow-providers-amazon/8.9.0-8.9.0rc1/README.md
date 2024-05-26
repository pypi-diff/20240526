# Comparing `tmp/apache-airflow-providers-amazon-8.9.0.tar.gz` & `tmp/apache-airflow-providers-amazon-8.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-amazon-8.9.0.tar", last modified: Wed Oct 18 17:39:39 2023, max compression
+gzip compressed data, was "apache-airflow-providers-amazon-8.9.0rc1.tar", last modified: Wed Oct 18 17:43:06 2023, max compression
```

## Comparing `apache-airflow-providers-amazon-8.9.0.tar` & `apache-airflow-providers-amazon-8.9.0rc1.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.760919 apache-airflow-providers-amazon-8.9.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1219 2023-10-18 17:39:38.000000 apache-airflow-providers-amazon-8.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.9.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8006 2023-10-18 17:39:39.761156 apache-airflow-providers-amazon-8.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5996 2023-10-18 17:39:38.000000 apache-airflow-providers-amazon-8.9.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.556863 apache-airflow-providers-amazon-8.9.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.557050 apache-airflow-providers-amazon-8.9.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.570559 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/
--rw-r--r--   0 root         (0) root         (0)     1575 2023-10-18 17:38:08.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.572943 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.616385 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5415 2023-09-01 12:43:02.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/appflow.py
--rw-r--r--   0 root         (0) root         (0)    12395 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/athena.py
--rw-r--r--   0 root         (0) root         (0)    47899 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/base_aws.py
--rw-r--r--   0 root         (0) root         (0)    21345 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/batch_client.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/batch_waiters.json
--rw-r--r--   0 root         (0) root         (0)    10579 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/batch_waiters.py
--rw-r--r--   0 root         (0) root         (0)     4400 2023-09-08 06:39:39.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/chime.py
--rw-r--r--   0 root         (0) root         (0)     3435 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    13592 2023-09-12 06:55:02.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/datasync.py
--rw-r--r--   0 root         (0) root         (0)     7903 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/dms.py
--rw-r--r--   0 root         (0) root         (0)     2665 2023-08-25 12:06:52.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     7928 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/ec2.py
--rw-r--r--   0 root         (0) root         (0)     3759 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/ecr.py
--rw-r--r--   0 root         (0) root         (0)     6666 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/ecs.py
--rw-r--r--   0 root         (0) root         (0)    23925 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/eks.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
--rw-r--r--   0 root         (0) root         (0)    21401 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/emr.py
--rw-r--r--   0 root         (0) root         (0)     3364 2023-08-09 10:37:33.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/eventbridge.py
--rw-r--r--   0 root         (0) root         (0)     3452 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/glacier.py
--rw-r--r--   0 root         (0) root         (0)    16819 2023-08-16 10:11:24.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/glue.py
--rw-r--r--   0 root         (0) root         (0)     9212 2023-08-15 06:48:52.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/glue_catalog.py
--rw-r--r--   0 root         (0) root         (0)     7926 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     2580 2023-10-17 12:02:21.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/glue_databrew.py
--rw-r--r--   0 root         (0) root         (0)     1996 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/kinesis.py
--rw-r--r--   0 root         (0) root         (0)     8931 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     6338 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/logs.py
--rw-r--r--   0 root         (0) root         (0)     7097 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    15476 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/rds.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-09-01 12:43:02.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     8294 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)     7164 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/redshift_sql.py
--rw-r--r--   0 root         (0) root         (0)    57970 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/s3.py
--rw-r--r--   0 root         (0) root         (0)    56182 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2667 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     4146 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/ses.py
--rw-r--r--   0 root         (0) root         (0)     3435 2023-09-01 12:43:02.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/sns.py
--rw-r--r--   0 root         (0) root         (0)     3121 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/sqs.py
--rw-r--r--   0 root         (0) root         (0)     2393 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/ssm.py
--rw-r--r--   0 root         (0) root         (0)     3073 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/step_function.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/sts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.621716 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/links/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2946 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/links/base_aws.py
--rw-r--r--   0 root         (0) root         (0)     1770 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/links/batch.py
--rw-r--r--   0 root         (0) root         (0)     2555 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/links/emr.py
--rw-r--r--   0 root         (0) root         (0)     1229 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/links/glue.py
--rw-r--r--   0 root         (0) root         (0)     1608 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/links/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.624951 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6846 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
--rw-r--r--   0 root         (0) root         (0)     9605 2023-09-04 20:57:44.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/log/s3_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.628723 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/notifications/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2401 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/notifications/chime.py
--rw-r--r--   0 root         (0) root         (0)     3360 2023-09-01 12:43:02.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/notifications/sns.py
--rw-r--r--   0 root         (0) root         (0)     3850 2023-09-01 12:43:02.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/notifications/sqs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.657606 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19995 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/appflow.py
--rw-r--r--   0 root         (0) root         (0)     7175 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/athena.py
--rw-r--r--   0 root         (0) root         (0)     3649 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/base_aws.py
--rw-r--r--   0 root         (0) root         (0)    21145 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)     3633 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    18451 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/datasync.py
--rw-r--r--   0 root         (0) root         (0)    10715 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/dms.py
--rw-r--r--   0 root         (0) root         (0)     9591 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/ec2.py
--rw-r--r--   0 root         (0) root         (0)    32779 2023-10-17 12:02:21.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/ecs.py
--rw-r--r--   0 root         (0) root         (0)    49922 2023-09-14 06:07:27.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/eks.py
--rw-r--r--   0 root         (0) root         (0)    75097 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/emr.py
--rw-r--r--   0 root         (0) root         (0)     9015 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/eventbridge.py
--rw-r--r--   0 root         (0) root         (0)     3707 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/glacier.py
--rw-r--r--   0 root         (0) root         (0)     9960 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/glue.py
--rw-r--r--   0 root         (0) root         (0)     4358 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     4303 2023-10-17 12:02:21.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/glue_databrew.py
--rw-r--r--   0 root         (0) root         (0)    10464 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3968 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    39172 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/rds.py
--rw-r--r--   0 root         (0) root         (0)    32209 2023-08-10 18:31:30.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     5982 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)    30229 2023-09-14 06:07:27.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/s3.py
--rw-r--r--   0 root         (0) root         (0)    76744 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2960 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/sns.py
--rw-r--r--   0 root         (0) root         (0)     3565 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/sqs.py
--rw-r--r--   0 root         (0) root         (0)     6411 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.660253 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15540 2023-08-10 18:31:30.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/secrets/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     8495 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/secrets/systems_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.682553 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3286 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/athena.py
--rw-r--r--   0 root         (0) root         (0)     3642 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/base_aws.py
--rw-r--r--   0 root         (0) root         (0)    10647 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/batch.py
--rw-r--r--   0 root         (0) root         (0)     4586 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)     4469 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/dms.py
--rw-r--r--   0 root         (0) root         (0)     4422 2023-09-01 12:43:02.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     3950 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/ec2.py
--rw-r--r--   0 root         (0) root         (0)     7326 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/ecs.py
--rw-r--r--   0 root         (0) root         (0)     9839 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/eks.py
--rw-r--r--   0 root         (0) root         (0)    24432 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/emr.py
--rw-r--r--   0 root         (0) root         (0)     4346 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/glacier.py
--rw-r--r--   0 root         (0) root         (0)     3540 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/glue.py
--rw-r--r--   0 root         (0) root         (0)     5485 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
--rw-r--r--   0 root         (0) root         (0)     3274 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3255 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3761 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/quicksight.py
--rw-r--r--   0 root         (0) root         (0)     6434 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/rds.py
--rw-r--r--   0 root         (0) root         (0)     2732 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)    15706 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/s3.py
--rw-r--r--   0 root         (0) root         (0)    12977 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)    10336 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/sqs.py
--rw-r--r--   0 root         (0) root         (0)     3641 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.702972 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6987 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2850 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/base.py
--rw-r--r--   0 root         (0) root         (0)     8294 2023-10-17 12:02:21.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     6359 2023-09-01 12:43:02.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)    10406 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4702 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     9042 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4173 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     4233 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/local_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     5990 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8064 2023-09-01 12:43:02.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
--rw-r--r--   0 root         (0) root         (0)     8543 2023-08-10 18:31:30.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
--rw-r--r--   0 root         (0) root         (0)     3185 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
--rw-r--r--   0 root         (0) root         (0)     4938 2023-08-24 07:43:29.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/s3_to_sql.py
--rw-r--r--   0 root         (0) root         (0)     5679 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     3637 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     9141 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/sql_to_s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.720982 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2469 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/athena.py
--rw-r--r--   0 root         (0) root         (0)     6384 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/base.py
--rw-r--r--   0 root         (0) root         (0)    10850 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/batch.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/ec2.py
--rw-r--r--   0 root         (0) root         (0)     9051 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/ecs.py
--rw-r--r--   0 root         (0) root         (0)    16086 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/eks.py
--rw-r--r--   0 root         (0) root         (0)    17814 2023-09-12 06:55:02.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/emr.py
--rw-r--r--   0 root         (0) root         (0)     5923 2023-08-15 06:48:52.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/glue.py
--rw-r--r--   0 root         (0) root         (0)     2678 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     2368 2023-10-17 12:02:21.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/glue_databrew.py
--rw-r--r--   0 root         (0) root         (0)     2670 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)    10948 2023-09-14 06:07:27.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/rds.py
--rw-r--r--   0 root         (0) root         (0)    10760 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     9099 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/s3.py
--rw-r--r--   0 root         (0) root         (0)     7854 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     7751 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/sqs.py
--rw-r--r--   0 root         (0) root         (0)     2538 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.737302 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/
--rw-r--r--   0 root         (0) root         (0)     3303 2023-09-08 06:39:39.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22616 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/connection_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/eks_get_token.py
--rw-r--r--   0 root         (0) root         (0)     1854 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/emailer.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-08-25 12:06:52.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/identifiers.py
--rw-r--r--   0 root         (0) root         (0)     5914 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/mixins.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/rds.py
--rw-r--r--   0 root         (0) root         (0)     1952 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/redshift.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     3168 2023-09-04 20:57:44.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/sqs.py
--rw-r--r--   0 root         (0) root         (0)     2360 2023-10-17 12:02:21.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/suppress.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     4528 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/task_log_fetcher.py
--rw-r--r--   0 root         (0) root         (0)     3509 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/waiter.py
--rw-r--r--   0 root         (0) root         (0)     5892 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/waiter_with_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.752799 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1014 2023-08-24 07:43:29.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/appflow.json
--rw-r--r--   0 root         (0) root         (0)      892 2023-06-24 10:23:43.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/athena.json
--rw-r--r--   0 root         (0) root         (0)     1910 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/base_waiter.py
--rw-r--r--   0 root         (0) root         (0)     1206 2023-08-24 07:43:29.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/batch.json
--rw-r--r--   0 root         (0) root         (0)     1017 2023-10-17 12:02:21.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/databrew.json
--rw-r--r--   0 root         (0) root         (0)      895 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/dynamodb.json
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/ecs.json
--rw-r--r--   0 root         (0) root         (0)      659 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/eks.json
--rw-r--r--   0 root         (0) root         (0)      851 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/emr-containers.json
--rw-r--r--   0 root         (0) root         (0)     4893 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/emr-serverless.json
--rw-r--r--   0 root         (0) root         (0)     5299 2023-09-12 06:55:02.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/emr.json
--rw-r--r--   0 root         (0) root         (0)      932 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/glue.json
--rw-r--r--   0 root         (0) root         (0)     1742 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/redshift.json
--rw-r--r--   0 root         (0) root         (0)     5254 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/sagemaker.json
--rw-r--r--   0 root         (0) root         (0)     1034 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/stepfunctions.json
--rw-r--r--   0 root         (0) root         (0)    45240 2023-10-18 17:39:38.000000 apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:39:39.760175 apache-airflow-providers-amazon-8.9.0/apache_airflow_providers_amazon.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8006 2023-10-18 17:39:39.000000 apache-airflow-providers-amazon-8.9.0/apache_airflow_providers_amazon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9418 2023-10-18 17:39:39.000000 apache-airflow-providers-amazon-8.9.0/apache_airflow_providers_amazon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-18 17:39:39.000000 apache-airflow-providers-amazon-8.9.0/apache_airflow_providers_amazon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-10-18 17:39:39.000000 apache-airflow-providers-amazon-8.9.0/apache_airflow_providers_amazon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-18 17:39:39.000000 apache-airflow-providers-amazon-8.9.0/apache_airflow_providers_amazon.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      895 2023-10-18 17:39:39.000000 apache-airflow-providers-amazon-8.9.0/apache_airflow_providers_amazon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-10-18 17:39:39.000000 apache-airflow-providers-amazon-8.9.0/apache_airflow_providers_amazon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     6076 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2130 2023-10-18 17:39:39.762038 apache-airflow-providers-amazon-8.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2571 2023-10-18 17:39:38.000000 apache-airflow-providers-amazon-8.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.819160 apache-airflow-providers-amazon-8.9.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.9.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-10-18 17:43:05.000000 apache-airflow-providers-amazon-8.9.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.9.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8012 2023-10-18 17:43:06.819412 apache-airflow-providers-amazon-8.9.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5999 2023-10-18 17:43:05.000000 apache-airflow-providers-amazon-8.9.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.617802 apache-airflow-providers-amazon-8.9.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.617970 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.630742 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-10-18 17:38:08.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.633214 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.675822 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5415 2023-09-01 12:43:02.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/appflow.py
+-rw-r--r--   0 root         (0) root         (0)    12395 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/athena.py
+-rw-r--r--   0 root         (0) root         (0)    47899 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)    21345 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json
+-rw-r--r--   0 root         (0) root         (0)    10579 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2023-09-08 06:39:39.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/chime.py
+-rw-r--r--   0 root         (0) root         (0)     3435 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    13592 2023-09-12 06:55:02.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/datasync.py
+-rw-r--r--   0 root         (0) root         (0)     7903 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/dms.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-08-25 12:06:52.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     7928 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     3759 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/ecr.py
+-rw-r--r--   0 root         (0) root         (0)     6666 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    23925 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/eks.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
+-rw-r--r--   0 root         (0) root         (0)    21401 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3364 2023-08-09 10:37:33.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/eventbridge.py
+-rw-r--r--   0 root         (0) root         (0)     3452 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/glacier.py
+-rw-r--r--   0 root         (0) root         (0)    16819 2023-08-16 10:11:24.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/glue.py
+-rw-r--r--   0 root         (0) root         (0)     9212 2023-08-15 06:48:52.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py
+-rw-r--r--   0 root         (0) root         (0)     7926 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     2580 2023-10-17 12:02:21.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/glue_databrew.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py
+-rw-r--r--   0 root         (0) root         (0)     8931 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     6338 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/logs.py
+-rw-r--r--   0 root         (0) root         (0)     7097 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    15476 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/rds.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-09-01 12:43:02.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     8294 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py
+-rw-r--r--   0 root         (0) root         (0)    57970 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/s3.py
+-rw-r--r--   0 root         (0) root         (0)    56182 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4146 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/ses.py
+-rw-r--r--   0 root         (0) root         (0)     3435 2023-09-01 12:43:02.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/ssm.py
+-rw-r--r--   0 root         (0) root         (0)     3073 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/step_function.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/sts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.681221 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/links/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/links/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/links/batch.py
+-rw-r--r--   0 root         (0) root         (0)     2555 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/links/emr.py
+-rw-r--r--   0 root         (0) root         (0)     1229 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/links/glue.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/links/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.684203 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6846 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
+-rw-r--r--   0 root         (0) root         (0)     9605 2023-09-04 20:57:44.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.688265 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/notifications/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2401 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/notifications/chime.py
+-rw-r--r--   0 root         (0) root         (0)     3360 2023-09-01 12:43:02.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/notifications/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3850 2023-09-01 12:43:02.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/notifications/sqs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.717837 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19995 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/appflow.py
+-rw-r--r--   0 root         (0) root         (0)     7175 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/athena.py
+-rw-r--r--   0 root         (0) root         (0)     3649 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)    21145 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    18451 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/datasync.py
+-rw-r--r--   0 root         (0) root         (0)    10715 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/dms.py
+-rw-r--r--   0 root         (0) root         (0)     9591 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/ec2.py
+-rw-r--r--   0 root         (0) root         (0)    32779 2023-10-17 12:02:21.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    49922 2023-09-14 06:07:27.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/eks.py
+-rw-r--r--   0 root         (0) root         (0)    75097 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/emr.py
+-rw-r--r--   0 root         (0) root         (0)     9015 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/eventbridge.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     9960 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/glue.py
+-rw-r--r--   0 root         (0) root         (0)     4358 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     4303 2023-10-17 12:02:21.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/glue_databrew.py
+-rw-r--r--   0 root         (0) root         (0)    10464 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3968 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    39172 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/rds.py
+-rw-r--r--   0 root         (0) root         (0)    32209 2023-08-10 18:31:30.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)    30229 2023-09-14 06:07:27.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/s3.py
+-rw-r--r--   0 root         (0) root         (0)    76744 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     6411 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.720885 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15540 2023-08-10 18:31:30.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8495 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.745164 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/athena.py
+-rw-r--r--   0 root         (0) root         (0)     3642 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)    10647 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/batch.py
+-rw-r--r--   0 root         (0) root         (0)     4586 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)     4469 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/dms.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-09-01 12:43:02.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     3950 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     9839 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/eks.py
+-rw-r--r--   0 root         (0) root         (0)    24432 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/emr.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/glue.py
+-rw-r--r--   0 root         (0) root         (0)     5485 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
+-rw-r--r--   0 root         (0) root         (0)     3274 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3255 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3761 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)     6434 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/rds.py
+-rw-r--r--   0 root         (0) root         (0)     2732 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    15706 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/s3.py
+-rw-r--r--   0 root         (0) root         (0)    12977 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)    10336 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2023-09-22 19:16:56.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.765429 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6987 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/base.py
+-rw-r--r--   0 root         (0) root         (0)     8294 2023-10-17 12:02:21.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-09-01 12:43:02.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)    10406 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4702 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     9042 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4173 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8064 2023-09-01 12:43:02.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
+-rw-r--r--   0 root         (0) root         (0)     8543 2023-08-10 18:31:30.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
+-rw-r--r--   0 root         (0) root         (0)     3185 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
+-rw-r--r--   0 root         (0) root         (0)     4938 2023-08-24 07:43:29.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     3637 2023-08-15 06:48:24.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     9141 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.782674 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2469 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/athena.py
+-rw-r--r--   0 root         (0) root         (0)     6384 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/base.py
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/batch.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     9051 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    16086 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/eks.py
+-rw-r--r--   0 root         (0) root         (0)    17814 2023-09-12 06:55:02.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/emr.py
+-rw-r--r--   0 root         (0) root         (0)     5923 2023-08-15 06:48:52.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/glue.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     2368 2023-10-17 12:02:21.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/glue_databrew.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)    10948 2023-09-14 06:07:27.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/rds.py
+-rw-r--r--   0 root         (0) root         (0)    10760 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     9099 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/s3.py
+-rw-r--r--   0 root         (0) root         (0)     7854 2023-09-21 10:53:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     7751 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.796741 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/
+-rw-r--r--   0 root         (0) root         (0)     3303 2023-09-08 06:39:39.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22616 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/emailer.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-08-25 12:06:52.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/identifiers.py
+-rw-r--r--   0 root         (0) root         (0)     5914 2023-10-13 10:07:37.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/mixins.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/rds.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/redshift.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     3168 2023-09-04 20:57:44.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     2360 2023-10-17 12:02:21.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/suppress.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     4528 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/task_log_fetcher.py
+-rw-r--r--   0 root         (0) root         (0)     3509 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/waiter.py
+-rw-r--r--   0 root         (0) root         (0)     5892 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/waiter_with_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.811682 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-08-24 07:43:29.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/appflow.json
+-rw-r--r--   0 root         (0) root         (0)      892 2023-06-24 10:23:43.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/athena.json
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-08-29 07:00:04.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     1206 2023-08-24 07:43:29.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/batch.json
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-10-17 12:02:21.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/databrew.json
+-rw-r--r--   0 root         (0) root         (0)      895 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/dynamodb.json
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/ecs.json
+-rw-r--r--   0 root         (0) root         (0)      659 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/eks.json
+-rw-r--r--   0 root         (0) root         (0)      851 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/emr-containers.json
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/emr-serverless.json
+-rw-r--r--   0 root         (0) root         (0)     5299 2023-09-12 06:55:02.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/emr.json
+-rw-r--r--   0 root         (0) root         (0)      932 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/glue.json
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/redshift.json
+-rw-r--r--   0 root         (0) root         (0)     5254 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/sagemaker.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/stepfunctions.json
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-10-18 17:43:05.000000 apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:06.818333 apache-airflow-providers-amazon-8.9.0rc1/apache_airflow_providers_amazon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8012 2023-10-18 17:43:06.000000 apache-airflow-providers-amazon-8.9.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9418 2023-10-18 17:43:06.000000 apache-airflow-providers-amazon-8.9.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-18 17:43:06.000000 apache-airflow-providers-amazon-8.9.0rc1/apache_airflow_providers_amazon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-10-18 17:43:06.000000 apache-airflow-providers-amazon-8.9.0rc1/apache_airflow_providers_amazon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-18 17:43:06.000000 apache-airflow-providers-amazon-8.9.0rc1/apache_airflow_providers_amazon.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      905 2023-10-18 17:43:06.000000 apache-airflow-providers-amazon-8.9.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-10-18 17:43:06.000000 apache-airflow-providers-amazon-8.9.0rc1/apache_airflow_providers_amazon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     6076 2023-10-01 07:10:43.000000 apache-airflow-providers-amazon-8.9.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-10-18 17:43:06.820294 apache-airflow-providers-amazon-8.9.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-10-18 17:43:05.000000 apache-airflow-providers-amazon-8.9.0rc1/setup.py
```

### Comparing `apache-airflow-providers-amazon-8.9.0/LICENSE` & `apache-airflow-providers-amazon-8.9.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/MANIFEST.in` & `apache-airflow-providers-amazon-8.9.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/PKG-INFO` & `apache-airflow-providers-amazon-8.9.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 8.9.0
+Version: 8.9.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.9.0/
@@ -81,15 +81,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.9.0``
+Release: ``8.9.0rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-amazon-8.9.0/README.rst` & `apache-airflow-providers-amazon-8.9.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.9.0``
+Release: ``8.9.0rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/__init__.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/__init__.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/exceptions.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/__init__.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/appflow.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/athena.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/base_aws.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/batch_client.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/batch_waiters.json` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/batch_waiters.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/chime.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/chime.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/cloud_formation.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/datasync.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/dms.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/dynamodb.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/ec2.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/ecr.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/ecr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/ecs.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/eks.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/emr.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/eventbridge.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/eventbridge.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/glacier.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/glue.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/glue_catalog.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/glue_crawler.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/glue_databrew.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/glue_databrew.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/kinesis.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/lambda_function.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/logs.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/quicksight.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/rds.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/redshift_cluster.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/redshift_data.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/redshift_sql.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/sagemaker.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/secrets_manager.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/ses.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/ses.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/sns.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/sqs.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/ssm.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/ssm.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/step_function.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/hooks/sts.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/hooks/sts.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/links/__init__.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/links/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/links/base_aws.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/links/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/links/batch.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/links/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/links/emr.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/links/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/links/glue.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/links/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/links/logs.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/links/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/log/__init__.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/log/s3_task_handler.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/notifications/__init__.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/notifications/chime.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/notifications/chime.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/notifications/sns.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/notifications/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/notifications/sqs.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/notifications/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/__init__.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/appflow.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/athena.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/base_aws.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/batch.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/cloud_formation.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/datasync.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/dms.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/ec2.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/ecs.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/eks.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/emr.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/eventbridge.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/eventbridge.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/glacier.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/glue.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/glue_crawler.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/glue_databrew.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/glue_databrew.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/lambda_function.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/quicksight.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/rds.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/redshift_cluster.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/redshift_data.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/sagemaker.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/sns.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/sqs.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/operators/step_function.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/operators/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/secrets/__init__.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/secrets/secrets_manager.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/secrets/systems_manager.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/__init__.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/athena.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/base_aws.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/batch.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/cloud_formation.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/dms.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/dynamodb.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/ec2.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/ecs.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/eks.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/emr.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/glacier.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/glue.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/glue_crawler.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/lambda_function.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/quicksight.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/rds.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/redshift_cluster.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/sagemaker.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/sqs.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/sensors/step_function.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/sensors/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/__init__.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/base.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/exasol_to_s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/ftp_to_s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/gcs_to_s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/google_api_to_s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/local_to_s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/mongo_to_s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/redshift_to_s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/s3_to_ftp.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/s3_to_redshift.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/s3_to_sftp.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/s3_to_sql.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/sftp_to_s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/transfers/sql_to_s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/__init__.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/athena.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/base.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/batch.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/ec2.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/ecs.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/eks.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/emr.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/glue.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/glue_crawler.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/glue_databrew.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/glue_databrew.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/lambda_function.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/rds.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/redshift_cluster.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/s3.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/sagemaker.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/sqs.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/triggers/step_function.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/triggers/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/__init__.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/connection_wrapper.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/eks_get_token.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/emailer.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/emailer.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/identifiers.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/identifiers.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/mixins.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/mixins.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/rds.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/redshift.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/sagemaker.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/sqs.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/suppress.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/suppress.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/tags.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/tags.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/task_log_fetcher.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/task_log_fetcher.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/waiter.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/utils/waiter_with_logging.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/utils/waiter_with_logging.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/__init__.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/appflow.json` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/appflow.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/athena.json` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/athena.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/base_waiter.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/batch.json` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/batch.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/databrew.json` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/databrew.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/dynamodb.json` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/dynamodb.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/ecs.json` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/ecs.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/eks.json` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/eks.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/emr-containers.json` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/emr-containers.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/emr-serverless.json` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/emr-serverless.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/emr.json` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/emr.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/glue.json` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/glue.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/redshift.json` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/redshift.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/sagemaker.json` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/sagemaker.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/aws/waiters/stepfunctions.json` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/aws/waiters/stepfunctions.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/airflow/providers/amazon/get_provider_info.py` & `apache-airflow-providers-amazon-8.9.0rc1/airflow/providers/amazon/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/apache_airflow_providers_amazon.egg-info/PKG-INFO` & `apache-airflow-providers-amazon-8.9.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 8.9.0
+Version: 8.9.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.9.0/
@@ -81,15 +81,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.9.0``
+Release: ``8.9.0rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-amazon-8.9.0/apache_airflow_providers_amazon.egg-info/SOURCES.txt` & `apache-airflow-providers-amazon-8.9.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/apache_airflow_providers_amazon.egg-info/requires.txt` & `apache-airflow-providers-amazon-8.9.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-apache-airflow-providers-common-sql>=1.3.1
+apache-airflow-providers-common-sql>=1.3.1.dev0
 apache-airflow-providers-http
-apache-airflow>=2.5.0
+apache-airflow>=2.5.0.dev0
 asgiref
 boto3>=1.28.0
 botocore>=1.31.0
 jsonpath_ng>=1.5.3
 redshift_connector>=2.0.888
 sqlalchemy_redshift>=0.8.6
 watchtower~=3.0.1
```

### Comparing `apache-airflow-providers-amazon-8.9.0/pyproject.toml` & `apache-airflow-providers-amazon-8.9.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.9.0/setup.cfg` & `apache-airflow-providers-amazon-8.9.0rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow-providers-common-sql>=1.3.1
+	apache-airflow-providers-common-sql>=1.3.1.dev0
 	apache-airflow-providers-http
-	apache-airflow>=2.5.0
+	apache-airflow>=2.5.0.dev0
 	asgiref
 	boto3>=1.28.0
 	botocore>=1.31.0
 	jsonpath_ng>=1.5.3
 	redshift_connector>=2.0.888
 	sqlalchemy_redshift>=0.8.6
 	watchtower~=3.0.1
@@ -62,10 +62,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.amazon.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.amazon
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-amazon-8.9.0/setup.py` & `apache-airflow-providers-amazon-8.9.0rc1/setup.py`

 * *Files identical despite different names*

