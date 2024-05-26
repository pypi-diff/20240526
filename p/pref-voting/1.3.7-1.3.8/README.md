# Comparing `tmp/pref_voting-1.3.7.tar.gz` & `tmp/pref_voting-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-1.3.7.tar", max compression
+gzip compressed data, was "pref_voting-1.3.8.tar", max compression
```

## Comparing `pref_voting-1.3.7.tar` & `pref_voting-1.3.8.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-1.3.7/LICENSE
--rw-r--r--   0        0        0     1770 2024-04-24 21:45:43.110237 pref_voting-1.3.7/README.md
--rw-r--r--   0        0        0       22 2024-05-25 21:10:22.002168 pref_voting-1.3.7/pref_voting/__init__.py
--rw-r--r--   0        0        0    22307 2024-05-10 21:48:51.212907 pref_voting-1.3.7/pref_voting/analysis.py
--rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-1.3.7/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-1.3.7/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-1.3.7/pref_voting/axioms.py
--rw-r--r--   0        0        0    34812 2024-05-23 19:59:31.870067 pref_voting-1.3.7/pref_voting/c1_methods.py
--rw-r--r--   0        0        0    15607 2024-05-23 19:52:35.351135 pref_voting-1.3.7/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    11802 2024-05-23 20:34:10.490649 pref_voting-1.3.7/pref_voting/data/voting_methods_properties.json
--rw-r--r--   0        0        0        0 2024-05-25 20:58:24.797587 pref_voting-1.3.7/pref_voting/data/voting_methods_properties.json.lock
--rw-r--r--   0        0        0    12837 2024-05-03 10:23:29.480445 pref_voting-1.3.7/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    24283 2024-04-24 20:51:32.848337 pref_voting-1.3.7/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-1.3.7/pref_voting/generate_spatial_profiles.py
--rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-1.3.7/pref_voting/generate_utility_profiles.py
--rw-r--r--   0        0        0    12631 2024-05-10 21:48:51.214555 pref_voting-1.3.7/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-1.3.7/pref_voting/grade_methods.py
--rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-1.3.7/pref_voting/grade_profiles.py
--rw-r--r--   0        0        0     8058 2024-05-05 11:00:01.292540 pref_voting-1.3.7/pref_voting/helper.py
--rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-1.3.7/pref_voting/invariance_axioms.py
--rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-1.3.7/pref_voting/io/__init__.py
--rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-1.3.7/pref_voting/io/readers.py
--rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-1.3.7/pref_voting/io/writers.py
--rw-r--r--   0        0        0    94636 2024-05-23 19:57:51.201863 pref_voting-1.3.7/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-1.3.7/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    23485 2024-05-23 19:37:48.841243 pref_voting-1.3.7/pref_voting/mappings.py
--rw-r--r--   0        0        0    76503 2024-05-23 19:59:35.003643 pref_voting-1.3.7/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    70814 2024-04-27 22:10:28.624211 pref_voting-1.3.7/pref_voting/margin_based_methods_old.py
--rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-1.3.7/pref_voting/monotonicity_axioms.py
--rw-r--r--   0        0        0    28588 2024-05-23 19:59:33.435734 pref_voting-1.3.7/pref_voting/other_methods.py
--rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-1.3.7/pref_voting/prob_voting_method.py
--rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-1.3.7/pref_voting/probabilistic_methods.py
--rw-r--r--   0        0        0    31662 2024-05-23 21:25:57.111322 pref_voting-1.3.7/pref_voting/profiles.py
--rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-1.3.7/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-1.3.7/pref_voting/rankings.py
--rw-r--r--   0        0        0    21877 2024-05-23 19:59:30.042191 pref_voting-1.3.7/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-1.3.7/pref_voting/social_welfare_function.py
--rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-1.3.7/pref_voting/social_welfare_functions.py
--rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-1.3.7/pref_voting/spatial_profiles.py
--rw-r--r--   0        0        0    15790 2024-04-30 00:43:41.503635 pref_voting-1.3.7/pref_voting/strategic_axioms.py
--rw-r--r--   0        0        0     7881 2024-05-01 10:27:56.905820 pref_voting-1.3.7/pref_voting/swf_axioms.py
--rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-1.3.7/pref_voting/tests/__init__.py
--rw-r--r--   0        0        0      745 2024-04-28 20:04:29.865701 pref_voting-1.3.7/pref_voting/tests/conftest.py
--rw-r--r--   0        0        0     5690 2024-04-28 20:01:53.768645 pref_voting-1.3.7/pref_voting/tests/test_c1_methods.py
--rw-r--r--   0        0        0     3092 2024-04-28 20:01:53.768816 pref_voting-1.3.7/pref_voting/tests/test_combined_methods.py
--rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-1.3.7/pref_voting/tests/test_generate_profiles.py
--rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-1.3.7/pref_voting/tests/test_generate_spatial_profile.py
--rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-1.3.7/pref_voting/tests/test_io.py
--rw-r--r--   0        0        0    11606 2024-04-28 20:41:27.682198 pref_voting-1.3.7/pref_voting/tests/test_iterative_methods.py
--rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-1.3.7/pref_voting/tests/test_majority_graph.py
--rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-1.3.7/pref_voting/tests/test_mapping.py
--rw-r--r--   0        0        0    10335 2024-04-28 12:01:51.077156 pref_voting-1.3.7/pref_voting/tests/test_margin_based_methods.py
--rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-1.3.7/pref_voting/tests/test_margin_graph.py
--rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-1.3.7/pref_voting/tests/test_other_methods.py
--rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-1.3.7/pref_voting/tests/test_prob_voting_method.py
--rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-1.3.7/pref_voting/tests/test_profile.py
--rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-1.3.7/pref_voting/tests/test_profile_with_ties.py
--rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-1.3.7/pref_voting/tests/test_ranking.py
--rw-r--r--   0        0        0     6234 2024-04-28 20:40:55.278187 pref_voting-1.3.7/pref_voting/tests/test_scoring_rules.py
--rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-1.3.7/pref_voting/tests/test_social_welfare_functions.py
--rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-1.3.7/pref_voting/tests/test_spatial_profile.py
--rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-1.3.7/pref_voting/tests/test_support_graph.py
--rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-1.3.7/pref_voting/tests/test_utility_function.py
--rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-1.3.7/pref_voting/tests/test_utility_functions.py
--rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-1.3.7/pref_voting/tests/test_voting_method.py
--rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-1.3.7/pref_voting/utility_functions.py
--rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-1.3.7/pref_voting/utility_methods.py
--rw-r--r--   0        0        0    12849 2024-05-23 18:23:59.371156 pref_voting-1.3.7/pref_voting/utility_profiles.py
--rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-1.3.7/pref_voting/variable_candidate_axioms.py
--rw-r--r--   0        0        0    91144 2024-05-03 10:23:29.483544 pref_voting-1.3.7/pref_voting/variable_voter_axioms.py
--rw-r--r--   0        0        0    10085 2024-05-23 20:33:22.860642 pref_voting-1.3.7/pref_voting/voting_method.py
--rw-r--r--   0        0        0     1268 2024-05-23 19:41:55.077984 pref_voting-1.3.7/pref_voting/voting_method_properties.py
--rw-r--r--   0        0        0      254 2024-05-04 20:05:10.058403 pref_voting-1.3.7/pref_voting/voting_methods.py
--rw-r--r--   0        0        0     4941 2024-05-25 20:58:19.182781 pref_voting-1.3.7/pref_voting/voting_methods_registry.py
--rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-1.3.7/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      781 2024-05-25 21:10:22.001325 pref_voting-1.3.7/pyproject.toml
--rw-r--r--   0        0        0     2910 1970-01-01 00:00:00.000000 pref_voting-1.3.7/setup.py
--rw-r--r--   0        0        0     3038 1970-01-01 00:00:00.000000 pref_voting-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-1.3.8/LICENSE
+-rw-r--r--   0        0        0     1770 2024-04-24 21:45:43.110237 pref_voting-1.3.8/README.md
+-rw-r--r--   0        0        0       22 2024-05-25 23:27:59.399120 pref_voting-1.3.8/pref_voting/__init__.py
+-rw-r--r--   0        0        0    22307 2024-05-10 21:48:51.212907 pref_voting-1.3.8/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-1.3.8/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-1.3.8/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-1.3.8/pref_voting/axioms.py
+-rw-r--r--   0        0        0    34812 2024-05-23 19:59:31.870067 pref_voting-1.3.8/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0    15607 2024-05-23 19:52:35.351135 pref_voting-1.3.8/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    11802 2024-05-23 20:34:10.490649 pref_voting-1.3.8/pref_voting/data/voting_methods_properties.json
+-rw-r--r--   0        0        0        0 2024-05-25 23:26:23.534645 pref_voting-1.3.8/pref_voting/data/voting_methods_properties.json.lock
+-rw-r--r--   0        0        0    12837 2024-05-03 10:23:29.480445 pref_voting-1.3.8/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    24283 2024-04-24 20:51:32.848337 pref_voting-1.3.8/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-1.3.8/pref_voting/generate_spatial_profiles.py
+-rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-1.3.8/pref_voting/generate_utility_profiles.py
+-rw-r--r--   0        0        0    12631 2024-05-10 21:48:51.214555 pref_voting-1.3.8/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-1.3.8/pref_voting/grade_methods.py
+-rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-1.3.8/pref_voting/grade_profiles.py
+-rw-r--r--   0        0        0     8058 2024-05-05 11:00:01.292540 pref_voting-1.3.8/pref_voting/helper.py
+-rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-1.3.8/pref_voting/invariance_axioms.py
+-rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-1.3.8/pref_voting/io/__init__.py
+-rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-1.3.8/pref_voting/io/readers.py
+-rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-1.3.8/pref_voting/io/writers.py
+-rw-r--r--   0        0        0    94747 2024-05-25 23:26:13.668871 pref_voting-1.3.8/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-1.3.8/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    23485 2024-05-23 19:37:48.841243 pref_voting-1.3.8/pref_voting/mappings.py
+-rw-r--r--   0        0        0    76503 2024-05-23 19:59:35.003643 pref_voting-1.3.8/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    70814 2024-04-27 22:10:28.624211 pref_voting-1.3.8/pref_voting/margin_based_methods_old.py
+-rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-1.3.8/pref_voting/monotonicity_axioms.py
+-rw-r--r--   0        0        0    28588 2024-05-23 19:59:33.435734 pref_voting-1.3.8/pref_voting/other_methods.py
+-rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-1.3.8/pref_voting/prob_voting_method.py
+-rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-1.3.8/pref_voting/probabilistic_methods.py
+-rw-r--r--   0        0        0    31662 2024-05-23 21:25:57.111322 pref_voting-1.3.8/pref_voting/profiles.py
+-rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-1.3.8/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-1.3.8/pref_voting/rankings.py
+-rw-r--r--   0        0        0    21877 2024-05-23 19:59:30.042191 pref_voting-1.3.8/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-1.3.8/pref_voting/social_welfare_function.py
+-rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-1.3.8/pref_voting/social_welfare_functions.py
+-rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-1.3.8/pref_voting/spatial_profiles.py
+-rw-r--r--   0        0        0    15790 2024-04-30 00:43:41.503635 pref_voting-1.3.8/pref_voting/strategic_axioms.py
+-rw-r--r--   0        0        0     7881 2024-05-01 10:27:56.905820 pref_voting-1.3.8/pref_voting/swf_axioms.py
+-rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-1.3.8/pref_voting/tests/__init__.py
+-rw-r--r--   0        0        0      745 2024-04-28 20:04:29.865701 pref_voting-1.3.8/pref_voting/tests/conftest.py
+-rw-r--r--   0        0        0     5690 2024-04-28 20:01:53.768645 pref_voting-1.3.8/pref_voting/tests/test_c1_methods.py
+-rw-r--r--   0        0        0     3092 2024-04-28 20:01:53.768816 pref_voting-1.3.8/pref_voting/tests/test_combined_methods.py
+-rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-1.3.8/pref_voting/tests/test_generate_profiles.py
+-rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-1.3.8/pref_voting/tests/test_generate_spatial_profile.py
+-rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-1.3.8/pref_voting/tests/test_io.py
+-rw-r--r--   0        0        0    11606 2024-04-28 20:41:27.682198 pref_voting-1.3.8/pref_voting/tests/test_iterative_methods.py
+-rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-1.3.8/pref_voting/tests/test_majority_graph.py
+-rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-1.3.8/pref_voting/tests/test_mapping.py
+-rw-r--r--   0        0        0    10335 2024-04-28 12:01:51.077156 pref_voting-1.3.8/pref_voting/tests/test_margin_based_methods.py
+-rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-1.3.8/pref_voting/tests/test_margin_graph.py
+-rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-1.3.8/pref_voting/tests/test_other_methods.py
+-rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-1.3.8/pref_voting/tests/test_prob_voting_method.py
+-rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-1.3.8/pref_voting/tests/test_profile.py
+-rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-1.3.8/pref_voting/tests/test_profile_with_ties.py
+-rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-1.3.8/pref_voting/tests/test_ranking.py
+-rw-r--r--   0        0        0     6234 2024-04-28 20:40:55.278187 pref_voting-1.3.8/pref_voting/tests/test_scoring_rules.py
+-rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-1.3.8/pref_voting/tests/test_social_welfare_functions.py
+-rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-1.3.8/pref_voting/tests/test_spatial_profile.py
+-rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-1.3.8/pref_voting/tests/test_support_graph.py
+-rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-1.3.8/pref_voting/tests/test_utility_function.py
+-rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-1.3.8/pref_voting/tests/test_utility_functions.py
+-rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-1.3.8/pref_voting/tests/test_voting_method.py
+-rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-1.3.8/pref_voting/utility_functions.py
+-rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-1.3.8/pref_voting/utility_methods.py
+-rw-r--r--   0        0        0    12849 2024-05-23 18:23:59.371156 pref_voting-1.3.8/pref_voting/utility_profiles.py
+-rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-1.3.8/pref_voting/variable_candidate_axioms.py
+-rw-r--r--   0        0        0    91144 2024-05-03 10:23:29.483544 pref_voting-1.3.8/pref_voting/variable_voter_axioms.py
+-rw-r--r--   0        0        0    10219 2024-05-25 23:15:03.604765 pref_voting-1.3.8/pref_voting/voting_method.py
+-rw-r--r--   0        0        0     1355 2024-05-25 23:14:53.050004 pref_voting-1.3.8/pref_voting/voting_method_properties.py
+-rw-r--r--   0        0        0      254 2024-05-04 20:05:10.058403 pref_voting-1.3.8/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0     5028 2024-05-25 23:11:19.277884 pref_voting-1.3.8/pref_voting/voting_methods_registry.py
+-rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-1.3.8/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      781 2024-05-25 23:27:59.397875 pref_voting-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0     2910 1970-01-01 00:00:00.000000 pref_voting-1.3.8/setup.py
+-rw-r--r--   0        0        0     3038 1970-01-01 00:00:00.000000 pref_voting-1.3.8/PKG-INFO
```

### Comparing `pref_voting-1.3.7/LICENSE` & `pref_voting-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/README.md` & `pref_voting-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/analysis.py` & `pref_voting-1.3.8/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/axiom.py` & `pref_voting-1.3.8/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/c1_methods.py` & `pref_voting-1.3.8/pref_voting/c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/combined_methods.py` & `pref_voting-1.3.8/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/data/voting_methods_properties.json` & `pref_voting-1.3.8/pref_voting/data/voting_methods_properties.json`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/dominance_axioms.py` & `pref_voting-1.3.8/pref_voting/dominance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/generate_profiles.py` & `pref_voting-1.3.8/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/generate_spatial_profiles.py` & `pref_voting-1.3.8/pref_voting/generate_spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/generate_utility_profiles.py` & `pref_voting-1.3.8/pref_voting/generate_utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-1.3.8/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/grade_methods.py` & `pref_voting-1.3.8/pref_voting/grade_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/grade_profiles.py` & `pref_voting-1.3.8/pref_voting/grade_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/helper.py` & `pref_voting-1.3.8/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/invariance_axioms.py` & `pref_voting-1.3.8/pref_voting/invariance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/io/readers.py` & `pref_voting-1.3.8/pref_voting/io/readers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/io/writers.py` & `pref_voting-1.3.8/pref_voting/io/writers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/iterative_methods.py` & `pref_voting-1.3.8/pref_voting/iterative_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     
     Implementations of iterative voting methods.
 '''
 from pref_voting.voting_method import  *
 from pref_voting.voting_method import _num_rank_last, _num_rank_first
 from pref_voting.profiles import  _borda_score, _find_updated_profile
 from pref_voting.margin_based_methods import split_cycle, minimax_scores
-from pref_voting.c1_methods import top_cycle, gocha
+from pref_voting.c1_methods import top_cycle, gocha 
 from pref_voting.rankings import Ranking
 from pref_voting.social_welfare_function import swf
 import copy
 from itertools import permutations, product
 import numpy as np
 from pref_voting.voting_method_properties import ElectionTypes
 
@@ -1868,24 +1868,25 @@
         cands_to_remove = [cand for cand, value in plurality_scores.items() if value == worst_score]
         
         if len(cands_to_remove) == len(vm_ws):
             return vm_ws
             
         else:
             return _ta(profile, curr_cands = [c for c in candidates if not c in cands_to_remove])
-
+        
+    _ta.__name__ = f"tideman_alternative_{vm.__name__}"
     return VotingMethod(_ta, name=f"Tideman Alternative {vm.name}")
 
 tideman_alternative_smith = tideman_alternative(top_cycle)
 tideman_alternative_smith.load_properties()
 tideman_alternative_smith.input_types = [ElectionTypes.PROFILE]
 
-tideman_alternative_schwartz = tideman_alternative(gocha)
-tideman_alternative_schwartz.load_properties()
-tideman_alternative_schwartz.input_types = [ElectionTypes.PROFILE]
+tideman_alternative_gocha = tideman_alternative(gocha)
+tideman_alternative_gocha.load_properties()
+tideman_alternative_gocha.input_types = [ElectionTypes.PROFILE]
 
 def tideman_alternative_put(vm):
     """Given a voting method vm, returns a voting method that restricts the profile to the set of vm winners, then eliminates the candidate with the fewest first-place votes, and then repeats until there is only one vm winner. Parallel-universe tiebreaking is used when there are multiple candidates with the fewest first-place votes.
 
     Args:
         vm (VotingMethod): A voting method.
 
@@ -1910,25 +1911,26 @@
         
             winners = []
             for cand_to_remove in cands_to_remove:
                 additional_winners = _ta(profile, curr_cands = [c for c in candidates if not c == cand_to_remove])
                 winners = winners + additional_winners
 
         return sorted(set(winners))
-
+    
+    _ta.__name__ = f"tideman_alternative_{vm.__name__}_put"
     return VotingMethod(_ta, name=f"Tideman Alternative {vm.name} PUT")
 
 
 tideman_alternative_smith_put = tideman_alternative_put(top_cycle)
 tideman_alternative_smith_put.load_properties()
 tideman_alternative_smith_put.input_types = [ElectionTypes.PROFILE]
 
-tideman_alternative_schwartz_put = tideman_alternative_put(gocha)
-tideman_alternative_schwartz_put.load_properties()
-tideman_alternative_schwartz_put.input_types = [ElectionTypes.PROFILE]
+tideman_alternative_gocha_put = tideman_alternative_put(gocha)
+tideman_alternative_gocha_put.load_properties()
+tideman_alternative_gocha_put.input_types = [ElectionTypes.PROFILE]
 
 
 @vm(name = "Woodall",
     input_types=[ElectionTypes.PROFILE])
 def woodall(profile, curr_cands = None):
     """
     If there is a single member of the Smith Set (i.e., a Condorcet winner) then that candidate is the winner.  If there the Smith Set contains more than one candidate, then remove all candidates that are ranked first by the fewest number of voters.  Continue removing candidates with the fewest number first-place votes until there is a single member of the originally Smith Set remaining.
```

### Comparing `pref_voting-1.3.7/pref_voting/maj_graph_ex1.png` & `pref_voting-1.3.8/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/mappings.py` & `pref_voting-1.3.8/pref_voting/mappings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/margin_based_methods.py` & `pref_voting-1.3.8/pref_voting/margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/margin_based_methods_old.py` & `pref_voting-1.3.8/pref_voting/margin_based_methods_old.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/monotonicity_axioms.py` & `pref_voting-1.3.8/pref_voting/monotonicity_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/other_methods.py` & `pref_voting-1.3.8/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/prob_voting_method.py` & `pref_voting-1.3.8/pref_voting/prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/probabilistic_methods.py` & `pref_voting-1.3.8/pref_voting/probabilistic_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/profiles.py` & `pref_voting-1.3.8/pref_voting/profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/profiles_with_ties.py` & `pref_voting-1.3.8/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/rankings.py` & `pref_voting-1.3.8/pref_voting/rankings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/scoring_methods.py` & `pref_voting-1.3.8/pref_voting/scoring_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/social_welfare_function.py` & `pref_voting-1.3.8/pref_voting/social_welfare_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/spatial_profiles.py` & `pref_voting-1.3.8/pref_voting/spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/strategic_axioms.py` & `pref_voting-1.3.8/pref_voting/strategic_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/swf_axioms.py` & `pref_voting-1.3.8/pref_voting/swf_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/conftest.py` & `pref_voting-1.3.8/pref_voting/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_c1_methods.py` & `pref_voting-1.3.8/pref_voting/tests/test_c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_combined_methods.py` & `pref_voting-1.3.8/pref_voting/tests/test_combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_generate_profiles.py` & `pref_voting-1.3.8/pref_voting/tests/test_generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_generate_spatial_profile.py` & `pref_voting-1.3.8/pref_voting/tests/test_generate_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_io.py` & `pref_voting-1.3.8/pref_voting/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_iterative_methods.py` & `pref_voting-1.3.8/pref_voting/tests/test_iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_majority_graph.py` & `pref_voting-1.3.8/pref_voting/tests/test_majority_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_mapping.py` & `pref_voting-1.3.8/pref_voting/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_margin_based_methods.py` & `pref_voting-1.3.8/pref_voting/tests/test_margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_margin_graph.py` & `pref_voting-1.3.8/pref_voting/tests/test_margin_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_other_methods.py` & `pref_voting-1.3.8/pref_voting/tests/test_other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_prob_voting_method.py` & `pref_voting-1.3.8/pref_voting/tests/test_prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_profile.py` & `pref_voting-1.3.8/pref_voting/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_profile_with_ties.py` & `pref_voting-1.3.8/pref_voting/tests/test_profile_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_ranking.py` & `pref_voting-1.3.8/pref_voting/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_scoring_rules.py` & `pref_voting-1.3.8/pref_voting/tests/test_scoring_rules.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_social_welfare_functions.py` & `pref_voting-1.3.8/pref_voting/tests/test_social_welfare_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_spatial_profile.py` & `pref_voting-1.3.8/pref_voting/tests/test_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_support_graph.py` & `pref_voting-1.3.8/pref_voting/tests/test_support_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_utility_function.py` & `pref_voting-1.3.8/pref_voting/tests/test_utility_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_utility_functions.py` & `pref_voting-1.3.8/pref_voting/tests/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/tests/test_voting_method.py` & `pref_voting-1.3.8/pref_voting/tests/test_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/utility_functions.py` & `pref_voting-1.3.8/pref_voting/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/utility_methods.py` & `pref_voting-1.3.8/pref_voting/utility_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/utility_profiles.py` & `pref_voting-1.3.8/pref_voting/utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/variable_candidate_axioms.py` & `pref_voting-1.3.8/pref_voting/variable_candidate_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/variable_voter_axioms.py` & `pref_voting-1.3.8/pref_voting/variable_voter_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pref_voting/voting_method.py` & `pref_voting-1.3.8/pref_voting/voting_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,19 @@
                 vm_props = {}
 
             if self.name in vm_props:
                 self.properties = VotingMethodProperties(**vm_props[self.name])
             else:
                 self.properties = VotingMethodProperties()
 
+    def has_property(self, prop):
+        """Check if the voting method has a property."""
+
+        return self.properties[prop]
+    
     def save_properties(self, filename=None, timeout=10):
         """Save the properties of the voting method to a JSON file."""
 
         # Determine the path to the properties file
         if filename is None:
             filename = pkg_resources.resource_filename('pref_voting', 'data/voting_methods_properties.json')
```

### Comparing `pref_voting-1.3.7/pref_voting/voting_method_properties.py` & `pref_voting-1.3.8/pref_voting/voting_method_properties.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,18 @@
         condorcet_consistent (bool): Indicates if the voting method always elects a Condorcet winner when one exists.
     """
     def __init__(self, **kwargs):
         for key, value in kwargs.items():
             setattr(self, key, value)
 
     def satisfied(self):
-        return [key for key, value in self.__dict__.items() if value==True]
+        return [key for key, value in self.__dict__.items() if value is True]
     
     def violated(self):
-        return [key for key, value in self.__dict__.items() if value==False]
+        return [key for key, value in self.__dict__.items() if value is False]
+
+    def __getitem__(self, prop):
+        return self.__dict__.get(prop, None)
 
     def __str__(self):
-        properties = [f"{key}: {'Satisfied' if value==True else ('Violated' if value==False else 'N/A')}" for key, value in self.__dict__.items()]
+        properties = [f"{key}: {'Satisfied' if value is True else ('Violated' if value is False else 'N/A')}" for key, value in self.__dict__.items()]
         return "\n".join(properties)
```

### Comparing `pref_voting-1.3.7/pref_voting/voting_methods_registry.py` & `pref_voting-1.3.8/pref_voting/voting_methods_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,13 +122,15 @@
 
 voting_methods = VotingMethodRegistry()
 
 import pref_voting.scoring_methods 
 voting_methods.discover_methods(pref_voting.scoring_methods)
 import pref_voting.iterative_methods 
 voting_methods.discover_methods(pref_voting.iterative_methods)
+import pref_voting.c1_methods 
+voting_methods.discover_methods(pref_voting.c1_methods)
 import pref_voting.margin_based_methods 
 voting_methods.discover_methods(pref_voting.margin_based_methods)
 import pref_voting.combined_methods 
 voting_methods.discover_methods(pref_voting.combined_methods)
 import pref_voting.other_methods 
 voting_methods.discover_methods(pref_voting.other_methods)
```

### Comparing `pref_voting-1.3.7/pref_voting/weighted_majority_graphs.py` & `pref_voting-1.3.8/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.7/pyproject.toml` & `pref_voting-1.3.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "1.3.7"
+version = "1.3.8"
 description = "pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-1.3.7/setup.py` & `pref_voting-1.3.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'prefsampling>=0.1.16,<0.2.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '1.3.7',
+    'version': '1.3.8',
     'description': 'pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.',
     'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n\n## Documentation\n\nOnline documentation is available at [https://pref-voting.readthedocs.io](https://pref-voting.readthedocs.io).\n\n## Example Usage\n\nA profile (of linear orders over the candidates) is created by initializing a `Profile` class object.  Simply provide a list of rankings (each ranking is a tuple of numbers) and a list giving the number of voters with each ranking:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [\n    (0, 1, 2, 3), \n    (2, 3, 1, 0), \n    (3, 1, 2, 0), \n    (1, 2, 0, 3), \n    (1, 3, 2, 0)]\n\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function `generate_profile` is used to generate a profile for a given number of candidates and voters:  \n\n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\nTo use one of the many voting methods, import the function from `pref_voting.voting_methods` and apply it to the profile: \n\n```python\nfrom pref_voting.generate_profiles import generate_profile\nfrom pref_voting.voting_methods import *\n\nprof = generate_profile(3, 4)\nsplit_cycle(prof) # returns the sorted list of winning candidates\nsplit_cycle.display(prof) # display the winning candidates\n\n```\n\n## Questions?\n\nFeel free to [send an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
```

### Comparing `pref_voting-1.3.7/PKG-INFO` & `pref_voting-1.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 1.3.7
+Version: 1.3.8
 Summary: pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```
