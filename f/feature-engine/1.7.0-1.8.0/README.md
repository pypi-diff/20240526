# Comparing `tmp/feature_engine-1.7.0.tar.gz` & `tmp/feature_engine-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feature_engine-1.7.0.tar", last modified: Sun Mar 24 13:29:40 2024, max compression
+gzip compressed data, was "feature_engine-1.8.0.tar", last modified: Sun May 26 13:28:06 2024, max compression
```

## Comparing `feature_engine-1.7.0.tar` & `feature_engine-1.8.0.tar`

### file list

```diff
@@ -1,284 +1,288 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.508363 feature_engine-1.7.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1541 2024-03-24 13:29:29.000000 feature_engine-1.7.0/LICENSE.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      245 2024-03-24 13:29:29.000000 feature_engine-1.7.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9603 2024-03-24 13:29:40.508363 feature_engine-1.7.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8939 2024-03-24 13:29:29.000000 feature_engine-1.7.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.480362 feature_engine-1.7.0/feature_engine/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/VERSION
--rw-r--r--   0 circleci  (3434) circleci  (3434)      267 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.480362 feature_engine-1.7.0/feature_engine/_base_transformers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_base_transformers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3866 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_base_transformers/base_numerical.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7141 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_base_transformers/mixins.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.480362 feature_engine-1.7.0/feature_engine/_check_init_parameters/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_check_init_parameters/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      493 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_check_init_parameters/check_init_input_params.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      916 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_check_init_parameters/check_input_dictionary.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1324 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_check_init_parameters/check_variables.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.480362 feature_engine-1.7.0/feature_engine/_docstrings/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_docstrings/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1457 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_docstrings/fit_attributes.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.480362 feature_engine-1.7.0/feature_engine/_docstrings/init_parameters/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_docstrings/init_parameters/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1245 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_docstrings/init_parameters/all_trasnformers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      714 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_docstrings/init_parameters/discretisers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1095 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_docstrings/init_parameters/encoders.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1464 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_docstrings/init_parameters/outliers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      605 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_docstrings/init_parameters/selection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1284 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_docstrings/methods.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.480362 feature_engine-1.7.0/feature_engine/_docstrings/selection/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_docstrings/selection/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3249 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_docstrings/selection/_docstring.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      725 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_docstrings/substitute.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.484362 feature_engine-1.7.0/feature_engine/_prediction/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_prediction/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9532 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_prediction/base_predictor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6291 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_prediction/target_mean_classifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4043 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/_prediction/target_mean_regressor.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.484362 feature_engine-1.7.0/feature_engine/creation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      374 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/creation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4170 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/creation/base_creation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5943 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/creation/cyclical_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7947 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/creation/math_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10655 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/creation/relative_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9813 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/dataframe_checks.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.484362 feature_engine-1.7.0/feature_engine/datasets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       62 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/datasets/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4107 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/datasets/titanic.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.484362 feature_engine-1.7.0/feature_engine/datetime/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      211 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/datetime/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2239 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/datetime/_datetime_constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13790 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/datetime/datetime.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12504 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/datetime/datetime_subtraction.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.484362 feature_engine-1.7.0/feature_engine/discretisation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      526 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/discretisation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6521 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/discretisation/arbitrary.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2622 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/discretisation/base_discretiser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9493 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/discretisation/decision_tree.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5004 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/discretisation/equal_frequency.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5293 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/discretisation/equal_width.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5362 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/discretisation/geometric_width.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.484362 feature_engine-1.7.0/feature_engine/encoding/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      636 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/encoding/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      499 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/encoding/_helper_functions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9818 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/encoding/base_encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6693 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/encoding/count_frequency.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11298 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/encoding/decision_tree.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8819 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/encoding/mean_encoding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11239 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/encoding/one_hot.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7202 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/encoding/ordinal.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9094 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/encoding/rare_label.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14120 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/encoding/similarity_encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9644 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/encoding/woe.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.488362 feature_engine-1.7.0/feature_engine/imputation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      600 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/imputation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4908 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/imputation/arbitrary_number.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2405 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/imputation/base_imputer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9089 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/imputation/categorical.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7794 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/imputation/drop_missing_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6789 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/imputation/end_tail.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4048 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/imputation/mean_median.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5604 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/imputation/missing_indicator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9513 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/imputation/random_sample.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.488362 feature_engine-1.7.0/feature_engine/outliers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      261 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/outliers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6162 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/outliers/artbitrary.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9221 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/outliers/base_outlier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5035 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/outliers/trimmer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7251 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/outliers/winsorizer.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.488362 feature_engine-1.7.0/feature_engine/pipeline/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       87 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/pipeline/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22630 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/pipeline/pipeline.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.488362 feature_engine-1.7.0/feature_engine/preprocessing/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      265 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/preprocessing/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6401 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/preprocessing/match_categories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9716 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/preprocessing/match_columns.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.492362 feature_engine-1.7.0/feature_engine/selection/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1276 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1015 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/_selection_constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7196 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/base_recursive_selector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6454 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/base_selection_functions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4227 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/base_selector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7346 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/drop_constant_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6769 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/drop_correlated_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5577 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/drop_duplicate_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3592 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/drop_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    29691 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/drop_psi_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9189 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/information_value.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10519 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/probe_feature_selection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6630 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/recursive_feature_addition.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6580 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/recursive_feature_elimination.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10008 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/shuffle_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7800 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/single_feature_performance.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11564 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/smart_correlation_selection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11165 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/selection/target_mean_selection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1598 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/tags.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.492362 feature_engine-1.7.0/feature_engine/timeseries/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/timeseries/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.492362 feature_engine-1.7.0/feature_engine/timeseries/forecasting/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/timeseries/forecasting/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7328 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/timeseries/forecasting/base_forecast_transformers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7838 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/timeseries/forecasting/expanding_window_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9223 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/timeseries/forecasting/lag_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9462 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/timeseries/forecasting/window_features.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.492362 feature_engine-1.7.0/feature_engine/transformation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      552 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/transformation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6873 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/transformation/arcsin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6765 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/transformation/boxcox.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13226 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/transformation/log.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4618 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/transformation/power.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5865 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/transformation/reciprocal.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6437 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/transformation/yeojohnson.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.492362 feature_engine-1.7.0/feature_engine/variable_handling/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      896 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/variable_handling/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2026 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/variable_handling/_variable_type_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5774 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/variable_handling/check_variables.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8866 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/variable_handling/find_variables.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1484 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/variable_handling/retain_variables.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.492362 feature_engine-1.7.0/feature_engine/wrappers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      254 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/wrappers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15010 2024-03-24 13:29:29.000000 feature_engine-1.7.0/feature_engine/wrappers/wrappers.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.480362 feature_engine-1.7.0/feature_engine.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9603 2024-03-24 13:29:40.000000 feature_engine-1.7.0/feature_engine.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11153 2024-03-24 13:29:40.000000 feature_engine-1.7.0/feature_engine.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-03-24 13:29:40.000000 feature_engine-1.7.0/feature_engine.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-03-24 13:29:40.000000 feature_engine-1.7.0/feature_engine.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2024-03-24 13:29:40.000000 feature_engine-1.7.0/feature_engine.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-03-24 13:29:40.000000 feature_engine-1.7.0/feature_engine.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2024-03-24 13:29:29.000000 feature_engine-1.7.0/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-03-24 13:29:40.508363 feature_engine-1.7.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1779 2024-03-24 13:29:29.000000 feature_engine-1.7.0/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      131 2024-03-24 13:29:29.000000 feature_engine-1.7.0/test_requirements.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.476362 feature_engine-1.7.0/tests/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.496362 feature_engine-1.7.0/tests/estimator_checks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/estimator_checks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1344 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/estimator_checks/dataframe_for_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4351 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/estimator_checks/estimator_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1117 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/estimator_checks/fit_functionality_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2653 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/estimator_checks/get_feature_names_out_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1907 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/estimator_checks/init_params_allowed_values_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6359 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/estimator_checks/init_params_triggered_functionality_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      659 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/estimator_checks/non_fitted_error_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7751 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/estimator_checks/variable_selection_checks.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.496362 feature_engine-1.7.0/tests/test_check_init_parameters/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_check_init_parameters/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      569 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_check_init_parameters/test_check_init_input_params.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      565 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_check_init_parameters/test_check_input_dictionary.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1480 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_check_init_parameters/test_check_variables.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.496362 feature_engine-1.7.0/tests/test_creation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_creation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1694 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_creation/test_check_estimator_creation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5574 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_creation/test_cyclical_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11048 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_creation/test_math_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13784 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_creation/test_relative_features.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.496362 feature_engine-1.7.0/tests/test_datetime/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_datetime/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4601 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_datetime/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1347 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_datetime/test_check_estimator_datetime.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18402 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_datetime/test_datetime_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12515 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_datetime/test_datetime_subtraction.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.496362 feature_engine-1.7.0/tests/test_discretisation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_discretisation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3928 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_discretisation/test_arbitrary_discretiser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2623 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_discretisation/test_base_discretizer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1668 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_discretisation/test_check_estimator_discretisers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3771 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_discretisation/test_decision_tree_discretiser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2532 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_discretisation/test_equal_frequency_discretiser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2494 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_discretisation/test_equal_width_discretiser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3148 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_discretisation/test_geometric_width_discretiser.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.500362 feature_engine-1.7.0/tests/test_encoding/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.500362 feature_engine-1.7.0/tests/test_encoding/test_base_encoders/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/test_base_encoders/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      628 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/test_base_encoders/test_categorical_init_mixin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1105 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/test_base_encoders/test_categorical_init_mixin_na.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5624 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/test_base_encoders/test_categorical_method_mixin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8340 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/test_check_estimator_encoders.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14151 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/test_count_frequency_encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6302 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/test_decision_tree_encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/test_helper_functions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13944 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/test_mean_encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17284 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/test_onehot_encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10605 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/test_ordinal_encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13875 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/test_rare_label_encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10991 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/test_similarity_encoder.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.500362 feature_engine-1.7.0/tests/test_encoding/test_woe/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/test_woe/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2053 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/test_woe/test_woe_class.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13157 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_encoding/test_woe/test_woe_encoder.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.500362 feature_engine-1.7.0/tests/test_imputation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_imputation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2891 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_imputation/test_arbitrary_number_imputer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10477 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_imputation/test_categorical_imputer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_imputation/test_check_estimator_imputers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4652 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_imputation/test_drop_missing_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3485 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_imputation/test_end_tail_imputer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2126 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_imputation/test_mean_mdian_imputer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3511 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_imputation/test_missing_indicator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9374 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_imputation/test_random_sample_imputer.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.500362 feature_engine-1.7.0/tests/test_outliers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_outliers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5685 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_outliers/test_arbitrary_capper.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1744 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_outliers/test_check_estimator_outliers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3520 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_outliers/test_outlier_trimmer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14155 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_outliers/test_winsorizer.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.504362 feature_engine-1.7.0/tests/test_prediction/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_prediction/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1162 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_prediction/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8815 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_prediction/test_check_estimator_prediction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7554 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_prediction/test_target_mean_classifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4363 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_prediction/test_target_mean_regressor.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.504362 feature_engine-1.7.0/tests/test_preprocessing/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_preprocessing/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1661 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_preprocessing/test_check_estimator_preprocessing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2531 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_preprocessing/test_match_categories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10774 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_preprocessing/test_match_columns.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.504362 feature_engine-1.7.0/tests/test_selection/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1669 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3965 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_base_selection_functions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1685 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_base_selector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4739 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_check_estimator_selectors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5848 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_drop_constant_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6764 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_drop_correlated_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3967 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_drop_duplicate_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3343 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_drop_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25466 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_drop_high_psi_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5105 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_information_value.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7039 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_probe_feature_selection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4591 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_recursive_feature_addition.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5257 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_recursive_feature_elimination.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4352 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_recursive_feature_selectors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4259 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_shuffle_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7173 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_single_feature_performance.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10871 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_smart_correlation_selection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6043 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_selection/test_target_mean_selection.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.504362 feature_engine-1.7.0/tests/test_time_series/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_time_series/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.508363 feature_engine-1.7.0/tests/test_time_series/test_forecasting/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_time_series/test_forecasting/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1684 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_time_series/test_forecasting/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2152 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_time_series/test_forecasting/test_check_estimator_forecasting.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14167 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_time_series/test_forecasting/test_expanding_window_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14608 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_time_series/test_forecasting/test_lag_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17335 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_time_series/test_forecasting/test_window_features.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.508363 feature_engine-1.7.0/tests/test_transformation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_transformation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2217 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_transformation/test_arcsin_transformer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2320 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_transformation/test_boxcox_transformer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1404 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_transformation/test_check_estimator_transformers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3987 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_transformation/test_log_transformer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8588 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_transformation/test_logcp_transformer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2634 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_transformation/test_power_transformer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2324 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_transformation/test_reciprocal_transformer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4614 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_transformation/test_yeojohnson_transformer.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.508363 feature_engine-1.7.0/tests/test_variable_handling/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_variable_handling/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1102 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_variable_handling/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5765 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_variable_handling/test_check_variables.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5426 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_variable_handling/test_find_variables.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      927 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_variable_handling/test_remove_variables.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:40.508363 feature_engine-1.7.0/tests/test_wrappers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_wrappers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1531 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_wrappers/test_check_estimator_wrappers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19764 2024-03-24 13:29:29.000000 feature_engine-1.7.0/tests/test_wrappers/test_sklearn_wrapper.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.616208 feature_engine-1.8.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5131 2024-05-26 13:27:54.000000 feature_engine-1.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1541 2024-05-26 13:27:54.000000 feature_engine-1.8.0/LICENSE.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      245 2024-05-26 13:27:54.000000 feature_engine-1.8.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9629 2024-05-26 13:28:06.616208 feature_engine-1.8.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8965 2024-05-26 13:27:54.000000 feature_engine-1.8.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.584208 feature_engine-1.8.0/feature_engine/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/VERSION
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      267 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.588208 feature_engine-1.8.0/feature_engine/_base_transformers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_base_transformers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3866 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_base_transformers/base_numerical.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7141 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_base_transformers/mixins.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.588208 feature_engine-1.8.0/feature_engine/_check_init_parameters/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_check_init_parameters/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      493 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_check_init_parameters/check_init_input_params.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      916 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_check_init_parameters/check_input_dictionary.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1324 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_check_init_parameters/check_variables.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.588208 feature_engine-1.8.0/feature_engine/_docstrings/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_docstrings/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1457 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_docstrings/fit_attributes.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.588208 feature_engine-1.8.0/feature_engine/_docstrings/init_parameters/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_docstrings/init_parameters/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1245 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_docstrings/init_parameters/all_trasnformers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2719 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_docstrings/init_parameters/creation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      714 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_docstrings/init_parameters/discretisers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1095 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_docstrings/init_parameters/encoders.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1728 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_docstrings/init_parameters/outliers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      605 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_docstrings/init_parameters/selection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1284 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_docstrings/methods.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.588208 feature_engine-1.8.0/feature_engine/_docstrings/selection/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_docstrings/selection/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3249 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_docstrings/selection/_docstring.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      725 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_docstrings/substitute.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.588208 feature_engine-1.8.0/feature_engine/_prediction/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_prediction/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9532 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_prediction/base_predictor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6291 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_prediction/target_mean_classifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4043 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/_prediction/target_mean_regressor.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.588208 feature_engine-1.8.0/feature_engine/creation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      428 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/creation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4170 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/creation/base_creation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5943 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/creation/cyclical_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17787 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/creation/decision_tree_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7947 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/creation/math_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10655 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/creation/relative_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9827 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/dataframe_checks.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.588208 feature_engine-1.8.0/feature_engine/datasets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       62 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/datasets/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4190 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/datasets/titanic.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.592208 feature_engine-1.8.0/feature_engine/datetime/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      211 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/datetime/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2239 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/datetime/_datetime_constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13790 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/datetime/datetime.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12504 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/datetime/datetime_subtraction.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.592208 feature_engine-1.8.0/feature_engine/discretisation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      526 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/discretisation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6521 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/discretisation/arbitrary.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2622 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/discretisation/base_discretiser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12903 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/discretisation/decision_tree.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5004 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/discretisation/equal_frequency.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5293 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/discretisation/equal_width.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5362 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/discretisation/geometric_width.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.592208 feature_engine-1.8.0/feature_engine/encoding/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      636 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/encoding/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      512 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/encoding/_helper_functions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9818 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/encoding/base_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6693 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/encoding/count_frequency.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12883 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/encoding/decision_tree.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8819 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/encoding/mean_encoding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11239 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/encoding/one_hot.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7202 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/encoding/ordinal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9094 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/encoding/rare_label.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14120 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/encoding/similarity_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9644 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/encoding/woe.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.592208 feature_engine-1.8.0/feature_engine/imputation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      600 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/imputation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4908 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/imputation/arbitrary_number.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2405 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/imputation/base_imputer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9089 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/imputation/categorical.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7794 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/imputation/drop_missing_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6789 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/imputation/end_tail.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4048 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/imputation/mean_median.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5604 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/imputation/missing_indicator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9513 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/imputation/random_sample.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.596208 feature_engine-1.8.0/feature_engine/outliers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      261 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/outliers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6162 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/outliers/artbitrary.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10019 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/outliers/base_outlier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5986 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/outliers/trimmer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8233 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/outliers/winsorizer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.596208 feature_engine-1.8.0/feature_engine/pipeline/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       87 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/pipeline/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22725 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/pipeline/pipeline.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.596208 feature_engine-1.8.0/feature_engine/preprocessing/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      265 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/preprocessing/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6401 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/preprocessing/match_categories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9716 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/preprocessing/match_columns.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.596208 feature_engine-1.8.0/feature_engine/selection/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1276 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1015 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/_selection_constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7196 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/base_recursive_selector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6454 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/base_selection_functions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4227 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/base_selector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7346 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/drop_constant_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6769 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/drop_correlated_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5577 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/drop_duplicate_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3592 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/drop_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    29691 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/drop_psi_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9189 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/information_value.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10519 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/probe_feature_selection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6630 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/recursive_feature_addition.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6580 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/recursive_feature_elimination.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10008 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/shuffle_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7800 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/single_feature_performance.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11564 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/smart_correlation_selection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11165 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/selection/target_mean_selection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1598 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/tags.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.596208 feature_engine-1.8.0/feature_engine/timeseries/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/timeseries/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.596208 feature_engine-1.8.0/feature_engine/timeseries/forecasting/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/timeseries/forecasting/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7328 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/timeseries/forecasting/base_forecast_transformers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7838 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/timeseries/forecasting/expanding_window_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9223 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/timeseries/forecasting/lag_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9462 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/timeseries/forecasting/window_features.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.600208 feature_engine-1.8.0/feature_engine/transformation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      552 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/transformation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6873 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/transformation/arcsin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6765 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/transformation/boxcox.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13352 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/transformation/log.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4618 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/transformation/power.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5865 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/transformation/reciprocal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6437 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/transformation/yeojohnson.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.600208 feature_engine-1.8.0/feature_engine/variable_handling/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      896 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/variable_handling/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2026 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/variable_handling/_variable_type_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5774 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/variable_handling/check_variables.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8866 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/variable_handling/find_variables.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1484 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/variable_handling/retain_variables.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.600208 feature_engine-1.8.0/feature_engine/wrappers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      254 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/wrappers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15010 2024-05-26 13:27:54.000000 feature_engine-1.8.0/feature_engine/wrappers/wrappers.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.584208 feature_engine-1.8.0/feature_engine.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9629 2024-05-26 13:28:06.000000 feature_engine-1.8.0/feature_engine.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11328 2024-05-26 13:28:06.000000 feature_engine-1.8.0/feature_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-05-26 13:28:06.000000 feature_engine-1.8.0/feature_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-05-26 13:28:06.000000 feature_engine-1.8.0/feature_engine.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2024-05-26 13:28:06.000000 feature_engine-1.8.0/feature_engine.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-05-26 13:28:06.000000 feature_engine-1.8.0/feature_engine.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2024-05-26 13:27:54.000000 feature_engine-1.8.0/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-05-26 13:28:06.616208 feature_engine-1.8.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1779 2024-05-26 13:27:54.000000 feature_engine-1.8.0/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      131 2024-05-26 13:27:54.000000 feature_engine-1.8.0/test_requirements.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.584208 feature_engine-1.8.0/tests/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.600208 feature_engine-1.8.0/tests/estimator_checks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/estimator_checks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1344 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/estimator_checks/dataframe_for_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4351 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/estimator_checks/estimator_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1117 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/estimator_checks/fit_functionality_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2653 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/estimator_checks/get_feature_names_out_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1907 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/estimator_checks/init_params_allowed_values_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6359 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/estimator_checks/init_params_triggered_functionality_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      659 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/estimator_checks/non_fitted_error_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7751 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/estimator_checks/variable_selection_checks.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.600208 feature_engine-1.8.0/tests/test_check_init_parameters/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_check_init_parameters/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      569 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_check_init_parameters/test_check_init_input_params.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      565 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_check_init_parameters/test_check_input_dictionary.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1480 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_check_init_parameters/test_check_variables.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.600208 feature_engine-1.8.0/tests/test_creation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_creation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1781 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_creation/test_check_estimator_creation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5574 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_creation/test_cyclical_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16011 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_creation/test_decision_tree_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11048 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_creation/test_math_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13784 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_creation/test_relative_features.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.604208 feature_engine-1.8.0/tests/test_datetime/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_datetime/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4601 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_datetime/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1347 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_datetime/test_check_estimator_datetime.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18402 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_datetime/test_datetime_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12515 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_datetime/test_datetime_subtraction.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.604208 feature_engine-1.8.0/tests/test_discretisation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_discretisation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3928 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_discretisation/test_arbitrary_discretiser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2623 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_discretisation/test_base_discretizer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1668 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_discretisation/test_check_estimator_discretisers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9274 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_discretisation/test_decision_tree_discretiser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2532 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_discretisation/test_equal_frequency_discretiser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2494 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_discretisation/test_equal_width_discretiser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3148 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_discretisation/test_geometric_width_discretiser.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.604208 feature_engine-1.8.0/tests/test_encoding/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.604208 feature_engine-1.8.0/tests/test_encoding/test_base_encoders/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/test_base_encoders/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      628 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/test_base_encoders/test_categorical_init_mixin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1105 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/test_base_encoders/test_categorical_init_mixin_na.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5624 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/test_base_encoders/test_categorical_method_mixin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8340 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/test_check_estimator_encoders.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14321 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/test_count_frequency_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11655 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/test_decision_tree_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      851 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/test_helper_functions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13944 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/test_mean_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17284 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/test_onehot_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10605 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/test_ordinal_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13875 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/test_rare_label_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10991 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/test_similarity_encoder.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.604208 feature_engine-1.8.0/tests/test_encoding/test_woe/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/test_woe/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2053 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/test_woe/test_woe_class.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13157 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_encoding/test_woe/test_woe_encoder.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.608208 feature_engine-1.8.0/tests/test_imputation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_imputation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2891 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_imputation/test_arbitrary_number_imputer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10477 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_imputation/test_categorical_imputer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_imputation/test_check_estimator_imputers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4652 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_imputation/test_drop_missing_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3485 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_imputation/test_end_tail_imputer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2126 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_imputation/test_mean_mdian_imputer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3511 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_imputation/test_missing_indicator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9374 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_imputation/test_random_sample_imputer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.608208 feature_engine-1.8.0/tests/test_outliers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_outliers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5685 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_outliers/test_arbitrary_capper.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1744 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_outliers/test_check_estimator_outliers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3577 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_outliers/test_outlier_trimmer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14212 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_outliers/test_winsorizer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.608208 feature_engine-1.8.0/tests/test_prediction/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_prediction/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1162 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_prediction/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8815 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_prediction/test_check_estimator_prediction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7554 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_prediction/test_target_mean_classifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4363 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_prediction/test_target_mean_regressor.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.608208 feature_engine-1.8.0/tests/test_preprocessing/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_preprocessing/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1661 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_preprocessing/test_check_estimator_preprocessing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2531 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_preprocessing/test_match_categories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10774 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_preprocessing/test_match_columns.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.612208 feature_engine-1.8.0/tests/test_selection/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1669 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3965 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_base_selection_functions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1685 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_base_selector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4739 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_check_estimator_selectors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5848 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_drop_constant_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6764 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_drop_correlated_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3967 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_drop_duplicate_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3343 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_drop_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25466 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_drop_high_psi_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5105 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_information_value.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7039 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_probe_feature_selection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4591 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_recursive_feature_addition.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5257 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_recursive_feature_elimination.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4352 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_recursive_feature_selectors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4259 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_shuffle_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7173 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_single_feature_performance.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10871 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_smart_correlation_selection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6043 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_selection/test_target_mean_selection.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.612208 feature_engine-1.8.0/tests/test_time_series/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_time_series/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.612208 feature_engine-1.8.0/tests/test_time_series/test_forecasting/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_time_series/test_forecasting/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1684 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_time_series/test_forecasting/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2152 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_time_series/test_forecasting/test_check_estimator_forecasting.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14167 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_time_series/test_forecasting/test_expanding_window_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14608 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_time_series/test_forecasting/test_lag_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17335 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_time_series/test_forecasting/test_window_features.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.612208 feature_engine-1.8.0/tests/test_transformation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_transformation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2217 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_transformation/test_arcsin_transformer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2320 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_transformation/test_boxcox_transformer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1404 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_transformation/test_check_estimator_transformers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4313 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_transformation/test_log_transformer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8588 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_transformation/test_logcp_transformer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2634 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_transformation/test_power_transformer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2324 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_transformation/test_reciprocal_transformer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4614 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_transformation/test_yeojohnson_transformer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.612208 feature_engine-1.8.0/tests/test_variable_handling/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_variable_handling/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1102 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_variable_handling/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5765 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_variable_handling/test_check_variables.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5426 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_variable_handling/test_find_variables.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      927 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_variable_handling/test_remove_variables.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:28:06.612208 feature_engine-1.8.0/tests/test_wrappers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_wrappers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1531 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_wrappers/test_check_estimator_wrappers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19764 2024-05-26 13:27:54.000000 feature_engine-1.8.0/tests/test_wrappers/test_sklearn_wrapper.py
```

### Comparing `feature_engine-1.7.0/LICENSE.md` & `feature_engine-1.8.0/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2018-2023 The Feature-engine developers.
+Copyright (c) 2018-2024 The Feature-engine developers.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `feature_engine-1.7.0/PKG-INFO` & `feature_engine-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature_engine
-Version: 1.7.0
+Version: 1.8.0
 Summary: Feature engineering and selection package with Scikit-learn's fit transform functionality
 Home-page: http://github.com/feature-engine/feature_engine
 Author: Soledad Galli
 Author-email: solegalli@protonmail.com
 License: BSD 3 clause
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# Feature Engine
+# Feature-engine
 
 [![feature-engine logo](https://raw.githubusercontent.com/feature-engine/feature_engine/main/docs/images/logo/FeatureEngine.png)](http://feature-engine.readthedocs.io)
 
 | | |
 | --- | --- |
 | Package | [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/feature_engine?logo=Python)](https://pypi.org/project/feature-engine/) [![PyPI](https://img.shields.io/pypi/v/feature_engine?logo=PyPI)](https://pypi.org/project/feature-engine) [![Conda](https://img.shields.io/conda/v/conda-forge/feature_engine?logo=Anaconda)](https://anaconda.org/conda-forge/feature_engine) [![Monthly Downloads](https://img.shields.io/pypi/dm/feature-engine)](https://img.shields.io/pypi/dm/feature-engine)  [![Downloads](https://static.pepy.tech/personalized-badge/feature-engine?period=total&units=international_system&left_color=grey&right_color=green&left_text=total-downloads%20(pypi))](https://pepy.tech/project/feature-engine)|
 | Meta | [![GitHub](https://img.shields.io/github/license/feature-engine/feature_engine)](https://github.com/feature-engine/feature_engine/blob/master/LICENSE.md) [![GitHub contributors](https://img.shields.io/github/contributors/feature-engine/feature_engine?logo=GitHub)](https://github.com/feature-engine/feature_engine/graphs/contributors) [![Gitter](https://img.shields.io/gitter/room/feature-engine/feaure_engine?logo=Gitter)](https://gitter.im/feature_engine/community) [![first-timers-only](https://img.shields.io/badge/first--timers--only-friendly-blue.svg?style=flat)](https://www.firsttimersonly.com/) [![Sponsorship](https://img.shields.io/badge/Powered%20By-TrainInData-orange.svg)](https://www.trainindata.com/) |
@@ -128,14 +128,15 @@
 * BoxCoxTransformer
 * YeoJohnsonTransformer
 
 ### Variable Creation:
  * MathFeatures
  * RelativeFeatures
  * CyclicalFeatures
+ * DecisionTreeFeatures()
 
 ### Feature Selection:
  * DropFeatures
  * DropConstantFeatures
  * DropDuplicateFeatures
  * DropCorrelatedFeatures
  * SmartCorrelationSelection
```

### Comparing `feature_engine-1.7.0/README.md` & `feature_engine-1.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Feature Engine
+# Feature-engine
 
 [![feature-engine logo](https://raw.githubusercontent.com/feature-engine/feature_engine/main/docs/images/logo/FeatureEngine.png)](http://feature-engine.readthedocs.io)
 
 | | |
 | --- | --- |
 | Package | [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/feature_engine?logo=Python)](https://pypi.org/project/feature-engine/) [![PyPI](https://img.shields.io/pypi/v/feature_engine?logo=PyPI)](https://pypi.org/project/feature-engine) [![Conda](https://img.shields.io/conda/v/conda-forge/feature_engine?logo=Anaconda)](https://anaconda.org/conda-forge/feature_engine) [![Monthly Downloads](https://img.shields.io/pypi/dm/feature-engine)](https://img.shields.io/pypi/dm/feature-engine)  [![Downloads](https://static.pepy.tech/personalized-badge/feature-engine?period=total&units=international_system&left_color=grey&right_color=green&left_text=total-downloads%20(pypi))](https://pepy.tech/project/feature-engine)|
 | Meta | [![GitHub](https://img.shields.io/github/license/feature-engine/feature_engine)](https://github.com/feature-engine/feature_engine/blob/master/LICENSE.md) [![GitHub contributors](https://img.shields.io/github/contributors/feature-engine/feature_engine?logo=GitHub)](https://github.com/feature-engine/feature_engine/graphs/contributors) [![Gitter](https://img.shields.io/gitter/room/feature-engine/feaure_engine?logo=Gitter)](https://gitter.im/feature_engine/community) [![first-timers-only](https://img.shields.io/badge/first--timers--only-friendly-blue.svg?style=flat)](https://www.firsttimersonly.com/) [![Sponsorship](https://img.shields.io/badge/Powered%20By-TrainInData-orange.svg)](https://www.trainindata.com/) |
@@ -110,14 +110,15 @@
 * BoxCoxTransformer
 * YeoJohnsonTransformer
 
 ### Variable Creation:
  * MathFeatures
  * RelativeFeatures
  * CyclicalFeatures
+ * DecisionTreeFeatures()
 
 ### Feature Selection:
  * DropFeatures
  * DropConstantFeatures
  * DropDuplicateFeatures
  * DropCorrelatedFeatures
  * SmartCorrelationSelection
```

### Comparing `feature_engine-1.7.0/feature_engine/_base_transformers/base_numerical.py` & `feature_engine-1.8.0/feature_engine/_base_transformers/base_numerical.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/_base_transformers/mixins.py` & `feature_engine-1.8.0/feature_engine/_base_transformers/mixins.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/_check_init_parameters/check_input_dictionary.py` & `feature_engine-1.8.0/feature_engine/_check_init_parameters/check_input_dictionary.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/_check_init_parameters/check_variables.py` & `feature_engine-1.8.0/feature_engine/_check_init_parameters/check_variables.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/_docstrings/fit_attributes.py` & `feature_engine-1.8.0/feature_engine/_docstrings/fit_attributes.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/_docstrings/init_parameters/all_trasnformers.py` & `feature_engine-1.8.0/feature_engine/_docstrings/init_parameters/all_trasnformers.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/_docstrings/init_parameters/discretisers.py` & `feature_engine-1.8.0/feature_engine/_docstrings/init_parameters/discretisers.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/_docstrings/init_parameters/encoders.py` & `feature_engine-1.8.0/feature_engine/_docstrings/init_parameters/encoders.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/_docstrings/init_parameters/outliers.py` & `feature_engine-1.8.0/feature_engine/_docstrings/init_parameters/outliers.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,22 @@
     """.rstrip()
 
 _tail_docstring = """tail: str, default='right'
         Whether to look for outliers on the right, left or both tails of the
         distribution. Can take 'left', 'right' or 'both'.
     """.rstrip()
 
-_fold_docstring = """fold: int or float, default=0.05 if `quantile`, or 3 otherwise.
+_fold_docstring = """fold: int, float or 'auto', default='auto'.
         The factor used to multiply the std, MAD or IQR to calculate
         the maximum or minimum allowed values.
-        Recommended values are 2 or 3 for the gaussian approximation,
+        When 'auto', `fold` is set based on the `capping_method`: \n
+         - If `capping_method='quantile'` then `'fold'` = 0.05; \n
+         - If `capping_method='gaussian'` then `'fold'` = 3.0; \n
+         - If `capping_method='mad'` then `'fold'` = 3.29; \n
+         - If `capping_method='iqr'` then `'fold'` = 1.5. \n
+        Recommended values are 2, 2.5 or 3 for the gaussian approximation,
         1.5 or 3 for the IQR proximity rule and 3 or 3.5 for MAD rule. \n
         If `capping_method='quantile'`, then `'fold'` indicates the percentile. So if
         `fold=0.05`, the limits will be the 95th and 5th percentiles. \n
-        **Note**: Outliers will be removed up to a maximum of the 20th percentiles on
-        both sides. Thus, when `capping_method='quantile'`, then `'fold'` takes values
-        between 0 and 0.20.
+        **Note**: When `capping_method='quantile'`, the maximum `fold` allowed is 0.2,
+        which will find boundaries at the 20th and 80th percentile.
     """.rstrip()
```

### Comparing `feature_engine-1.7.0/feature_engine/_docstrings/init_parameters/selection.py` & `feature_engine-1.8.0/feature_engine/_docstrings/init_parameters/selection.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/_docstrings/methods.py` & `feature_engine-1.8.0/feature_engine/_docstrings/methods.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/_docstrings/selection/_docstring.py` & `feature_engine-1.8.0/feature_engine/_docstrings/selection/_docstring.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/_docstrings/substitute.py` & `feature_engine-1.8.0/feature_engine/_docstrings/substitute.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/_prediction/base_predictor.py` & `feature_engine-1.8.0/feature_engine/_prediction/base_predictor.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/_prediction/target_mean_classifier.py` & `feature_engine-1.8.0/feature_engine/_prediction/target_mean_classifier.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/_prediction/target_mean_regressor.py` & `feature_engine-1.8.0/feature_engine/_prediction/target_mean_regressor.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/creation/base_creation.py` & `feature_engine-1.8.0/feature_engine/creation/base_creation.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/creation/cyclical_features.py` & `feature_engine-1.8.0/feature_engine/creation/cyclical_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/creation/math_features.py` & `feature_engine-1.8.0/feature_engine/creation/math_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/creation/relative_features.py` & `feature_engine-1.8.0/feature_engine/creation/relative_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/dataframe_checks.py` & `feature_engine-1.8.0/feature_engine/dataframe_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,18 +134,18 @@
             raise ValueError("y contains infinity values.")
         y = y.copy()
 
     else:
         try:
             y = column_or_1d(y)
             y = _check_y(y, multi_output=False, y_numeric=y_numeric)
-            y = pd.Series(y)
+            y = pd.Series(y).copy()
         except ValueError:
             y = _check_y(y, multi_output=True, y_numeric=y_numeric)
-            y = pd.DataFrame(y)
+            y = pd.DataFrame(y).copy()
     return y
 
 
 def check_X_y(
     X: Union[np.generic, np.ndarray, pd.DataFrame],
     y: Union[np.generic, np.ndarray, pd.Series, List],
     y_numeric: bool = False,
```

### Comparing `feature_engine-1.7.0/feature_engine/datasets/titanic.py` & `feature_engine-1.8.0/feature_engine/datasets/titanic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import pandas as pd
 from sklearn.pipeline import Pipeline
 
 from feature_engine.imputation import CategoricalImputer, MeanMedianImputer
 
 
+# TODO: loading the dataset from the internet is not the best, we need to store it
 def load_titanic(
     return_X_y_frame=False, predictors_only=False, handle_missing=False, cabin=None
 ):
     """
     The load_titanic() function returns the well-known titanic dataset.
 
     Note that you need to have an internet connection for this function to work, as we
```

### Comparing `feature_engine-1.7.0/feature_engine/datetime/_datetime_constants.py` & `feature_engine-1.8.0/feature_engine/datetime/_datetime_constants.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/datetime/datetime.py` & `feature_engine-1.8.0/feature_engine/datetime/datetime.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/datetime/datetime_subtraction.py` & `feature_engine-1.8.0/feature_engine/datetime/datetime_subtraction.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/discretisation/__init__.py` & `feature_engine-1.8.0/feature_engine/discretisation/__init__.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/discretisation/arbitrary.py` & `feature_engine-1.8.0/feature_engine/discretisation/arbitrary.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/discretisation/base_discretiser.py` & `feature_engine-1.8.0/feature_engine/discretisation/base_discretiser.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/discretisation/decision_tree.py` & `feature_engine-1.8.0/feature_engine/discretisation/decision_tree.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Authors: Soledad Galli <solegalli@protonmail.com>
 # License: BSD 3 clause
 
 from typing import Dict, List, Optional, Union
 
+import numpy as np
 import pandas as pd
 from sklearn.model_selection import GridSearchCV
 from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
 from sklearn.utils.multiclass import check_classification_targets, type_of_target
 
 from feature_engine._base_transformers.base_numerical import BaseNumericalTransformer
 from feature_engine._check_init_parameters.check_variables import (
@@ -31,33 +32,46 @@
     feature_names_in_=_feature_names_in_docstring,
     n_features_in_=_n_features_in_docstring,
     fit_transform=_fit_transform_docstring,
 )
 class DecisionTreeDiscretiser(BaseNumericalTransformer):
     """
     The DecisionTreeDiscretiser() replaces numerical variables by discrete, i.e.,
-    finite variables, which values are the predictions of a decision tree.
+    finite variables, whose values are the predictions of a decision tree, the  bin
+    number, or the bin limits.
 
     The method is inspired by the following article from the winners of the KDD
     2009 competition:
     http://www.mtome.com/Publications/CiML/CiML-v3-book.pdf
 
-    The DecisionTreeDiscretiser() trains a decision tree per variable. Then, it
-    transforms the variables, with predictions of the decision tree.
+    The DecisionTreeDiscretiser() trains a decision tree per variable. Then it finds
+    the boundaries of each bin. Finally, it replaces the variable values with
+    the predictions of the decision tree, the bin number, or the bin limits.
 
-    The DecisionTreeDiscretiser() works only with numerical variables. A list of
-    variables to transform can be indicated. Alternatively, the discretiser will
+    The DecisionTreeDiscretiser() works only with numerical variables. You can pass a
+    list with the variables you wish to transform. Alternatively, the discretiser will
     automatically select all numerical variables.
 
     More details in the :ref:`User Guide <decisiontree_discretiser>`.
 
     Parameters
     ----------
     {variables}
 
+    bin_output: str, default = "prediction"
+        Whether to return the predictions of the tree, the bin number, or the interval
+        boundaries. Takes values "prediction", "bin_number" and "boundaries",
+        respectively.
+
+    precision: int, default=None
+        The precision at which to store and display the bins labels. In other words,
+        the number of decimals after the comma. Only used when `bin_output` is
+        "prediction" or "boundaries". If `bin_output="boundaries"` then precision
+        cannot be None.
+
     cv: int, cross-validation generator or an iterable, default=3
         Determines the cross-validation splitting strategy. Possible inputs for cv are:
 
             - None, to use cross_validate's default 5-fold cross validation
 
             - int, to specify the number of folds in a (Stratified)KFold,
 
@@ -93,34 +107,35 @@
         of the parameters of the Scikit-learn's DecisionTreeRegressor() or
         DecisionTreeClassifier(). For reproducibility it is recommended to set
         the random_state to an integer.
 
     Attributes
     ----------
     binner_dict_:
-        Dictionary containing the fitted tree per variable.
+         Dictionary with the interval limits per variable or the fitted tree per
+         variable, depending on how `bin_output` was set up.
 
     scores_dict_:
         Dictionary with the score of the best decision tree per variable.
 
     {variables_}
 
     {feature_names_in_}
 
     {n_features_in_}
 
     Methods
     -------
     fit:
-        Fit a decision tree per variable.
+        Fit a decision tree per variable and find the interval limits.
 
     {fit_transform}
 
     transform:
-        Replace continuous variable values by the predictions of the decision tree.
+        Sort continuous variables into intervals or replace them with the predictions.
 
     See Also
     --------
     sklearn.tree.DecisionTreeClassifier
     sklearn.tree.DecisionTreeRegressor
 
     References
@@ -128,16 +143,16 @@
     .. [1] Niculescu-Mizil, et al. "Winning the KDD Cup Orange Challenge with Ensemble
         Selection". JMLR: Workshop and Conference Proceedings 7: 23-34. KDD 2009
         http://proceedings.mlr.press/v7/niculescu09/niculescu09.pdf
 
     Examples
     --------
 
-    >>> import pandas as pd
     >>> import numpy as np
+    >>> import pandas as pd
     >>> from feature_engine.discretisation import DecisionTreeDiscretiser
     >>> np.random.seed(42)
     >>> X = pd.DataFrame(dict(x= np.random.randint(1,100, 100)))
     >>> y_reg = pd.Series(np.random.randn(100))
     >>> dtd = DecisionTreeDiscretiser(random_state=42)
     >>> dtd.fit(X, y_reg)
     >>> dtd.transform(X)["x"].value_counts()
@@ -155,24 +170,47 @@
     0.687500    48
     Name: x, dtype: int64
     """
 
     def __init__(
         self,
         variables: Union[None, int, str, List[Union[str, int]]] = None,
+        bin_output: str = "prediction",
+        precision: Union[int, None] = None,
         cv=3,
         scoring: str = "neg_mean_squared_error",
         param_grid: Optional[Dict[str, Union[str, int, float, List[int]]]] = None,
         regression: bool = True,
         random_state: Optional[int] = None,
     ) -> None:
 
+        if bin_output not in ["prediction", "bin_number", "boundaries"]:
+            raise ValueError(
+                "bin_output takes values  'prediction', 'bin_number' or 'boundaries'. "
+                f"Got {bin_output} instead."
+            )
+
+        if precision is not None and (not isinstance(precision, int) or precision < 1):
+            raise ValueError(
+                "precision must be None or a positive integer. "
+                f"Got {precision} instead."
+            )
+
+        if bin_output == "boundaries" and precision is None:
+            raise ValueError(
+                "When `bin_output == 'boundaries', `precision` cannot be None. "
+                "Change precision's value to a positive integer."
+            )
         if not isinstance(regression, bool):
-            raise ValueError("regression can only take True or False")
+            raise ValueError(
+                f"regression can only take True or False. Got {regression} instead."
+            )
 
+        self.bin_output = bin_output
+        self.precision = precision
         self.cv = cv
         self.scoring = scoring
         self.regression = regression
         self.variables = _check_variables_input_value(variables)
         self.param_grid = param_grid
         self.random_state = random_state
 
@@ -206,16 +244,16 @@
         X = super().fit(X)
 
         if self.param_grid:
             param_grid = self.param_grid
         else:
             param_grid = {"max_depth": [1, 2, 3, 4]}
 
-        self.binner_dict_ = {}
-        self.scores_dict_ = {}
+        binner_dict_ = {}
+        scores_dict_ = {}
 
         for var in self.variables_:
 
             if self.regression:
                 model = DecisionTreeRegressor(random_state=self.random_state)
             else:
                 model = DecisionTreeClassifier(random_state=self.random_state)
@@ -223,17 +261,29 @@
             tree_model = GridSearchCV(
                 model, cv=self.cv, scoring=self.scoring, param_grid=param_grid
             )
 
             # fit the model to the variable
             tree_model.fit(X[var].to_frame(), y)
 
-            self.binner_dict_[var] = tree_model
-            self.scores_dict_[var] = tree_model.score(X[var].to_frame(), y)
+            binner_dict_[var] = tree_model
+            scores_dict_[var] = tree_model.score(X[var].to_frame(), y)
+
+        if self.bin_output != "prediction":
+            for var in self.variables_:
+                clf = binner_dict_[var].best_estimator_
+                threshold = clf.tree_.threshold
+                feature = clf.tree_.feature
+                feature_threshold = threshold[feature == 0]
+                thresholds = sorted(feature_threshold)
+                thresholds = [-np.inf] + thresholds + [np.inf]
+                binner_dict_[var] = thresholds
 
+        self.binner_dict_ = binner_dict_
+        self.scores_dict_ = scores_dict_
         return self
 
     def transform(self, X: pd.DataFrame) -> pd.DataFrame:
         """
         Replaces original variable values with the predictions of the tree. The
         decision tree predictions are finite, aka, discrete.
 
@@ -247,20 +297,50 @@
         X_new: pandas dataframe of shape = [n_samples, n_features]
             The dataframe with transformed variables.
         """
 
         # check input dataframe and if class was fitted
         X = self._check_transform_input_and_state(X)
 
-        for feature in self.variables_:
-            if self.regression:
-                X[feature] = self.binner_dict_[feature].predict(X[feature].to_frame())
-            else:
-                tmp = self.binner_dict_[feature].predict_proba(X[feature].to_frame())
-                X[feature] = tmp[:, 1]
+        if self.bin_output == "prediction":
+            for feature in self.variables_:
+                if self.regression:
+                    preds = self.binner_dict_[feature].predict(X[feature].to_frame())
+                    if self.precision is None:
+                        X[feature] = preds
+                    else:
+                        X[feature] = np.round(preds, self.precision)
+                else:
+                    tmp = self.binner_dict_[feature].predict_proba(
+                        X[feature].to_frame()
+                    )
+                    preds = tmp[:, 1]
+                    if self.precision is None:
+                        X[feature] = preds
+                    else:
+                        X[feature] = np.round(preds, self.precision)
+
+        elif self.bin_output == "boundaries":
+            for feature in self.variables_:
+                X[feature] = pd.cut(
+                    X[feature],
+                    self.binner_dict_[feature],
+                    precision=self.precision,
+                    include_lowest=True,
+                )
+            X[self.variables_] = X[self.variables_].astype(str)
+
+        else:
+            for feature in self.variables_:
+                X[feature] = pd.cut(
+                    X[feature],
+                    self.binner_dict_[feature],
+                    labels=False,
+                    include_lowest=True,
+                )
 
         return X
 
     def _more_tags(self):
         tags_dict = _return_tags()
         tags_dict["variables"] = "numerical"
         tags_dict["requires_y"] = True
```

### Comparing `feature_engine-1.7.0/feature_engine/discretisation/equal_frequency.py` & `feature_engine-1.8.0/feature_engine/discretisation/equal_frequency.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/discretisation/equal_width.py` & `feature_engine-1.8.0/feature_engine/discretisation/equal_width.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/discretisation/geometric_width.py` & `feature_engine-1.8.0/feature_engine/discretisation/geometric_width.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/encoding/__init__.py` & `feature_engine-1.8.0/feature_engine/encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/encoding/base_encoder.py` & `feature_engine-1.8.0/feature_engine/encoding/base_encoder.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/encoding/count_frequency.py` & `feature_engine-1.8.0/feature_engine/encoding/count_frequency.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/encoding/decision_tree.py` & `feature_engine-1.8.0/feature_engine/encoding/decision_tree.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,70 @@
 # Authors: Soledad Galli <solegalli@protonmail.com>
 # License: BSD 3 clause
 
 from typing import List, Optional, Union
 
+import numpy as np
 import pandas as pd
 from sklearn.pipeline import Pipeline
 from sklearn.utils.multiclass import check_classification_targets, type_of_target
 
 from feature_engine._docstrings.fit_attributes import (
     _feature_names_in_docstring,
     _n_features_in_docstring,
     _variables_attribute_docstring,
 )
 from feature_engine._docstrings.init_parameters.all_trasnformers import (
     _variables_categorical_docstring,
 )
-from feature_engine._docstrings.init_parameters.encoders import _ignore_format_docstring
-from feature_engine._docstrings.methods import _fit_transform_docstring
+from feature_engine._docstrings.init_parameters.encoders import (
+    _ignore_format_docstring,
+    _unseen_docstring,
+)
+from feature_engine._docstrings.methods import (
+    _fit_transform_docstring,
+    _inverse_transform_docstring,
+)
 from feature_engine._docstrings.substitute import Substitution
 from feature_engine.dataframe_checks import _check_contains_na, check_X_y
 from feature_engine.discretisation import DecisionTreeDiscretiser
+from feature_engine.encoding._helper_functions import check_parameter_unseen
 from feature_engine.encoding.base_encoder import (
     CategoricalInitMixin,
     CategoricalMethodsMixin,
 )
 from feature_engine.encoding.ordinal import OrdinalEncoder
 from feature_engine.tags import _return_tags
 
 
+_unseen_docstring = (
+    _unseen_docstring
+    + """ If `'encode'` unseen categories will be encoded as `fill_value`."""
+)
+
+
 @Substitution(
     ignore_format=_ignore_format_docstring,
     variables=_variables_categorical_docstring,
     variables_=_variables_attribute_docstring,
+    unseen=_unseen_docstring,
     feature_names_in_=_feature_names_in_docstring,
     n_features_in_=_n_features_in_docstring,
     fit_transform=_fit_transform_docstring,
+    inverse_transform=_inverse_transform_docstring,
 )
 class DecisionTreeEncoder(CategoricalInitMixin, CategoricalMethodsMixin):
     """
-    The DecisionTreeEncoder() encodes categorical variables with predictions
+    The DecisionTreeEncoder() encodes categorical variables with the predictions
     of a decision tree.
 
-    The encoder first fits a decision tree using a single feature and the target (fit),
-    and then replaces the values of the original feature by the predictions of the
-    tree (transform). The transformer will train a decision tree per every feature to
-    encode.
+    The encoder fits a single feature decision tree to predict the target, and
+    with that, it creates mappings from category to prediction value. Then, it uses
+    these mappings to replace the categories of the feature. The encoder trains a
+    decision tree per feature to encode.
 
     The DecisionTreeEncoder() will encode only categorical variables by default
     (type 'object' or 'categorical'). You can pass a list of variables to encode or the
     encoder will find and encode all categorical variables.
 
     With `ignore_format=True` you have the option to encode numerical variables as
     well. In this case, you can either enter the list of variables to encode, or the
@@ -107,46 +123,53 @@
         DecisionTreeClassifier(). For reproducibility it is recommended to set
         the random_state to an integer.
 
     {variables}
 
     {ignore_format}
 
+    precision: int, default=None
+        The precision at which to store and display the category mappings. In other
+        words, the number of decimals after the comma for the tree predictions.
+
+    {unseen}
+
+    fill_value: float, default=None
+        The value used to encode unseen categories. Only used when `unseen='encode'`.
+
     Attributes
     ----------
-    encoder_:
-        sklearn Pipeline containing the ordinal encoder and the decision tree.
+    encoder_dict_:
+        Dictionary with the prediction per category, per variable.
 
     {variables_}
 
     {feature_names_in_}
 
     {n_features_in_}
 
     Methods
     -------
     fit:
         Fit a decision tree per variable.
 
     {fit_transform}
 
+    {inverse_transform}
+
     transform:
         Replace categorical variable by the predictions of the decision tree.
 
     Notes
     -----
     The authors designed this method originally to work with numerical variables. We
     can replace numerical variables by the predictions of a decision tree utilising the
-    DecisionTreeDiscretiser(). Here we extend this functionality to work also with
+    DecisionTreeDiscretiser(). Here, we extend this functionality to work also with
     categorical variables.
 
-    NAN are introduced when encoding categories that were not present in the training
-    dataset. If this happens, try grouping infrequent categories using the
-    RareLabelEncoder().
-
     See Also
     --------
     sklearn.ensemble.DecisionTreeRegressor
     sklearn.ensemble.DecisionTreeClassifier
     feature_engine.discretisation.DecisionTreeDiscretiser
     feature_engine.encoding.RareLabelEncoder
     feature_engine.encoding.OrdinalEncoder
@@ -194,23 +217,50 @@
         cv=3,
         scoring: str = "neg_mean_squared_error",
         param_grid: Optional[dict] = None,
         regression: bool = True,
         random_state: Optional[int] = None,
         variables: Union[None, int, str, List[Union[str, int]]] = None,
         ignore_format: bool = False,
+        precision: Optional[int] = None,
+        unseen: str = "raise",
+        fill_value: Optional[float] = None,
     ) -> None:
 
+        if encoding_method not in ["ordered", "arbitrary"]:
+            raise ValueError(
+                "`encoding_method` takes only values 'ordered' and 'arbitrary'."
+                f" Got {encoding_method} instead."
+            )
+
+        if unseen == "encode" and (
+            fill_value is None or not isinstance(fill_value, (int, float))
+        ):
+            raise ValueError(
+                "When `unseen='encode'` you need to pass a number to `fill_value`. "
+                f"Got {fill_value} instead."
+            )
+
+        if precision is not None and (not isinstance(precision, int) or precision < 0):
+            raise ValueError(
+                "Parameter `precision` takes integers or None. "
+                f"Got {precision} instead."
+            )
+
+        check_parameter_unseen(unseen, ["ignore", "raise", "encode"])
         super().__init__(variables, ignore_format)
         self.encoding_method = encoding_method
         self.cv = cv
         self.scoring = scoring
         self.regression = regression
         self.param_grid = param_grid
         self.random_state = random_state
+        self.precision = precision
+        self.unseen = unseen
+        self.fill_value = fill_value
 
     def fit(self, X: pd.DataFrame, y: pd.Series):
         """
         Fit a decision tree per variable.
 
         Parameters
         ----------
@@ -237,44 +287,52 @@
             check_classification_targets(y)
 
         variables_ = self._check_or_select_variables(X)
         _check_contains_na(X, variables_)
 
         param_grid = self._assign_param_grid()
 
-        # initialize categorical encoder
-        cat_encoder = OrdinalEncoder(
+        encoder = OrdinalEncoder(
             encoding_method=self.encoding_method,
             variables=variables_,
             missing_values="raise",
             ignore_format=self.ignore_format,
-            unseen="raise",
         )
 
-        # initialize decision tree discretiser
-        tree_discretiser = DecisionTreeDiscretiser(
+        tree = DecisionTreeDiscretiser(
             cv=self.cv,
             scoring=self.scoring,
             variables=variables_,
             param_grid=param_grid,
             regression=self.regression,
             random_state=self.random_state,
         )
 
         # pipeline for the encoder
-        encoder_ = Pipeline(
+        pipe = Pipeline(
             [
-                ("categorical_encoder", cat_encoder),
-                ("tree_discretiser", tree_discretiser),
+                ("encoder", encoder),
+                ("tree", tree),
             ]
         )
 
-        encoder_.fit(X, y)
+        Xt = pipe.fit_transform(X, y)
+
+        encoder_ = {}
+        if self.precision is None:
+            for var in variables_:
+                encoder_[var] = dict(zip(X[var], Xt[var]))
+        else:
+            for var in variables_:
+                encoder_[var] = dict(zip(X[var], np.round(Xt[var], self.precision)))
+
+        if self.unseen == "encode":
+            self._unseen = self.fill_value
 
-        self.encoder_ = encoder_
+        self.encoder_dict_ = encoder_
         self.variables_ = variables_
         self._get_feature_names_in(X)
         return self
 
     def transform(self, X: pd.DataFrame) -> pd.DataFrame:
         """
         Replace categorical variables by the predictions of the decision tree.
@@ -287,22 +345,17 @@
         Returns
         -------
         X_new : pandas dataframe of shape = [n_samples, n_features].
             Dataframe with variables encoded with decision tree predictions.
         """
         X = self._check_transform_input_and_state(X)
         _check_contains_na(X, self.variables_)
-        X = self.encoder_.transform(X)
-        return X
+        X = self._encode(X)
 
-    def inverse_transform(self, X: pd.DataFrame):
-        """inverse_transform is not implemented for this transformer."""
-        raise NotImplementedError(
-            "inverse_transform is not implemented for this transformer."
-        )
+        return X
 
     def _assign_param_grid(self):
         if self.param_grid:
             param_grid = self.param_grid
         else:
             param_grid = {"max_depth": [1, 2, 3, 4]}
         return param_grid
```

### Comparing `feature_engine-1.7.0/feature_engine/encoding/mean_encoding.py` & `feature_engine-1.8.0/feature_engine/encoding/mean_encoding.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/encoding/one_hot.py` & `feature_engine-1.8.0/feature_engine/encoding/one_hot.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/encoding/ordinal.py` & `feature_engine-1.8.0/feature_engine/encoding/ordinal.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/encoding/rare_label.py` & `feature_engine-1.8.0/feature_engine/encoding/rare_label.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/encoding/similarity_encoder.py` & `feature_engine-1.8.0/feature_engine/encoding/similarity_encoder.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/encoding/woe.py` & `feature_engine-1.8.0/feature_engine/encoding/woe.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/imputation/__init__.py` & `feature_engine-1.8.0/feature_engine/imputation/__init__.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/imputation/arbitrary_number.py` & `feature_engine-1.8.0/feature_engine/imputation/arbitrary_number.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/imputation/base_imputer.py` & `feature_engine-1.8.0/feature_engine/imputation/base_imputer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/imputation/categorical.py` & `feature_engine-1.8.0/feature_engine/imputation/categorical.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/imputation/drop_missing_data.py` & `feature_engine-1.8.0/feature_engine/imputation/drop_missing_data.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/imputation/end_tail.py` & `feature_engine-1.8.0/feature_engine/imputation/end_tail.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/imputation/mean_median.py` & `feature_engine-1.8.0/feature_engine/imputation/mean_median.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/imputation/missing_indicator.py` & `feature_engine-1.8.0/feature_engine/imputation/missing_indicator.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/imputation/random_sample.py` & `feature_engine-1.8.0/feature_engine/imputation/random_sample.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/outliers/artbitrary.py` & `feature_engine-1.8.0/feature_engine/outliers/artbitrary.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/outliers/base_outlier.py` & `feature_engine-1.8.0/feature_engine/outliers/base_outlier.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Union
+from typing import List, Literal, Optional, Union
 
 import pandas as pd
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_is_fitted
 
 from feature_engine._base_transformers.mixins import GetFeatureNamesOutMixin
 from feature_engine._check_init_parameters.check_variables import (
@@ -110,23 +110,23 @@
     **Gaussian limits:**
 
     - right tail: mean + 3* std
     - left tail: mean - 3* std
 
     **IQR limits:**
 
-    - right tail: 75th quantile + 3* IQR
-    - left tail:  25th quantile - 3* IQR
+    - right tail: 75th quantile + 1.5* IQR
+    - left tail:  25th quantile - 1.5* IQR
 
     where IQR is the inter-quartile range: 75th quantile - 25th quantile.
 
     **MAD limits:**
 
-    - right tail: median + 3* MAD
-    - left tail:  median - 3* MAD
+    - right tail: median + 3.29* MAD
+    - left tail:  median - 3.29* MAD
 
     where MAD is the median absoulte deviation from the median.
 
     **percentiles:**
 
     - right tail: 95th percentile
     - left tail:  5th percentile
@@ -145,42 +145,56 @@
     percentiles. If fold=0.1, the limits will be the 10th and 90th percentiles.
     """.rstrip()
 
     def __init__(
         self,
         capping_method: str = "gaussian",
         tail: str = "right",
-        fold: Union[int, float] = 3,
+        fold: Union[int, float, Literal["auto"]] = "auto",
         variables: Union[None, int, str, List[Union[str, int]]] = None,
         missing_values: str = "raise",
     ) -> None:
 
-        if capping_method not in ["gaussian", "iqr", "quantiles", "mad"]:
+        if capping_method not in ("gaussian", "iqr", "quantiles", "mad"):
             raise ValueError(
-                "capping_method takes only values 'gaussian', 'iqr', 'mad', 'quantiles'"
+                f"capping_method must be 'gaussian', 'iqr', 'mad', 'quantiles'."
+                f" Got {capping_method} instead."
             )
 
-        if tail not in ["right", "left", "both"]:
-            raise ValueError("tail takes only values 'right', 'left' or 'both'")
+        if tail not in ("right", "left", "both"):
+            raise ValueError(
+                f"tail must be 'right', 'left' or 'both'. Got {tail} instead."
+            )
 
-        if fold <= 0:
-            raise ValueError("fold takes only positive numbers")
+        if (isinstance(fold, str) and (fold != "auto")) or (
+            isinstance(fold, (int, float)) and (fold <= 0)
+        ):
+            raise ValueError(
+                f"fold must be a positive number or 'auto'. Got {fold} instead."
+            )
 
-        if capping_method == "quantiles" and fold > 0.2 and fold != 3:
+        if (
+            capping_method == "quantiles"
+            and isinstance(fold, (int, float))
+            and fold > 0.2
+        ):
             raise ValueError(
                 "with capping_method ='quantiles', fold takes values between 0 and "
                 "0.20 only."
             )
 
-        if missing_values not in ["raise", "ignore"]:
-            raise ValueError("missing_values takes only values 'raise' or 'ignore'")
+        if missing_values not in ("raise", "ignore"):
+            raise ValueError(
+                f"missing_values must be 'raise' or 'ignore'."
+                f" Got {missing_values} instead."
+            )
 
         self.capping_method = capping_method
         self.tail = tail
-        self.fold = 0.05 if (capping_method == "quantiles") & (fold == 3) else fold
+        self.fold = fold
         self.variables = _check_variables_input_value(variables)
         self.missing_values = missing_values
 
     def fit(self, X: pd.DataFrame, y: Optional[pd.Series] = None):
         """
         Learn the values that should be used to replace outliers.
 
@@ -206,60 +220,75 @@
             # check if dataset contains na
             _check_contains_na(X, self.variables_)
             _check_contains_inf(X, self.variables_)
 
         self.right_tail_caps_ = {}
         self.left_tail_caps_ = {}
 
+        if self.fold == "auto":
+            self.fold_ = self._calculate_fold()
+        else:
+            self.fold_ = self.fold
+
         if self.capping_method == "gaussian":
             bias = X[self.variables_].mean()
             scale = X[self.variables_].std(ddof=0)
         elif self.capping_method == "iqr":
             bias = X[self.variables_].quantile((0.75, 0.25))
             scale = bias.loc[0.75] - bias.loc[0.25]
         elif self.capping_method == "quantiles":
-            bias = X[self.variables_].quantile((1 - self.fold, self.fold))
-            scale = bias.loc[1 - self.fold] - bias.loc[self.fold]
+            bias = X[self.variables_].quantile((1 - self.fold_, self.fold_))
+            scale = bias.loc[1 - self.fold_] - bias.loc[self.fold_]
         elif self.capping_method == "mad":
             bias = X[self.variables_].median()
             # scaling factor for normal distribution
             scale = (X[self.variables_] - bias).abs().median() / 0.67449
         if (scale == 0).any():
             raise ValueError(
                 f"Input columns {scale[scale == 0].index.tolist()!r}"
                 f" have low variation for method {self.capping_method!r}."
                 f" Try other capping methods or drop these columns."
             )
 
         # estimate the end values
-        if self.tail in ["right", "both"]:
+        if self.tail in ("right", "both"):
             if self.capping_method in ("gaussian", "mad"):
-                self.right_tail_caps_ = (bias + self.fold * scale).to_dict()
+                self.right_tail_caps_ = (bias + self.fold_ * scale).to_dict()
 
             elif self.capping_method == "iqr":
-                self.right_tail_caps_ = (bias.loc[0.75] + self.fold * scale).to_dict()
+                self.right_tail_caps_ = (bias.loc[0.75] + self.fold_ * scale).to_dict()
 
             elif self.capping_method == "quantiles":
-                self.right_tail_caps_ = bias.loc[1 - self.fold].to_dict()
+                self.right_tail_caps_ = bias.loc[1 - self.fold_].to_dict()
 
-        if self.tail in ["left", "both"]:
+        if self.tail in ("left", "both"):
             if self.capping_method in ("gaussian", "mad"):
-                self.left_tail_caps_ = (bias - self.fold * scale).to_dict()
+                self.left_tail_caps_ = (bias - self.fold_ * scale).to_dict()
 
             elif self.capping_method == "iqr":
-                self.left_tail_caps_ = (bias.loc[0.25] - self.fold * scale).to_dict()
+                self.left_tail_caps_ = (bias.loc[0.25] - self.fold_ * scale).to_dict()
 
             elif self.capping_method == "quantiles":
-                self.left_tail_caps_ = bias.loc[self.fold].to_dict()
+                self.left_tail_caps_ = bias.loc[self.fold_].to_dict()
 
         self.feature_names_in_ = X.columns.to_list()
         self.n_features_in_ = X.shape[1]
 
         return self
 
+    def _calculate_fold(self) -> float:
+        if self.capping_method == "quantiles":
+            return 0.05
+        elif self.capping_method == "iqr":
+            return 1.5
+        elif self.capping_method == "mad":
+            return 3.29
+        else:
+            return 3.0
+
     def _more_tags(self):
         tags_dict = _return_tags()
         tags_dict["variables"] = "numerical"
         # =======  this tests fail because the transformers throw an error
         # when variance of the any input feature is 0.
         # Nothing to do with the test itself but
         # mostly with the data created and used in the test
```

### Comparing `feature_engine-1.7.0/feature_engine/outliers/trimmer.py` & `feature_engine-1.8.0/feature_engine/outliers/trimmer.py`

 * *Files 20% similar despite different names*

```diff
@@ -76,27 +76,47 @@
 
     {variables_}
 
     {feature_names_in_}
 
     {n_features_in_}
 
+    fold_:
+        Factor multiplying the std, mad, iqr or alternative the percentile. Only
+        different from `fold` when `fold="auto"`.
+
     Methods
     -------
     fit:
         Find maximum and minimum values.
 
     {fit_transform}
 
     transform:
         Remove outliers.
 
     transform_x_y:
         Remove rows with outliers from X set and y.
 
+    References
+    ----------
+    .. [1] Rousseeuw, Croux. "Alternatives to the mean absolute deviation". Journal of
+       the American Statistical Association, 1993. http://www.jstor.org/stable/2291267 .
+
+    .. [2] Leys, et. al. "Do not use standard deviation around the mean, use absolute
+       deviation around the median". Journal of Experimental Social Psychology, 2013.
+       http://dx.doi.org/10.1016/j.jesp.2013.03.013.
+
+    .. [3] Thériault, et. al. Check your outliers! An introduction to identifying
+       statistical outliers in R with easystats. Behavior Research Methods, 2024.
+       https://doi.org/10.3758/s13428-024-02356-w
+
+    .. [4] Dixon. Simplified Estimation from Censored Normal Samples. The Annals of
+       Mathematical Statistics, 1960. http://www.jstor.org/stable/2237953
+
     Examples
     --------
 
     >>> import pandas as pd
     >>> from feature_engine.outliers import OutlierTrimmer
     >>> X = pd.DataFrame(dict(x = [0.49671,
     >>>                         -0.1382,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `feature_engine-1.7.0/feature_engine/outliers/winsorizer.py` & `feature_engine-1.8.0/feature_engine/outliers/winsorizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Authors: Soledad Galli <solegalli@protonmail.com>
 # License: BSD 3 clause
 
-from typing import List, Union
+from typing import List, Literal, Union
 
 import numpy as np
 import pandas as pd
 
 from feature_engine._docstrings.fit_attributes import (
     _feature_names_in_docstring,
     _left_tail_caps_docstring,
@@ -83,24 +83,44 @@
 
     {variables_}
 
     {feature_names_in_}
 
     {n_features_in_}
 
+    fold_:
+        Factor multiplying the std, mad, iqr or alternative the percentile. Only
+        different from `fold` when `fold="auto"`.
+
     Methods
     -------
     fit:
         Learn the values that will replace the outliers.
 
     {fit_transform}
 
     transform:
         Cap the variables.
 
+    References
+    ----------
+    .. [1] Rousseeuw, Croux. "Alternatives to the mean absolute deviation". Journal of
+       the American Statistical Association, 1993. http://www.jstor.org/stable/2291267 .
+
+    .. [2] Leys, et. al. "Do not use standard deviation around the mean, use absolute
+       deviation around the median". Journal of Experimental Social Psychology, 2013.
+       http://dx.doi.org/10.1016/j.jesp.2013.03.013.
+
+    .. [3] Thériault, et. al. Check your outliers! An introduction to identifying
+       statistical outliers in R with easystats. Behavior Research Methods, 2024.
+       https://doi.org/10.3758/s13428-024-02356-w
+
+    .. [4] Dixon. Simplified Estimation from Censored Normal Samples. The Annals of
+       Mathematical Statistics, 1960. http://www.jstor.org/stable/2237953
+
     Examples
     --------
 
     >>> import numpy as np
     >>> import pandas as pd
     >>> from feature_engine.outliers import Winsorizer
     >>> np.random.seed(42)
@@ -141,15 +161,15 @@
     9  0.542560
     """
 
     def __init__(
         self,
         capping_method: str = "gaussian",
         tail: str = "right",
-        fold: Union[int, float] = 3,
+        fold: Union[int, float, Literal["auto"]] = "auto",
         add_indicators: bool = False,
         variables: Union[None, int, str, List[Union[str, int]]] = None,
         missing_values: str = "raise",
     ) -> None:
         if not isinstance(add_indicators, bool):
             raise ValueError(
                 "add_indicators takes only booleans True and False"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `feature_engine-1.7.0/feature_engine/pipeline/pipeline.py` & `feature_engine-1.8.0/feature_engine/pipeline/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 
 # Looked at imbalanced learn pipeline as template:
 # https://github.com/scikit-learn-contrib/imbalanced-learn
 
 from sklearn import pipeline
 from sklearn.base import _fit_context, clone
 from sklearn.pipeline import _final_estimator_has, _fit_transform_one
-from sklearn.utils import _print_elapsed_time
+try:
+    from sklearn.utils import _print_elapsed_time
+except ImportError:
+    from sklearn.utils._user_interface import _print_elapsed_time
 from sklearn.utils._metadata_requests import METHODS
 from sklearn.utils._param_validation import HasMethods, Hidden
 from sklearn.utils.metadata_routing import _routing_enabled, process_routing
 from sklearn.utils.metaestimators import available_if
 from sklearn.utils.validation import check_memory
 
 METHODS.append("transform_x_y")
```

### Comparing `feature_engine-1.7.0/feature_engine/preprocessing/match_categories.py` & `feature_engine-1.8.0/feature_engine/preprocessing/match_categories.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/preprocessing/match_columns.py` & `feature_engine-1.8.0/feature_engine/preprocessing/match_columns.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/__init__.py` & `feature_engine-1.8.0/feature_engine/selection/__init__.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/_selection_constants.py` & `feature_engine-1.8.0/feature_engine/selection/_selection_constants.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/base_recursive_selector.py` & `feature_engine-1.8.0/feature_engine/selection/base_recursive_selector.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/base_selection_functions.py` & `feature_engine-1.8.0/feature_engine/selection/base_selection_functions.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/base_selector.py` & `feature_engine-1.8.0/feature_engine/selection/base_selector.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/drop_constant_features.py` & `feature_engine-1.8.0/feature_engine/selection/drop_constant_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/drop_correlated_features.py` & `feature_engine-1.8.0/feature_engine/selection/drop_correlated_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/drop_duplicate_features.py` & `feature_engine-1.8.0/feature_engine/selection/drop_duplicate_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/drop_features.py` & `feature_engine-1.8.0/feature_engine/selection/drop_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/drop_psi_features.py` & `feature_engine-1.8.0/feature_engine/selection/drop_psi_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/information_value.py` & `feature_engine-1.8.0/feature_engine/selection/information_value.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/probe_feature_selection.py` & `feature_engine-1.8.0/feature_engine/selection/probe_feature_selection.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/recursive_feature_addition.py` & `feature_engine-1.8.0/feature_engine/selection/recursive_feature_addition.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/recursive_feature_elimination.py` & `feature_engine-1.8.0/feature_engine/selection/recursive_feature_elimination.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/shuffle_features.py` & `feature_engine-1.8.0/feature_engine/selection/shuffle_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/single_feature_performance.py` & `feature_engine-1.8.0/feature_engine/selection/single_feature_performance.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/smart_correlation_selection.py` & `feature_engine-1.8.0/feature_engine/selection/smart_correlation_selection.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/selection/target_mean_selection.py` & `feature_engine-1.8.0/feature_engine/selection/target_mean_selection.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/tags.py` & `feature_engine-1.8.0/feature_engine/tags.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/timeseries/forecasting/base_forecast_transformers.py` & `feature_engine-1.8.0/feature_engine/timeseries/forecasting/base_forecast_transformers.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/timeseries/forecasting/expanding_window_features.py` & `feature_engine-1.8.0/feature_engine/timeseries/forecasting/expanding_window_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/timeseries/forecasting/lag_features.py` & `feature_engine-1.8.0/feature_engine/timeseries/forecasting/lag_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/timeseries/forecasting/window_features.py` & `feature_engine-1.8.0/feature_engine/timeseries/forecasting/window_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/transformation/__init__.py` & `feature_engine-1.8.0/feature_engine/transformation/__init__.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/transformation/arcsin.py` & `feature_engine-1.8.0/feature_engine/transformation/arcsin.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/transformation/boxcox.py` & `feature_engine-1.8.0/feature_engine/transformation/boxcox.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/transformation/log.py` & `feature_engine-1.8.0/feature_engine/transformation/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,14 +158,16 @@
 
         # check contains zero or negative values
         if (X[self.variables_] <= 0).any().any():
             raise ValueError(
                 "Some variables contain zero or negative values, can't apply log"
             )
 
+        X[self.variables_] = X[self.variables_].astype(float)
+
         # transform
         if self.base == "e":
             X.loc[:, self.variables_] = np.log(X.loc[:, self.variables_])
         elif self.base == "10":
             X.loc[:, self.variables_] = np.log10(X.loc[:, self.variables_])
 
         return X
@@ -379,14 +381,16 @@
         # check variable is positive after adding c
         if (X[self.variables_] + self.C_ <= 0).any().any():
             raise ValueError(
                 "Some variables contain zero or negative values after adding"
                 + "constant C, can't apply log"
             )
 
+        X[self.variables_] = X[self.variables_].astype(float)
+
         # transform
         if self.base == "e":
             X.loc[:, self.variables_] = np.log(X.loc[:, self.variables_] + self.C_)
         elif self.base == "10":
             X.loc[:, self.variables_] = np.log10(X.loc[:, self.variables_] + self.C_)
 
         return X
```

### Comparing `feature_engine-1.7.0/feature_engine/transformation/power.py` & `feature_engine-1.8.0/feature_engine/transformation/power.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/transformation/reciprocal.py` & `feature_engine-1.8.0/feature_engine/transformation/reciprocal.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/transformation/yeojohnson.py` & `feature_engine-1.8.0/feature_engine/transformation/yeojohnson.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/variable_handling/__init__.py` & `feature_engine-1.8.0/feature_engine/variable_handling/__init__.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/variable_handling/_variable_type_checks.py` & `feature_engine-1.8.0/feature_engine/variable_handling/_variable_type_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/variable_handling/check_variables.py` & `feature_engine-1.8.0/feature_engine/variable_handling/check_variables.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/variable_handling/find_variables.py` & `feature_engine-1.8.0/feature_engine/variable_handling/find_variables.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/variable_handling/retain_variables.py` & `feature_engine-1.8.0/feature_engine/variable_handling/retain_variables.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine/wrappers/wrappers.py` & `feature_engine-1.8.0/feature_engine/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/feature_engine.egg-info/PKG-INFO` & `feature_engine-1.8.0/feature_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature-engine
-Version: 1.7.0
+Version: 1.8.0
 Summary: Feature engineering and selection package with Scikit-learn's fit transform functionality
 Home-page: http://github.com/feature-engine/feature_engine
 Author: Soledad Galli
 Author-email: solegalli@protonmail.com
 License: BSD 3 clause
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# Feature Engine
+# Feature-engine
 
 [![feature-engine logo](https://raw.githubusercontent.com/feature-engine/feature_engine/main/docs/images/logo/FeatureEngine.png)](http://feature-engine.readthedocs.io)
 
 | | |
 | --- | --- |
 | Package | [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/feature_engine?logo=Python)](https://pypi.org/project/feature-engine/) [![PyPI](https://img.shields.io/pypi/v/feature_engine?logo=PyPI)](https://pypi.org/project/feature-engine) [![Conda](https://img.shields.io/conda/v/conda-forge/feature_engine?logo=Anaconda)](https://anaconda.org/conda-forge/feature_engine) [![Monthly Downloads](https://img.shields.io/pypi/dm/feature-engine)](https://img.shields.io/pypi/dm/feature-engine)  [![Downloads](https://static.pepy.tech/personalized-badge/feature-engine?period=total&units=international_system&left_color=grey&right_color=green&left_text=total-downloads%20(pypi))](https://pepy.tech/project/feature-engine)|
 | Meta | [![GitHub](https://img.shields.io/github/license/feature-engine/feature_engine)](https://github.com/feature-engine/feature_engine/blob/master/LICENSE.md) [![GitHub contributors](https://img.shields.io/github/contributors/feature-engine/feature_engine?logo=GitHub)](https://github.com/feature-engine/feature_engine/graphs/contributors) [![Gitter](https://img.shields.io/gitter/room/feature-engine/feaure_engine?logo=Gitter)](https://gitter.im/feature_engine/community) [![first-timers-only](https://img.shields.io/badge/first--timers--only-friendly-blue.svg?style=flat)](https://www.firsttimersonly.com/) [![Sponsorship](https://img.shields.io/badge/Powered%20By-TrainInData-orange.svg)](https://www.trainindata.com/) |
@@ -128,14 +128,15 @@
 * BoxCoxTransformer
 * YeoJohnsonTransformer
 
 ### Variable Creation:
  * MathFeatures
  * RelativeFeatures
  * CyclicalFeatures
+ * DecisionTreeFeatures()
 
 ### Feature Selection:
  * DropFeatures
  * DropConstantFeatures
  * DropDuplicateFeatures
  * DropCorrelatedFeatures
  * SmartCorrelationSelection
```

### Comparing `feature_engine-1.7.0/feature_engine.egg-info/SOURCES.txt` & `feature_engine-1.8.0/feature_engine.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+CODE_OF_CONDUCT.md
 LICENSE.md
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 test_requirements.txt
 ./requirements.txt
@@ -24,27 +25,29 @@
 feature_engine/_check_init_parameters/check_variables.py
 feature_engine/_docstrings/__init__.py
 feature_engine/_docstrings/fit_attributes.py
 feature_engine/_docstrings/methods.py
 feature_engine/_docstrings/substitute.py
 feature_engine/_docstrings/init_parameters/__init__.py
 feature_engine/_docstrings/init_parameters/all_trasnformers.py
+feature_engine/_docstrings/init_parameters/creation.py
 feature_engine/_docstrings/init_parameters/discretisers.py
 feature_engine/_docstrings/init_parameters/encoders.py
 feature_engine/_docstrings/init_parameters/outliers.py
 feature_engine/_docstrings/init_parameters/selection.py
 feature_engine/_docstrings/selection/__init__.py
 feature_engine/_docstrings/selection/_docstring.py
 feature_engine/_prediction/__init__.py
 feature_engine/_prediction/base_predictor.py
 feature_engine/_prediction/target_mean_classifier.py
 feature_engine/_prediction/target_mean_regressor.py
 feature_engine/creation/__init__.py
 feature_engine/creation/base_creation.py
 feature_engine/creation/cyclical_features.py
+feature_engine/creation/decision_tree_features.py
 feature_engine/creation/math_features.py
 feature_engine/creation/relative_features.py
 feature_engine/datasets/__init__.py
 feature_engine/datasets/titanic.py
 feature_engine/datetime/__init__.py
 feature_engine/datetime/_datetime_constants.py
 feature_engine/datetime/datetime.py
@@ -136,14 +139,15 @@
 tests/test_check_init_parameters/__init__.py
 tests/test_check_init_parameters/test_check_init_input_params.py
 tests/test_check_init_parameters/test_check_input_dictionary.py
 tests/test_check_init_parameters/test_check_variables.py
 tests/test_creation/__init__.py
 tests/test_creation/test_check_estimator_creation.py
 tests/test_creation/test_cyclical_features.py
+tests/test_creation/test_decision_tree_features.py
 tests/test_creation/test_math_features.py
 tests/test_creation/test_relative_features.py
 tests/test_datetime/__init__.py
 tests/test_datetime/conftest.py
 tests/test_datetime/test_check_estimator_datetime.py
 tests/test_datetime/test_datetime_features.py
 tests/test_datetime/test_datetime_subtraction.py
```

### Comparing `feature_engine-1.7.0/setup.py` & `feature_engine-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/estimator_checks/dataframe_for_checks.py` & `feature_engine-1.8.0/tests/estimator_checks/dataframe_for_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/estimator_checks/estimator_checks.py` & `feature_engine-1.8.0/tests/estimator_checks/estimator_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/estimator_checks/fit_functionality_checks.py` & `feature_engine-1.8.0/tests/estimator_checks/fit_functionality_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/estimator_checks/get_feature_names_out_checks.py` & `feature_engine-1.8.0/tests/estimator_checks/get_feature_names_out_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/estimator_checks/init_params_allowed_values_checks.py` & `feature_engine-1.8.0/tests/estimator_checks/init_params_allowed_values_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/estimator_checks/init_params_triggered_functionality_checks.py` & `feature_engine-1.8.0/tests/estimator_checks/init_params_triggered_functionality_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/estimator_checks/non_fitted_error_checks.py` & `feature_engine-1.8.0/tests/estimator_checks/non_fitted_error_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/estimator_checks/variable_selection_checks.py` & `feature_engine-1.8.0/tests/estimator_checks/variable_selection_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_check_init_parameters/test_check_init_input_params.py` & `feature_engine-1.8.0/tests/test_check_init_parameters/test_check_init_input_params.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_check_init_parameters/test_check_input_dictionary.py` & `feature_engine-1.8.0/tests/test_check_init_parameters/test_check_input_dictionary.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_check_init_parameters/test_check_variables.py` & `feature_engine-1.8.0/tests/test_check_init_parameters/test_check_variables.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_creation/test_check_estimator_creation.py` & `feature_engine-1.8.0/tests/test_creation/test_check_estimator_creation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import pandas as pd
 import pytest
 from sklearn.pipeline import Pipeline
 from sklearn.utils.estimator_checks import check_estimator
 
-from feature_engine.creation import CyclicalFeatures, MathFeatures, RelativeFeatures
+from feature_engine.creation import (
+    CyclicalFeatures,
+    DecisionTreeFeatures,
+    MathFeatures,
+    RelativeFeatures,
+)
 from tests.estimator_checks.estimator_checks import check_feature_engine_estimator
 
 _estimators = [
     MathFeatures(variables=["x0", "x1"], func="mean", missing_values="ignore"),
     RelativeFeatures(
         variables=["x0", "x1"], reference=["x0"], func=["add"], missing_values="ignore"
     ),
     CyclicalFeatures(),
+    DecisionTreeFeatures(regression=False),
 ]
 
 
 @pytest.mark.parametrize("estimator", _estimators)
 def test_check_estimator_from_sklearn(estimator):
     return check_estimator(estimator)
```

### Comparing `feature_engine-1.7.0/tests/test_creation/test_cyclical_features.py` & `feature_engine-1.8.0/tests/test_creation/test_cyclical_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_creation/test_math_features.py` & `feature_engine-1.8.0/tests/test_creation/test_math_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_creation/test_relative_features.py` & `feature_engine-1.8.0/tests/test_creation/test_relative_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_datetime/conftest.py` & `feature_engine-1.8.0/tests/test_datetime/conftest.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_datetime/test_check_estimator_datetime.py` & `feature_engine-1.8.0/tests/test_datetime/test_check_estimator_datetime.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_datetime/test_datetime_features.py` & `feature_engine-1.8.0/tests/test_datetime/test_datetime_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_datetime/test_datetime_subtraction.py` & `feature_engine-1.8.0/tests/test_datetime/test_datetime_subtraction.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_discretisation/test_arbitrary_discretiser.py` & `feature_engine-1.8.0/tests/test_discretisation/test_arbitrary_discretiser.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_discretisation/test_base_discretizer.py` & `feature_engine-1.8.0/tests/test_discretisation/test_base_discretizer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_discretisation/test_check_estimator_discretisers.py` & `feature_engine-1.8.0/tests/test_discretisation/test_check_estimator_discretisers.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_discretisation/test_decision_tree_discretiser.py` & `feature_engine-1.8.0/tests/test_discretisation/test_equal_width_discretiser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,134 +1,70 @@
-import numpy as np
 import pandas as pd
 import pytest
 from sklearn.exceptions import NotFittedError
 
-from feature_engine.discretisation import DecisionTreeDiscretiser, EqualWidthDiscretiser
+from feature_engine.discretisation import EqualWidthDiscretiser
 
 
-def test_classification(df_normal_dist):
-
-    transformer = DecisionTreeDiscretiser(
-        cv=3,
-        scoring="roc_auc",
-        variables=None,
-        param_grid={"max_depth": [1, 2, 3, 4]},
-        regression=False,
-        random_state=0,
-    )
-    np.random.seed(0)
-    y = pd.Series(np.random.binomial(1, 0.7, 100))
-    X = transformer.fit_transform(df_normal_dist, y)
-    X_t = [1.0, 0.71, 0.93, 0.0]
+def test_automatically_find_variables_and_return_as_numeric(df_normal_dist):
+    # test case 1: automatically select variables, return_object=False
+    transformer = EqualWidthDiscretiser(bins=10, variables=None, return_object=False)
+    X = transformer.fit_transform(df_normal_dist)
+
+    # fit parameters
+    _, bins = pd.cut(x=df_normal_dist["var"], bins=10, retbins=True, duplicates="drop")
+    bins[0] = float("-inf")
+    bins[len(bins) - 1] = float("inf")
+
+    # transform output
+    X_t = [x for x in range(0, 10)]
+    val_counts = [18, 17, 16, 13, 11, 7, 7, 5, 5, 1]
 
     # init params
-    assert transformer.cv == 3
+    assert transformer.bins == 10
     assert transformer.variables is None
-    assert transformer.scoring == "roc_auc"
-    assert transformer.regression is False
+    assert transformer.return_object is False
     # fit params
     assert transformer.variables_ == ["var"]
     assert transformer.n_features_in_ == 1
     # transform params
-    assert all(x for x in np.round(X["var"].unique(), 2) if x not in X_t)
-    assert np.round(transformer.scores_dict_["var"], 3) == np.round(
-        0.717391304347826, 3
-    )
-
-
-def test_regression(df_normal_dist):
-
-    transformer = DecisionTreeDiscretiser(
-        cv=3,
-        scoring="neg_mean_squared_error",
-        variables=None,
-        param_grid={"max_depth": [1, 2, 3, 4]},
-        regression=True,
-        random_state=0,
-    )
-    np.random.seed(0)
-    y = pd.Series(pd.Series(np.random.normal(0, 0.1, 100)))
-    X = transformer.fit_transform(df_normal_dist, y)
-    X_t = [
-        0.19,
-        0.04,
-        0.11,
-        0.23,
-        -0.09,
-        -0.02,
-        0.01,
-        0.15,
-        0.07,
-        -0.26,
-        0.09,
-        -0.07,
-        -0.16,
-        -0.2,
-        -0.04,
-        -0.12,
-    ]
+    assert (transformer.binner_dict_["var"] == bins).all()
+    assert all(x for x in X["var"].unique() if x not in X_t)
+    # in equal width discretisation, intervals get different number of values
+    assert all(x for x in X["var"].value_counts() if x not in val_counts)
 
-    # init params
-    assert transformer.cv == 3
-    assert transformer.variables is None
-    assert transformer.scoring == "neg_mean_squared_error"
-    assert transformer.regression is True
-    # fit params
-    assert transformer.variables_ == ["var"]
-    assert transformer.n_features_in_ == 1
-    assert np.round(transformer.scores_dict_["var"], 3) == np.round(
-        -4.4373314584616444e-05, 3
-    )
-    # transform params
-    assert all(x for x in np.round(X["var"].unique(), 2) if x not in X_t)
+
+def test_automatically_find_variables_and_return_as_object(df_normal_dist):
+    transformer = EqualWidthDiscretiser(bins=10, variables=None, return_object=True)
+    X = transformer.fit_transform(df_normal_dist)
+    assert X["var"].dtypes == "O"
 
 
-def test_error_when_regression_is_not_bool():
+def test_error_when_bins_not_number():
     with pytest.raises(ValueError):
-        DecisionTreeDiscretiser(regression="other")
+        EqualWidthDiscretiser(bins="other")
 
 
-def test_error_if_y_not_passed(df_normal_dist):
-    # test case 3: raises error if target is not passed
-    with pytest.raises(TypeError):
-        encoder = DecisionTreeDiscretiser()
-        encoder.fit(df_normal_dist)
+def test_error_if_return_object_not_bool():
+    with pytest.raises(ValueError):
+        EqualWidthDiscretiser(return_object="other")
 
 
-def test_non_fitted_error(df_vartypes):
-    with pytest.raises(NotFittedError):
+def test_error_if_input_df_contains_na_in_fit(df_na):
+    # test case 3: when dataset contains na, fit method
+    with pytest.raises(ValueError):
         transformer = EqualWidthDiscretiser()
-        transformer.transform(df_vartypes)
-
-
-@pytest.fixture(scope="module")
-def df_discretise():
-    np.random.seed(42)
-    mu1, sigma1 = 0, 3
-    s1 = np.random.normal(mu1, sigma1, 20)
-    mu2, sigma2 = 3, 5
-    s2 = np.random.normal(mu2, sigma2, 20)
-    data = {
-        "var_A": s1,
-        "var_B": s2,
-        "target": [0, 1, 1, 0, 1, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1, 1],
-    }
+        transformer.fit(df_na)
 
-    df = pd.DataFrame(data)
 
-    return df
-
-
-def test_error_when_regression_is_true_and_target_is_binary(df_discretise):
+def test_error_if_input_df_contains_na_in_transform(df_vartypes, df_na):
+    # test case 4: when dataset contains na, transform method
     with pytest.raises(ValueError):
-        transformer = DecisionTreeDiscretiser(regression=True)
-        transformer.fit(df_discretise[["var_A", "var_B"]], df_discretise["target"])
+        transformer = EqualWidthDiscretiser()
+        transformer.fit(df_vartypes)
+        transformer.transform(df_na[["Name", "City", "Age", "Marks", "dob"]])
 
 
-def test_error_when_regression_is_false_and_target_is_continuous(df_discretise):
-    np.random.seed(42)
-    mu, sigma = 0, 3
-    y = np.random.normal(mu, sigma, len(df_discretise))
-    with pytest.raises(ValueError):
-        transformer = DecisionTreeDiscretiser(regression=False)
-        transformer.fit(df_discretise[["var_A", "var_B"]], y)
+def test_non_fitted_error(df_vartypes):
+    with pytest.raises(NotFittedError):
+        transformer = EqualWidthDiscretiser()
+        transformer.transform(df_vartypes)
```

### Comparing `feature_engine-1.7.0/tests/test_discretisation/test_equal_frequency_discretiser.py` & `feature_engine-1.8.0/tests/test_discretisation/test_equal_frequency_discretiser.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_discretisation/test_equal_width_discretiser.py` & `feature_engine-1.8.0/tests/test_discretisation/test_geometric_width_discretiser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,91 @@
+import numpy as np
 import pandas as pd
 import pytest
 from sklearn.exceptions import NotFittedError
 
-from feature_engine.discretisation import EqualWidthDiscretiser
+from feature_engine.discretisation import GeometricWidthDiscretiser
 
 
-def test_automatically_find_variables_and_return_as_numeric(df_normal_dist):
-    # test case 1: automatically select variables, return_object=False
-    transformer = EqualWidthDiscretiser(bins=10, variables=None, return_object=False)
+# test init params
+@pytest.mark.parametrize("param", [0.1, "hola", (True, False), {"a": True}, 2])
+def test_raises_error_when_return_object_not_bool(param):
+    with pytest.raises(ValueError):
+        GeometricWidthDiscretiser(return_object=param)
+
+
+@pytest.mark.parametrize("param", [0.1, "hola", (True, False), {"a": True}, 2])
+def test_raises_error_when_return_boundaries_not_bool(param):
+    with pytest.raises(ValueError):
+        GeometricWidthDiscretiser(return_boundaries=param)
+
+
+@pytest.mark.parametrize("param", [0.1, "hola", (True, False), {"a": True}, 0, -1])
+def test_raises_error_when_precision_not_int(param):
+    with pytest.raises(ValueError):
+        GeometricWidthDiscretiser(precision=param)
+
+
+@pytest.mark.parametrize("param", [0.1, "hola", (True, False), {"a": True}])
+def test_raises_error_when_bins_not_int(param):
+    with pytest.raises(ValueError):
+        GeometricWidthDiscretiser(bins=param)
+
+
+@pytest.mark.parametrize("params", [(False, 1), (True, 10)])
+def test_correct_param_assignment_at_init(params):
+    param1, param2 = params
+    t = GeometricWidthDiscretiser(
+        return_object=param1, return_boundaries=param1, precision=param2, bins=param2
+    )
+    assert t.return_object is param1
+    assert t.return_boundaries is param1
+    assert t.precision == param2
+    assert t.bins == param2
+
+
+def test_fit_and_transform_methods(df_normal_dist):
+    transformer = GeometricWidthDiscretiser(
+        bins=10, variables=None, return_object=False
+    )
     X = transformer.fit_transform(df_normal_dist)
 
-    # fit parameters
-    _, bins = pd.cut(x=df_normal_dist["var"], bins=10, retbins=True, duplicates="drop")
-    bins[0] = float("-inf")
-    bins[len(bins) - 1] = float("inf")
-
-    # transform output
-    X_t = [x for x in range(0, 10)]
-    val_counts = [18, 17, 16, 13, 11, 7, 7, 5, 5, 1]
-
-    # init params
-    assert transformer.bins == 10
-    assert transformer.variables is None
-    assert transformer.return_object is False
+    # manual calculation
+    min_, max_ = df_normal_dist["var"].min(), df_normal_dist["var"].max()
+    increment = np.power(max_ - min_, 1.0 / 10)
+    bins = np.r_[-np.inf, min_ + np.power(increment, np.arange(1, 10)), np.inf]
+    bins = np.sort(bins)
+
     # fit params
-    assert transformer.variables_ == ["var"]
-    assert transformer.n_features_in_ == 1
-    # transform params
     assert (transformer.binner_dict_["var"] == bins).all()
-    assert all(x for x in X["var"].unique() if x not in X_t)
-    # in equal width discretisation, intervals get different number of values
-    assert all(x for x in X["var"].value_counts() if x not in val_counts)
+
+    # transform params
+    assert (
+        X["var"] == pd.cut(df_normal_dist["var"], bins=bins, precision=7).cat.codes
+    ).all()
 
 
 def test_automatically_find_variables_and_return_as_object(df_normal_dist):
-    transformer = EqualWidthDiscretiser(bins=10, variables=None, return_object=True)
+    transformer = GeometricWidthDiscretiser(bins=10, variables=None, return_object=True)
     X = transformer.fit_transform(df_normal_dist)
     assert X["var"].dtypes == "O"
 
 
-def test_error_when_bins_not_number():
-    with pytest.raises(ValueError):
-        EqualWidthDiscretiser(bins="other")
-
-
-def test_error_if_return_object_not_bool():
-    with pytest.raises(ValueError):
-        EqualWidthDiscretiser(return_object="other")
-
-
 def test_error_if_input_df_contains_na_in_fit(df_na):
     # test case 3: when dataset contains na, fit method
+    transformer = GeometricWidthDiscretiser()
     with pytest.raises(ValueError):
-        transformer = EqualWidthDiscretiser()
         transformer.fit(df_na)
 
 
 def test_error_if_input_df_contains_na_in_transform(df_vartypes, df_na):
     # test case 4: when dataset contains na, transform method
+    transformer = GeometricWidthDiscretiser()
+    transformer.fit(df_vartypes)
     with pytest.raises(ValueError):
-        transformer = EqualWidthDiscretiser()
-        transformer.fit(df_vartypes)
         transformer.transform(df_na[["Name", "City", "Age", "Marks", "dob"]])
 
 
 def test_non_fitted_error(df_vartypes):
+    transformer = GeometricWidthDiscretiser()
     with pytest.raises(NotFittedError):
-        transformer = EqualWidthDiscretiser()
         transformer.transform(df_vartypes)
```

### Comparing `feature_engine-1.7.0/tests/test_encoding/test_base_encoders/test_categorical_init_mixin.py` & `feature_engine-1.8.0/tests/test_encoding/test_base_encoders/test_categorical_init_mixin.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_encoding/test_base_encoders/test_categorical_init_mixin_na.py` & `feature_engine-1.8.0/tests/test_encoding/test_base_encoders/test_categorical_init_mixin_na.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_encoding/test_base_encoders/test_categorical_method_mixin.py` & `feature_engine-1.8.0/tests/test_encoding/test_base_encoders/test_categorical_method_mixin.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_encoding/test_check_estimator_encoders.py` & `feature_engine-1.8.0/tests/test_encoding/test_check_estimator_encoders.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_encoding/test_count_frequency_encoder.py` & `feature_engine-1.8.0/tests/test_encoding/test_count_frequency_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,20 +23,24 @@
         CountFrequencyEncoder(unseen=errors)
 
 
 @pytest.mark.parametrize(
     "params", [("count", "raise", True), ("frequency", "ignore", False)]
 )
 def test_init_param_assignment(params):
-    CountFrequencyEncoder(
+    enc = CountFrequencyEncoder(
         encoding_method=params[0],
         missing_values=params[1],
         ignore_format=params[2],
         unseen=params[1],
     )
+    assert enc.encoding_method == params[0]
+    assert enc.missing_values == params[1]
+    assert enc.ignore_format == params[2]
+    assert enc.unseen == params[1]
 
 
 # fit and transform
 def test_encode_1_variable_with_counts(df_enc):
     # test case 1: 1 variable, counts
     encoder = CountFrequencyEncoder(encoding_method="count", variables=["var_A"])
     X = encoder.fit_transform(df_enc)
```

### Comparing `feature_engine-1.7.0/tests/test_encoding/test_helper_functions.py` & `feature_engine-1.8.0/tests/test_encoding/test_helper_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,9 +11,12 @@
     assert str(record.value) == msg
 
 
 @pytest.mark.parametrize("accepted", [["one", "two"], ["three", "four"]])
 def test_raises_error_when_error_not_in_accepted_values(accepted):
     with pytest.raises(ValueError) as record:
         check_parameter_unseen("zero", accepted)
-    msg = f"errors takes only values {', '.join(accepted)}." f"Got zero instead."
+    msg = (
+        f"Parameter `unseen` takes only values {', '.join(accepted)}."
+        " Got zero instead."
+    )
     assert str(record.value) == msg
```

### Comparing `feature_engine-1.7.0/tests/test_encoding/test_mean_encoder.py` & `feature_engine-1.8.0/tests/test_encoding/test_mean_encoder.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_encoding/test_onehot_encoder.py` & `feature_engine-1.8.0/tests/test_encoding/test_onehot_encoder.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_encoding/test_ordinal_encoder.py` & `feature_engine-1.8.0/tests/test_encoding/test_ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_encoding/test_rare_label_encoder.py` & `feature_engine-1.8.0/tests/test_encoding/test_rare_label_encoder.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_encoding/test_similarity_encoder.py` & `feature_engine-1.8.0/tests/test_encoding/test_similarity_encoder.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_encoding/test_woe/test_woe_class.py` & `feature_engine-1.8.0/tests/test_encoding/test_woe/test_woe_class.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_encoding/test_woe/test_woe_encoder.py` & `feature_engine-1.8.0/tests/test_encoding/test_woe/test_woe_encoder.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_imputation/test_arbitrary_number_imputer.py` & `feature_engine-1.8.0/tests/test_imputation/test_arbitrary_number_imputer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_imputation/test_categorical_imputer.py` & `feature_engine-1.8.0/tests/test_imputation/test_categorical_imputer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_imputation/test_check_estimator_imputers.py` & `feature_engine-1.8.0/tests/test_imputation/test_check_estimator_imputers.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_imputation/test_drop_missing_data.py` & `feature_engine-1.8.0/tests/test_imputation/test_drop_missing_data.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_imputation/test_end_tail_imputer.py` & `feature_engine-1.8.0/tests/test_imputation/test_end_tail_imputer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_imputation/test_mean_mdian_imputer.py` & `feature_engine-1.8.0/tests/test_imputation/test_mean_mdian_imputer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_imputation/test_missing_indicator.py` & `feature_engine-1.8.0/tests/test_imputation/test_missing_indicator.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_imputation/test_random_sample_imputer.py` & `feature_engine-1.8.0/tests/test_imputation/test_random_sample_imputer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_outliers/test_arbitrary_capper.py` & `feature_engine-1.8.0/tests/test_outliers/test_arbitrary_capper.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_outliers/test_check_estimator_outliers.py` & `feature_engine-1.8.0/tests/test_outliers/test_check_estimator_outliers.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_outliers/test_outlier_trimmer.py` & `feature_engine-1.8.0/tests/test_outliers/test_outlier_trimmer.py`

 * *Files 11% similar despite different names*

```diff
@@ -91,18 +91,21 @@
 
     Xt, yt = transformer.transform_x_y(df_normal_dist, y)
     assert len(Xt) == len(yt)
     assert len(Xt) != len(df_normal_dist)
     assert (Xt.index == yt.index).all()
 
 
-def test_quantile_fold_default_value():
-    # test case 1: Test quantiles, with fold default = 0.05
-    transformer = OutlierTrimmer(capping_method="quantiles")
-    assert transformer.fold == 0.05
+@pytest.mark.parametrize(
+    "strings,expected",
+    [("gaussian", 3), ("iqr", 1.5), ("mad", 3.29), ("quantiles", 0.05)],
+)
+def test_auto_fold_default_value(strings, expected, df_normal_dist):
+    transformer = OutlierTrimmer(capping_method=strings, fold="auto")
+    transformer.fit(df_normal_dist)
+    assert transformer.fold_ == expected
 
 
-@pytest.mark.parametrize("strings", ["gaussian", "iqr", "mad"])
-def test_other_fold_default_value(strings):
-    # test case 2: Test gaussian, iqr, mad, with fold default = 3
-    transformer = OutlierTrimmer(capping_method=strings)
-    assert transformer.fold == 3
+def test_low_variation(df_normal_dist):
+    transformer = OutlierTrimmer(capping_method="mad")
+    with pytest.raises(ValueError):
+        transformer.fit(df_normal_dist // 10)
```

### Comparing `feature_engine-1.7.0/tests/test_outliers/test_winsorizer.py` & `feature_engine-1.8.0/tests/test_outliers/test_winsorizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,25 +122,22 @@
     assert transformer.left_tail_caps_ == {}
     # test transform output
     pd.testing.assert_frame_equal(X, df_transf)
     assert math.isclose(X["var"].max(), 0.11823196128033647)
     assert math.isclose(df_transf["var"].max(), 0.11823196128033647)
 
 
-def test_quantile_fold_default_value():
-    # test case 1: Test quantiles, with fold default = 0.05
-    transformer = Winsorizer(capping_method="quantiles")
-    assert transformer.fold == 0.05
-
-
-@pytest.mark.parametrize("strings", ["gaussian", "iqr", "mad"])
-def test_other_fold_default_value(strings):
-    # test case 2: Test gaussian, iqr, mad, with fold default = 3
-    transformer = Winsorizer(capping_method=strings)
-    assert transformer.fold == 3
+@pytest.mark.parametrize(
+    "strings,expected",
+    [("gaussian", 3), ("iqr", 1.5), ("mad", 3.29), ("quantiles", 0.05)],
+)
+def test_auto_fold_default_value(strings, expected, df_normal_dist):
+    transformer = Winsorizer(capping_method=strings, fold="auto")
+    transformer.fit(df_normal_dist)
+    assert transformer.fold_ == expected
 
 
 def test_mad_capping_right_tail_with_fold_1(df_normal_dist):
     # test case 1: median and mad, right tail
     transformer = Winsorizer(capping_method="mad", tail="right", fold=1)
     X = transformer.fit_transform(df_normal_dist)
 
@@ -362,7 +359,13 @@
 
     tr = Winsorizer(tail="both", add_indicators=True, missing_values="ignore")
     tr.fit(df_na)
 
     out = ["Age_left", "Age_right", "Marks_left", "Marks_right"]
     assert tr.get_feature_names_out() == original_features + out
     assert tr.get_feature_names_out(original_features) == original_features + out
+
+
+def test_low_variation(df_normal_dist):
+    transformer = Winsorizer(capping_method="mad")
+    with pytest.raises(ValueError):
+        transformer.fit(df_normal_dist // 10)
```

### Comparing `feature_engine-1.7.0/tests/test_prediction/conftest.py` & `feature_engine-1.8.0/tests/test_prediction/conftest.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_prediction/test_check_estimator_prediction.py` & `feature_engine-1.8.0/tests/test_prediction/test_check_estimator_prediction.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_prediction/test_target_mean_classifier.py` & `feature_engine-1.8.0/tests/test_prediction/test_target_mean_classifier.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_prediction/test_target_mean_regressor.py` & `feature_engine-1.8.0/tests/test_prediction/test_target_mean_regressor.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_preprocessing/test_check_estimator_preprocessing.py` & `feature_engine-1.8.0/tests/test_preprocessing/test_check_estimator_preprocessing.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_preprocessing/test_match_categories.py` & `feature_engine-1.8.0/tests/test_preprocessing/test_match_categories.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_preprocessing/test_match_columns.py` & `feature_engine-1.8.0/tests/test_preprocessing/test_match_columns.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/conftest.py` & `feature_engine-1.8.0/tests/test_selection/conftest.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_base_selection_functions.py` & `feature_engine-1.8.0/tests/test_selection/test_base_selection_functions.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_base_selector.py` & `feature_engine-1.8.0/tests/test_selection/test_base_selector.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_check_estimator_selectors.py` & `feature_engine-1.8.0/tests/test_selection/test_check_estimator_selectors.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_drop_constant_features.py` & `feature_engine-1.8.0/tests/test_selection/test_drop_constant_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_drop_correlated_features.py` & `feature_engine-1.8.0/tests/test_selection/test_drop_correlated_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_drop_duplicate_features.py` & `feature_engine-1.8.0/tests/test_selection/test_drop_duplicate_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_drop_features.py` & `feature_engine-1.8.0/tests/test_selection/test_drop_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_drop_high_psi_features.py` & `feature_engine-1.8.0/tests/test_selection/test_drop_high_psi_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_information_value.py` & `feature_engine-1.8.0/tests/test_selection/test_information_value.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_probe_feature_selection.py` & `feature_engine-1.8.0/tests/test_selection/test_probe_feature_selection.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_recursive_feature_addition.py` & `feature_engine-1.8.0/tests/test_selection/test_recursive_feature_addition.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_recursive_feature_elimination.py` & `feature_engine-1.8.0/tests/test_selection/test_recursive_feature_elimination.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_recursive_feature_selectors.py` & `feature_engine-1.8.0/tests/test_selection/test_recursive_feature_selectors.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_shuffle_features.py` & `feature_engine-1.8.0/tests/test_selection/test_shuffle_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_single_feature_performance.py` & `feature_engine-1.8.0/tests/test_selection/test_single_feature_performance.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_smart_correlation_selection.py` & `feature_engine-1.8.0/tests/test_selection/test_smart_correlation_selection.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_selection/test_target_mean_selection.py` & `feature_engine-1.8.0/tests/test_selection/test_target_mean_selection.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_time_series/test_forecasting/conftest.py` & `feature_engine-1.8.0/tests/test_time_series/test_forecasting/conftest.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_time_series/test_forecasting/test_check_estimator_forecasting.py` & `feature_engine-1.8.0/tests/test_time_series/test_forecasting/test_check_estimator_forecasting.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_time_series/test_forecasting/test_expanding_window_features.py` & `feature_engine-1.8.0/tests/test_time_series/test_forecasting/test_expanding_window_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_time_series/test_forecasting/test_lag_features.py` & `feature_engine-1.8.0/tests/test_time_series/test_forecasting/test_lag_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_time_series/test_forecasting/test_window_features.py` & `feature_engine-1.8.0/tests/test_time_series/test_forecasting/test_window_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_transformation/test_arcsin_transformer.py` & `feature_engine-1.8.0/tests/test_transformation/test_arcsin_transformer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_transformation/test_boxcox_transformer.py` & `feature_engine-1.8.0/tests/test_transformation/test_boxcox_transformer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_transformation/test_check_estimator_transformers.py` & `feature_engine-1.8.0/tests/test_transformation/test_check_estimator_transformers.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_transformation/test_log_transformer.py` & `feature_engine-1.8.0/tests/test_transformation/test_log_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,28 @@
+import numpy as np
 import pandas as pd
 import pytest
 from sklearn.exceptions import NotFittedError
 
 from feature_engine.transformation import LogTransformer
 
 
+def test_transforming_int_vars():
+    df = pd.DataFrame(
+        {
+            "var1": [1, 2, 3],
+            "var2": [4, 5, 3],
+        }
+    )
+    dft = np.log(df)
+    transformer = LogTransformer(base="e", variables=None)
+    X = transformer.fit_transform(df)
+    pd.testing.assert_frame_equal(X, dft)
+
+
 def test_log_base_e_plus_automatically_find_variables(df_vartypes):
     # test case 1: log base e, automatically select variables
     transformer = LogTransformer(base="e", variables=None)
     X = transformer.fit_transform(df_vartypes)
 
     # expected output
     transf_df = df_vartypes.copy()
```

### Comparing `feature_engine-1.7.0/tests/test_transformation/test_logcp_transformer.py` & `feature_engine-1.8.0/tests/test_transformation/test_logcp_transformer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_transformation/test_power_transformer.py` & `feature_engine-1.8.0/tests/test_transformation/test_power_transformer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_transformation/test_reciprocal_transformer.py` & `feature_engine-1.8.0/tests/test_transformation/test_reciprocal_transformer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_transformation/test_yeojohnson_transformer.py` & `feature_engine-1.8.0/tests/test_transformation/test_yeojohnson_transformer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_variable_handling/conftest.py` & `feature_engine-1.8.0/tests/test_variable_handling/conftest.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_variable_handling/test_check_variables.py` & `feature_engine-1.8.0/tests/test_variable_handling/test_check_variables.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_variable_handling/test_find_variables.py` & `feature_engine-1.8.0/tests/test_variable_handling/test_find_variables.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_variable_handling/test_remove_variables.py` & `feature_engine-1.8.0/tests/test_variable_handling/test_remove_variables.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_wrappers/test_check_estimator_wrappers.py` & `feature_engine-1.8.0/tests/test_wrappers/test_check_estimator_wrappers.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.7.0/tests/test_wrappers/test_sklearn_wrapper.py` & `feature_engine-1.8.0/tests/test_wrappers/test_sklearn_wrapper.py`

 * *Files identical despite different names*

