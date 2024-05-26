# Comparing `tmp/skpro-2.3.0.tar.gz` & `tmp/skpro-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skpro-2.3.0.tar", last modified: Thu May 16 22:42:03 2024, max compression
+gzip compressed data, was "skpro-2.3.1.tar", last modified: Sat May 25 22:49:07 2024, max compression
```

## Comparing `skpro-2.3.0.tar` & `skpro-2.3.1.tar`

### file list

```diff
@@ -1,284 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.415758 skpro-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-16 22:41:53.000000 skpro-2.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-16 22:41:53.000000 skpro-2.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16220 2024-05-16 22:42:03.415758 skpro-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-16 22:41:53.000000 skpro-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.383757 skpro-2.3.0/build_tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-16 22:41:53.000000 skpro-2.3.0/build_tools/changelog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.379757 skpro-2.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.383757 skpro-2.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-05-16 22:41:53.000000 skpro-2.3.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.383757 skpro-2.3.0/extension_templates/
--rw-r--r--   0 runner    (1001) docker     (127)    15567 2024-05-16 22:41:53.000000 skpro-2.3.0/extension_templates/distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14948 2024-05-16 22:41:53.000000 skpro-2.3.0/extension_templates/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    14309 2024-05-16 22:41:53.000000 skpro-2.3.0/extension_templates/survival.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-16 22:41:53.000000 skpro-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-16 22:42:03.419757 skpro-2.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.383757 skpro-2.3.0/skpro/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.387757 skpro-2.3.0/skpro/base/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    22066 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/base/old_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.387757 skpro-2.3.0/skpro/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/benchmarking/evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.387757 skpro-2.3.0/skpro/benchmarking/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/benchmarking/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/benchmarking/tests/test_evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.387757 skpro-2.3.0/skpro/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.387757 skpro-2.3.0/skpro/datatypes/_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_adapter/polars.py
--rw-r--r--   0 runner    (1001) docker     (127)    20992 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11559 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.387757 skpro-2.3.0/skpro/datatypes/_convert_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_convert_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_convert_utils/_coerce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_convert_utils/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.391757 skpro-2.3.0/skpro/datatypes/_proba/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_proba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_proba/_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_proba/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_proba/_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_proba/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.391757 skpro-2.3.0/skpro/datatypes/_table/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_table/_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_table/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_table/_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_table/_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.391757 skpro-2.3.0/skpro/datatypes/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/tests/test_convert_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/tests/test_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.391757 skpro-2.3.0/skpro/distributions/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/distributions/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/distributions/adapters/scipy/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/adapters/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/adapters/scipy/_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/adapters/scipy/_empirical.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/distributions/adapters/scipy/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/adapters/scipy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/adapters/scipy/tests/test_scipy_adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/distributions/adapters/statsmodels/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/adapters/statsmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/adapters/statsmodels/_empirical.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/distributions/base/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68328 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/base/_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/chi_squared.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)    21324 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/empirical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/fisk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/laplace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/logistic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/lognormal.py
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/poisson.py
--rw-r--r--   0 runner    (1001) docker     (127)    25929 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/qpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/qpd_empirical.py
--rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/t.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/distributions/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/tests/test_all_distrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/tests/test_base_default_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/tests/test_base_scalar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/tests/test_proba_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/tests/test_qpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/weibull.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16917 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/_coerce.py
--rw-r--r--   0 runner    (1001) docker     (127)    22237 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/metrics/survival/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/survival/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/survival/_c_harrell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/survival/_spll.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/metrics/survival/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/survival/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/survival/tests/test_c_harrell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/metrics/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/tests/test_distr_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/tests/test_probabilistic_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/model_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/model_selection/_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/registry/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12805 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/registry/_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/registry/_scitype.py
--rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/registry/_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/registry/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/registry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/registry/tests/test_scitype.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/registry/tests/test_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/regression/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/regression/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/regression/adapters/ngboost/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/adapters/ngboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/adapters/ngboost/_ngboost_proba.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/regression/adapters/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/adapters/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/adapters/sklearn/_sklearn_proba.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/regression/base/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30706 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/base/_delegate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/regression/base/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/base/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/base/adapters/_sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/regression/baselines/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/baselines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/baselines/density.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/regression/compose/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/compose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21530 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/compose/_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    20226 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/cyclic_boosting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/density.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/regression/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/ensemble/_bagging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/ensemble/_ngboost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/regression/gp/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/gp/_sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/regression/linear/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/linear/_glm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/linear/_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/linear/_sklearn_poisson.py
--rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/mapie.py
--rw-r--r--   0 runner    (1001) docker     (127)    13604 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/multiquantile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/regression/parametric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/parametric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/parametric/estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/parametric/parametric.py
--rw-r--r--   0 runner    (1001) docker     (127)    14702 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/residual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/regression/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/tests/test_all_regressors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/tests/test_cyclic_boosting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/regression/vendors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/vendors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/vendors/pymc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/survival/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/survival/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/adapters/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/adapters/lifelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/adapters/sksurv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/survival/additive/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/additive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/additive/_aalen_lifelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/survival/aft/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/aft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/aft/_aft_lifelines_fisk.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/aft/_aft_lifelines_lognormal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/aft/_aft_lifelines_weibull.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.407757 skpro-2.3.0/skpro/survival/compose/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/compose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/compose/_reduce_cond_unc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/compose/_reduce_uncensored.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.407757 skpro-2.3.0/skpro/survival/coxph/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/coxph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/coxph/_coxnet_sksurv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/coxph/_coxph_lifelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/coxph/_coxph_sksurv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/coxph/_coxph_statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.407757 skpro-2.3.0/skpro/survival/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19654 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/ensemble/_grad_boost_sksurv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/ensemble/_ngboost_surv.py
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/ensemble/_survforest_sksurv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.407757 skpro-2.3.0/skpro/survival/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/tree/_tree_sksurv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.407757 skpro-2.3.0/skpro/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/_config_test_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.407757 skpro-2.3.0/skpro/tests/scenarios/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/scenarios/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/scenarios/scenarios_getter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/scenarios/scenarios_regressor_proba.py
--rw-r--r--   0 runner    (1001) docker     (127)    16275 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/test_all_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/test_baselines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/test_class_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/test_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/test_vendors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/tests/test_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/utils/_maint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/_maint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/_maint/_show_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/utils/_maint/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/_maint/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/_maint/tests/test_show_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/utils/deep_equals/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/deep_equals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/deep_equals/_deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/estimator_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/git_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/index.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/random_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/utils/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14906 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/validation/_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/cross_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/workflow/manager/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/manager/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/manager/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.415758 skpro-2.3.0/skpro/workflow/table/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/table/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.415758 skpro-2.3.0/skpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16220 2024-05-16 22:42:03.000000 skpro-2.3.0/skpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-05-16 22:42:03.000000 skpro-2.3.0/skpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:42:03.000000 skpro-2.3.0/skpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-16 22:42:03.000000 skpro-2.3.0/skpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 22:42:03.000000 skpro-2.3.0/skpro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:42:00.000000 skpro-2.3.0/skpro.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.467069 skpro-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-25 22:49:00.000000 skpro-2.3.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-25 22:49:00.000000 skpro-2.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15936 2024-05-25 22:49:07.467069 skpro-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-25 22:49:00.000000 skpro-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.435069 skpro-2.3.1/build_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-25 22:49:00.000000 skpro-2.3.1/build_tools/changelog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.427069 skpro-2.3.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.435069 skpro-2.3.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-05-25 22:49:00.000000 skpro-2.3.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.435069 skpro-2.3.1/extension_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    15785 2024-05-25 22:49:00.000000 skpro-2.3.1/extension_templates/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14948 2024-05-25 22:49:00.000000 skpro-2.3.1/extension_templates/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14309 2024-05-25 22:49:00.000000 skpro-2.3.1/extension_templates/survival.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-25 22:49:00.000000 skpro-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-25 22:49:07.467069 skpro-2.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.435069 skpro-2.3.1/skpro/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.435069 skpro-2.3.1/skpro/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/base/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.435069 skpro-2.3.1/skpro/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/benchmarking/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.435069 skpro-2.3.1/skpro/benchmarking/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/benchmarking/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/benchmarking/tests/test_evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.439069 skpro-2.3.1/skpro/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.439069 skpro-2.3.1/skpro/datatypes/_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_adapter/polars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11559 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.439069 skpro-2.3.1/skpro/datatypes/_convert_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_convert_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_convert_utils/_coerce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_convert_utils/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.439069 skpro-2.3.1/skpro/datatypes/_proba/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_proba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_proba/_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_proba/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_proba/_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_proba/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.439069 skpro-2.3.1/skpro/datatypes/_table/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_table/_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_table/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_table/_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/_table/_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.439069 skpro-2.3.1/skpro/datatypes/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/tests/test_convert_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/datatypes/tests/test_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.443069 skpro-2.3.1/skpro/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.443069 skpro-2.3.1/skpro/distributions/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.443069 skpro-2.3.1/skpro/distributions/adapters/scipy/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/adapters/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/adapters/scipy/_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/adapters/scipy/_empirical.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.443069 skpro-2.3.1/skpro/distributions/adapters/scipy/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/adapters/scipy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/adapters/scipy/tests/test_scipy_adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.443069 skpro-2.3.1/skpro/distributions/adapters/statsmodels/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/adapters/statsmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/adapters/statsmodels/_empirical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/alpha.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.443069 skpro-2.3.1/skpro/distributions/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68983 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7761 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/base/_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/chi_squared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.443069 skpro-2.3.1/skpro/distributions/compose/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/compose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/compose/_iid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21639 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/fisk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/laplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/logistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25929 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/qpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/qpd_empirical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/t.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.443069 skpro-2.3.1/skpro/distributions/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/tests/test_all_distrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/tests/test_base_default_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/tests/test_base_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/tests/test_empirical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/tests/test_proba_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/tests/test_qpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/distributions/weibull.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.447069 skpro-2.3.1/skpro/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16917 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/metrics/_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/metrics/_coerce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22237 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/metrics/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.447069 skpro-2.3.1/skpro/metrics/survival/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/metrics/survival/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/metrics/survival/_c_harrell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/metrics/survival/_spll.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.447069 skpro-2.3.1/skpro/metrics/survival/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/metrics/survival/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/metrics/survival/tests/test_c_harrell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.447069 skpro-2.3.1/skpro/metrics/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/metrics/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/metrics/tests/test_distr_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/metrics/tests/test_probabilistic_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.447069 skpro-2.3.1/skpro/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30761 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/model_selection/_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.447069 skpro-2.3.1/skpro/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/registry/_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/registry/_scitype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/registry/_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.447069 skpro-2.3.1/skpro/registry/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/registry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/registry/tests/test_scitype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/registry/tests/test_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.451069 skpro-2.3.1/skpro/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.451069 skpro-2.3.1/skpro/regression/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.451069 skpro-2.3.1/skpro/regression/adapters/ngboost/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/adapters/ngboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/adapters/ngboost/_ngboost_proba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.451069 skpro-2.3.1/skpro/regression/adapters/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/adapters/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/adapters/sklearn/_sklearn_proba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.451069 skpro-2.3.1/skpro/regression/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30706 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/base/_delegate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.451069 skpro-2.3.1/skpro/regression/base/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/base/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/base/adapters/_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.451069 skpro-2.3.1/skpro/regression/compose/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/compose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21530 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/compose/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20226 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/cyclic_boosting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12319 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/enbpi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.451069 skpro-2.3.1/skpro/regression/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/ensemble/_bagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/ensemble/_ngboost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.451069 skpro-2.3.1/skpro/regression/gp/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/gp/_sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.451069 skpro-2.3.1/skpro/regression/linear/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/linear/_glm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/linear/_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/linear/_sklearn_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/mapie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13604 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/multiquantile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.455069 skpro-2.3.1/skpro/regression/parametric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/parametric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/parametric/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14702 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/residual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.455069 skpro-2.3.1/skpro/regression/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/tests/test_all_regressors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/regression/tests/test_cyclic_boosting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.455069 skpro-2.3.1/skpro/survival/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.455069 skpro-2.3.1/skpro/survival/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/adapters/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/adapters/lifelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/adapters/sksurv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.455069 skpro-2.3.1/skpro/survival/additive/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/additive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/additive/_aalen_lifelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.455069 skpro-2.3.1/skpro/survival/aft/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/aft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/aft/_aft_lifelines_fisk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/aft/_aft_lifelines_lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/aft/_aft_lifelines_weibull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.455069 skpro-2.3.1/skpro/survival/compose/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/compose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/compose/_reduce_cond_unc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/compose/_reduce_uncensored.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.455069 skpro-2.3.1/skpro/survival/coxph/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/coxph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/coxph/_coxnet_sksurv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/coxph/_coxph_lifelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/coxph/_coxph_sksurv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/coxph/_coxph_statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.459069 skpro-2.3.1/skpro/survival/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19654 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/ensemble/_grad_boost_sksurv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/ensemble/_ngboost_surv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/ensemble/_survforest_sksurv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.459069 skpro-2.3.1/skpro/survival/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/survival/tree/_tree_sksurv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.459069 skpro-2.3.1/skpro/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/tests/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/tests/_config_test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.459069 skpro-2.3.1/skpro/tests/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/tests/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/tests/scenarios/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/tests/scenarios/scenarios_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/tests/scenarios/scenarios_regressor_proba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16275 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/tests/test_all_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/tests/test_class_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/tests/test_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/tests/test_switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.459069 skpro-2.3.1/skpro/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/tests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/tests/tests/test_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.463069 skpro-2.3.1/skpro/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.463069 skpro-2.3.1/skpro/utils/_maint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/_maint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/_maint/_show_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.463069 skpro-2.3.1/skpro/utils/_maint/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/_maint/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/_maint/tests/test_show_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.463069 skpro-2.3.1/skpro/utils/deep_equals/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/deep_equals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/deep_equals/_deep_equals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/estimator_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/git_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/random_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.463069 skpro-2.3.1/skpro/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.463069 skpro-2.3.1/skpro/utils/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14906 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/utils/validation/_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.463069 skpro-2.3.1/skpro/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/workflow/cross_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.463069 skpro-2.3.1/skpro/workflow/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/workflow/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/workflow/manager/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/workflow/manager/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.463069 skpro-2.3.1/skpro/workflow/table/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/workflow/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/workflow/table/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-25 22:49:00.000000 skpro-2.3.1/skpro/workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:07.463069 skpro-2.3.1/skpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15936 2024-05-25 22:49:07.000000 skpro-2.3.1/skpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-05-25 22:49:07.000000 skpro-2.3.1/skpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 22:49:07.000000 skpro-2.3.1/skpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-25 22:49:07.000000 skpro-2.3.1/skpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-25 22:49:07.000000 skpro-2.3.1/skpro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 22:49:04.000000 skpro-2.3.1/skpro.egg-info/zip-safe
```

### Comparing `skpro-2.3.0/LICENSE.txt` & `skpro-2.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/PKG-INFO` & `skpro-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skpro
-Version: 2.3.0
+Version: 2.3.1
 Summary: A unified framework for probability distributions and probabilistic supervised regression
 Author: Franz Király, Frithjof Gressmann, Vitaly Davydov
 Author-email: skpro developers <sktime.toolbox@gmail.com>
 Maintainer: Franz Király, Frithjof Gressmann
 Maintainer-email: skpro developers <sktime.toolbox@gmail.com>
 Project-URL: Homepage, https://github.com/sktime/skpro
 Project-URL: Repository, https://github.com/sktime/skpro
@@ -31,16 +31,16 @@
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 Requires-Dist: numpy<1.27,>=1.21.0
 Requires-Dist: pandas<2.3.0,>=1.1.0
 Requires-Dist: packaging
-Requires-Dist: scikit-base<0.8.0,>=0.6.1
-Requires-Dist: scikit-learn<1.5.0,>=0.24.0
+Requires-Dist: scikit-base<0.9.0,>=0.6.1
+Requires-Dist: scikit-learn<1.6.0,>=0.24.0
 Requires-Dist: scipy<2.0.0,>=1.2.0
 Provides-Extra: all-extras
 Requires-Dist: attrs; extra == "all-extras"
 Requires-Dist: cyclic-boosting>=1.4.0; python_version < "3.12" and extra == "all-extras"
 Requires-Dist: distfit; extra == "all-extras"
 Requires-Dist: lifelines<0.29.0; extra == "all-extras"
 Requires-Dist: mapie; extra == "all-extras"
@@ -67,23 +67,23 @@
 Provides-Extra: docs
 Requires-Dist: jupyter; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: nbsphinx>=0.8.6; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Requires-Dist: sphinx!=7.2.0,<8.0.0; extra == "docs"
-Requires-Dist: sphinx-design<0.6.0; extra == "docs"
+Requires-Dist: sphinx-design<0.7.0; extra == "docs"
 Requires-Dist: sphinx-issues<5.0.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.17.0; extra == "docs"
 Requires-Dist: sphinx-panels; extra == "docs"
 Requires-Dist: tabulate; extra == "docs"
 
 <a href="https://skpro.readthedocs.io/en/latest"><img src="https://github.com/sktime/skpro/blob/main/docs/source/images/skpro-banner.png" width="500" align="right" /></a>
 
-:rocket: **Version 2.3.0 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
+:rocket: **Version 2.3.1 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
 
 `skpro` is a library for supervised probabilistic prediction in python.
 It provides `scikit-learn`-like, `scikit-base` compatible interfaces to:
 
 * tabular **supervised regressors for probabilistic prediction** - interval, quantile and distribution predictions
 * tabular **probabilistic time-to-event and survival prediction** - instance-individual survival distributions
 * **metrics to evaluate probabilistic predictions**, e.g., pinball loss, empirical coverage, CRPS, survival losses
@@ -94,15 +94,15 @@
 | Overview | |
 |---|---|
 | **Open Source** |  [![BSD 3-clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/sktime/sktime/blob/main/LICENSE) |
 | **Tutorials** | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sktime/skpro/main?filepath=examples) [![!youtube](https://img.shields.io/static/v1?logo=youtube&label=YouTube&message=tutorials&color=red)](https://www.youtube.com/playlist?list=PLKs3UgGjlWHqNzu0LEOeLKvnjvvest2d0) |
 | **Community** | [![!discord](https://img.shields.io/static/v1?logo=discord&label=discord&message=chat&color=lightgreen)](https://discord.com/invite/54ACzaFsn7) [![!slack](https://img.shields.io/static/v1?logo=linkedin&label=LinkedIn&message=news&color=lightblue)](https://www.linkedin.com/company/scikit-time/) |
 | **CI/CD** | [![github-actions](https://img.shields.io/github/actions/workflow/status/sktime/sktime/wheels.yml?logo=github)](https://github.com/sktime/skpro/actions/workflows/wheels.yml) [![!codecov](https://img.shields.io/codecov/c/github/sktime/skpro?label=codecov&logo=codecov)](https://codecov.io/gh/sktime/skpro) [![readthedocs](https://img.shields.io/readthedocs/skpro?logo=readthedocs)](https://skpro.readthedocs.io/en/latest/) [![platform](https://img.shields.io/conda/pn/conda-forge/skpro)](https://github.com/sktime/skpro) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/skpro?color=orange)](https://pypi.org/project/skpro/) [![!conda](https://img.shields.io/conda/vn/conda-forge/skpro)](https://anaconda.org/conda-forge/skpro) [![!python-versions](https://img.shields.io/pypi/pyversions/skpro)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
-| **Downloads** | [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skpro) |
+| **Downloads** | ![PyPI - Downloads](https://img.shields.io/pypi/dw/skpro) ![PyPI - Downloads](https://img.shields.io/pypi/dm/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skpro) |
 | **Citation** | [![DOI](https://zenodo.org/badge/103107372.svg)](https://zenodo.org/doi/10.5281/zenodo.11002671) |
 
 ## :books: Documentation
 
 | Documentation              |                                                                |
 | -------------------------- | -------------------------------------------------------------- |
 | :star: **[Tutorials]**        | New to skpro? Here's everything you need to know!              |
@@ -162,15 +162,15 @@
 [cyclic-boosting]:  https://cyclic-boosting.readthedocs.io/en/latest/
 
 ``skpro`` curates libraries of components of the following types:
 
 | Module | Status | Links |
 |---|---|---|
 | **[Probabilistic tabular regression]** | maturing | [Tutorial](https://github.com/sktime/skpro/blob/main/examples/01_skpro_intro.ipynb) · [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/regression.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/regression.py) |
-| **[Time-to-event (survival) prediction]** | experimental | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/survival.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/survival.py) |
+| **[Time-to-event (survival) prediction]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/survival.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/survival.py) |
 | **[Performance metrics]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/metrics.html) |
 | **[Probability distributions]** | maturing | [Tutorial](https://github.com/sktime/skpro/blob/main/examples/03_skpro_distributions.ipynb) · [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/distributions.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/distributions.py) |
 
 [Probabilistic tabular regression]: https://github.com/sktime/skpro/tree/main/skpro/regression
 [Time-to-event (survival) prediction]: https://github.com/sktime/skpro/tree/main/skpro/survival
 [Performance metrics]: https://github.com/sktime/skpro/tree/main/skpro/metrics
 [Probability distributions]: https://github.com/sktime/skpro/tree/main/skpro/distributions
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skpro Version: 2.3.0 Summary: A unified framework
+Metadata-Version: 2.1 Name: skpro Version: 2.3.1 Summary: A unified framework
 for probability distributions and probabilistic supervised regression Author:
 Franz KirÃ¡ly, Frithjof Gressmann, Vitaly Davydov Author-email: skpro
 developers
 gmail.com> Maintainer: Franz KirÃ¡ly, Frithjof Gressmann Maintainer-email:
 skpro developers
 gmail.com> Project-URL: Homepage, https://github.com/sktime/skpro Project-URL:
 Repository, https://github.com/sktime/skpro Project-URL: Documentation, https:/
@@ -18,15 +18,15 @@
 Classifier: Operating System :: MacOS Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Python: <3.13,>=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.txt License-File: AUTHORS.rst Requires-Dist: numpy<1.27,>=1.21.0
 Requires-Dist: pandas<2.3.0,>=1.1.0 Requires-Dist: packaging Requires-Dist:
-scikit-base<0.8.0,>=0.6.1 Requires-Dist: scikit-learn<1.5.0,>=0.24.0 Requires-
+scikit-base<0.9.0,>=0.6.1 Requires-Dist: scikit-learn<1.6.0,>=0.24.0 Requires-
 Dist: scipy<2.0.0,>=1.2.0 Provides-Extra: all-extras Requires-Dist: attrs;
 extra == "all-extras" Requires-Dist: cyclic-boosting>=1.4.0; python_version <
 "3.12" and extra == "all-extras" Requires-Dist: distfit; extra == "all-extras"
 Requires-Dist: lifelines<0.29.0; extra == "all-extras" Requires-Dist: mapie;
 extra == "all-extras" Requires-Dist: matplotlib>=3.3.2; extra == "all-extras"
 Requires-Dist: ngboost<0.6.0; extra == "all-extras" Requires-Dist:
 polars<0.21.0; extra == "all-extras" Requires-Dist: pyarrow<14.0.0;
@@ -39,19 +39,19 @@
 pytest-cov; extra == "dev" Requires-Dist: pytest-randomly; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev" Requires-Dist: pytest-xdist;
 extra == "dev" Requires-Dist: wheel; extra == "dev" Provides-Extra: binder
 Requires-Dist: jupyter; extra == "binder" Provides-Extra: docs Requires-Dist:
 jupyter; extra == "docs" Requires-Dist: myst-parser; extra == "docs" Requires-
 Dist: nbsphinx>=0.8.6; extra == "docs" Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs" Requires-Dist:
-sphinx!=7.2.0,<8.0.0; extra == "docs" Requires-Dist: sphinx-design<0.6.0; extra
+sphinx!=7.2.0,<8.0.0; extra == "docs" Requires-Dist: sphinx-design<0.7.0; extra
 == "docs" Requires-Dist: sphinx-issues<5.0.0; extra == "docs" Requires-Dist:
 sphinx-gallery<0.17.0; extra == "docs" Requires-Dist: sphinx-panels; extra ==
 "docs" Requires-Dist: tabulate; extra == "docs" _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_k_t_i_m_e_/
-_s_k_p_r_o_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_p_r_o_-_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.3.0
+_s_k_p_r_o_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_p_r_o_-_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.3.1
 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/
 latest/changelog.html). `skpro` is a library for supervised probabilistic
 prediction in python. It provides `scikit-learn`-like, `scikit-base` compatible
 interfaces to: * tabular **supervised regressors for probabilistic prediction**
 - interval, quantile and distribution predictions * tabular **probabilistic
 time-to-event and survival prediction** - instance-individual survival
 distributions * **metrics to evaluate probabilistic predictions**, e.g.,
@@ -80,22 +80,17 @@
 (https://skpro.readthedocs.io/en/latest/) [![platform](https://img.shields.io/
 conda/pn/conda-forge/skpro)](https://github.com/sktime/skpro) | | **Code** | [!
 [!pypi](https://img.shields.io/pypi/v/skpro?color=orange)](https://pypi.org/
 project/skpro/) [![!conda](https://img.shields.io/conda/vn/conda-forge/skpro)]
 (https://anaconda.org/conda-forge/skpro) [![!python-versions](https://
 img.shields.io/pypi/pyversions/skpro)](https://www.python.org/) [![!black]
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
-github.com/psf/black) | | **Downloads** | [![Downloads](https://
-static.pepy.tech/personalized-badge/
-skpro?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20
-(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
-static.pepy.tech/personalized-badge/
-skpro?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20
-(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
-static.pepy.tech/personalized-badge/
+github.com/psf/black) | | **Downloads** | ![PyPI - Downloads](https://
+img.shields.io/pypi/dw/skpro) ![PyPI - Downloads](https://img.shields.io/pypi/
+dm/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/
 skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20
 (pypi))](https://pepy.tech/project/skpro) | | **Citation** | [![DOI](https://
 zenodo.org/badge/103107372.svg)](https://zenodo.org/doi/10.5281/
 zenodo.11002671) | ## :books: Documentation | Documentation | | | -------------
 ------------- | -------------------------------------------------------------
 - | | :star: **[Tutorials]** | New to skpro? Here's everything you need to
 know! | | :clipboard: **[Binder Notebooks]** | Example notebooks to play with
@@ -140,15 +135,15 @@
 boosting.readthedocs.io/en/latest/ ``skpro`` curates libraries of components of
 the following types: | Module | Status | Links | |---|---|---| | **
 [Probabilistic tabular regression]** | maturing | [Tutorial](https://
 github.com/sktime/skpro/blob/main/examples/01_skpro_intro.ipynb) Â· [API
 Reference](https://skpro.readthedocs.io/en/latest/api_reference/
 regression.html) Â· [Extension Template](https://github.com/sktime/skpro/blob/
 main/extension_templates/regression.py) | | **[Time-to-event (survival)
-prediction]** | experimental | [API Reference](https://skpro.readthedocs.io/en/
+prediction]** | maturing | [API Reference](https://skpro.readthedocs.io/en/
 latest/api_reference/survival.html) Â· [Extension Template](https://github.com/
 sktime/skpro/blob/main/extension_templates/survival.py) | | **[Performance
 metrics]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/
 api_reference/metrics.html) | | **[Probability distributions]** | maturing |
 [Tutorial](https://github.com/sktime/skpro/blob/main/examples/
 03_skpro_distributions.ipynb) Â· [API Reference](https://skpro.readthedocs.io/
 en/latest/api_reference/distributions.html) Â· [Extension Template](https://
```

### Comparing `skpro-2.3.0/README.md` & `skpro-2.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <a href="https://skpro.readthedocs.io/en/latest"><img src="https://github.com/sktime/skpro/blob/main/docs/source/images/skpro-banner.png" width="500" align="right" /></a>
 
-:rocket: **Version 2.3.0 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
+:rocket: **Version 2.3.1 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
 
 `skpro` is a library for supervised probabilistic prediction in python.
 It provides `scikit-learn`-like, `scikit-base` compatible interfaces to:
 
 * tabular **supervised regressors for probabilistic prediction** - interval, quantile and distribution predictions
 * tabular **probabilistic time-to-event and survival prediction** - instance-individual survival distributions
 * **metrics to evaluate probabilistic predictions**, e.g., pinball loss, empirical coverage, CRPS, survival losses
@@ -15,15 +15,15 @@
 | Overview | |
 |---|---|
 | **Open Source** |  [![BSD 3-clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/sktime/sktime/blob/main/LICENSE) |
 | **Tutorials** | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sktime/skpro/main?filepath=examples) [![!youtube](https://img.shields.io/static/v1?logo=youtube&label=YouTube&message=tutorials&color=red)](https://www.youtube.com/playlist?list=PLKs3UgGjlWHqNzu0LEOeLKvnjvvest2d0) |
 | **Community** | [![!discord](https://img.shields.io/static/v1?logo=discord&label=discord&message=chat&color=lightgreen)](https://discord.com/invite/54ACzaFsn7) [![!slack](https://img.shields.io/static/v1?logo=linkedin&label=LinkedIn&message=news&color=lightblue)](https://www.linkedin.com/company/scikit-time/) |
 | **CI/CD** | [![github-actions](https://img.shields.io/github/actions/workflow/status/sktime/sktime/wheels.yml?logo=github)](https://github.com/sktime/skpro/actions/workflows/wheels.yml) [![!codecov](https://img.shields.io/codecov/c/github/sktime/skpro?label=codecov&logo=codecov)](https://codecov.io/gh/sktime/skpro) [![readthedocs](https://img.shields.io/readthedocs/skpro?logo=readthedocs)](https://skpro.readthedocs.io/en/latest/) [![platform](https://img.shields.io/conda/pn/conda-forge/skpro)](https://github.com/sktime/skpro) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/skpro?color=orange)](https://pypi.org/project/skpro/) [![!conda](https://img.shields.io/conda/vn/conda-forge/skpro)](https://anaconda.org/conda-forge/skpro) [![!python-versions](https://img.shields.io/pypi/pyversions/skpro)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
-| **Downloads** | [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skpro) |
+| **Downloads** | ![PyPI - Downloads](https://img.shields.io/pypi/dw/skpro) ![PyPI - Downloads](https://img.shields.io/pypi/dm/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skpro) |
 | **Citation** | [![DOI](https://zenodo.org/badge/103107372.svg)](https://zenodo.org/doi/10.5281/zenodo.11002671) |
 
 ## :books: Documentation
 
 | Documentation              |                                                                |
 | -------------------------- | -------------------------------------------------------------- |
 | :star: **[Tutorials]**        | New to skpro? Here's everything you need to know!              |
@@ -83,15 +83,15 @@
 [cyclic-boosting]:  https://cyclic-boosting.readthedocs.io/en/latest/
 
 ``skpro`` curates libraries of components of the following types:
 
 | Module | Status | Links |
 |---|---|---|
 | **[Probabilistic tabular regression]** | maturing | [Tutorial](https://github.com/sktime/skpro/blob/main/examples/01_skpro_intro.ipynb) · [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/regression.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/regression.py) |
-| **[Time-to-event (survival) prediction]** | experimental | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/survival.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/survival.py) |
+| **[Time-to-event (survival) prediction]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/survival.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/survival.py) |
 | **[Performance metrics]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/metrics.html) |
 | **[Probability distributions]** | maturing | [Tutorial](https://github.com/sktime/skpro/blob/main/examples/03_skpro_distributions.ipynb) · [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/distributions.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/distributions.py) |
 
 [Probabilistic tabular regression]: https://github.com/sktime/skpro/tree/main/skpro/regression
 [Time-to-event (survival) prediction]: https://github.com/sktime/skpro/tree/main/skpro/survival
 [Performance metrics]: https://github.com/sktime/skpro/tree/main/skpro/metrics
 [Probability distributions]: https://github.com/sktime/skpro/tree/main/skpro/distributions
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_k_t_i_m_e_/_s_k_p_r_o_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_p_r_o_-
-_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.3.0 out now!** [Read the release notes here.]
+_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.3.1 out now!** [Read the release notes here.]
 (https://skpro.readthedocs.io/en/latest/changelog.html). `skpro` is a library
 for supervised probabilistic prediction in python. It provides `scikit-learn`-
 like, `scikit-base` compatible interfaces to: * tabular **supervised regressors
 for probabilistic prediction** - interval, quantile and distribution
 predictions * tabular **probabilistic time-to-event and survival prediction** -
 instance-individual survival distributions * **metrics to evaluate
 probabilistic predictions**, e.g., pinball loss, empirical coverage, CRPS,
@@ -32,22 +32,17 @@
 (https://skpro.readthedocs.io/en/latest/) [![platform](https://img.shields.io/
 conda/pn/conda-forge/skpro)](https://github.com/sktime/skpro) | | **Code** | [!
 [!pypi](https://img.shields.io/pypi/v/skpro?color=orange)](https://pypi.org/
 project/skpro/) [![!conda](https://img.shields.io/conda/vn/conda-forge/skpro)]
 (https://anaconda.org/conda-forge/skpro) [![!python-versions](https://
 img.shields.io/pypi/pyversions/skpro)](https://www.python.org/) [![!black]
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
-github.com/psf/black) | | **Downloads** | [![Downloads](https://
-static.pepy.tech/personalized-badge/
-skpro?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20
-(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
-static.pepy.tech/personalized-badge/
-skpro?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20
-(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
-static.pepy.tech/personalized-badge/
+github.com/psf/black) | | **Downloads** | ![PyPI - Downloads](https://
+img.shields.io/pypi/dw/skpro) ![PyPI - Downloads](https://img.shields.io/pypi/
+dm/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/
 skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20
 (pypi))](https://pepy.tech/project/skpro) | | **Citation** | [![DOI](https://
 zenodo.org/badge/103107372.svg)](https://zenodo.org/doi/10.5281/
 zenodo.11002671) | ## :books: Documentation | Documentation | | | -------------
 ------------- | -------------------------------------------------------------
 - | | :star: **[Tutorials]** | New to skpro? Here's everything you need to
 know! | | :clipboard: **[Binder Notebooks]** | Example notebooks to play with
@@ -92,15 +87,15 @@
 boosting.readthedocs.io/en/latest/ ``skpro`` curates libraries of components of
 the following types: | Module | Status | Links | |---|---|---| | **
 [Probabilistic tabular regression]** | maturing | [Tutorial](https://
 github.com/sktime/skpro/blob/main/examples/01_skpro_intro.ipynb) Â· [API
 Reference](https://skpro.readthedocs.io/en/latest/api_reference/
 regression.html) Â· [Extension Template](https://github.com/sktime/skpro/blob/
 main/extension_templates/regression.py) | | **[Time-to-event (survival)
-prediction]** | experimental | [API Reference](https://skpro.readthedocs.io/en/
+prediction]** | maturing | [API Reference](https://skpro.readthedocs.io/en/
 latest/api_reference/survival.html) Â· [Extension Template](https://github.com/
 sktime/skpro/blob/main/extension_templates/survival.py) | | **[Performance
 metrics]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/
 api_reference/metrics.html) | | **[Probability distributions]** | maturing |
 [Tutorial](https://github.com/sktime/skpro/blob/main/examples/
 03_skpro_distributions.ipynb) Â· [API Reference](https://skpro.readthedocs.io/
 en/latest/api_reference/distributions.html) Â· [Extension Template](https://
```

### Comparing `skpro-2.3.0/build_tools/changelog.py` & `skpro-2.3.1/build_tools/changelog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """RestructuredText changelog generator."""
 
 import os
 from collections import defaultdict
 from typing import Dict, List
 
-import httpx
-from dateutil import parser
-
 HEADERS = {
     "Accept": "application/vnd.github.v3+json",
 }
 
 if os.getenv("GITHUB_TOKEN") is not None:
     HEADERS["Authorization"] = f"token {os.getenv('GITHUB_TOKEN')}"
 
 OWNER = "sktime"
 REPO = "skpro"
 GITHUB_REPOS = "https://api.github.com/repos"
 
 
 def fetch_merged_pull_requests(page: int = 1) -> List[Dict]:  # noqa
     "Fetch a page of pull requests"
+    import httpx
+
     params = {
         "base": "main",
         "state": "closed",
         "page": page,
         "per_page": 50,
         "sort": "updated",
         "direction": "desc",
@@ -34,26 +33,29 @@
         headers=HEADERS,
         params=params,
     )
     return [pr for pr in r.json() if pr["merged_at"]]
 
 
 def fetch_latest_release():  # noqa
+    import httpx
+
     response = httpx.get(
         f"{GITHUB_REPOS}/{OWNER}/{REPO}/releases/latest", headers=HEADERS
     )
 
     if response.status_code == 200:
         return response.json()
     else:
         raise ValueError(response.text, response.status_code)
 
 
 def fetch_pull_requests_since_last_release() -> List[Dict]:  # noqa
     "Fetch pull requests and filter based on merged date"
+    from dateutil import parser
 
     release = fetch_latest_release()
     published_at = parser.parse(release["published_at"])
     print(  # noqa
         f"Latest release {release['tag_name']} was published at {published_at}"
     )
 
@@ -68,14 +70,16 @@
         is_exhausted = any(parser.parse(p["merged_at"]) < published_at for p in pulls)
         page += 1
     return all_pulls
 
 
 def github_compare_tags(tag_left: str, tag_right: str = "HEAD"):  # noqa
     "Compare commit between two tags"
+    import httpx
+
     response = httpx.get(
         f"{GITHUB_REPOS}/{OWNER}/{REPO}/compare/{tag_left}...{tag_right}"
     )
     if response.status_code == 200:
         return response.json()
     else:
         raise ValueError(response.text, response.status_code)
@@ -124,14 +128,16 @@
         f":user:`{pr['user']['login']}`",
     )
 
 
 def render_changelog(prs, assigned):  # noqa
     # sourcery skip: use-named-expression
     "Render changelog"
+    from dateutil import parser
+
     for title, _ in assigned.items():
         pr_group = [prs[i] for i in assigned[title]]
         if pr_group:
             print(f"\n{title}")  # noqa
             print("~" * len(title), end="\n\n")  # noqa
 
             for pr in sorted(pr_group, key=lambda x: parser.parse(x["merged_at"])):
```

### Comparing `skpro-2.3.0/docs/source/conf.py` & `skpro-2.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/extension_templates/distributions.py` & `skpro-2.3.1/extension_templates/distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,24 +296,30 @@
     # if not implemented, uses _ppf for sampling (inverse cdf on uniform)
     def sample(self, n_samples=None):
         """Sample from the distribution.
 
         Parameters
         ----------
         n_samples : int, optional, default = None
+            number of samples to draw from the distribution
 
         Returns
         -------
-        if `n_samples` is `None`:
-        returns a sample that contains a single sample from `self`,
-        in `pd.DataFrame` mtype format convention, with `index` and `columns` as `self`
-        if n_samples is `int`:
-        returns a `pd.DataFrame` that contains `n_samples` i.i.d. samples from `self`,
-        in `pd-multiindex` mtype format convention, with same `columns` as `self`,
-        and `MultiIndex` that is product of `RangeIndex(n_samples)` and `self.index`
+        pd.DataFrame
+            samples from the distribution
+
+            * if ``n_samples`` is ``None``:
+            returns a sample that contains a single sample from ``self``,
+            in ``pd.DataFrame`` mtype format convention, with ``index`` and ``columns``
+            as ``self``
+            * if n_samples is ``int``:
+            returns a ``pd.DataFrame`` that contains ``n_samples`` i.i.d.
+            samples from ``self``, in ``pd-multiindex`` mtype format convention,
+            with same ``columns`` as ``self``, and row ``MultiIndex`` that is product
+            of ``RangeIndex(n_samples)`` and ``self.index``
         """
         param1 = self._bc_params["param1"]  # returns broadcast params to x.shape
         param2 = self._bc_params["param2"]  # returns broadcast params to x.shape
 
         res = "do_sth_with(" + param1 + param2 + ")"  # replace this by internal logic
         return res
```

### Comparing `skpro-2.3.0/extension_templates/regression.py` & `skpro-2.3.1/extension_templates/regression.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/extension_templates/survival.py` & `skpro-2.3.1/extension_templates/survival.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/pyproject.toml` & `skpro-2.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "skpro"
-version = "2.3.0"
+version = "2.3.1"
 description = "A unified framework for probability distributions and probabilistic supervised regression"
 authors = [
     {name = "skpro developers", email = "sktime.toolbox@gmail.com"},
     {name = "Franz Király"},
     {name = "Frithjof Gressmann"},
     {name = "Vitaly Davydov"},
 ]
@@ -40,16 +40,16 @@
     "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">=3.8,<3.13"
 dependencies = [
     "numpy>=1.21.0,<1.27",
     "pandas>=1.1.0,<2.3.0",
     "packaging",
-    "scikit-base>=0.6.1,<0.8.0",
-    "scikit-learn>=0.24.0,<1.5.0",
+    "scikit-base>=0.6.1,<0.9.0",
+    "scikit-learn>=0.24.0,<1.6.0",
     "scipy<2.0.0,>=1.2.0",
 ]
 
 [project.optional-dependencies]
 all_extras = [
     "attrs",
     "cyclic-boosting>=1.4.0; python_version < '3.12'",
@@ -85,15 +85,15 @@
 docs = [
     "jupyter",
     "myst-parser",
     "nbsphinx>=0.8.6",
     "numpydoc",
     "pydata-sphinx-theme",
     "sphinx<8.0.0,!=7.2.0",
-    "sphinx-design<0.6.0",
+    "sphinx-design<0.7.0",
     "sphinx-issues<5.0.0",
     "sphinx-gallery<0.17.0",
     "sphinx-panels",
     "tabulate",
 ]
 
 [project.urls]
```

### Comparing `skpro-2.3.0/setup.cfg` & `skpro-2.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/base/_base.py` & `skpro-2.3.1/skpro/base/_base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/base/old_base.py` & `skpro-2.3.1/skpro/datatypes/_check.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,803 +1,543 @@
-"""LEGACY MODULE - TODO: remove or refactor."""
+# copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
+"""Machine type checkers for scitypes.
 
-import abc
-import functools
-import warnings
+Exports
+-------
+check_is_mtype(obj, mtype: str, scitype: str)
+    checks whether obj is mtype for scitype
+    returns boolean yes/no and metadata
+
+check_raise(obj, mtype: str, scitype:str)
+    checks whether obj is mtype for scitype
+    returns True if passes, otherwise raises error
+
+mtype(obj, as_scitype: str = None)
+    infer the mtype of obj, considering it as as_scitype
+"""
+
+__author__ = ["fkiraly"]
+
+__all__ = [
+    "check_is_mtype",
+    "check_raise",
+    "mtype",
+]
 
 import numpy as np
-from sklearn.base import BaseEstimator, clone
 
-from skpro.regression.density import DensityAdapter, KernelDensityAdapter
-from skpro.utils.utils import ensure_existence
+from skpro.datatypes._common import _metadata_requested, _ret
+from skpro.datatypes._proba import check_dict_Proba
+from skpro.datatypes._registry import AMBIGUOUS_MTYPES, SCITYPE_LIST, mtype_to_scitype
+from skpro.datatypes._table import check_dict_Table
 
+# pool convert_dict-s
+check_dict = dict()
+check_dict.update(check_dict_Table)
+check_dict.update(check_dict_Proba)
 
-def vectorvalued(f):
-    """Decorate a distribution function to disable automatic vectorization.
 
-    Parameters
-    ----------
-    f: The function to decorate
+def _check_scitype_valid(scitype: str = None):
+    """Check validity of scitype."""
+    valid_scitypes = list({x[1] for x in check_dict.keys()})
 
-    Returns
-    -------
-    Decorated function
-    """
-    f.already_vectorized = True
-    return f
+    if not isinstance(scitype, str):
+        raise TypeError(f"scitype should be a str but found {type(scitype)}")
 
+    if scitype is not None and scitype not in valid_scitypes:
+        raise TypeError(scitype + " is not a supported scitype")
 
-def _forward_meta(wrapper, f):
-    """Forward meta information from decorated method to decoration.
+
+def _coerce_list_of_str(obj, var_name="obj"):
+    """Check whether object is string or list of string.
 
     Parameters
     ----------
-    wrapper
-    f
+    obj - object to check
+    var_name: str, optional, default="obj" - name of input in error messages
 
     Returns
     -------
-    Method with meta information
+    list of str
+        equal to obj if was a list; equal to [obj] if obj was a str
+        note: if obj was a list, return is not a copy, but identical
+
+    Raises
+    ------
+    TypeError if obj is not a str or list of str
     """
-    wrapper.already_vectorized = getattr(f, "already_vectorized", False)
-    wrapper.non_existing = getattr(f, "not_existing", False)
-
-    return wrapper
-
-
-def _generalize(f):
-    """Generalize the signature to allow for the use with np.std() etc.
+    if isinstance(obj, str):
+        obj = [obj]
+    elif isinstance(obj, list):
+        if not np.all([isinstance(x, str) for x in obj]):
+            raise TypeError(f"{var_name} must be a string or list of strings")
+    else:
+        raise TypeError(f"{var_name} must be a string or list of strings")
+
+    return obj
+
+
+def check_is_mtype(
+    obj,
+    mtype,
+    scitype: str = None,
+    return_metadata=False,
+    var_name="obj",
+    msg_return_dict="dict",
+):
+    """Check object for compliance with mtype specification, return metadata.
 
     Parameters
     ----------
-    f: The function to decorate
+    obj - object to check
+    mtype: str or list of str, mtype to check obj as
+        valid mtype strings are in datatypes.MTYPE_REGISTER (1st column)
+    scitype: str, optional, scitype to check obj as; default = inferred from mtype
+        if inferred from mtype, list elements of mtype need not have same scitype
+        valid mtype strings are in datatypes.SCITYPE_REGISTER (1st column)
+    return_metadata - bool, str, or list of str, optional, default=False
+        if False, returns only "valid" return
+        if True, returns all three return objects
+        if str, list of str, metadata return dict is subset to keys in return_metadata
+    var_name: str, optional, default="obj"
+        name of input in error messages
+
+    msg_return_dict: str, one of ``"list"`` or ``"dict"``, optional, default="dict"
+        whether returned msg, if returned, is a str, dict or list
+
+        * if ``msg_return_dict="list"``,
+          returned ``msg`` is ``str`` if ``mtype`` is ``str``,
+          returned ``msg`` is ``list`` of ``str`` if ``mtype`` is ``list``
+
+        * if ``msg_return_dict="dict"``,
+          returned ``msg`` is ``str`` if ``mtype`` is ``str``,
+          returned ``msg`` is ``dict`` of ``str`` if ``mtype`` is ``list``.
+          If ``dict``, has str in ``mtype`` as key,
+          and error message for mtype as value.
 
     Returns
     -------
-    Decorated function
+    valid: bool
+        whether obj is a valid object of mtype/scitype
+    msg: str or list/dict of str
+        error messages if object is not valid, otherwise None,
+        returned only if return_metadata is True or str, list of str
+
+        whether ``list`` or ``dict`` type is controlled via msg_return_dict
+
+        * if ``str``: error message for tested mtype
+        * if ``list``:
+          list of len(mtype) with message per mtype if list, same order as mtype
+        * if ``dict``: dict with mtype as key and error message for mtype as value
+
+    metadata: dict - metadata about obj if valid, otherwise None
+        returned only if ``return_metadata`` is True or str, list of str
+
+        Keys populated depend on (assumed, otherwise identified) scitype of obj.
+
+        Always returned:
+        * "mtype": str, mtype of obj (assumed or inferred)
+        * "scitype": str, scitype of obj (assumed or inferred)
+
+        For scitype "Table":
+
+        * "is_univariate": bool, True iff table has one variable
+        * "is_empty": bool, True iff table has no variables or no instances
+        * "has_nans": bool, True iff the panel contains NaN values
+        * "n_instances": int, number of instances/rows in the table
+        * "n_features": int, number of variables in table
+        * "feature_names": list of int or object, names of variables in table
+
+    Raises
+    ------
+    TypeError if no checks defined for mtype/scitype combination
+    TypeError if mtype input argument is not of expected type
     """
+    mtype = _coerce_list_of_str(mtype, var_name="mtype")
 
-    def wrapper(self, *args, **kwargs):
-        return f(self)
+    valid_keys = check_dict.keys()
 
-    return _forward_meta(wrapper, f)
-
-
-def _vectorize(f):
-    """Enable automatic vectorization of a function.
-
-    The wrapper vectorizes a interface function unless
-    it is decorated with the vectorvalued decorator
-
-    Parameters
-    ----------
-    f: The function to decorate
-
-    Returns
-    -------
-    Decorated function
-    """
+    # we loop through individual mtypes in mtype and see whether they pass the check
+    #  for each check we remember whether it passed and what it returned
+    if msg_return_dict == "list":
+        msg = []
+    elif msg_return_dict == "dict":
+        msg = dict()
+    else:
+        raise ValueError(
+            f"Error in check_is_mtype, msg_return_dict argument "
+            f"must be 'list' or 'dict', found {msg_return_dict}"
+        )
 
-    def wrapper(self, *args, **kwargs):
-        # cache index
-        index_ = self.index
-        self.index = slice(None)
+    found_mtype = []
+    found_scitype = []
 
-        if getattr(f, "already_vectorized", False):
-            result = f(self, *args, **kwargs)
+    for m in mtype:
+        if scitype is None:
+            scitype_of_m = mtype_to_scitype(m)
         else:
-            result = []
-            for index in range(len(self.X)):
-                self.index = index
-                result.append(f(self, *args, **kwargs))
+            _check_scitype_valid(scitype)
+            scitype_of_m = scitype
+        key = (m, scitype_of_m)
+        if (m, scitype_of_m) not in valid_keys:
+            raise TypeError(f"no check defined for mtype {m}, scitype {scitype_of_m}")
 
-        # rollback index
-        self.index = index_
+        res = check_dict[key](obj, return_metadata=return_metadata, var_name=var_name)
 
-        if len(result) > 1:
-            return np.array(result)
+        if _metadata_requested(return_metadata):
+            check_passed = res[0]
         else:
-            return result[0]
-
-    return _forward_meta(wrapper, f)
+            check_passed = res
 
+        if check_passed:
+            found_mtype.append(m)
+            found_scitype.append(scitype_of_m)
+            final_result = res
+        elif _metadata_requested(return_metadata):
+            if msg_return_dict == "list":
+                msg.append(res[1])
+            else:
+                msg[m] = res[1]
 
-def _elementwise(f):
-    """Enable elementwise operations.
+    # there are three options on the result of check_is_mtype:
+    # a. two or more mtypes are found - this is unexpected and an error with checks
+    if len(found_mtype) > 1:
+        raise TypeError(
+            f"Error in check_is_mtype, more than one mtype identified: {found_mtype}"
+        )
+    # b. one mtype is found - then return that mtype
+    elif len(found_mtype) == 1:
+        if _metadata_requested(return_metadata):
+            # add the mtype return to the metadata
+            final_result[2]["mtype"] = found_mtype[0]
+            final_result[2]["scitype"] = found_scitype[0]
+            # final_result already has right shape and dependency on return_metadata
+            return final_result
+        else:
+            return True
+    # c. no mtype is found - then return False and all error messages if requested
+    else:
+        if len(msg) == 1:
+            msg = msg[0]
 
-    The wrapper implements two different modes of argument evaluation
-    for given p_1,..., p_k that represent the predicted distributions
-    and and x_1,...,x_m that represent the values to evaluate them on.
+        return _ret(False, msg, None, return_metadata)
 
-    "elementwise" (default): Repeat the sequence of p_i until there are m,
-                            i.e., p_1,...,p_k,p_1,p_2,...,p_k,p_1,...,p_m'
-                            where m' is the remainder of dividing m by k.
 
-    "batch": x_1, ..., x_m is evaluated on every distribution p_i
-            resulting in a matrix m columns and k rows.
+def check_raise(obj, mtype: str, scitype: str = None, var_name: str = "input"):
+    """Check object for compliance with mtype specification, raise errors.
 
     Parameters
     ----------
-    f: The function to decorate
+    obj - object to check
+    mtype: str or list of str, mtype to check obj as
+        valid mtype strings are in datatypes.MTYPE_REGISTER (1st column)
+    scitype: str, optional, scitype to check obj as; default = inferred from mtype
+        if inferred from mtype, list elements of mtype need not have same scitype
+        valid mtype strings are in datatypes.SCITYPE_REGISTER (1st column)
+    var_name: str, optional, default="input" - name of input in error messages
 
     Returns
     -------
-    Decorated function
+    valid: bool - True if obj complies with the specification
+            same as when return argument of check_is_mtype is True
+            otherwise raises an error
+
+    Raises
+    ------
+    TypeError with informative message if obj does not comply
+    TypeError if no checks defined for mtype/scitype combination
+    ValueError if mtype input argument is not of expected type
     """
+    obj_long_name_for_avoiding_linter_clash = obj
+    valid, msg, _ = check_is_mtype(
+        obj=obj_long_name_for_avoiding_linter_clash,
+        mtype=mtype,
+        scitype=scitype,
+        return_metadata=[],
+        var_name=var_name,
+        msg_return_dict="list",
+    )
+
+    if valid:
+        return True
+    else:
+        raise TypeError(msg)
 
-    def wrapper(self, x, *args, **kwargs):
-        if len(np.array(x).shape) > 1:
-            x = x.flatten()
-
-        # cache index
-        index_ = self.index
-        self.index = slice(None)
 
-        # disable elementwise mode if x is scalar
-        elementwise = self.mode == "elementwise" and len(np.array(x).shape) != 0
-
-        if elementwise:
-            evaluations = len(x)
-        else:
-            evaluations = len(self.X)
+def mtype(obj, as_scitype=None, exclude_mtypes=AMBIGUOUS_MTYPES):
+    """Infer the mtype of an object considered as a specific scitype.
 
-        # compose result
-        result = []
-        number_of_points = len(self.X)
-        for index in range(evaluations):
-            # set evaluation index and point
-            if elementwise:
-                self.index = index % number_of_points
-                at = x[index]
-            else:
-                self.index = index
-                at = x
-
-            # evaluate the function at this point
-            result.append(f(self, at, *args, **kwargs))
+    Parameters
+    ----------
+    obj : object to infer type of - any type, should comply with some mtype spec
+        if as_scitype is provided, this needs to be mtype belonging to scitype
+    as_scitype : str, list of str, or None, optional, default=None
+        name of scitype(s) the object "obj" is considered as, finds mtype for that
+        if None (default), does not assume a specific as_scitype and tests all mtypes
+            generally, as_scitype should be provided for maximum efficiency
+        valid scitype type strings are in datatypes.SCITYPE_REGISTER (1st column)
+    exclude_mtypes : list of str, default = AMBIGUOUS_MTYPES
+        which mtypes to ignore in inferring mtype, default = ambiguous ones
 
-        # rollback index
-        self.index = index_
+    Returns
+    -------
+    str - the inferred mtype of "obj", a valid mtype string
+            or None, if obj is None
+        mtype strings with explanation are in datatypes.MTYPE_REGISTER
+
+    Raises
+    ------
+    TypeError if no type can be identified, or more than one type is identified
+    """
+    if obj is None:
+        return None
 
-        if len(result) > 1:
-            return np.array(result)
+    if as_scitype is not None:
+        as_scitype = _coerce_list_of_str(as_scitype, var_name="as_scitype")
+        for scitype in as_scitype:
+            _check_scitype_valid(scitype)
+
+    m_plus_scitypes = [
+        (x[0], x[1]) for x in check_dict.keys() if x[0] not in exclude_mtypes
+    ]
+
+    if as_scitype is not None:
+        m_plus_scitypes = [(x[0], x[1]) for x in m_plus_scitypes if x[1] in as_scitype]
+
+    # collects mtypes that are tested as valid for obj
+    mtypes_positive = []
+
+    # collects error messages from mtypes that are tested as invalid for obj
+    mtypes_negative = dict()
+
+    for m_plus_scitype in m_plus_scitypes:
+        valid, msg, _ = check_is_mtype(
+            obj,
+            mtype=m_plus_scitype[0],
+            scitype=m_plus_scitype[1],
+            return_metadata=[],
+            msg_return_dict="list",
+        )
+        if valid:
+            mtypes_positive += [m_plus_scitype[0]]
         else:
-            return result[0]
+            mtypes_negative[m_plus_scitype[0]] = msg
 
-    return _forward_meta(wrapper, f)
-
-
-def _cached(f):
-    """Enable caching.
+    if len(mtypes_positive) > 1:
+        raise TypeError(
+            f"Error in check_is_mtype, more than one mtype identified:"
+            f" {mtypes_positive}"
+        )
 
-    Wrapper uses lru_cache to cache function result
+    if len(mtypes_positive) < 1:
+        msg = ""
+        for mtype, error in mtypes_negative.items():
+            msg += f"{mtype}: {error}\r\n"
+        msg = (
+            f"No valid mtype could be identified for object of type {type(obj)}. "
+            f"Errors returned are as follows, in format [mtype]: [error message] \r\n"
+        ) + msg
+        raise TypeError(msg)
+
+    return mtypes_positive[0]
+
+
+def check_is_scitype(
+    obj,
+    scitype,
+    return_metadata=False,
+    var_name="obj",
+    exclude_mtypes=AMBIGUOUS_MTYPES,
+):
+    """Check object for compliance with scitype specification, return metadata.
 
     Parameters
     ----------
-    f: The function to decorate
+    obj - object to check
+    scitype: str or list of str, scitype to check obj as
+        valid mtype strings are in datatypes.SCITYPE_REGISTER
+    return_metadata - bool, optional, default=False
+        if False, returns only "valid" return
+        if True, returns all three return objects
+        if str, list of str, metadata return dict is subset to keys in return_metadata
+    var_name: str, optional, default="obj" - name of input in error messages
+    exclude_mtypes : list of str, default = AMBIGUOUS_MTYPES
+        which mtypes to ignore in inferring mtype, default = ambiguous ones
 
     Returns
     -------
-    Decorated function
+    valid: bool - whether obj is a valid object of mtype/scitype
+    msg: dict[str, str] or None
+        error messages if object is not valid, otherwise None
+        keys are all mtypes tested, value for key is error message for that key
+    metadata: dict - metadata about obj if valid, otherwise None
+            returned only if return_metadata is True
+        Fields depend on scitpe.
+        Always returned:
+            "mtype": str, mtype of obj (assumed or inferred)
+                mtype strings with explanation are in datatypes.MTYPE_REGISTER
+            "scitype": str, scitype of obj (assumed or inferred)
+                scitype strings with explanation are in datatypes.SCITYPE_REGISTER
+        For scitype "Series":
+            "is_univariate": bool, True iff series has one variable
+            "is_equally_spaced": bool, True iff series index is equally spaced
+            "is_empty": bool, True iff series has no variables or no instances
+            "has_nans": bool, True iff the series contains NaN values
+        For scitype "Panel":
+            "is_univariate": bool, True iff all series in panel have one variable
+            "is_equally_spaced": bool, True iff all series indices are equally spaced
+            "is_equal_length": bool, True iff all series in panel are of equal length
+            "is_empty": bool, True iff one or more of the series in the panel are empty
+            "is_one_series": bool, True iff there is only one series in the panel
+            "has_nans": bool, True iff the panel contains NaN values
+            "n_instances": int, number of instances in the panel
+        For scitype "Table":
+            "is_univariate": bool, True iff table has one variable
+            "is_empty": bool, True iff table has no variables or no instances
+            "has_nans": bool, True iff the panel contains NaN values
+        For scitype "Alignment":
+            currently none
+    Raises
+    ------
+    TypeError if scitype input argument is not of expected type
     """
+    scitype = _coerce_list_of_str(scitype, var_name="scitype")
 
-    @functools.lru_cache
-    def wrapper(self, *args, **kwargs):
-        return f(self, *args, **kwargs)
+    for x in scitype:
+        _check_scitype_valid(x)
 
-    return _forward_meta(wrapper, f)
+    valid_keys = check_dict.keys()
 
+    # find all the mtype keys corresponding to the scitypes
+    keys = [x for x in valid_keys if x[1] in scitype and x[0] not in exclude_mtypes]
 
-class ProbabilisticEstimator(BaseEstimator, metaclass=abc.ABCMeta):
-    """Abstract base class for probabilistic prediction models.
-
-    Notes
-    -----
-    All probabilistic estimators should specify all the parameters
-    that can be set at the class level in their ``__init__``
-    as explicit keyword arguments (no ``*args`` or ``**kwargs``).
-    """
+    # storing the msg return
+    msg = {}
+    found_mtype = []
+    found_scitype = []
 
-    class ImplementsEnhancedInterface(abc.ABCMeta):
-        """Meta-class for distribution interface.
+    for key in keys:
+        res = check_dict[key](obj, return_metadata=return_metadata, var_name=var_name)
 
-        Enhances the distribution interface behind the scenes
-        with automatic caching and syntactic sugar for
-        element-wise access of the distributions
-        """
-
-        def __init__(cls, name, bases, clsdict):
-            for method in ["pdf", "cdf"]:
-                if method in clsdict:
-                    setattr(
-                        cls, method, _elementwise(ensure_existence(clsdict[method]))
-                    )
-
-            for method in ["point", "std", "lp2"]:
-                if method in clsdict:
-                    setattr(
-                        cls,
-                        method,
-                        _cached(
-                            _vectorize(_generalize(ensure_existence(clsdict[method])))
-                        ),
-                    )
-
-    class Distribution(metaclass=ImplementsEnhancedInterface):
-        """Abstract base class for the distributions returned by estimators.
-
-        Parameters
-        ----------
-        estimator: ``skpro.base.ProbabilisticEstimator``
-            Parent probabilistic estimator object
-        X: np.array
-            Features
-        selection: slice | int (optional)
-            Subset point selection of the features
-        mode: str
-            Interface mode ('elementwise' or 'batch')
-        """
-
-        def __init__(  # noqa
-            self, estimator, X, selection=slice(None), mode="elementwise"  # noqa
-        ):  # noqa
-            self.estimator = estimator
-            self._X = X
-            self.index = slice(None)
-            self.selection = selection
-            if mode not in ["elementwise", "batch"]:
-                mode = "elementwise"
-            self.mode = mode
-
-            if callable(getattr(self, "_init", None)):
-                self._init()
-
-        @property
-        def X(self):
-            """Test features.
-
-            Reference of the test features that are ought to correspond
-            with the predictive distribution represented by the interface.
-
-            The interface methods (e.g. pdf) can use X to
-            construct and exhibit the predictive distribution properties
-            of the interface (e.g. construct the predicted pdf based on X)
-
-            Note that X automatically reflects the feature point for which
-            the interface is ought to represent the distributional
-            prediction. For given M x n features, X will thus represent
-            an 1 x n vector that provides the bases for the predicted
-            distribution. However, if the :func:`.vectorvalued` decorator
-            is applied X will represent the full M x n matrix for an
-            efficient vectorized implementation.
-
-            :getter: Returns the test features based on the current subset selection
-            :setter: Sets the data reference
-            :type: array
-            """
-            return self._X[self.selection, :][self.index]
-
-        @X.setter
-        def X(self, value):
-            self._X = value
-
-        def __len__(self):
-            """Return the number of distributions represented by the interface."""
-            shape = self.X.shape
-            return shape[0] if len(shape) > 1 else 1
-
-        def __setitem__(self, key, value):
-            """Set a subset of the distribution object."""
-            raise Exception("skpro distributions are readonly")
-
-        def __delitem__(self, key):
-            """Delete a subset of the distribution object."""
-            raise Exception("skpro distributions are readonly")
-
-        def replicate(self, selection=None, mode=None):
-            """Replicatesthe distribution object.
-
-            Parameters
-            ----------
-            selection: None | slice | int (optional)
-                Subset point selection of the distribution copy
-            mode: str (optional)
-                Interface mode ('elementwise' or 'batch')
-
-            Returns
-            -------
-            ``skpro.base.ProbabilisticEstimator.Distribution``
-            """
-            if selection is None:
-                selection = self.selection
-
-            if mode is None:
-                mode = self.mode
-
-            return self.__class__(self.estimator, self._X, selection, mode)
-
-        def __getitem__(self, key):
-            """Return a subset of the distribution object.
-
-            Parameters
-            ----------
-            - slice indexing, mode (optional)
-            - mode only (in which full subset is returned)
-
-            Returns
-            -------
-            ``skpro.base.ProbabilisticEstimator.Distribution``
-            """
-            # cache index
-            index_ = self.index
-            self.index = slice(None)
-
-            # parse key
-            if isinstance(key, tuple) and len(key) == 2:
-                selection = key[0]
-                mode = key[1]
-            elif isinstance(key, str):
-                selection = slice(None)
-                mode = key
-            else:
-                selection = key
-                mode = None
+        if _metadata_requested(return_metadata):
+            check_passed = res[0]
+        else:
+            check_passed = res
 
-            # convert index to slice for consistent usage
-            if isinstance(selection, int):
-                if selection >= len(self):
-                    raise IndexError("Selection is out of bounds")
-
-                selection = slice(selection, selection + 1)
-
-            # check for out of bounds subsets
-            if len(range(*selection.indices(len(self)))) == 0:
-                raise IndexError("Selection is out of bounds")
-
-            # create subset replication
-            replication = self.replicate(selection, mode)
-
-            # rollback index
-            self.index = index_
-
-            return replication
-
-        def __point__(self, name):
-            """Point prediction."""
-            if len(self) > 1:
-                raise TypeError(
-                    "Multiple distributions can not be converted to " + name
-                )
-
-            return self.point()
-
-        def __float__(self):
-            """Float prediction."""
-            return float(self.__point__("float"))
-
-        def __int__(self):
-            """Int prediction."""
-            return int(self.__point__("int"))
-
-        @abc.abstractmethod
-        def point(self):
-            """Point prediction.
-
-            Returns
-            -------
-            The point prediction that corresponds to self.X
-            """
-            raise NotImplementedError()
-
-        def mean(self, *args, **kwargs):
-            """Mean prediction.
-
-            Returns
-            -------
-            The mean prediction that corresponds to self.X
-            """
-            return self.point()
-
-        @abc.abstractmethod
-        def std(self):
-            """Variance prediction.
-
-            Returns
-            -------
-            The estimated standard deviation that corresponds to self.X
-            """
-            raise NotImplementedError()
-
-        def pdf(self, x):
-            """Probability density function.
-
-            Parameters
-            ----------
-            x
-
-            Returns
-            -------
-            mixed  Density function evaluated at x
-            """
-            warnings.warn(  # noqa
-                self.__class__.__name__ + " does not implement a pdf function",
-                UserWarning,
-            )
-
-        def cdf(self, x):
-            """Cumulative density function.
-
-            Parameters
-            ----------
-            x
-
-            Returns
-            -------
-            mixed  Cumulative density function evaluated at x
-            """
-            warnings.warn(  # noqa
-                self.__class__.__name__ + " does not implement a cdf function",
-                UserWarning,
-            )
-
-        def ppf(self, q, *args, **kwargs):
-            """Percent point function (inverse of cdf — percentiles).
-
-            Parameters
-            ----------
-            q
-
-            Returns
-            -------
-            float
-            """
-            warnings.warn(  # noqa
-                self.__class__.__name__ + " does not implement a ppf function",
-                UserWarning,
-            )
-
-        def lp2(self):
-            r"""Compute Lp2 norm of the probability density function.
-
-            ..math::
-            L^2 = \int PDF(x)^2 dx
-
-            Returns
-            -------
-            float: Lp2-norm of the density function
-            """
-            warnings.warn(  # noqa
-                f"{self.__class__.__name__} "
-                "does not implement a lp2 function, "
-                "defaulting to numerical approximation",
-                UserWarning,
-            )
-
-            from scipy.integrate import quad as integrate
-
-            # y, y_err of
-            return integrate(lambda x: self[self.index].pdf(x) ** 2, -np.inf, np.inf)[0]
-
-    def name(self):
-        """Return the name of the estimator."""
-        return self.__class__.__name__
-
-    def __str__(self):
-        """Return the name of the estimator."""
-        return "%s()" % self.__class__.__name__
-
-    def __repr__(self):
-        """Return the repr of the estimator."""
-        return "%s()" % self.__class__.__name__
-
-    @classmethod
-    def _distribution(cls):
-        return cls.Distribution
-
-    def predict(self, X):
-        """Predict using the model.
-
-        Parameters
-        ----------
-        X : {array-like, sparse matrix}, shape = (n_samples, n_features)
-            Samples.
-
-        Returns
-        -------
-        :class:`.Distribution` interface representing n_samples predictions
-            Returns predicted distributions
-        """
-        return self._distribution()(self, X)
-
-    def fit(self, X, y):
-        """Fit the model.
-
-        Parameters
-        ----------
-        X : numpy array or sparse matrix of shape [n_samples,n_features]
-            Training data
-        y : numpy array of shape [n_samples, n_targets]
-            Target values. Will be cast to X's dtype if necessary
-
-        Returns
-        -------
-        self : returns an instance of self.
-        """
-        warnings.warn(  # noqa
-            "The estimator doesn't implement a fit procedure", UserWarning  # noqa
-        )  # noqa
-
-        return self  # noqa
-
-    def score(self, X, y, sample=True, return_std=False):
-        """Return the log-loss score.
-
-        Parameters
-        ----------
-            X:  np.array
-                Features
-            y:  np.array
-                Labels
-            sample: boolean, default=True
-                If true, loss will be averaged across the sample
-            return_std: boolean, default=False
-                If true, the standard deviation of the
-                loss sample will be returned
-
-        Returns
-        -------
-        mixed
-            Log-loss score
-        """
-        return make_scorer(log_loss, greater_is_better=False)(  # noqa
-            self, X, y, sample=sample, return_std=return_std
+        if check_passed:
+            final_result = res
+            found_mtype.append(key[0])
+            found_scitype.append(key[1])
+        elif _metadata_requested(return_metadata):
+            msg[key[0]] = res[1]
+
+    # there are three options on the result of check_is_mtype:
+    # a. two or more mtypes are found - this is unexpected and an error with checks
+    if len(found_mtype) > 1:
+        raise TypeError(
+            f"Error in check_is_mtype, more than one mtype identified: {found_mtype}"
         )
+    # b. one mtype is found - then return that mtype
+    elif len(found_mtype) == 1:
+        if _metadata_requested(return_metadata):
+            # add the mtype return to the metadata
+            final_result[2]["mtype"] = found_mtype[0]
+            # add the scitype return to the metadata
+            final_result[2]["scitype"] = found_scitype[0]
+            # final_result already has right shape and dependency on return_metadata
+            return final_result
+        else:
+            return True
+    # c. no mtype is found - then return False and all error messages if requested
+    else:
+        return _ret(False, msg, None, return_metadata)
 
 
-###############################################################################
-
-
-class VendorInterface(metaclass=abc.ABCMeta):  # noqa
-    """Abstract base class for a vendor interface."""
-
-    def on_fit(self, X, y):  # noqa
-        """Vendor fit procedure.
-
-        Parameters
-        ----------
-        X : np.array
-            Training features
-        y : np.array
-            Training labels
-
-        Returns
-        -------
-        None
-        """
-        pass
-
-    def on_predict(self, X):  # noqa
-        """Vendor predict procedure.
-
-        Parameters
-        ----------
-        X : np.array
-            Test features
-
-        Returns
-        -------
-        None
-        """
-        pass
-
-
-class VendorEstimator(ProbabilisticEstimator):
-    """VendorEstimator.
-
-    ProbabilisticEstimator that interfaces a vendor using
-    a VendorInterface and Adapter.
+def check_is_error_msg(msg, var_name="obj", allowed_msg=None, raise_exception=False):
+    """Format and possibly raise error message from check_is_mtype or check_is_scitype.
 
     Parameters
     ----------
-    model: skpro.base.VendorInterface
-        Vendor interface
-    adapter: skpro.density.DensityAdapter
-        Density adapter
-    """
-
-    class Distribution(ProbabilisticEstimator.Distribution, metaclass=abc.ABCMeta):
-        """Distribution class returned by VendorEstimator.predict(X)."""
-
-        pass
+    msg: dict[str, str]
+        error message from check_is_scitype, or from check_is_mtype with dict return
+    var_name: str, optional, default="obj"
+        name of input in error messages
+    allowed_msg: str, optional, default=None
+        message component detailing allowed mtypes or scitype combinations
+    raise_exception: bool or Exception, optional, default=False
+        whether to raise exception or return error message
+        if False, returns formatted error message
+        if True, raises TypeError with formatted error message
+        if Exception, raises that Exception with formatted error message
 
-    def __init__(self, model=None, adapter=None):
-        """Construct self.
-
-        Parameters
-        ----------
-        model : :class:`.VendorInterface`
-            The vendor model
-        adapter :class:`.DensityAdapter`
-            Used density adapter
-        """
-        self.model = self._check_model(model)
-        self.adapter = self._check_adapter(adapter)
-
-    def _check_model(self, model=None):
-        """Check the model.
-
-        Checks if vendor interface is valid
-
-        Parameters
-        ----------
-        model: skpro.base.VendorInterface
-            Vendor interface
-        Returns
-        -------
-        skpro.base.VendorInterface
-        """
-        if not issubclass(model.__class__, VendorInterface):
-            raise ValueError(
-                "model has to be a VendorInterface" "%s given." % model.__class__
-            )
-
-        return model
-
-    def _check_adapter(self, adapter):
-        """Check the adapter.
-
-        Can be overwritten to implement checking procedures for a
-        density adapter that are applied during the object
-        initialisation.
-
-        Parameters
-        ----------
-        adapter: skpro.density.DensityAdapter
-            Adapter
-
-        Returns
-        -------
-        skpro.density.DensityAdapter
-        """
-        return adapter
-
-    def fit(self, X, y):
-        """Fit the vendor model.
-
-        Parameters
-        ----------
-        X : numpy array or sparse matrix of shape [n_samples,n_features]
-            Training data
-        y : numpy array of shape [n_samples, n_targets]
-            Target values. Will be cast to X's dtype if necessary
-
-        Returns
-        -------
-        self : returns an instance of self.
-        """
-        self.model.on_fit(X, y)
-
-        return self
-
-    def predict(self, X):
-        """Predict using the vendor model.
-
-        Parameters
-        ----------
-        X : {array-like, sparse matrix}, shape = (n_samples, n_features)
-            Samples.
-
-        Returns
-        -------
-        :class:`.Distribution` interface representing n_samples predictions
-            Returns predicted distributions
-        """
-        self.model.on_predict(X)
-
-        return super().predict(X)
-
-
-class BayesianVendorInterface(VendorInterface):
-    """Abstract base class for a Bayesian vendor.
-
-    Notes
-    -----
-    Must implement the samples method that returns
-    Bayesian posterior samples. The sample method
-    should be cached using the ``functools.lru_cache``
-    decorator to increase performance
+    Returns
+    -------
+    str - formatted error message
     """
-
-    @abc.abstractmethod
-    @functools.lru_cache  # noqa
-    def samples(self):
-        """Return the predictive posterior samples.
-
-        Returns
-        -------
-        np.array
-            Predictive posterior sample
-        """
-        raise NotImplementedError()
+    msg_invalid_input = (
+        f"{var_name} must be in an skpro compatible format. {allowed_msg}"
+        f"If you think the data is already in an skpro supported input format, "
+        f"run skpro.datatypes.check_raise(data, mtype) to diagnose the error, "
+        f"where mtype is the string of the type specification you want. "
+        f"Error message for checked mtypes, in format [mtype: message], as follows:"
+    )
+    for mtype, err in msg.items():
+        msg_invalid_input += f" [{mtype}: {err}] "
+
+    if raise_exception is True:
+        raise TypeError(msg_invalid_input)
+    elif raise_exception is False:
+        return msg_invalid_input
+    else:
+        raise raise_exception(msg_invalid_input)
 
 
-class BayesianVendorEstimator(VendorEstimator):
-    """Vendor estimator for Bayesian methods.
+def scitype(obj, candidate_scitypes=SCITYPE_LIST, exclude_mtypes=AMBIGUOUS_MTYPES):
+    """Infer the scitype of an object.
 
-    ProbabilisticEstimator that interfaces a Bayesian vendor using
-    a BayesianVendorInterface and and sample-based Adapter.
+    Parameters
+    ----------
+    obj : object to infer type of - any type, should comply with some mtype spec
+        if as_scitype is provided, this needs to be mtype belonging to scitype
+    candidate_scitypes: str or list of str, scitypes to pick from
+        valid scitype strings are in datatypes.SCITYPE_REGISTER
+    exclude_mtypes : list of str, default = AMBIGUOUS_MTYPES
+        which mtypes to ignore in inferring mtype, default = ambiguous ones
+        valid mtype strings are in datatypes.MTYPE_REGISTER
 
+    Returns
+    -------
+    str - the inferred sciype of "obj", a valid scitype string
+            or None, if obj is None
+        scitype strings with explanation are in datatypes.SCITYPE_REGISTER
+
+    Raises
+    ------
+    TypeError if no type can be identified, or more than one type is identified
     """
+    candidate_scitypes = _coerce_list_of_str(
+        candidate_scitypes, var_name="candidate_scitypes"
+    )
+
+    valid_scitypes = []
+
+    for scitype in candidate_scitypes:
+        valid = check_is_scitype(
+            obj,
+            scitype=scitype,
+            return_metadata=False,
+            exclude_mtypes=exclude_mtypes,
+        )
+        if valid:
+            valid_scitypes += [scitype]
 
-    class Distribution(VendorEstimator.Distribution):
-        """Distribution class returned by BayesianVendorEstimator.predict(X)."""
-
-        def _init(self):
-            # initialise adapter with samples
-            self.adapters_ = []
-            self.samples = self.estimator.model.samples()
-            for index in range(len(self.X)):
-                adapter = clone(self.estimator.adapter)
-                adapter(self.samples[index, :])
-                self.adapters_.append(adapter)
-
-        @vectorvalued
-        def point(self):
-            """Point prediction."""
-            return self.samples.mean(axis=1)
-
-        @vectorvalued
-        def std(self):
-            """Std prediction."""
-            return self.samples.std(axis=1)
-
-        def cdf(self, x):
-            """Cumulative density function.
-
-            Parameters
-            ----------
-            x
-
-            Returns
-            -------
-            mixed  Cumulative density function evaluated at x
-            """
-            ensure_existence(self.adapters_[self.index].cdf)
-
-            return self.adapters_[self.index].cdf(x)
-
-        def pdf(self, x):
-            """Probability density function.
-
-            Parameters
-            ----------
-            x
-
-            Returns
-            -------
-            mixed  Density function evaluated at x
-            """
-            ensure_existence(self.adapters_[self.index].pdf)
-
-            return self.adapters_[self.index].pdf(x)
-
-    def _check_model(self, model=None):
-        if not issubclass(model.__class__, BayesianVendorInterface):
-            raise ValueError(
-                "model has to be a subclass of skpro.base.BayesianVendorInterface"
-                "%s given." % model.__class__
-            )
-
-        return model
-
-    def _check_adapter(self, adapter=None):
-        if adapter is None:
-            # default adapter
-            adapter = KernelDensityAdapter()
-
-        if not issubclass(adapter.__class__, DensityAdapter):
-            raise ValueError(
-                "adapter has to be a subclass of skpro.density.DensityAdapter"
-                "%s given." % adapter.__class__
-            )
+    if len(valid_scitypes) > 1:
+        raise TypeError(
+            "Error in function scitype, more than one valid scitype identified:"
+            f"{ valid_scitypes}"
+        )
+    if len(valid_scitypes) == 0:
+        raise TypeError(
+            "Error in function scitype, no valid scitype could be identified."
+        )
 
-        return adapter
+    return valid_scitypes[0]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `skpro-2.3.0/skpro/benchmarking/evaluate.py` & `skpro-2.3.1/skpro/benchmarking/evaluate.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/benchmarking/tests/test_evaluate.py` & `skpro-2.3.1/skpro/benchmarking/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/__init__.py` & `skpro-2.3.1/skpro/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_adapter/polars.py` & `skpro-2.3.1/skpro/datatypes/_adapter/polars.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_common.py` & `skpro-2.3.1/skpro/datatypes/_common.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_convert.py` & `skpro-2.3.1/skpro/datatypes/_convert.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_convert_utils/_coerce.py` & `skpro-2.3.1/skpro/datatypes/_convert_utils/_coerce.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_convert_utils/_convert.py` & `skpro-2.3.1/skpro/datatypes/_convert_utils/_convert.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_examples.py` & `skpro-2.3.1/skpro/datatypes/_examples.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_proba/__init__.py` & `skpro-2.3.1/skpro/datatypes/_proba/__init__.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_proba/_check.py` & `skpro-2.3.1/skpro/datatypes/_proba/_check.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_proba/_convert.py` & `skpro-2.3.1/skpro/datatypes/_proba/_convert.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_proba/_examples.py` & `skpro-2.3.1/skpro/datatypes/_proba/_examples.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_proba/_registry.py` & `skpro-2.3.1/skpro/datatypes/_proba/_registry.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_registry.py` & `skpro-2.3.1/skpro/datatypes/_registry.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_table/__init__.py` & `skpro-2.3.1/skpro/datatypes/_table/__init__.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_table/_check.py` & `skpro-2.3.1/skpro/datatypes/_table/_check.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_table/_convert.py` & `skpro-2.3.1/skpro/datatypes/_table/_convert.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_table/_examples.py` & `skpro-2.3.1/skpro/datatypes/_table/_examples.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/_table/_registry.py` & `skpro-2.3.1/skpro/datatypes/_table/_registry.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/tests/test_check.py` & `skpro-2.3.1/skpro/datatypes/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/tests/test_convert.py` & `skpro-2.3.1/skpro/datatypes/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/tests/test_convert_to.py` & `skpro-2.3.1/skpro/datatypes/tests/test_convert_to.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/datatypes/tests/test_lookup.py` & `skpro-2.3.1/skpro/datatypes/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/__init__.py` & `skpro-2.3.1/skpro/distributions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Probability distribution objects."""
 
 # copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
 # adapted from sktime
 
 __all__ = [
+    "Alpha",
     "Beta",
     "ChiSquared",
     "Delta",
     "Empirical",
     "Exponential",
     "Fisk",
+    "Gamma",
+    "IID",
     "Laplace",
     "Logistic",
     "LogNormal",
     "Mixture",
     "Normal",
     "Poisson",
     "QPD_Empirical",
@@ -22,20 +25,23 @@
     "QPD_U",
     "QPD_Johnson",
     "TDistribution",
     "Uniform",
     "Weibull",
 ]
 
+from skpro.distributions.alpha import Alpha
 from skpro.distributions.beta import Beta
 from skpro.distributions.chi_squared import ChiSquared
+from skpro.distributions.compose import IID
 from skpro.distributions.delta import Delta
 from skpro.distributions.empirical import Empirical
 from skpro.distributions.exponential import Exponential
 from skpro.distributions.fisk import Fisk
+from skpro.distributions.gamma import Gamma
 from skpro.distributions.laplace import Laplace
 from skpro.distributions.logistic import Logistic
 from skpro.distributions.lognormal import LogNormal
 from skpro.distributions.mixture import Mixture
 from skpro.distributions.normal import Normal
 from skpro.distributions.poisson import Poisson
 from skpro.distributions.qpd import QPD_B, QPD_S, QPD_U, QPD_Johnson
```

### Comparing `skpro-2.3.0/skpro/distributions/adapters/scipy/_distribution.py` & `skpro-2.3.1/skpro/distributions/adapters/scipy/_distribution.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/adapters/scipy/_empirical.py` & `skpro-2.3.1/skpro/distributions/adapters/scipy/_empirical.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/adapters/scipy/tests/test_scipy_adapters.py` & `skpro-2.3.1/skpro/distributions/adapters/scipy/tests/test_scipy_adapters.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/adapters/statsmodels/_empirical.py` & `skpro-2.3.1/skpro/distributions/adapters/statsmodels/_empirical.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/base/_base.py` & `skpro-2.3.1/skpro/distributions/base/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1452,24 +1452,30 @@
 
     def sample(self, n_samples=None):
         """Sample from the distribution.
 
         Parameters
         ----------
         n_samples : int, optional, default = None
+            number of samples to draw from the distribution
 
         Returns
         -------
-        if `n_samples` is `None`:
-        returns a sample that contains a single sample from `self`,
-        in `pd.DataFrame` mtype format convention, with `index` and `columns` as `self`
-        if n_samples is `int`:
-        returns a `pd.DataFrame` that contains `n_samples` i.i.d. samples from `self`,
-        in `pd-multiindex` mtype format convention, with same `columns` as `self`,
-        and `MultiIndex` that is product of `RangeIndex(n_samples)` and `self.index`
+        pd.DataFrame
+            samples from the distribution
+
+            * if ``n_samples`` is ``None``:
+            returns a sample that contains a single sample from ``self``,
+            in ``pd.DataFrame`` mtype format convention, with ``index`` and ``columns``
+            as ``self``
+            * if n_samples is ``int``:
+            returns a ``pd.DataFrame`` that contains ``n_samples`` i.i.d.
+            samples from ``self``, in ``pd-multiindex`` mtype format convention,
+            with same ``columns`` as ``self``, and row ``MultiIndex`` that is product
+            of ``RangeIndex(n_samples)`` and ``self.index``
         """
 
         def gen_unif():
             np_unif = np.random.uniform(size=self.shape)
             if self.ndim > 0:
                 return pd.DataFrame(np_unif, index=self.index, columns=self.columns)
             return np_unif
@@ -1484,28 +1490,28 @@
                 df_spl = pd.concat(pd_smpl, keys=range(n_samples))
             else:
                 df_spl = pd.DataFrame(pd_smpl)
             return df_spl
 
         raise NotImplementedError(self._method_error_msg("sample", "error"))
 
-    def plot(self, fun="pdf", ax=None, **kwargs):
+    def plot(self, fun=None, ax=None, **kwargs):
         """Plot the distribution.
 
         Different distribution defining functions can be selected for plotting
         via the ``fun`` parameter.
         The functions available are the same as the methods of the distribution class,
         e.g., ``"pdf"``, ``"cdf"``, ``"ppf"``.
 
         For array distribution, the marginal distribution at each entry is plotted,
         as a separate subplot.
 
         Parameters
         ----------
-        fun : str, optional, default="pdf"
+        fun : str, optional, default="pdf" for continuous distributions, otherwise "cdf"
             the function to plot, one of "pdf", "cdf", "ppf"
         ax : matplotlib Axes object, optional
             matplotlib Axes to plot in
             if not provided, defaults to current axes (``plot.gca``)
         kwargs : keyword arguments
             passed to the plotting function
 
@@ -1516,14 +1522,20 @@
         ax : matplotlib.Axes
             the axis or axes on which the plot is drawn
         """
         _check_soft_dependencies("matplotlib", obj="distribution plot")
 
         from matplotlib.pyplot import subplots
 
+        if fun is None:
+            if self.get_tag("distr:measuretype", "mixed") == "continuous":
+                fun = "pdf"
+            else:
+                fun = "cdf"
+
         if self.ndim > 0:
             if "x_bounds" not in kwargs:
                 upper = self.ppf(0.999).values.flatten().max()
                 lower = self.ppf(0.001).values.flatten().min()
                 x_bounds = (lower, upper)
             else:
                 x_bounds = kwargs.pop("x_bounds")
@@ -1764,24 +1776,30 @@
 
     def sample(self, n_samples=None):
         """Sample from the distribution.
 
         Parameters
         ----------
         n_samples : int, optional, default = None
+            number of samples to draw from the distribution
 
         Returns
         -------
-        if `n_samples` is `None`:
-        returns a sample that contains a single sample from `self`,
-        in `pd.DataFrame` mtype format convention, with `index` and `columns` as `self`
-        if n_samples is `int`:
-        returns a `pd.DataFrame` that contains `n_samples` i.i.d. samples from `self`,
-        in `pd-multiindex` mtype format convention, with same `columns` as `self`,
-        and `MultiIndex` that is product of `RangeIndex(n_samples)` and `self.index`
+        pd.DataFrame
+            samples from the distribution
+
+            * if ``n_samples`` is ``None``:
+            returns a sample that contains a single sample from ``self``,
+            in ``pd.DataFrame`` mtype format convention, with ``index`` and ``columns``
+            as ``self``
+            * if n_samples is ``int``:
+            returns a ``pd.DataFrame`` that contains ``n_samples`` i.i.d.
+            samples from ``self``, in ``pd-multiindex`` mtype format convention,
+            with same ``columns`` as ``self``, and row ``MultiIndex`` that is product
+            of ``RangeIndex(n_samples)`` and ``self.index``
         """
         if n_samples is None:
             np_spl = self.distr.sample().numpy()
             return pd.DataFrame(np_spl, index=self.index, columns=self.columns)
         else:
             np_spl = self.distr.sample(n_samples).numpy()
             np_spl = np_spl.reshape(-1, np_spl.shape[-1])
```

### Comparing `skpro-2.3.0/skpro/distributions/base/_delegate.py` & `skpro-2.3.1/skpro/distributions/base/_delegate.py`

 * *Files 6% similar despite different names*

```diff
@@ -189,20 +189,26 @@
 
     def sample(self, n_samples=None):
         """Sample from the distribution.
 
         Parameters
         ----------
         n_samples : int, optional, default = None
+            number of samples to draw from the distribution
 
         Returns
         -------
-        if `n_samples` is `None`:
-        returns a sample that contains a single sample from `self`,
-        in `pd.DataFrame` mtype format convention, with `index` and `columns` as `self`
-        if n_samples is `int`:
-        returns a `pd.DataFrame` that contains `n_samples` i.i.d. samples from `self`,
-        in `pd-multiindex` mtype format convention, with same `columns` as `self`,
-        and `MultiIndex` that is product of `RangeIndex(n_samples)` and `self.index`
+        pd.DataFrame
+            samples from the distribution
+
+            * if ``n_samples`` is ``None``:
+            returns a sample that contains a single sample from ``self``,
+            in ``pd.DataFrame`` mtype format convention, with ``index`` and ``columns``
+            as ``self``
+            * if n_samples is ``int``:
+            returns a ``pd.DataFrame`` that contains ``n_samples`` i.i.d.
+            samples from ``self``, in ``pd-multiindex`` mtype format convention,
+            with same ``columns`` as ``self``, and row ``MultiIndex`` that is product
+            of ``RangeIndex(n_samples)`` and ``self.index``
         """
         delegate = self._get_delegate()
         return delegate.sample(n_samples=n_samples)
```

### Comparing `skpro-2.3.0/skpro/distributions/beta.py` & `skpro-2.3.1/skpro/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/chi_squared.py` & `skpro-2.3.1/skpro/distributions/chi_squared.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/delta.py` & `skpro-2.3.1/skpro/distributions/delta.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/empirical.py` & `skpro-2.3.1/skpro/distributions/empirical.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,17 +270,18 @@
             columns=subs_colidx,
         )
 
     def _iat(self, rowidx=None, colidx=None):
         if rowidx is None or colidx is None:
             raise ValueError("iat method requires both row and column index")
         self_subset = self.iloc[[rowidx], [colidx]]
-        spl_subset = self_subset.spl.droplevel(0)
+        levels_to_drop = list(range(1, self_subset.spl.index.nlevels))
+        spl_subset = self_subset.spl.droplevel(levels_to_drop)
         if self.weights is not None:
-            wts_subset = self_subset.weights.droplevel(0)
+            wts_subset = self_subset.weights.droplevel(levels_to_drop)
         else:
             wts_subset = None
 
         subset_params = {"spl": spl_subset, "weights": wts_subset}
         return type(self)(**subset_params)
 
     def _energy_default(self, x=None):
@@ -398,24 +399,30 @@
 
     def sample(self, n_samples=None):
         """Sample from the distribution.
 
         Parameters
         ----------
         n_samples : int, optional, default = None
+            number of samples to draw from the distribution
 
         Returns
         -------
-        if `n_samples` is `None`:
-        returns a sample that contains a single sample from `self`,
-        in `pd.DataFrame` mtype format convention, with `index` and `columns` as `self`
-        if n_samples is `int`:
-        returns a `pd.DataFrame` that contains `n_samples` i.i.d. samples from `self`,
-        in `pd-multiindex` mtype format convention, with same `columns` as `self`,
-        and `MultiIndex` that is product of `RangeIndex(n_samples)` and `self.index`
+        pd.DataFrame
+            samples from the distribution
+
+            * if ``n_samples`` is ``None``:
+            returns a sample that contains a single sample from ``self``,
+            in ``pd.DataFrame`` mtype format convention, with ``index`` and ``columns``
+            as ``self``
+            * if n_samples is ``int``:
+            returns a ``pd.DataFrame`` that contains ``n_samples`` i.i.d.
+            samples from ``self``, in ``pd-multiindex`` mtype format convention,
+            with same ``columns`` as ``self``, and row ``MultiIndex`` that is product
+            of ``RangeIndex(n_samples)`` and ``self.index``
         """
         # for now, always defaulting to the standard logic
         # todo: address issue #283
         if self.ndim >= 0:
             return super().sample(n_samples=n_samples)
 
         spl = self.spl
```

### Comparing `skpro-2.3.0/skpro/distributions/exponential.py` & `skpro-2.3.1/skpro/distributions/exponential.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/fisk.py` & `skpro-2.3.1/skpro/distributions/fisk.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/laplace.py` & `skpro-2.3.1/skpro/distributions/laplace.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/logistic.py` & `skpro-2.3.1/skpro/distributions/logistic.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/lognormal.py` & `skpro-2.3.1/skpro/distributions/lognormal.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/mixture.py` & `skpro-2.3.1/skpro/distributions/mixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,24 +179,30 @@
 
     def sample(self, n_samples=None):
         """Sample from the distribution.
 
         Parameters
         ----------
         n_samples : int, optional, default = None
+            number of samples to draw from the distribution
 
         Returns
         -------
-        if `n_samples` is `None`:
-        returns a sample that contains a single sample from `self`,
-        in `pd.DataFrame` mtype format convention, with `index` and `columns` as `self`
-        if n_samples is `int`:
-        returns a `pd.DataFrame` that contains `n_samples` i.i.d. samples from `self`,
-        in `pd-multiindex` mtype format convention, with same `columns` as `self`,
-        and `MultiIndex` that is product of `RangeIndex(n_samples)` and `self.index`
+        pd.DataFrame
+            samples from the distribution
+
+            * if ``n_samples`` is ``None``:
+            returns a sample that contains a single sample from ``self``,
+            in ``pd.DataFrame`` mtype format convention, with ``index`` and ``columns``
+            as ``self``
+            * if n_samples is ``int``:
+            returns a ``pd.DataFrame`` that contains ``n_samples`` i.i.d.
+            samples from ``self``, in ``pd-multiindex`` mtype format convention,
+            with same ``columns`` as ``self``, and row ``MultiIndex`` that is product
+            of ``RangeIndex(n_samples)`` and ``self.index``
         """
         indep_rows = self.indep_rows
         indep_cols = self.indep_cols
 
         if n_samples is None:
             N = 1
         else:
```

### Comparing `skpro-2.3.0/skpro/distributions/normal.py` & `skpro-2.3.1/skpro/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/poisson.py` & `skpro-2.3.1/skpro/distributions/poisson.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/qpd.py` & `skpro-2.3.1/skpro/distributions/qpd.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/qpd_empirical.py` & `skpro-2.3.1/skpro/distributions/qpd_empirical.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/t.py` & `skpro-2.3.1/skpro/distributions/t.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/tests/test_all_distrs.py` & `skpro-2.3.1/skpro/distributions/tests/test_all_distrs.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/tests/test_base_default_methods.py` & `skpro-2.3.1/skpro/distributions/tests/test_base_default_methods.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/tests/test_base_scalar.py` & `skpro-2.3.1/skpro/distributions/tests/test_base_scalar.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/tests/test_proba_basic.py` & `skpro-2.3.1/skpro/distributions/tests/test_proba_basic.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/tests/test_qpd.py` & `skpro-2.3.1/skpro/distributions/tests/test_qpd.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/uniform.py` & `skpro-2.3.1/skpro/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/distributions/weibull.py` & `skpro-2.3.1/skpro/distributions/weibull.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/metrics/__init__.py` & `skpro-2.3.1/skpro/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/metrics/_classes.py` & `skpro-2.3.1/skpro/metrics/_classes.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/metrics/_coerce.py` & `skpro-2.3.1/skpro/metrics/_coerce.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/metrics/base.py` & `skpro-2.3.1/skpro/metrics/base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/metrics/survival/_c_harrell.py` & `skpro-2.3.1/skpro/metrics/survival/_c_harrell.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/metrics/survival/_spll.py` & `skpro-2.3.1/skpro/metrics/survival/_spll.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/metrics/survival/tests/test_c_harrell.py` & `skpro-2.3.1/skpro/metrics/survival/tests/test_c_harrell.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/metrics/tests/test_distr_metrics.py` & `skpro-2.3.1/skpro/metrics/tests/test_distr_metrics.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/metrics/tests/test_probabilistic_metrics.py` & `skpro-2.3.1/skpro/metrics/tests/test_probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/model_selection/_tuning.py` & `skpro-2.3.1/skpro/model_selection/_tuning.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class BaseGridSearch(_DelegatedProbaRegressor):
     _tags = {
         "estimator_type": "regressor",
         "capability:multioutput": True,
         "capability:missing": True,
     }
 
-    # todo 2.3.0: remove pre_dispatch and n_jobs params
+    # todo 2.5.0: remove pre_dispatch and n_jobs params
     def __init__(
         self,
         estimator,
         cv,
         n_jobs=None,
         pre_dispatch=None,
         backend="loky",
@@ -113,26 +113,27 @@
         """
         cv = check_cv(self.cv)
 
         # scoring = check_scoring(self.scoring, obj=self)
         scoring = self.scoring
         scoring_name = f"test_{scoring.name}"
 
-        # todo 2.3.0: remove this logic and only use backend_params
+        # todo 2.5.0: remove this logic and only use backend_params
         backend = self.backend
         backend_params = self.backend_params if self.backend_params else {}
         if backend in ["threading", "multiprocessing", "loky"]:
             n_jobs = self.n_jobs
             pre_dispatch = self.pre_dispatch
             backend_params["n_jobs"] = n_jobs
             backend_params["pre_dispatch"] = pre_dispatch
             if n_jobs is not None or pre_dispatch is not None:
                 warn(
                     f"in {self.__class__.__name__}, n_jobs and pre_dispatch "
-                    "parameters are deprecated and will be removed in 2.3.0. "
+                    "parameters in skpro GridSearchCV and RandomizedSearchCV "
+                    "are deprecated and will be removed in skpro 2.5.0. "
                     "Please use n_jobs and pre_dispatch directly in the backend_params "
                     "argument instead.",
                     stacklevel=2,
                 )
 
         def _fit_and_score(params, meta):
             # Clone estimator.
@@ -251,14 +252,15 @@
                 f"In {self.__class__.__name__}, refit must be True to make predictions,"
                 f" but found refit=False. If refit=False, {self.__class__.__name__} can"
                 " be used only to tune hyper-parameters, as a parameter estimator."
             )
         return getattr(self, self._delegate_name)
 
 
+# todo 2.5.0: remove pre_dispatch and n_jobs params
 class GridSearchCV(BaseGridSearch):
     """Perform grid-search cross-validation to find optimal model parameters.
 
     The estimator is fit on the initial window and then temporal
     cross-validation is used to find the optimal parameter.
 
     Grid-search cross-validation is performed based on a cross-validation
@@ -417,26 +419,28 @@
         n_jobs=None,
         refit=True,
         verbose=0,
         return_n_best_estimators=1,
         pre_dispatch="2*n_jobs",
         backend="loky",
         error_score=np.nan,
+        backend_params=None,
     ):
         super().__init__(
             estimator=estimator,
             scoring=scoring,
             n_jobs=n_jobs,
             refit=refit,
             cv=cv,
             verbose=verbose,
             return_n_best_estimators=return_n_best_estimators,
             pre_dispatch=pre_dispatch,
             backend=backend,
             error_score=error_score,
+            backend_params=backend_params,
         )
         self.param_grid = param_grid
 
     def _check_param_grid(self, param_grid):
         """_check_param_grid from sklearn 1.0.2, before it was removed."""
         if hasattr(param_grid, "items"):
             param_grid = [param_grid]
@@ -518,14 +522,15 @@
                 "error_score": "raise",
             }
             params.append(param3)
 
         return params
 
 
+# todo 2.5.0: remove pre_dispatch and n_jobs params
 class RandomizedSearchCV(BaseGridSearch):
     """Perform randomized-search cross-validation to find optimal model parameters.
 
     The estimator is fit on the initial window and then
     cross-validation is used to find the optimal parameter
 
     Randomized cross-validation is performed based on a cross-validation
@@ -692,26 +697,28 @@
         refit=True,
         verbose=0,
         return_n_best_estimators=1,
         random_state=None,
         pre_dispatch="2*n_jobs",
         backend="loky",
         error_score=np.nan,
+        backend_params=None,
     ):
         super().__init__(
             estimator=estimator,
             scoring=scoring,
             n_jobs=n_jobs,
             refit=refit,
             cv=cv,
             verbose=verbose,
             return_n_best_estimators=return_n_best_estimators,
             pre_dispatch=pre_dispatch,
             backend=backend,
             error_score=error_score,
+            backend_params=backend_params,
         )
         self.param_distributions = param_distributions
         self.n_iter = n_iter
         self.random_state = random_state
 
     def _run_search(self, evaluate_candidates):
         """Search n_iter candidates from param_distributions."""
```

### Comparing `skpro-2.3.0/skpro/registry/_lookup.py` & `skpro-2.3.1/skpro/registry/_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,23 +118,23 @@
             passed in return_tags will serve as column names for all columns of
             tags that were optionally requested.
 
     Examples
     --------
     >>> from skpro.registry import all_objects
     >>> # return a complete list of objects as pd.Dataframe
-    >>> all_objects(as_dataframe=True)
+    >>> all_objects(as_dataframe=True)  # doctest: +SKIP
     >>> # return all probabilistic regressors by filtering for object type
-    >>> all_objects("regressor_proba", as_dataframe=True)
+    >>> all_objects("regressor_proba", as_dataframe=True)  # doctest: +SKIP
     >>> # return all regressors which handle missing data in the input by tag filtering
     >>> all_objects(
     ...     "regressor_proba",
     ...     filter_tags={"capability:missing": True},
     ...     as_dataframe=True
-    ... )
+    ... )  # doctest: +SKIP
 
     References
     ----------
     Adapted version of sktime's ``all_estimators``,
     which is an evolution of scikit-learn's ``all_estimators``
     """
     MODULES_TO_IGNORE = (
```

### Comparing `skpro-2.3.0/skpro/registry/_scitype.py` & `skpro-2.3.1/skpro/registry/_scitype.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/registry/_tags.py` & `skpro-2.3.1/skpro/registry/_tags.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/registry/tests/test_scitype.py` & `skpro-2.3.1/skpro/registry/tests/test_scitype.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/registry/tests/test_tags.py` & `skpro-2.3.1/skpro/registry/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/adapters/ngboost/_ngboost_proba.py` & `skpro-2.3.1/skpro/regression/adapters/ngboost/_ngboost_proba.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/adapters/sklearn/_sklearn_proba.py` & `skpro-2.3.1/skpro/regression/adapters/sklearn/_sklearn_proba.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/base/_base.py` & `skpro-2.3.1/skpro/regression/base/_base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/base/_delegate.py` & `skpro-2.3.1/skpro/regression/base/_delegate.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/base/adapters/_sklearn.py` & `skpro-2.3.1/skpro/regression/base/adapters/_sklearn.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/bootstrap.py` & `skpro-2.3.1/skpro/regression/linear/_sklearn_poisson.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,116 @@
-"""Probabilistic regression by bootstrap."""
+"""Adapters to sklearn linear regressors with probabilistic components."""
+# copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
+# based on sktime pipelines
 
-__author__ = ["fkiraly"]
-__all__ = ["BootstrapRegressor"]
-
-import numpy as np
 import pandas as pd
-from sklearn import clone
 
-from skpro.distributions.empirical import Empirical
 from skpro.regression.base import BaseProbaRegressor
-from skpro.utils.numpy import flatten_to_1D_if_colvector
 from skpro.utils.sklearn import prep_skl_df
 
 
-class BootstrapRegressor(BaseProbaRegressor):
-    """Bootstrap ensemble of a tabular regressor.
-
-    Fits ``n_estimators`` clones of an skpro regressor on
-    datasets which are bootstrap sub-samples, i.e.,
-    independent row samples with replacement.
-
-    On ``predict_proba``, an empirical distribution with the bootstrap
-    sample is returned.
-
-    The estimator allows to choose sample sizes for instances, variables,
-    and whether sampling is with or without replacement.
+class PoissonRegressor(BaseProbaRegressor):
+    """Poisson regression, direct adapter to sklearn PoissonRegressor.
 
-    Direct generalization of ``sklearn``'s ``BaggingClassifier``
-    to the probabilistic regression task.
+    Generalized Linear Model with a Poisson distribution.
+    This regressor uses the 'log' link function.
 
     Parameters
     ----------
-    estimator : sklearn regressor
-        regressor to use in the bootstrap
-    n_bootstrap_samples : int, default=100
-        The number of bootstrap samples drawn
-        If int, then indicates number of instances precisely
-        Note: this is not the same as the size of each bootstrap sample.
-        The size of the bootstrap sample is always equal to X.
-    random_state : int, RandomState instance or None, optional (default=None)
-        If int, ``random_state`` is the seed used by the random number generator;
-        If ``RandomState`` instance, ``random_state`` is the random number generator;
-        If None, the random number generator is the ``RandomState`` instance used
-        by ``np.random``.
+    alpha : float, default=1.0
+        Constant that multiplies the penalty term. Defaults to 1.0.
+        See the notes for the exact mathematical meaning of this
+        parameter. alpha = 0 is equivalent to unpenalized GLMs.
+
+    fit_intercept : bool, default=True
+        Whether to fit an intercept term.
+
+    solver : {'lbfgs', 'newton-cholesky'}, default='lbfgs'
+        Algorithm to use in the optimization problem.
+
+    'lbfgs' is an optimization algorithm that approximates the BFGS algorithm
+    'newton-cholesky' uses a Newton-CG variant of Newton's method.
+
+    max_iter : int, default=100
+        The maximal number of iterations for the solver.
+
+    tol : float, default=1e-4
+        The convergence tolerance. If it is not None, training will stop
+        when (loss > best_loss - tol) for n_iter_no_change consecutive
+        epochs.
+
+    verbose : int, default=0
+        For the 'sag' and 'lbfgs' solvers set verbose to any positive
+        number for verbosity.
+
+    warm_start : bool, default=False
+        When set to True, reuse the solution of the previous call to fit as
+        initialization, otherwise, just erase the previous solution.
 
     Attributes
     ----------
-    estimators_ : list of of skpro regressors
-        clones of regressor in `estimator` fitted in the ensemble
+    coef_ : array-like of shape (n_features,)
+        Coefficients of the regression model (mean of distribution)
 
-    Examples
-    --------
-    >>> from skpro.regression.bootstrap import BootstrapRegressor
-    >>> from sklearn.linear_model import LinearRegression
-    >>> from sklearn.datasets import load_diabetes
-    >>> from sklearn.model_selection import train_test_split
-    >>>
-    >>> X, y = load_diabetes(return_X_y=True, as_frame=True)
-    >>> X_train, X_test, y_train, y_test = train_test_split(X, y)
-    >>>
-    >>> reg_tabular = LinearRegression()
-    >>>
-    >>> reg_proba = BootstrapRegressor(reg_tabular)
-    >>> reg_proba.fit(X_train, y_train)
-    BootstrapRegressor(...)
-    >>> y_pred = reg_proba.predict_proba(X_test)
+    intercept_ : float
+        Independent term in decision function.
+
+    n_iter_ : int
+        The actual number of iterations before reaching the stopping criterion.
+
+    n_features_in_ : int
+        Number of features seen during :term:'fit'.
+
+    feature_names_in_ : ndarray of shape (n_features,)
+        Names of features seen during :term:'fit'.
     """
 
-    _tags = {"authors": "fkiraly", "capability:missing": True}
+    _tags = {
+        "capability:multioutput": False,
+        "capability:missing": False,
+        "X_inner_mtype": "pd_DataFrame_Table",
+        "y_inner_mtype": "pd_DataFrame_Table",
+    }
 
     def __init__(
         self,
-        estimator,
-        n_bootstrap_samples=100,
-        random_state=None,
+        alpha=1.0,
+        fit_intercept=True,
+        max_iter=100,
+        tol=1e-4,
+        verbose=0,
+        warm_start=False,
     ):
-        self.estimator = estimator
-        self.n_bootstrap_samples = n_bootstrap_samples
-        self.random_state = random_state
+        self.alpha = alpha
+        self.fit_intercept = fit_intercept
+        self.max_iter = max_iter
+        self.tol = tol
+        self.verbose = verbose
+        self.warm_start = warm_start
 
         super().__init__()
 
-        # todo: find the equivalent tag in sklearn for missing data handling
-        # tags_to_clone = ["capability:missing"]
-        # self.clone_tags(estimator, tags_to_clone)
+        from sklearn.linear_model import PoissonRegressor
+
+        skl_estimator = PoissonRegressor(
+            alpha=alpha,
+            fit_intercept=fit_intercept,
+            max_iter=max_iter,
+            tol=tol,
+            verbose=verbose,
+            warm_start=warm_start,
+        )
+
+        self.estimator_ = skl_estimator
+
+    FITTED_PARAMS_TO_FORWARD = [
+        "coef_",
+        "intercept_",
+        "n_iter_",
+    ]
 
     def _fit(self, X, y):
         """Fit regressor to training data.
 
         Writes to self:
             Sets fitted model attributes ending in "_".
 
@@ -98,80 +121,83 @@
         y : pandas DataFrame, must be same length as X
             labels to fit regressor to
 
         Returns
         -------
         self : reference to self
         """
-        estimator = self.estimator
-        n_bootstrap_samples = self.n_bootstrap_samples
-        np.random.seed(self.random_state)
+        X_inner = prep_skl_df(X).to_numpy()
+        y_inner = prep_skl_df(y).to_numpy()
 
-        inst_ix = X.index
-        n = len(inst_ix)
+        self._y_cols = y.columns
 
-        self.estimators_ = []
-        self._cols = y.columns
+        if len(y_inner.shape) > 1 and y_inner.shape[1] == 1:
+            y_inner = y_inner[:, 0]
 
-        # coerce X to pandas DataFrame with string column names
-        X = prep_skl_df(X, copy_df=True)
+        estimator = self.estimator_
+        estimator.fit(X=X_inner, y=y_inner)
 
-        for _i in range(n_bootstrap_samples):
-            esti = clone(estimator)
-            row_iloc = pd.RangeIndex(n)
-            row_ss = _random_ss_ix(row_iloc, size=n, replace=True)
-            inst_ix_i = inst_ix[row_ss]
-
-            Xi = X.loc[inst_ix_i]
-            Xi = Xi.reset_index(drop=True)
-
-            yi = y.loc[inst_ix_i].values
-            yi = flatten_to_1D_if_colvector(yi)
-
-            self.estimators_ += [esti.fit(Xi, yi)]
+        for attr in self.FITTED_PARAMS_TO_FORWARD:
+            setattr(self, attr, getattr(estimator, attr))
 
         return self
 
-    def _predict_proba(self, X) -> np.ndarray:
-        """Predict distribution over labels for data from features.
+    def _predict(self, X):
+        """Predict labels for data from features.
 
         State required:
-            Requires state to be "fitted".
+            Requires state to be "fitted" = self.is_fitted=True
 
         Accesses in self:
             Fitted model attributes ending in "_"
 
         Parameters
         ----------
         X : pandas DataFrame, must have same columns as X in `fit`
             data to predict labels for
 
         Returns
         -------
-        y : skpro BaseDistribution, same length as `X`
+        y : pandas DataFrame, same length as `X`, same columns as `y` in `fit`
             labels predicted for `X`
         """
-        cols = self._cols
+        X_inner = prep_skl_df(X).to_numpy()
+        y_pred = self.estimator_.predict(X_inner)
+        y_pred_df = pd.DataFrame(y_pred, index=X.index, columns=self._y_cols)
+        return y_pred_df
+
+    def _predict_var(self, X):
+        """Compute/return variance predictions."""
+        return self._predict(X)  # Poisson variance is equal to mean
 
-        # coerce X to pandas DataFrame with string column names
-        X = prep_skl_df(X, copy_df=True)
+    def _predict_proba(self, X):
+        """Predict distribution over labels for data from features.
 
-        y_preds = [est.predict(X) for est in self.estimators_]
+        State required:
+            Requires state to be "fitted".
 
-        def _coerce_df(x):
-            if not isinstance(x, pd.DataFrame):
-                x = pd.DataFrame(x, columns=cols, index=X.index)
-            return x
+        Accesses in self:
+            Fitted model attributes ending in "_"
 
-        y_preds = [_coerce_df(x) for x in y_preds]
+        Parameters
+        ----------
+        X : pandas DataFrame, must have same columns as X in `fit`
+            data to predict labels for
 
-        y_pred_df = pd.concat(y_preds, axis=0, keys=range(len(y_preds)))
+        Returns
+        -------
+        y_pred : skpro BaseDistribution, same length as `X`
+            labels predicted for `X`
+        """
+        from skpro.distributions.poisson import Poisson
 
-        y_proba = Empirical(y_pred_df)
-        return y_proba
+        y_cols = self._y_cols
+        y_pred = self.predict(X).values
+        y_pred_proba = Poisson(y_pred, index=X.index, columns=y_cols)
+        return y_pred_proba
 
     @classmethod
     def get_test_params(cls, parameter_set="default"):
         """Return testing parameter settings for the estimator.
 
         Parameters
         ----------
@@ -183,23 +209,17 @@
         -------
         params : dict or list of dict, default = {}
             Parameters to create testing instances of the class
             Each dict are parameters to construct an "interesting" test instance, i.e.,
             `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
             `create_test_instance` uses the first (or only) dictionary in `params`
         """
-        from sklearn.linear_model import LinearRegression
-
-        params1 = {"estimator": LinearRegression()}
-        params2 = {
-            "estimator": LinearRegression(),
-            "n_bootstrap_samples": 10,
+        param1 = {}
+        param2 = {
+            "alpha": 2.0,
+            "fit_intercept": False,
+            "max_iter": 200,
+            "tol": 2e-4,
+            "verbose": 1,
+            "warm_start": True,
         }
-
-        return [params1, params2]
-
-
-def _random_ss_ix(ix, size, replace=True):
-    """Randomly uniformly sample indices from a list of indices."""
-    a = range(len(ix))
-    ixs = ix[np.random.choice(a, size=size, replace=replace)]
-    return ixs
+        return [param1, param2]
```

### Comparing `skpro-2.3.0/skpro/regression/compose/_pipeline.py` & `skpro-2.3.1/skpro/regression/compose/_pipeline.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/cyclic_boosting.py` & `skpro-2.3.1/skpro/regression/cyclic_boosting.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/delta.py` & `skpro-2.3.1/skpro/regression/delta.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/density.py` & `skpro-2.3.1/skpro/regression/density.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/ensemble/_bagging.py` & `skpro-2.3.1/skpro/regression/ensemble/_bagging.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/ensemble/_ngboost.py` & `skpro-2.3.1/skpro/regression/ensemble/_ngboost.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/gp/_sklearn.py` & `skpro-2.3.1/skpro/regression/gp/_sklearn.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/linear/_glm.py` & `skpro-2.3.1/skpro/regression/linear/_glm.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/linear/_sklearn.py` & `skpro-2.3.1/skpro/regression/linear/_sklearn.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/linear/_sklearn_poisson.py` & `skpro-2.3.1/skpro/survival/compose/_reduce_cond_unc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,150 +1,91 @@
-"""Adapters to sklearn linear regressors with probabilistic components."""
-# copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
-# based on sktime pipelines
+"""Reducer to supervised regression - condition on uncensored."""
+
+__author__ = ["fkiraly"]
 
 import pandas as pd
 
 from skpro.regression.base import BaseProbaRegressor
-from skpro.utils.sklearn import prep_skl_df
 
 
-class PoissonRegressor(BaseProbaRegressor):
-    """Poisson regression, direct adapter to sklearn PoissonRegressor.
+class ConditionUncensored(BaseProbaRegressor):
+    """Reduction to tabular probabilistic regression - conditioning on uncensored.
+
+    Simple baseline reduction strategy for predictive survival analysis.
+
+    Fits a probabilistic regressor on X padded with censoring information C,
+    in predict applies the fitted regressor to X padded with 0 (non-censored).
 
-    Generalized Linear Model with a Poisson distribution.
-    This regressor uses the 'log' link function.
+    In ``fit``, passes column concat of ``X`` and ``C`` to ``regressor.fit``.
+
+    In ``predict_[method]``, calls ``regressor.predict_[method]``
+    on ``X`` with an additional ``C``-like column, padded with 0,
+    and returns the result.
 
     Parameters
     ----------
-    alpha : float, default=1.0
-        Constant that multiplies the penalty term. Defaults to 1.0.
-        See the notes for the exact mathematical meaning of this
-        parameter. alpha = 0 is equivalent to unpenalized GLMs.
-
-    fit_intercept : bool, default=True
-        Whether to fit an intercept term.
-
-    solver : {'lbfgs', 'newton-cholesky'}, default='lbfgs'
-        Algorithm to use in the optimization problem.
-
-    'lbfgs' is an optimization algorithm that approximates the BFGS algorithm
-    'newton-cholesky' uses a Newton-CG variant of Newton's method.
-
-    max_iter : int, default=100
-        The maximal number of iterations for the solver.
-
-    tol : float, default=1e-4
-        The convergence tolerance. If it is not None, training will stop
-        when (loss > best_loss - tol) for n_iter_no_change consecutive
-        epochs.
-
-    verbose : int, default=0
-        For the 'sag' and 'lbfgs' solvers set verbose to any positive
-        number for verbosity.
-
-    warm_start : bool, default=False
-        When set to True, reuse the solution of the previous call to fit as
-        initialization, otherwise, just erase the previous solution.
+    estimator : skpro regressor, BaseProbaRegressor descendant
+        probabilistic regressor to predict survival time from features
 
     Attributes
     ----------
-    coef_ : array-like of shape (n_features,)
-        Coefficients of the regression model (mean of distribution)
-
-    intercept_ : float
-        Independent term in decision function.
-
-    n_iter_ : int
-        The actual number of iterations before reaching the stopping criterion.
-
-    n_features_in_ : int
-        Number of features seen during :term:'fit'.
-
-    feature_names_in_ : ndarray of shape (n_features,)
-        Names of features seen during :term:'fit'.
+    estimator_ : skpro regressor, BaseProbaRegressor descendant
+        fitted probabilistic regressor, clone of ``regressor``
     """
 
-    _tags = {
-        "capability:multioutput": False,
-        "capability:missing": False,
-        "X_inner_mtype": "pd_DataFrame_Table",
-        "y_inner_mtype": "pd_DataFrame_Table",
-    }
-
-    def __init__(
-        self,
-        alpha=1.0,
-        fit_intercept=True,
-        max_iter=100,
-        tol=1e-4,
-        verbose=0,
-        warm_start=False,
-    ):
-        self.alpha = alpha
-        self.fit_intercept = fit_intercept
-        self.max_iter = max_iter
-        self.tol = tol
-        self.verbose = verbose
-        self.warm_start = warm_start
+    _tags = {"capability:survival": True}
 
-        super().__init__()
+    def __init__(self, estimator):
+        self.estimator = estimator
 
-        from sklearn.linear_model import PoissonRegressor
-
-        skl_estimator = PoissonRegressor(
-            alpha=alpha,
-            fit_intercept=fit_intercept,
-            max_iter=max_iter,
-            tol=tol,
-            verbose=verbose,
-            warm_start=warm_start,
-        )
-
-        self.estimator_ = skl_estimator
-
-    FITTED_PARAMS_TO_FORWARD = [
-        "coef_",
-        "intercept_",
-        "n_iter_",
-    ]
+        super().__init__()
 
-    def _fit(self, X, y):
+    def _fit(self, X, y, C=None):
         """Fit regressor to training data.
 
         Writes to self:
             Sets fitted model attributes ending in "_".
 
+        Changes state to "fitted" = sets is_fitted flag to True
+
         Parameters
         ----------
         X : pandas DataFrame
             feature instances to fit regressor to
-        y : pandas DataFrame, must be same length as X
+        y : pd.DataFrame, must be same length as X
             labels to fit regressor to
-
-        Returns
-        -------
-        self : reference to self
+        C : pd.DataFrame, optional (default=None)
+            censoring information for survival analysis,
+            should have same column name as y, same length as X and y
+            should have entries 0 and 1 (float or int)
+            0 = uncensored, 1 = (right) censored
+            if None, all observations are assumed to be uncensored
+            Can be passed to any probabilistic regressor,
+            but is ignored if capability:survival tag is False.
         """
-        X_inner = prep_skl_df(X).to_numpy()
-        y_inner = prep_skl_df(y).to_numpy()
-
         self._y_cols = y.columns
 
-        if len(y_inner.shape) > 1 and y_inner.shape[1] == 1:
-            y_inner = y_inner[:, 0]
-
-        estimator = self.estimator_
-        estimator.fit(X=X_inner, y=y_inner)
-
-        for attr in self.FITTED_PARAMS_TO_FORWARD:
-            setattr(self, attr, getattr(estimator, attr))
+        X_and_C = self._get_padded_X(X, C)
+        self.estimator_ = self.estimator.clone().fit(X_and_C, y)
 
         return self
 
+    def _get_padded_X(self, X, C=None):
+        """Get one-padded X to use in fit and predict methods."""
+        X = X.copy()
+        columns = self._y_cols
+        index = X.index
+
+        if C is None:
+            C = pd.DataFrame(0, index=index, columns=columns)
+        else:
+            C = C.copy().astype("float")
+        X_and_C = pd.concat([X, C], axis=1)
+        return X_and_C
+
     def _predict(self, X):
         """Predict labels for data from features.
 
         State required:
             Requires state to be "fitted" = self.is_fitted=True
 
         Accesses in self:
@@ -156,22 +97,17 @@
             data to predict labels for
 
         Returns
         -------
         y : pandas DataFrame, same length as `X`, same columns as `y` in `fit`
             labels predicted for `X`
         """
-        X_inner = prep_skl_df(X).to_numpy()
-        y_pred = self.estimator_.predict(X_inner)
-        y_pred_df = pd.DataFrame(y_pred, index=X.index, columns=self._y_cols)
-        return y_pred_df
-
-    def _predict_var(self, X):
-        """Compute/return variance predictions."""
-        return self._predict(X)  # Poisson variance is equal to mean
+        X_and_C = self._get_padded_X(X)
+        y_pred = self.estimator_.predict(X_and_C)
+        return y_pred
 
     def _predict_proba(self, X):
         """Predict distribution over labels for data from features.
 
         State required:
             Requires state to be "fitted".
 
@@ -184,20 +120,74 @@
             data to predict labels for
 
         Returns
         -------
         y_pred : skpro BaseDistribution, same length as `X`
             labels predicted for `X`
         """
-        from skpro.distributions.poisson import Poisson
+        X_and_C = self._get_padded_X(X)
+        y_pred = self.estimator_.predict_proba(X_and_C)
+        return y_pred
+
+    def _predict_interval(self, X, coverage):
+        """Compute/return interval predictions.
+
+        private _predict_interval containing the core logic,
+            called from predict_interval and default _predict_quantiles
+
+        Parameters
+        ----------
+        X : pandas DataFrame, must have same columns as X in `fit`
+            data to predict labels for
+        coverage : guaranteed list of float of unique values
+           nominal coverage(s) of predictive interval(s)
+
+        Returns
+        -------
+        pred_int : pd.DataFrame
+            Column has multi-index: first level is variable name from ``y`` in fit,
+            second level coverage fractions for which intervals were computed,
+            in the same order as in input `coverage`.
+            Third level is string "lower" or "upper", for lower/upper interval end.
+            Row index is equal to row index of ``X``.
+            Entries are lower/upper bounds of interval predictions,
+            for var in col index, at nominal coverage in second col index,
+            lower/upper depending on third col index, for the row index.
+            Upper/lower interval end are equivalent to
+            quantile predictions at alpha = 0.5 - c/2, 0.5 + c/2 for c in coverage.
+        """
+        X_and_C = self._get_padded_X(X)
+        y_pred = self.estimator_.predict_interval(X_and_C, coverage=coverage)
+        return y_pred
 
-        y_cols = self._y_cols
-        y_pred = self.predict(X).values
-        y_pred_proba = Poisson(y_pred, index=X.index, columns=y_cols)
-        return y_pred_proba
+    def _predict_quantiles(self, X, alpha):
+        """Compute/return quantile predictions.
+
+        private _predict_quantiles containing the core logic,
+            called from predict_quantiles and default _predict_interval
+
+        Parameters
+        ----------
+        X : pandas DataFrame, must have same columns as X in `fit`
+            data to predict labels for
+        alpha : guaranteed list of float
+            A list of probabilities at which quantile predictions are computed.
+
+        Returns
+        -------
+        quantiles : pd.DataFrame
+            Column has multi-index: first level is variable name from ``y`` in fit,
+                second level being the values of alpha passed to the function.
+            Row index is equal to row index of ``X``.
+            Entries are quantile predictions, for var in col index,
+                at quantile probability in second col index, for the row index.
+        """
+        X_and_C = self._get_padded_X(X)
+        y_pred = self.estimator_.predict_quantiles(X_and_C, alpha=alpha)
+        return y_pred
 
     @classmethod
     def get_test_params(cls, parameter_set="default"):
         """Return testing parameter settings for the estimator.
 
         Parameters
         ----------
@@ -209,17 +199,14 @@
         -------
         params : dict or list of dict, default = {}
             Parameters to create testing instances of the class
             Each dict are parameters to construct an "interesting" test instance, i.e.,
             `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
             `create_test_instance` uses the first (or only) dictionary in `params`
         """
-        param1 = {}
-        param2 = {
-            "alpha": 2.0,
-            "fit_intercept": False,
-            "max_iter": 200,
-            "tol": 2e-4,
-            "verbose": 1,
-            "warm_start": True,
-        }
+        from skpro.regression.bootstrap import BootstrapRegressor
+        from skpro.regression.residual import ResidualDouble
+
+        param1 = {"estimator": ResidualDouble.create_test_instance()}
+        param2 = {"estimator": BootstrapRegressor.create_test_instance()}
+
         return [param1, param2]
```

### Comparing `skpro-2.3.0/skpro/regression/mapie.py` & `skpro-2.3.1/skpro/regression/mapie.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/multiquantile.py` & `skpro-2.3.1/skpro/regression/multiquantile.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/parametric/estimators.py` & `skpro-2.3.1/skpro/regression/parametric/estimators.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/residual.py` & `skpro-2.3.1/skpro/regression/residual.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/tests/test_all_regressors.py` & `skpro-2.3.1/skpro/regression/tests/test_all_regressors.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/regression/tests/test_cyclic_boosting.py` & `skpro-2.3.1/skpro/regression/tests/test_cyclic_boosting.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/survival/adapters/_common.py` & `skpro-2.3.1/skpro/survival/adapters/_common.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/survival/adapters/lifelines.py` & `skpro-2.3.1/skpro/survival/adapters/lifelines.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/survival/adapters/sksurv.py` & `skpro-2.3.1/skpro/survival/adapters/sksurv.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/survival/additive/_aalen_lifelines.py` & `skpro-2.3.1/skpro/survival/additive/_aalen_lifelines.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/survival/aft/_aft_lifelines_fisk.py` & `skpro-2.3.1/skpro/survival/aft/_aft_lifelines_fisk.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/survival/aft/_aft_lifelines_lognormal.py` & `skpro-2.3.1/skpro/survival/aft/_aft_lifelines_lognormal.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/survival/aft/_aft_lifelines_weibull.py` & `skpro-2.3.1/skpro/survival/aft/_aft_lifelines_weibull.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/survival/base.py` & `skpro-2.3.1/skpro/survival/base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/survival/compose/_reduce_cond_unc.py` & `skpro-2.3.1/skpro/survival/ensemble/_ngboost_surv.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,98 @@
-"""Reducer to supervised regression - condition on uncensored."""
+"""class for NGBoost probabilistic survival regression."""
+# copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
 
-__author__ = ["fkiraly"]
+__author__ = ["ShreeshaM07"]
 
-import pandas as pd
+import numpy as np
 
-from skpro.regression.base import BaseProbaRegressor
+from skpro.regression.adapters.ngboost._ngboost_proba import NGBoostAdapter
+from skpro.survival.base import BaseSurvReg
 
 
-class ConditionUncensored(BaseProbaRegressor):
-    """Reduction to tabular probabilistic regression - conditioning on uncensored.
+class NGBoostSurvival(BaseSurvReg, NGBoostAdapter):
+    """Interface of NGBSurvival of ngboost in skpro.
 
-    Simple baseline reduction strategy for predictive survival analysis.
-
-    Fits a probabilistic regressor on X padded with censoring information C,
-    in predict applies the fitted regressor to X padded with 0 (non-censored).
-
-    In ``fit``, passes column concat of ``X`` and ``C`` to ``regressor.fit``.
-
-    In ``predict_[method]``, calls ``regressor.predict_[method]``
-    on ``X`` with an additional ``C``-like column, padded with 0,
-    and returns the result.
+    NGBSurvival is a wrapper for the generic NGBoost class that
+    facilitates survival analysis.
+    Use this class if you want to predict an outcome that
+    could take an infinite number of
+    (ordered) values, but right-censoring is present in the observed data.
 
     Parameters
     ----------
-    estimator : skpro regressor, BaseProbaRegressor descendant
-        probabilistic regressor to predict survival time from features
-
-    Attributes
-    ----------
-    estimator_ : skpro regressor, BaseProbaRegressor descendant
-        fitted probabilistic regressor, clone of ``regressor``
+    dist : string , default = "LogNormal"
+        assumed distributional form of Y|X=x.
+        A distribution from ngboost.distns, e.g. LogNormal
+        Available distribution types
+        1. "LogNormal"
+        2. "Exponential"
+    score : string , default = "LogScore"
+        rule to compare probabilistic predictions P̂ to the observed data y.
+        A score from ngboost.scores, e.g. LogScore
+    estimator : default learner/estimator: DecisionTreeRegressor()
+        base learner to use in the boosting algorithm.
+        Any instantiated sklearn regressor.
+    natural_gradient : boolean , default = True
+        whether natural gradient must be used or not.
+    n_estimators : int , default = 500
+        the number of boosting iterations to fit
+    learning_rate : float , default = 0.01
+        the learning rate
+    minibatch_frac : float, default = 1.0
+        the percent subsample of rows to
+        use in each boosting iteration
+    verbose : boolean, default=True
+        flag indicating whether output
+        should be printed during fitting
+    verbose_eval : int ,default=100
+        increment (in boosting iterations) at
+        which output should be printed
+    tol : float, default = 1e-4
+        numerical tolerance to be used in optimization
+    random_state : int, RandomState instance or None, optional (default=None)
+
+    Returns
+    -------
+        An NGBSurvival object that can be fit.
     """
 
-    _tags = {"capability:survival": True}
-
-    def __init__(self, estimator):
+    _tags = {
+        "authors": ["ShreeshaM07"],
+        "maintainers": ["ShreeshaM07"],
+        "python_dependencies": "ngboost",
+    }
+
+    def __init__(
+        self,
+        dist="LogNormal",
+        score="LogScore",
+        estimator=None,
+        natural_gradient=True,
+        n_estimators=500,
+        learning_rate=0.01,
+        minibatch_frac=1.0,
+        col_sample=1.0,
+        verbose=True,
+        verbose_eval=100,
+        tol=1e-4,
+        random_state=None,
+    ):
+        self.dist = dist
+        self.score = score
         self.estimator = estimator
+        self.natural_gradient = natural_gradient
+        self.n_estimators = n_estimators
+        self.learning_rate = learning_rate
+        self.minibatch_frac = minibatch_frac
+        self.col_sample = col_sample
+        self.verbose = verbose
+        self.verbose_eval = verbose_eval
+        self.tol = tol
+        self.random_state = random_state
 
         super().__init__()
 
     def _fit(self, X, y, C=None):
         """Fit regressor to training data.
 
         Writes to self:
@@ -55,36 +108,82 @@
             labels to fit regressor to
         C : pd.DataFrame, optional (default=None)
             censoring information for survival analysis,
             should have same column name as y, same length as X and y
             should have entries 0 and 1 (float or int)
             0 = uncensored, 1 = (right) censored
             if None, all observations are assumed to be uncensored
-            Can be passed to any probabilistic regressor,
-            but is ignored if capability:survival tag is False.
+
+        Returns
+        -------
+        self : reference to self
         """
-        self._y_cols = y.columns
+        import pandas as pd
+        from ngboost import NGBSurvival
+        from ngboost.scores import LogScore
+        from sklearn.tree import DecisionTreeRegressor
+
+        # skpro => 0 = uncensored, 1 = (right) censored
+        # ngboost => 1 = uncensored, else (right) censored
+        # If C is None then C is set as 1s (uncensored)
+        # else it is converted from skpro to ngboost format
+        # by doing C = 1-C
+        if C is None:
+            C = pd.DataFrame(np.ones(len(y)), index=y.index, columns=y.columns)
+        else:
+            C = 1 - C
 
-        X_and_C = self._get_padded_X(X, C)
-        self.estimator_ = self.estimator.clone().fit(X_and_C, y)
+        # coerce y to numpy array
+        y = self._check_y(y=y)
+        y = y[0]
+        # remember y columns to predict_proba
+        self._y_cols = y.columns
+        y = y.values.ravel()
 
-        return self
+        if self.estimator is None:
+            self.estimator_ = DecisionTreeRegressor(
+                criterion="friedman_mse",
+                min_samples_split=2,
+                min_samples_leaf=1,
+                min_weight_fraction_leaf=0.0,
+                max_depth=3,
+                splitter="best",
+                random_state=None,
+            )
+
+        dist_ngboost = self._dist_to_ngboost_instance(self.dist, survival=True)
+
+        # Score argument for NGBSurvival
+        ngboost_score = {
+            "LogScore": LogScore,
+        }
+        score = None
+        if self.score in ngboost_score:
+            score = ngboost_score[self.score]
+
+        self.ngbsurv_ = NGBSurvival(
+            Dist=dist_ngboost,
+            Score=score,
+            Base=self.estimator_,
+            natural_gradient=True,
+            n_estimators=self.n_estimators,
+            learning_rate=self.learning_rate,
+            minibatch_frac=self.minibatch_frac,
+            col_sample=self.col_sample,
+            verbose=self.verbose,
+            verbose_eval=self.verbose_eval,
+            tol=self.tol,
+            random_state=self.random_state,
+        )
 
-    def _get_padded_X(self, X, C=None):
-        """Get one-padded X to use in fit and predict methods."""
-        X = X.copy()
-        columns = self._y_cols
-        index = X.index
+        # from sklearn.base import clone
 
-        if C is None:
-            C = pd.DataFrame(0, index=index, columns=columns)
-        else:
-            C = C.copy().astype("float")
-        X_and_C = pd.concat([X, C], axis=1)
-        return X_and_C
+        # self.ngbsurv_ = clone(self.ngbsurv)
+        self.ngbsurv_.fit(X, y, C)
+        return self
 
     def _predict(self, X):
         """Predict labels for data from features.
 
         State required:
             Requires state to be "fitted" = self.is_fitted=True
 
@@ -97,17 +196,21 @@
             data to predict labels for
 
         Returns
         -------
         y : pandas DataFrame, same length as `X`, same columns as `y` in `fit`
             labels predicted for `X`
         """
-        X_and_C = self._get_padded_X(X)
-        y_pred = self.estimator_.predict(X_and_C)
-        return y_pred
+        import pandas as pd
+
+        df = pd.DataFrame(self.ngbsurv_.predict(X), index=X.index, columns=self._y_cols)
+        return df
+
+    def _pred_dist(self, X):
+        return self.ngbsurv_.pred_dist(X)
 
     def _predict_proba(self, X):
         """Predict distribution over labels for data from features.
 
         State required:
             Requires state to be "fitted".
 
@@ -117,77 +220,31 @@
         Parameters
         ----------
         X : pandas DataFrame, must have same columns as X in `fit`
             data to predict labels for
 
         Returns
         -------
-        y_pred : skpro BaseDistribution, same length as `X`
+        y : skpro BaseDistribution, same length as `X`
             labels predicted for `X`
         """
-        X_and_C = self._get_padded_X(X)
-        y_pred = self.estimator_.predict_proba(X_and_C)
-        return y_pred
+        X = self._check_X(X)
 
-    def _predict_interval(self, X, coverage):
-        """Compute/return interval predictions.
-
-        private _predict_interval containing the core logic,
-            called from predict_interval and default _predict_quantiles
-
-        Parameters
-        ----------
-        X : pandas DataFrame, must have same columns as X in `fit`
-            data to predict labels for
-        coverage : guaranteed list of float of unique values
-           nominal coverage(s) of predictive interval(s)
-
-        Returns
-        -------
-        pred_int : pd.DataFrame
-            Column has multi-index: first level is variable name from ``y`` in fit,
-            second level coverage fractions for which intervals were computed,
-            in the same order as in input `coverage`.
-            Third level is string "lower" or "upper", for lower/upper interval end.
-            Row index is equal to row index of ``X``.
-            Entries are lower/upper bounds of interval predictions,
-            for var in col index, at nominal coverage in second col index,
-            lower/upper depending on third col index, for the row index.
-            Upper/lower interval end are equivalent to
-            quantile predictions at alpha = 0.5 - c/2, 0.5 + c/2 for c in coverage.
-        """
-        X_and_C = self._get_padded_X(X)
-        y_pred = self.estimator_.predict_interval(X_and_C, coverage=coverage)
-        return y_pred
-
-    def _predict_quantiles(self, X, alpha):
-        """Compute/return quantile predictions.
+        kwargs = {}
+        pred_dist = self._pred_dist(X)
+        index = X.index
+        columns = self._y_cols
 
-        private _predict_quantiles containing the core logic,
-            called from predict_quantiles and default _predict_interval
+        # Convert NGBoost Distribution return params into a dict
+        kwargs = self._ngb_skpro_dist_params(pred_dist, index, columns, **kwargs)
 
-        Parameters
-        ----------
-        X : pandas DataFrame, must have same columns as X in `fit`
-            data to predict labels for
-        alpha : guaranteed list of float
-            A list of probabilities at which quantile predictions are computed.
+        # Convert NGBoost Distribution to skpro BaseDistribution
+        pred_dist = self._ngb_dist_to_skpro(**kwargs)
 
-        Returns
-        -------
-        quantiles : pd.DataFrame
-            Column has multi-index: first level is variable name from ``y`` in fit,
-                second level being the values of alpha passed to the function.
-            Row index is equal to row index of ``X``.
-            Entries are quantile predictions, for var in col index,
-                at quantile probability in second col index, for the row index.
-        """
-        X_and_C = self._get_padded_X(X)
-        y_pred = self.estimator_.predict_quantiles(X_and_C, alpha=alpha)
-        return y_pred
+        return pred_dist
 
     @classmethod
     def get_test_params(cls, parameter_set="default"):
         """Return testing parameter settings for the estimator.
 
         Parameters
         ----------
@@ -199,14 +256,22 @@
         -------
         params : dict or list of dict, default = {}
             Parameters to create testing instances of the class
             Each dict are parameters to construct an "interesting" test instance, i.e.,
             `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
             `create_test_instance` uses the first (or only) dictionary in `params`
         """
-        from skpro.regression.bootstrap import BootstrapRegressor
-        from skpro.regression.residual import ResidualDouble
-
-        param1 = {"estimator": ResidualDouble.create_test_instance()}
-        param2 = {"estimator": BootstrapRegressor.create_test_instance()}
+        params1 = {}
+        params2 = {
+            "dist": "LogNormal",
+            "learning_rate": 0.001,
+        }
+        params3 = {
+            "n_estimators": 800,
+            "minibatch_frac": 0.8,
+        }
+        params4 = {
+            "dist": "Exponential",
+            "n_estimators": 600,
+        }
 
-        return [param1, param2]
+        return [params1, params2, params3, params4]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `skpro-2.3.0/skpro/survival/compose/_reduce_uncensored.py` & `skpro-2.3.1/skpro/survival/compose/_reduce_uncensored.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/survival/coxph/_coxnet_sksurv.py` & `skpro-2.3.1/skpro/survival/coxph/_coxnet_sksurv.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/survival/coxph/_coxph_lifelines.py` & `skpro-2.3.1/skpro/survival/coxph/_coxph_lifelines.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/survival/coxph/_coxph_sksurv.py` & `skpro-2.3.1/skpro/survival/coxph/_coxph_sksurv.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/survival/coxph/_coxph_statsmodels.py` & `skpro-2.3.1/skpro/survival/coxph/_coxph_statsmodels.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/survival/ensemble/_grad_boost_sksurv.py` & `skpro-2.3.1/skpro/survival/ensemble/_grad_boost_sksurv.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/survival/ensemble/_survforest_sksurv.py` & `skpro-2.3.1/skpro/survival/ensemble/_survforest_sksurv.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/survival/tree/_tree_sksurv.py` & `skpro-2.3.1/skpro/survival/tree/_tree_sksurv.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/tests/scenarios/scenarios.py` & `skpro-2.3.1/skpro/tests/scenarios/scenarios.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/tests/scenarios/scenarios_getter.py` & `skpro-2.3.1/skpro/tests/scenarios/scenarios_getter.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/tests/scenarios/scenarios_regressor_proba.py` & `skpro-2.3.1/skpro/tests/scenarios/scenarios_regressor_proba.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/tests/test_all_estimators.py` & `skpro-2.3.1/skpro/tests/test_all_estimators.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/tests/test_class_register.py` & `skpro-2.3.1/skpro/tests/test_class_register.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/tests/test_density.py` & `skpro-2.3.1/skpro/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/tests/test_ensemble.py` & `skpro-2.3.1/skpro/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/tests/test_switch.py` & `skpro-2.3.1/skpro/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/tests/tests/test_test_utils.py` & `skpro-2.3.1/skpro/tests/tests/test_test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,20 +73,20 @@
     elif run_nodep:
         # otherwise, if we run, it must be due to changes in class or pyproject
         assert reason_nodep in POS_REASONS
     else:  # not run and only changed modules
         assert reason_nodep == "False_no_change"
 
     # now check estimator with soft deps
-    run_nodep = run_test_for_class(f_with_deps)
+    run_wdep = run_test_for_class(f_with_deps)
     assert isinstance(run, bool)
 
     dep_present = _check_estimator_deps(f_with_deps, severity="none")
     if not dep_present:
-        assert not run_nodep
+        assert not run_wdep
 
     res = run_test_for_class(f_with_deps, return_reason=True)
     assert isinstance(res, tuple)
     assert len(res) == 2
     run_wdep, reason_wdep = res
 
     if not dep_present:
```

### Comparing `skpro-2.3.0/skpro/tests/utils.py` & `skpro-2.3.1/skpro/tests/utils.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/utils/_maint/_show_versions.py` & `skpro-2.3.1/skpro/utils/_maint/_show_versions.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/utils/_maint/tests/test_show_versions.py` & `skpro-2.3.1/skpro/utils/_maint/tests/test_show_versions.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/utils/deep_equals/_deep_equals.py` & `skpro-2.3.1/skpro/utils/deep_equals/_deep_equals.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/utils/estimator_checks.py` & `skpro-2.3.1/skpro/utils/estimator_checks.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/utils/git_diff.py` & `skpro-2.3.1/skpro/utils/git_diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,22 +122,35 @@
 
         return changed_lines
 
     except subprocess.CalledProcessError:
         return []
 
 
-@lru_cache
 def get_packages_with_changed_specs():
     """Get packages with changed or added specs.
 
     Returns
     -------
     list of str : names of packages with changed or added specs
     """
+    return list(_get_packages_with_changed_specs())
+
+
+@lru_cache
+def _get_packages_with_changed_specs():
+    """Get packages with changed or added specs.
+
+    Private version of get_packages_with_changed_specs,
+    to avoid side effects on the list return.
+
+    Returns
+    -------
+    tuple of str : names of packages with changed or added specs
+    """
     from packaging.requirements import Requirement
 
     changed_lines = get_changed_lines("pyproject.toml")
 
     packages = []
     for line in changed_lines:
         if line.find("'") > line.find('"') and line.find('"') != -1:
@@ -157,10 +170,10 @@
         if ";" in req:
             req = req.split(";")[0]
 
         pkg = Requirement(req).name
         packages.append(pkg)
 
     # make unique
-    packages = list(set(packages))
+    packages = tuple(set(packages))
 
     return packages
```

### Comparing `skpro-2.3.0/skpro/utils/index.py` & `skpro-2.3.1/skpro/utils/index.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/utils/numpy.py` & `skpro-2.3.1/skpro/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/utils/pandas.py` & `skpro-2.3.1/skpro/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/utils/parallel.py` & `skpro-2.3.1/skpro/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/utils/plotting.py` & `skpro-2.3.1/skpro/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/utils/random_state.py` & `skpro-2.3.1/skpro/utils/random_state.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/utils/sklearn.py` & `skpro-2.3.1/skpro/utils/sklearn.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/utils/tests/test_plots.py` & `skpro-2.3.1/skpro/utils/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/utils/utils.py` & `skpro-2.3.1/skpro/utils/utils.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/utils/validation/_dependencies.py` & `skpro-2.3.1/skpro/utils/validation/_dependencies.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/workflow/base.py` & `skpro-2.3.1/skpro/workflow/base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/workflow/cross_validation.py` & `skpro-2.3.1/skpro/workflow/cross_validation.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/workflow/manager/data.py` & `skpro-2.3.1/skpro/workflow/manager/data.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/workflow/manager/models.py` & `skpro-2.3.1/skpro/workflow/manager/models.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/workflow/table/table.py` & `skpro-2.3.1/skpro/workflow/table/table.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro/workflow/utils.py` & `skpro-2.3.1/skpro/workflow/utils.py`

 * *Files identical despite different names*

### Comparing `skpro-2.3.0/skpro.egg-info/PKG-INFO` & `skpro-2.3.1/skpro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skpro
-Version: 2.3.0
+Version: 2.3.1
 Summary: A unified framework for probability distributions and probabilistic supervised regression
 Author: Franz Király, Frithjof Gressmann, Vitaly Davydov
 Author-email: skpro developers <sktime.toolbox@gmail.com>
 Maintainer: Franz Király, Frithjof Gressmann
 Maintainer-email: skpro developers <sktime.toolbox@gmail.com>
 Project-URL: Homepage, https://github.com/sktime/skpro
 Project-URL: Repository, https://github.com/sktime/skpro
@@ -31,16 +31,16 @@
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 Requires-Dist: numpy<1.27,>=1.21.0
 Requires-Dist: pandas<2.3.0,>=1.1.0
 Requires-Dist: packaging
-Requires-Dist: scikit-base<0.8.0,>=0.6.1
-Requires-Dist: scikit-learn<1.5.0,>=0.24.0
+Requires-Dist: scikit-base<0.9.0,>=0.6.1
+Requires-Dist: scikit-learn<1.6.0,>=0.24.0
 Requires-Dist: scipy<2.0.0,>=1.2.0
 Provides-Extra: all-extras
 Requires-Dist: attrs; extra == "all-extras"
 Requires-Dist: cyclic-boosting>=1.4.0; python_version < "3.12" and extra == "all-extras"
 Requires-Dist: distfit; extra == "all-extras"
 Requires-Dist: lifelines<0.29.0; extra == "all-extras"
 Requires-Dist: mapie; extra == "all-extras"
@@ -67,23 +67,23 @@
 Provides-Extra: docs
 Requires-Dist: jupyter; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: nbsphinx>=0.8.6; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Requires-Dist: sphinx!=7.2.0,<8.0.0; extra == "docs"
-Requires-Dist: sphinx-design<0.6.0; extra == "docs"
+Requires-Dist: sphinx-design<0.7.0; extra == "docs"
 Requires-Dist: sphinx-issues<5.0.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.17.0; extra == "docs"
 Requires-Dist: sphinx-panels; extra == "docs"
 Requires-Dist: tabulate; extra == "docs"
 
 <a href="https://skpro.readthedocs.io/en/latest"><img src="https://github.com/sktime/skpro/blob/main/docs/source/images/skpro-banner.png" width="500" align="right" /></a>
 
-:rocket: **Version 2.3.0 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
+:rocket: **Version 2.3.1 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
 
 `skpro` is a library for supervised probabilistic prediction in python.
 It provides `scikit-learn`-like, `scikit-base` compatible interfaces to:
 
 * tabular **supervised regressors for probabilistic prediction** - interval, quantile and distribution predictions
 * tabular **probabilistic time-to-event and survival prediction** - instance-individual survival distributions
 * **metrics to evaluate probabilistic predictions**, e.g., pinball loss, empirical coverage, CRPS, survival losses
@@ -94,15 +94,15 @@
 | Overview | |
 |---|---|
 | **Open Source** |  [![BSD 3-clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/sktime/sktime/blob/main/LICENSE) |
 | **Tutorials** | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sktime/skpro/main?filepath=examples) [![!youtube](https://img.shields.io/static/v1?logo=youtube&label=YouTube&message=tutorials&color=red)](https://www.youtube.com/playlist?list=PLKs3UgGjlWHqNzu0LEOeLKvnjvvest2d0) |
 | **Community** | [![!discord](https://img.shields.io/static/v1?logo=discord&label=discord&message=chat&color=lightgreen)](https://discord.com/invite/54ACzaFsn7) [![!slack](https://img.shields.io/static/v1?logo=linkedin&label=LinkedIn&message=news&color=lightblue)](https://www.linkedin.com/company/scikit-time/) |
 | **CI/CD** | [![github-actions](https://img.shields.io/github/actions/workflow/status/sktime/sktime/wheels.yml?logo=github)](https://github.com/sktime/skpro/actions/workflows/wheels.yml) [![!codecov](https://img.shields.io/codecov/c/github/sktime/skpro?label=codecov&logo=codecov)](https://codecov.io/gh/sktime/skpro) [![readthedocs](https://img.shields.io/readthedocs/skpro?logo=readthedocs)](https://skpro.readthedocs.io/en/latest/) [![platform](https://img.shields.io/conda/pn/conda-forge/skpro)](https://github.com/sktime/skpro) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/skpro?color=orange)](https://pypi.org/project/skpro/) [![!conda](https://img.shields.io/conda/vn/conda-forge/skpro)](https://anaconda.org/conda-forge/skpro) [![!python-versions](https://img.shields.io/pypi/pyversions/skpro)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
-| **Downloads** | [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skpro) |
+| **Downloads** | ![PyPI - Downloads](https://img.shields.io/pypi/dw/skpro) ![PyPI - Downloads](https://img.shields.io/pypi/dm/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skpro) |
 | **Citation** | [![DOI](https://zenodo.org/badge/103107372.svg)](https://zenodo.org/doi/10.5281/zenodo.11002671) |
 
 ## :books: Documentation
 
 | Documentation              |                                                                |
 | -------------------------- | -------------------------------------------------------------- |
 | :star: **[Tutorials]**        | New to skpro? Here's everything you need to know!              |
@@ -162,15 +162,15 @@
 [cyclic-boosting]:  https://cyclic-boosting.readthedocs.io/en/latest/
 
 ``skpro`` curates libraries of components of the following types:
 
 | Module | Status | Links |
 |---|---|---|
 | **[Probabilistic tabular regression]** | maturing | [Tutorial](https://github.com/sktime/skpro/blob/main/examples/01_skpro_intro.ipynb) · [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/regression.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/regression.py) |
-| **[Time-to-event (survival) prediction]** | experimental | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/survival.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/survival.py) |
+| **[Time-to-event (survival) prediction]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/survival.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/survival.py) |
 | **[Performance metrics]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/metrics.html) |
 | **[Probability distributions]** | maturing | [Tutorial](https://github.com/sktime/skpro/blob/main/examples/03_skpro_distributions.ipynb) · [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/distributions.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/distributions.py) |
 
 [Probabilistic tabular regression]: https://github.com/sktime/skpro/tree/main/skpro/regression
 [Time-to-event (survival) prediction]: https://github.com/sktime/skpro/tree/main/skpro/survival
 [Performance metrics]: https://github.com/sktime/skpro/tree/main/skpro/metrics
 [Probability distributions]: https://github.com/sktime/skpro/tree/main/skpro/distributions
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skpro Version: 2.3.0 Summary: A unified framework
+Metadata-Version: 2.1 Name: skpro Version: 2.3.1 Summary: A unified framework
 for probability distributions and probabilistic supervised regression Author:
 Franz KirÃ¡ly, Frithjof Gressmann, Vitaly Davydov Author-email: skpro
 developers
 gmail.com> Maintainer: Franz KirÃ¡ly, Frithjof Gressmann Maintainer-email:
 skpro developers
 gmail.com> Project-URL: Homepage, https://github.com/sktime/skpro Project-URL:
 Repository, https://github.com/sktime/skpro Project-URL: Documentation, https:/
@@ -18,15 +18,15 @@
 Classifier: Operating System :: MacOS Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Python: <3.13,>=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.txt License-File: AUTHORS.rst Requires-Dist: numpy<1.27,>=1.21.0
 Requires-Dist: pandas<2.3.0,>=1.1.0 Requires-Dist: packaging Requires-Dist:
-scikit-base<0.8.0,>=0.6.1 Requires-Dist: scikit-learn<1.5.0,>=0.24.0 Requires-
+scikit-base<0.9.0,>=0.6.1 Requires-Dist: scikit-learn<1.6.0,>=0.24.0 Requires-
 Dist: scipy<2.0.0,>=1.2.0 Provides-Extra: all-extras Requires-Dist: attrs;
 extra == "all-extras" Requires-Dist: cyclic-boosting>=1.4.0; python_version <
 "3.12" and extra == "all-extras" Requires-Dist: distfit; extra == "all-extras"
 Requires-Dist: lifelines<0.29.0; extra == "all-extras" Requires-Dist: mapie;
 extra == "all-extras" Requires-Dist: matplotlib>=3.3.2; extra == "all-extras"
 Requires-Dist: ngboost<0.6.0; extra == "all-extras" Requires-Dist:
 polars<0.21.0; extra == "all-extras" Requires-Dist: pyarrow<14.0.0;
@@ -39,19 +39,19 @@
 pytest-cov; extra == "dev" Requires-Dist: pytest-randomly; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev" Requires-Dist: pytest-xdist;
 extra == "dev" Requires-Dist: wheel; extra == "dev" Provides-Extra: binder
 Requires-Dist: jupyter; extra == "binder" Provides-Extra: docs Requires-Dist:
 jupyter; extra == "docs" Requires-Dist: myst-parser; extra == "docs" Requires-
 Dist: nbsphinx>=0.8.6; extra == "docs" Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs" Requires-Dist:
-sphinx!=7.2.0,<8.0.0; extra == "docs" Requires-Dist: sphinx-design<0.6.0; extra
+sphinx!=7.2.0,<8.0.0; extra == "docs" Requires-Dist: sphinx-design<0.7.0; extra
 == "docs" Requires-Dist: sphinx-issues<5.0.0; extra == "docs" Requires-Dist:
 sphinx-gallery<0.17.0; extra == "docs" Requires-Dist: sphinx-panels; extra ==
 "docs" Requires-Dist: tabulate; extra == "docs" _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_k_t_i_m_e_/
-_s_k_p_r_o_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_p_r_o_-_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.3.0
+_s_k_p_r_o_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_p_r_o_-_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.3.1
 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/
 latest/changelog.html). `skpro` is a library for supervised probabilistic
 prediction in python. It provides `scikit-learn`-like, `scikit-base` compatible
 interfaces to: * tabular **supervised regressors for probabilistic prediction**
 - interval, quantile and distribution predictions * tabular **probabilistic
 time-to-event and survival prediction** - instance-individual survival
 distributions * **metrics to evaluate probabilistic predictions**, e.g.,
@@ -80,22 +80,17 @@
 (https://skpro.readthedocs.io/en/latest/) [![platform](https://img.shields.io/
 conda/pn/conda-forge/skpro)](https://github.com/sktime/skpro) | | **Code** | [!
 [!pypi](https://img.shields.io/pypi/v/skpro?color=orange)](https://pypi.org/
 project/skpro/) [![!conda](https://img.shields.io/conda/vn/conda-forge/skpro)]
 (https://anaconda.org/conda-forge/skpro) [![!python-versions](https://
 img.shields.io/pypi/pyversions/skpro)](https://www.python.org/) [![!black]
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
-github.com/psf/black) | | **Downloads** | [![Downloads](https://
-static.pepy.tech/personalized-badge/
-skpro?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20
-(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
-static.pepy.tech/personalized-badge/
-skpro?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20
-(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
-static.pepy.tech/personalized-badge/
+github.com/psf/black) | | **Downloads** | ![PyPI - Downloads](https://
+img.shields.io/pypi/dw/skpro) ![PyPI - Downloads](https://img.shields.io/pypi/
+dm/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/
 skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20
 (pypi))](https://pepy.tech/project/skpro) | | **Citation** | [![DOI](https://
 zenodo.org/badge/103107372.svg)](https://zenodo.org/doi/10.5281/
 zenodo.11002671) | ## :books: Documentation | Documentation | | | -------------
 ------------- | -------------------------------------------------------------
 - | | :star: **[Tutorials]** | New to skpro? Here's everything you need to
 know! | | :clipboard: **[Binder Notebooks]** | Example notebooks to play with
@@ -140,15 +135,15 @@
 boosting.readthedocs.io/en/latest/ ``skpro`` curates libraries of components of
 the following types: | Module | Status | Links | |---|---|---| | **
 [Probabilistic tabular regression]** | maturing | [Tutorial](https://
 github.com/sktime/skpro/blob/main/examples/01_skpro_intro.ipynb) Â· [API
 Reference](https://skpro.readthedocs.io/en/latest/api_reference/
 regression.html) Â· [Extension Template](https://github.com/sktime/skpro/blob/
 main/extension_templates/regression.py) | | **[Time-to-event (survival)
-prediction]** | experimental | [API Reference](https://skpro.readthedocs.io/en/
+prediction]** | maturing | [API Reference](https://skpro.readthedocs.io/en/
 latest/api_reference/survival.html) Â· [Extension Template](https://github.com/
 sktime/skpro/blob/main/extension_templates/survival.py) | | **[Performance
 metrics]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/
 api_reference/metrics.html) | | **[Probability distributions]** | maturing |
 [Tutorial](https://github.com/sktime/skpro/blob/main/examples/
 03_skpro_distributions.ipynb) Â· [API Reference](https://skpro.readthedocs.io/
 en/latest/api_reference/distributions.html) Â· [Extension Template](https://
```

### Comparing `skpro-2.3.0/skpro.egg-info/SOURCES.txt` & `skpro-2.3.1/skpro.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 skpro.egg-info/SOURCES.txt
 skpro.egg-info/dependency_links.txt
 skpro.egg-info/requires.txt
 skpro.egg-info/top_level.txt
 skpro.egg-info/zip-safe
 skpro/base/__init__.py
 skpro/base/_base.py
-skpro/base/old_base.py
 skpro/benchmarking/__init__.py
 skpro/benchmarking/evaluate.py
 skpro/benchmarking/tests/__init__.py
 skpro/benchmarking/tests/test_evaluate.py
 skpro/datatypes/__init__.py
 skpro/datatypes/_check.py
 skpro/datatypes/_common.py
@@ -45,20 +44,22 @@
 skpro/datatypes/_table/_registry.py
 skpro/datatypes/tests/__init__.py
 skpro/datatypes/tests/test_check.py
 skpro/datatypes/tests/test_convert.py
 skpro/datatypes/tests/test_convert_to.py
 skpro/datatypes/tests/test_lookup.py
 skpro/distributions/__init__.py
+skpro/distributions/alpha.py
 skpro/distributions/beta.py
 skpro/distributions/chi_squared.py
 skpro/distributions/delta.py
 skpro/distributions/empirical.py
 skpro/distributions/exponential.py
 skpro/distributions/fisk.py
+skpro/distributions/gamma.py
 skpro/distributions/laplace.py
 skpro/distributions/logistic.py
 skpro/distributions/lognormal.py
 skpro/distributions/mixture.py
 skpro/distributions/normal.py
 skpro/distributions/poisson.py
 skpro/distributions/qpd.py
@@ -73,18 +74,21 @@
 skpro/distributions/adapters/scipy/tests/__init__.py
 skpro/distributions/adapters/scipy/tests/test_scipy_adapters.py
 skpro/distributions/adapters/statsmodels/__init__.py
 skpro/distributions/adapters/statsmodels/_empirical.py
 skpro/distributions/base/__init__.py
 skpro/distributions/base/_base.py
 skpro/distributions/base/_delegate.py
+skpro/distributions/compose/__init__.py
+skpro/distributions/compose/_iid.py
 skpro/distributions/tests/__init__.py
 skpro/distributions/tests/test_all_distrs.py
 skpro/distributions/tests/test_base_default_methods.py
 skpro/distributions/tests/test_base_scalar.py
+skpro/distributions/tests/test_empirical.py
 skpro/distributions/tests/test_proba_basic.py
 skpro/distributions/tests/test_qpd.py
 skpro/metrics/__init__.py
 skpro/metrics/_classes.py
 skpro/metrics/_coerce.py
 skpro/metrics/base.py
 skpro/metrics/survival/__init__.py
@@ -105,48 +109,44 @@
 skpro/registry/tests/test_scitype.py
 skpro/registry/tests/test_tags.py
 skpro/regression/__init__.py
 skpro/regression/bootstrap.py
 skpro/regression/cyclic_boosting.py
 skpro/regression/delta.py
 skpro/regression/density.py
+skpro/regression/enbpi.py
 skpro/regression/mapie.py
 skpro/regression/multiquantile.py
 skpro/regression/residual.py
 skpro/regression/adapters/__init__.py
 skpro/regression/adapters/ngboost/__init__.py
 skpro/regression/adapters/ngboost/_ngboost_proba.py
 skpro/regression/adapters/sklearn/__init__.py
 skpro/regression/adapters/sklearn/_sklearn_proba.py
 skpro/regression/base/__init__.py
 skpro/regression/base/_base.py
 skpro/regression/base/_delegate.py
 skpro/regression/base/adapters/__init__.py
 skpro/regression/base/adapters/_sklearn.py
-skpro/regression/baselines/__init__.py
-skpro/regression/baselines/density.py
 skpro/regression/compose/__init__.py
 skpro/regression/compose/_pipeline.py
 skpro/regression/ensemble/__init__.py
 skpro/regression/ensemble/_bagging.py
 skpro/regression/ensemble/_ngboost.py
 skpro/regression/gp/__init__.py
 skpro/regression/gp/_sklearn.py
 skpro/regression/linear/__init__.py
 skpro/regression/linear/_glm.py
 skpro/regression/linear/_sklearn.py
 skpro/regression/linear/_sklearn_poisson.py
 skpro/regression/parametric/__init__.py
 skpro/regression/parametric/estimators.py
-skpro/regression/parametric/parametric.py
 skpro/regression/tests/__init__.py
 skpro/regression/tests/test_all_regressors.py
 skpro/regression/tests/test_cyclic_boosting.py
-skpro/regression/vendors/__init__.py
-skpro/regression/vendors/pymc.py
 skpro/survival/__init__.py
 skpro/survival/base.py
 skpro/survival/adapters/__init__.py
 skpro/survival/adapters/_common.py
 skpro/survival/adapters/lifelines.py
 skpro/survival/adapters/sksurv.py
 skpro/survival/additive/__init__.py
@@ -169,21 +169,18 @@
 skpro/survival/ensemble/_survforest_sksurv.py
 skpro/survival/tree/__init__.py
 skpro/survival/tree/_tree_sksurv.py
 skpro/tests/__init__.py
 skpro/tests/_config.py
 skpro/tests/_config_test_dummy.py
 skpro/tests/test_all_estimators.py
-skpro/tests/test_base.py
-skpro/tests/test_baselines.py
 skpro/tests/test_class_register.py
 skpro/tests/test_density.py
 skpro/tests/test_ensemble.py
 skpro/tests/test_switch.py
-skpro/tests/test_vendors.py
 skpro/tests/utils.py
 skpro/tests/scenarios/__init__.py
 skpro/tests/scenarios/scenarios.py
 skpro/tests/scenarios/scenarios_getter.py
 skpro/tests/scenarios/scenarios_regressor_proba.py
 skpro/tests/tests/__init__.py
 skpro/tests/tests/test_test_utils.py
```

### Comparing `skpro-2.3.0/skpro.egg-info/requires.txt` & `skpro-2.3.1/skpro.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 numpy<1.27,>=1.21.0
 pandas<2.3.0,>=1.1.0
 packaging
-scikit-base<0.8.0,>=0.6.1
-scikit-learn<1.5.0,>=0.24.0
+scikit-base<0.9.0,>=0.6.1
+scikit-learn<1.6.0,>=0.24.0
 scipy<2.0.0,>=1.2.0
 
 [all_extras]
 attrs
 distfit
 lifelines<0.29.0
 mapie
@@ -39,12 +39,12 @@
 [docs]
 jupyter
 myst-parser
 nbsphinx>=0.8.6
 numpydoc
 pydata-sphinx-theme
 sphinx!=7.2.0,<8.0.0
-sphinx-design<0.6.0
+sphinx-design<0.7.0
 sphinx-issues<5.0.0
 sphinx-gallery<0.17.0
 sphinx-panels
 tabulate
```

