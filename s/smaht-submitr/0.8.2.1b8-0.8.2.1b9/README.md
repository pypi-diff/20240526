# Comparing `tmp/smaht_submitr-0.8.2.1b8.tar.gz` & `tmp/smaht_submitr-0.8.2.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.8.2.1b8.tar", max compression
+gzip compressed data, was "smaht_submitr-0.8.2.1b9.tar", max compression
```

## Comparing `smaht_submitr-0.8.2.1b8.tar` & `smaht_submitr-0.8.2.1b9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1098 2024-05-19 01:57:37.499175 smaht_submitr-0.8.2.1b8/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-05-19 01:57:37.499175 smaht_submitr-0.8.2.1b8/README.rst
--rw-r--r--   0        0        0     3465 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/base.py
--rw-r--r--   0        0        0      294 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/exceptions.py
--rw-r--r--   0        0        0    17885 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/file_for_upload.py
--rw-r--r--   0        0        0    11097 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/metadata_template.py
--rw-r--r--   0        0        0     2628 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/output.py
--rw-r--r--   0        0        0      353 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/__init__.py
--rw-r--r--   0        0        0     6343 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_amazon.py
--rw-r--r--   0        0        0     9391 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_commands.py
--rw-r--r--   0        0        0     6986 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_config.py
--rw-r--r--   0        0        0     9916 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_google.py
--rw-r--r--   0        0        0     5152 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_installation.py
--rw-r--r--   0        0        0     3348 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_utils.py
--rw-r--r--   0        0        0    11817 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/rcloner.py
--rw-r--r--   0        0        0    19885 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/testing/rclone_utils_for_testing_amazon.py
--rw-r--r--   0        0        0     8157 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/testing/rclone_utils_for_testing_google.py
--rw-r--r--   0        0        0    17135 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/s3_upload.py
--rw-r--r--   0        0        0     3512 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     4779 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     9895 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     2824 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/get_metadata_template.py
--rw-r--r--   0        0        0     1822 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5483 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/rcloner.py
--rw-r--r--   0        0        0     7143 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    21810 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   127795 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/submission.py
--rw-r--r--   0        0        0    14817 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/submission_uploads.py
--rw-r--r--   0        0        0        0 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0     6395 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/data/ingestion_submission.json
--rw-r--r--   0        0        0  1032804 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/data/profiles.json
--rw-r--r--   0        0        0      272 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0    12067 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_file_for_upload.py
--rw-r--r--   0        0        0     1620 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    48503 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_rclone_support.py
--rw-r--r--   0        0        0    11766 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0    37993 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     4353 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0     5085 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/testing_rclone_helpers.py
--rw-r--r--   0        0        0     8677 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/utils.py
--rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 smaht_submitr-0.8.2.1b8/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-05-19 15:27:56.519499 smaht_submitr-0.8.2.1b9/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-05-19 15:27:56.519499 smaht_submitr-0.8.2.1b9/README.rst
+-rw-r--r--   0        0        0     3465 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/exceptions.py
+-rw-r--r--   0        0        0    17885 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/file_for_upload.py
+-rw-r--r--   0        0        0    11097 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/metadata_template.py
+-rw-r--r--   0        0        0     2628 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/output.py
+-rw-r--r--   0        0        0      353 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/rclone/__init__.py
+-rw-r--r--   0        0        0     6343 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/rclone/rclone_amazon.py
+-rw-r--r--   0        0        0     9391 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/rclone/rclone_commands.py
+-rw-r--r--   0        0        0     6986 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/rclone/rclone_config.py
+-rw-r--r--   0        0        0     9916 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/rclone/rclone_google.py
+-rw-r--r--   0        0        0     5152 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/rclone/rclone_installation.py
+-rw-r--r--   0        0        0     3348 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/rclone/rclone_utils.py
+-rw-r--r--   0        0        0    11817 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/rclone/rcloner.py
+-rw-r--r--   0        0        0    19965 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/rclone/testing/rclone_utils_for_testing_amazon.py
+-rw-r--r--   0        0        0     8157 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/rclone/testing/rclone_utils_for_testing_google.py
+-rw-r--r--   0        0        0    17135 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/s3_upload.py
+-rw-r--r--   0        0        0     3512 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     4779 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     9895 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     2824 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/scripts/get_metadata_template.py
+-rw-r--r--   0        0        0     1822 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5483 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/scripts/rcloner.py
+-rw-r--r--   0        0        0     7143 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    21810 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-05-19 15:27:56.559499 smaht_submitr-0.8.2.1b9/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   127795 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/submission.py
+-rw-r--r--   0        0        0    14817 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/submission_uploads.py
+-rw-r--r--   0        0        0        0 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0     6395 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/data/ingestion_submission.json
+-rw-r--r--   0        0        0  1032804 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/data/profiles.json
+-rw-r--r--   0        0        0      272 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0    12067 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/test_file_for_upload.py
+-rw-r--r--   0        0        0     1620 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    49678 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/test_rclone_support.py
+-rw-r--r--   0        0        0    11766 2024-05-19 15:27:56.563499 smaht_submitr-0.8.2.1b9/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0    37993 2024-05-19 15:27:56.567499 smaht_submitr-0.8.2.1b9/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-05-19 15:27:56.567499 smaht_submitr-0.8.2.1b9/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-05-19 15:27:56.567499 smaht_submitr-0.8.2.1b9/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-05-19 15:27:56.567499 smaht_submitr-0.8.2.1b9/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-05-19 15:27:56.567499 smaht_submitr-0.8.2.1b9/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     4353 2024-05-19 15:27:56.567499 smaht_submitr-0.8.2.1b9/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-05-19 15:27:56.567499 smaht_submitr-0.8.2.1b9/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0     5085 2024-05-19 15:27:56.567499 smaht_submitr-0.8.2.1b9/submitr/tests/testing_rclone_helpers.py
+-rw-r--r--   0        0        0     8677 2024-05-19 15:27:56.567499 smaht_submitr-0.8.2.1b9/submitr/utils.py
+-rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 smaht_submitr-0.8.2.1b9/PKG-INFO
```

### Comparing `smaht_submitr-0.8.2.1b8/LICENSE.txt` & `smaht_submitr-0.8.2.1b9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/README.rst` & `smaht_submitr-0.8.2.1b9/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/pyproject.toml` & `smaht_submitr-0.8.2.1b9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.8.2.1b8"  # TODO: To become 0.8.3
+version = "0.8.2.1b9"  # TODO: To become 0.8.3
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
```

### Comparing `smaht_submitr-0.8.2.1b8/submitr/base.py` & `smaht_submitr-0.8.2.1b9/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/file_for_upload.py` & `smaht_submitr-0.8.2.1b9/submitr/file_for_upload.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/metadata_template.py` & `smaht_submitr-0.8.2.1b9/submitr/metadata_template.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/output.py` & `smaht_submitr-0.8.2.1b9/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_amazon.py` & `smaht_submitr-0.8.2.1b9/submitr/rclone/rclone_amazon.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_commands.py` & `smaht_submitr-0.8.2.1b9/submitr/rclone/rclone_commands.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_config.py` & `smaht_submitr-0.8.2.1b9/submitr/rclone/rclone_config.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_google.py` & `smaht_submitr-0.8.2.1b9/submitr/rclone/rclone_google.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_installation.py` & `smaht_submitr-0.8.2.1b9/submitr/rclone/rclone_installation.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_utils.py` & `smaht_submitr-0.8.2.1b9/submitr/rclone/rclone_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/rclone/rcloner.py` & `smaht_submitr-0.8.2.1b9/submitr/rclone/rcloner.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/rclone/testing/rclone_utils_for_testing_amazon.py` & `smaht_submitr-0.8.2.1b9/submitr/rclone/testing/rclone_utils_for_testing_amazon.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,15 +333,15 @@
                 "aws_access_key_id": self.access_key_id,
                 "aws_secret_access_key": self.secret_access_key,
                 "aws_session_token": self.session_token
             }
 
     @staticmethod
     def from_file(credentials_file: str, credentials_section: str = None,
-                  kms_key_id: Optional[str] = None) -> Optional[AwsCredentials]:
+                  region: Optional[str] = None, kms_key_id: Optional[str] = None) -> Optional[AwsCredentials]:
         if not credentials_section:
             credentials_section = "default"
         try:
             credentials_file = normalize_path(credentials_file, expand_home=True)
             if not os.path.isfile(credentials_file):
                 if os.path.isdir(credentials_file):
                     credentials_file = os.path.join(credentials_file, "credentials")
@@ -349,15 +349,16 @@
                     credentials_file = os.path.join("~", f".aws_test.{credentials_file}", "credentials")
                     credentials_file = normalize_path(credentials_file, expand_home=True)
                 if not os.path.isfile(credentials_file):
                     return None
             config = configparser.ConfigParser()
             config.read(os.path.expanduser(credentials_file))
             section = config[credentials_section]
-            region = (section.get("region", None) or
+            region = (normalize_string(region) or
+                      section.get("region", None) or
                       section.get("region_name", None) or
                       section.get("aws_default_region", None))
             access_key_id = (section.get("aws_access_key_id", None) or
                              section.get("access_key_id", None))
             secret_access_key = (section.get("aws_secret_access_key", None) or
                                  section.get("secret_access_key", None))
             session_token = (section.get("aws_session_token", None) or
```

### Comparing `smaht_submitr-0.8.2.1b8/submitr/rclone/testing/rclone_utils_for_testing_google.py` & `smaht_submitr-0.8.2.1b9/submitr/rclone/testing/rclone_utils_for_testing_google.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/s3_upload.py` & `smaht_submitr-0.8.2.1b9/submitr/s3_upload.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/s3_utils.py` & `smaht_submitr-0.8.2.1b9/submitr/s3_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/scripts/check_submission.py` & `smaht_submitr-0.8.2.1b9/submitr/scripts/check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/scripts/cli_utils.py` & `smaht_submitr-0.8.2.1b9/submitr/scripts/cli_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/scripts/get_metadata_template.py` & `smaht_submitr-0.8.2.1b9/submitr/scripts/get_metadata_template.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/scripts/list_submissions.py` & `smaht_submitr-0.8.2.1b9/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.8.2.1b9/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/scripts/rcloner.py` & `smaht_submitr-0.8.2.1b9/submitr/scripts/rcloner.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.8.2.1b9/submitr/scripts/resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.8.2.1b9/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.8.2.1b9/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.8.2.1b9/submitr/scripts/submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.8.2.1b9/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.8.2.1b9/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.8.2.1b9/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/submission.py` & `smaht_submitr-0.8.2.1b9/submitr/submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/submission_uploads.py` & `smaht_submitr-0.8.2.1b9/submitr/submission_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/data/ingestion_submission.json` & `smaht_submitr-0.8.2.1b9/submitr/tests/data/ingestion_submission.json`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/data/profiles.json` & `smaht_submitr-0.8.2.1b9/submitr/tests/data/profiles.json`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.8.2.1b9/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.8.2.1b9/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.8.2.1b9/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.8.2.1b9/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/test_base.py` & `smaht_submitr-0.8.2.1b9/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/test_check_submission.py` & `smaht_submitr-0.8.2.1b9/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/test_exceptions.py` & `smaht_submitr-0.8.2.1b9/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/test_file_for_upload.py` & `smaht_submitr-0.8.2.1b9/submitr/tests/test_file_for_upload.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.8.2.1b9/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/test_misc.py` & `smaht_submitr-0.8.2.1b9/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/test_rclone_support.py` & `smaht_submitr-0.8.2.1b9/submitr/tests/test_rclone_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,45 +27,54 @@
     setup_module as rclone_setup_module, teardown_module as rclone_teardown_module,
     load_test_data_json, Mock_LocalStorage, Mock_Portal, RANDOM_TMPFILE_SIZE)
 
 
 pytestmark = pytest.mark.integration
 
 
-# Integration tests for RCloner related functionality within smaht-submitr.
-# Need valid AWS credentials (currently for: smaht-wolf).
-# Need valid Google Cloud credentials (currently for: smaht-dac).
-# With these to variables set to True to default to getting credentials
-# from environment variables (as is done in GA), these are the environment
-# variables that need to be set:
-# - AWS_ACCESS_KEY_ID (required)
-# - AWS_SECRET_ACCESS_KEY (required)
-# - AWS_SESSION_TOKEN (optional)
-# - AWS_KMS_KEY_ID (optional / not a standard AWS variable fyi / and actually not secret)
-# - GOOGLE_CLOUD_SERVICE_ACCOUNT_JSON (required / JSON text for GCP service account file)
-AMAZON_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES = True
-GOOGLE_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES = True
-
-# If environment variables are not set for credentials (as the should be in GA)
-# then these are two things likely needing updates for running locally:
-# - The AWS environment-name (per use_test_creds).
-#   I.e. e.g. load AWS credentials from: ~/.aws_test.{environment-name}/credentials
-# - The Google service-account-file path.
-#   As exported from Google account.
+# This integration test actually talks to AWS S3 and Google Cloud Storage (GCS);
+# both directly (via Python boto3 and google.cloud.storage) and via rclone.
+# The access credentials are defined by the variables as described below.
+
+# If running from within GitHub actions these environment variables assumed to be
+# setup; via .github/workflows/main-integration-tests.yml file and GitHub secrets.
+#
+# These are setup in GitHub as "secrets". The AWS access key values are currently,
+# May 2024, for the special user test-integration-user in the smaht-wolf account;
+# the access key was created on 2024-05-15. The Google value is the JSON from the
+# service account file exported from the HMS Google account for the smaht-dac project;
+# the service account email is ga4-service-account@smaht-dac.iam.gserviceaccount.com;
+# its key ID is b488dd9cfde6b59b1aa347aabd9add86c7ff9057; it was created on 2024-04-28.
+#
+# - AWS_ACCESS_KEY_ID
+# - AWS_SECRET_ACCESS_KEY
+# - GOOGLE_CLOUD_SERVICE_ACCOUNT_JSON
+
+# If NOT running from within GitHub actions (i.e. locally) these variables assumed to be setup.
+#
+# - AMAZON_CREDENTIALS_FILE_PATH
+#   Full path to your AWS credentials file (e.g. ~/.aws_test.smaht-wolf/credentials).
+# - GOOGLE_SERVICE_ACCOUNT_FILE_PATH
+#   Full path to GCP credential "service account file" exported from Google account.
 AMAZON_CREDENTIALS_FILE_PATH = "~/.aws_test.smaht-test/credentials"
 GOOGLE_SERVICE_ACCOUNT_FILE_PATH = "~/.config/google-cloud/smaht-dac-617e0480d8e2.json"
 
-# These are slightly less likely to need updates for running locally (or in GA):
+# These credentials related values are less likely to need updating and are thus hard-coded here.
 AMAZON_TEST_BUCKET_NAME = "smaht-unit-testing-files"
+AMAZON_REGION = "us-east-1"
 AMAZON_KMS_KEY_ID = "27d040a3-ead1-4f5a-94ce-0fa6e7f84a95"  # not secret fyi
-GOOGLE_ACCOUNT_NAME = "smaht-dac"
 GOOGLE_TEST_BUCKET_NAME = "smaht-submitr-rclone-testing"
 GOOGLE_LOCATION = "us-east1"
 
 
+def is_github_actions_context():
+    # Returns True iff we are running within GitHub Actions.
+    return "GITHUB_ACTIONS" in os.environ
+
+
 class Env:
 
     test_file_prefix = "test-smaht-submitr-"
     test_file_suffix = ".txt"
     test_file_size = 2048
 
     def __init__(self, use_cloud_subfolder_key: bool = False):
@@ -92,25 +101,27 @@
 
     class CredentialsType(Enum):
         TEMPORARY = "temporary"
         TEMPORARY_KEY_SPECIFIC = "temporary-key-specific"
 
     def __init__(self, use_cloud_subfolder_key: bool = False):
         super().__init__(use_cloud_subfolder_key=use_cloud_subfolder_key)
-        self.kms_key_id = AMAZON_KMS_KEY_ID
+        self.credentials_file = AMAZON_CREDENTIALS_FILE_PATH
         self.bucket = AMAZON_TEST_BUCKET_NAME
+        self.region = AMAZON_REGION
+        self.kms_key_id = AMAZON_KMS_KEY_ID
         self.main_credentials = self.credentials()
 
     def credentials(self, nokms: bool = False) -> AmazonCredentials:
-        kms_key_id = None if nokms is True else self.kms_key_id
-        credentials = AwsCredentials.from_file(AMAZON_CREDENTIALS_FILE_PATH, kms_key_id=kms_key_id)
+        credentials = AwsCredentials.from_file(self.credentials_file,
+                                               region=self.region,
+                                               kms_key_id=None if nokms is True else self.kms_key_id)
         assert isinstance(credentials.region, str) and credentials.region
         assert isinstance(credentials.access_key_id, str) and credentials.access_key_id
         assert isinstance(credentials.secret_access_key, str) and credentials.secret_access_key
-        assert credentials.kms_key_id == (None if nokms is True else self.kms_key_id)
         return credentials
 
     def temporary_credentials(self,
                               bucket: Optional[str] = None, key: Optional[str] = None,
                               nokms: bool = False) -> AmazonCredentials:
         s3 = self.s3_non_rclone()
         kms_key_id = None if nokms else self.kms_key_id
@@ -123,88 +134,105 @@
         return AwsS3(self.main_credentials)
 
 
 class EnvGoogle(Env):
 
     def __init__(self, use_cloud_subfolder_key: bool = False):
         super().__init__(use_cloud_subfolder_key=use_cloud_subfolder_key)
-        self.location = GOOGLE_LOCATION
         self.service_account_file = GOOGLE_SERVICE_ACCOUNT_FILE_PATH
-        self.project_id = GOOGLE_ACCOUNT_NAME
         self.bucket = GOOGLE_TEST_BUCKET_NAME
+        self.location = GOOGLE_LOCATION
+        self.main_credentials = self.credentials()
 
     def credentials(self) -> GoogleCredentials:
         credentials = GcpCredentials.from_file(self.service_account_file, location=self.location)
         assert (credentials is not None) or RCloneGoogle.is_google_compute_engine()
         if credentials is not None:
             assert credentials.location == self.location
             assert credentials.service_account_file == normalize_path(self.service_account_file, expand_home=True)
             assert os.path.isfile(credentials.service_account_file)
         return credentials
 
     def gcs_non_rclone(self):
-        return Gcs(self.credentials())
+        return Gcs(self.main_credentials)
 
 
 def setup_module():
 
     rclone_setup_module()
 
-    global AMAZON_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES
-    global GOOGLE_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES
     global AMAZON_CREDENTIALS_FILE_PATH
     global GOOGLE_SERVICE_ACCOUNT_FILE_PATH
 
     assert RCloneInstallation.install() is not None
     assert RCloneInstallation.is_installed() is True
 
-    if AMAZON_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES:
-        amazon_credentials_file_path = create_temporary_file_name()
-        region = os.environ.get("AWS_DEFAULT_REGION", None)
+    if is_github_actions_context():
+        print("\nRunning in GitHub Actions")
+    else:
+        print("\nNot running in GitHub Actions")
+    if RCloneGoogle.is_google_compute_engine():
+        print("Running on a Google Compute Engine")
+    else:
+        print("Not running on a Google Compute Engine")
+
+    if is_github_actions_context():
         access_key_id = os.environ.get("AWS_ACCESS_KEY_ID", None)
         secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY", None)
         session_token = os.environ.get("AWS_SESSION_TOKEN", None)
-        if access_key_id and secret_access_key:
-            with open(amazon_credentials_file_path, "w") as f:
-                f.write(f"[default]\n")
-                f.write(f"aws_default_region={region}\n") if region else None
-                f.write(f"aws_access_key_id={access_key_id}\n")
-                f.write(f"aws_secret_access_key={secret_access_key}\n")
-                f.write(f"aws_session_token={session_token}\n") if session_token else None
-            os.chmod(amazon_credentials_file_path, 0o600)  # for security
-            AMAZON_CREDENTIALS_FILE_PATH = amazon_credentials_file_path
-    if not (AMAZON_CREDENTIALS_FILE_PATH and
-            os.path.isfile(normalize_path(AMAZON_CREDENTIALS_FILE_PATH, expand_home=True))):
-        print("No Amazon credentials file defined. Skippping this test module: test_rclone_support")
-        pytest.skip()
-
-    if GOOGLE_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES:
-        if service_account_json_string := os.environ.get("GOOGLE_CLOUD_SERVICE_ACCOUNT_JSON"):
-            service_account_json = json.loads(service_account_json_string)
-            google_service_account_file_path = create_temporary_file_name(suffix=".json")
-            with open(google_service_account_file_path, "w") as f:
-                json.dump(service_account_json, f)
-            os.chmod(google_service_account_file_path, 0o600)  # for security
-            GOOGLE_SERVICE_ACCOUNT_FILE_PATH = google_service_account_file_path
-    if not (GOOGLE_SERVICE_ACCOUNT_FILE_PATH and
-            os.path.isfile(normalize_path(GOOGLE_SERVICE_ACCOUNT_FILE_PATH, expand_home=True))):
-        if not RCloneGoogle.is_google_compute_engine():
-            print("No Google credentials file defined. Skippping this test module: test_rclone_support")
-            pytest.skip()
-            return
-        # Google credentials can be None on a GCE instance; i.e. no service account file needed.
-        GOOGLE_SERVICE_ACCOUNT_FILE_PATH = None
+        if not (access_key_id and secret_access_key):
+            pytest.fail("Integration test setup error: AWS acesss keys not defined!")
+        AMAZON_CREDENTIALS_FILE_PATH = create_temporary_file_name()
+        with open(AMAZON_CREDENTIALS_FILE_PATH, "w") as f:
+            f.write(f"[default]\n")
+            f.write(f"aws_access_key_id={access_key_id}\n")
+            f.write(f"aws_secret_access_key={secret_access_key}\n")
+            f.write(f"aws_session_token={session_token}\n") if session_token else None
+        os.chmod(AMAZON_CREDENTIALS_FILE_PATH, 0o600)  # for security
+        print(f"Amazon Credentials:")
+        print(f"- AWS_ACCESS_KEY_ID: {len(access_key_id) * '*'}")
+        print(f"- AWS_SECRET_ACCESS_KEY: {len(secret_access_key) * '*'}")
+        print(f"- AMAZON_CREDENTIALS_FILE_PATH: {AMAZON_CREDENTIALS_FILE_PATH}")
+    else:
+        if not (AMAZON_CREDENTIALS_FILE_PATH and
+                os.path.isfile(normalize_path(AMAZON_CREDENTIALS_FILE_PATH, expand_home=True))):
+            pytest.fail("No Amazon credentials file defined. Skippping this test module: test_rclone_support")
+        print(f"Amazon Credentials:")
+        print(f"- AMAZON_CREDENTIALS_FILE_PATH: {AMAZON_CREDENTIALS_FILE_PATH}")
+
+    if is_github_actions_context():
+        if not (service_account_json_string := os.environ.get("GOOGLE_CLOUD_SERVICE_ACCOUNT_JSON")):
+            pytest.fail("Integration test setup error: Google credentials defined!")
+        service_account_json = json.loads(service_account_json_string)
+        google_service_account_file_path = create_temporary_file_name(suffix=".json")
+        with open(google_service_account_file_path, "w") as f:
+            json.dump(service_account_json, f)
+        os.chmod(google_service_account_file_path, 0o600)  # for security
+        GOOGLE_SERVICE_ACCOUNT_FILE_PATH = google_service_account_file_path
+        print(f"Google Credentials:")
+        print(f"- GOOGLE_CLOUD_SERVICE_ACCOUNT_JSON: {len(service_account_json_string) * '*'}")
+        print(f"- GOOGLE_SERVICE_ACCOUNT_FILE_PATH: {GOOGLE_SERVICE_ACCOUNT_FILE_PATH}")
+    else:
+        if not (GOOGLE_SERVICE_ACCOUNT_FILE_PATH and
+                os.path.isfile(normalize_path(GOOGLE_SERVICE_ACCOUNT_FILE_PATH, expand_home=True))):
+            if not RCloneGoogle.is_google_compute_engine():
+                print("No Google credentials file defined. Skippping this test module: test_rclone_support")
+                pytest.skip()
+                return
+            # Google credentials can be None on a GCE instance; i.e. no service account file needed.
+            GOOGLE_SERVICE_ACCOUNT_FILE_PATH = None
+        print(f"Google Credentials:")
+        print(f"- GOOGLE_SERVICE_ACCOUNT_FILE_PATH: {GOOGLE_SERVICE_ACCOUNT_FILE_PATH}")
 
     initial_setup_and_sanity_checking(env_amazon=EnvAmazon(), env_google=EnvGoogle())
 
 
 def teardown_module():
-    if AMAZON_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES:
+    if is_github_actions_context:
         remove_temporary_file(AMAZON_CREDENTIALS_FILE_PATH)
-    if GOOGLE_CREDENTIALS_FROM_ENVIRONMENT_VARIABLES:
         remove_temporary_file(GOOGLE_SERVICE_ACCOUNT_FILE_PATH)
     rclone_teardown_module()
 
 
 def initial_setup_and_sanity_checking(env_amazon: EnvAmazon, env_google: EnvGoogle) -> None:
 
     AwsCredentials.remove_credentials_from_environment_variables()
@@ -261,15 +289,14 @@
     if credentials:
         # Google credentials can be None on a GCE instance.
         assert config.location == credentials.location
         assert config.service_account_file == credentials.service_account_file
     assert config == config
     assert not (config != config)
     assert RCloneGoogle(config, bucket="mismatch") != config  # checking equals override
-    assert config.project == env_google.project_id
     return config
 
 
 def create_rclone(source: Optional[RCloneConfig] = None, destination: Optional[RCloneConfig] = None) -> RCloner:
     rcloner = RCloner(source=source, destination=destination)
     assert rcloner.source == source
     assert rcloner.destination == destination
```

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.8.2.1b9/submitr/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/test_submission.py` & `smaht_submitr-0.8.2.1b9/submitr/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.8.2.1b9/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.8.2.1b9/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.8.2.1b9/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.8.2.1b9/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/test_utils.py` & `smaht_submitr-0.8.2.1b9/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/testing_helpers.py` & `smaht_submitr-0.8.2.1b9/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/tests/testing_rclone_helpers.py` & `smaht_submitr-0.8.2.1b9/submitr/tests/testing_rclone_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/submitr/utils.py` & `smaht_submitr-0.8.2.1b9/submitr/utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b8/PKG-INFO` & `smaht_submitr-0.8.2.1b9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.8.2.1b8
+Version: 0.8.2.1b9
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.13
```

