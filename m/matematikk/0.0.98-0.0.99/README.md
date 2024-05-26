# Comparing `tmp/matematikk-0.0.98.tar.gz` & `tmp/matematikk-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matematikk-0.0.98.tar", last modified: Fri Feb  2 14:12:14 2024, max compression
+gzip compressed data, was "matematikk-0.0.99.tar", last modified: Fri Feb  2 14:17:18 2024, max compression
```

## Comparing `matematikk-0.0.98.tar` & `matematikk-0.0.99.tar`

### file list

```diff
@@ -1,384 +1,383 @@
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.805889 matematikk-0.0.98/
--rw-r--r--   0 krj        (502) staff       (20)     1073 2024-02-02 07:00:53.000000 matematikk-0.0.98/LICENCE
--rw-r--r--   0 krj        (502) staff       (20)      625 2024-02-02 14:12:14.805269 matematikk-0.0.98/PKG-INFO
--rw-r--r--   0 krj        (502) staff       (20)      170 2024-02-02 07:00:53.000000 matematikk-0.0.98/README.md
--rw-r--r--   0 krj        (502) staff       (20)      435 2024-02-02 14:12:06.000000 matematikk-0.0.98/pyproject.toml
--rw-r--r--   0 krj        (502) staff       (20)       38 2024-02-02 14:12:14.805949 matematikk-0.0.98/setup.cfg
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.752106 matematikk-0.0.98/src/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.761271 matematikk-0.0.98/src/matematikk/
--rw-r--r--   0 krj        (502) staff       (20)     1570 2024-02-02 14:11:29.000000 matematikk-0.0.98/src/matematikk/__init__.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.752277 matematikk-0.0.98/src/matematikk/_ch_1/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.752328 matematikk-0.0.98/src/matematikk/_ch_1/ch_2/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.761862 matematikk-0.0.98/src/matematikk/_ch_1/ch_2/ch_3/
--rw-r--r--   0 krj        (502) staff       (20)      252 2024-02-02 14:11:29.000000 matematikk-0.0.98/src/matematikk/_ch_1/ch_2/ch_3/ch_4_fil.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.761975 matematikk-0.0.98/src/matematikk/eksamen/
--rw-r--r--   0 krj        (502) staff       (20)      861 2024-02-02 14:11:29.000000 matematikk-0.0.98/src/matematikk/eksamen/oppg_test.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.758751 matematikk-0.0.98/src/matematikk/python/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.752957 matematikk-0.0.98/src/matematikk/python/eksamen/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.752781 matematikk-0.0.98/src/matematikk/python/eksamen/1t/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.752665 matematikk-0.0.98/src/matematikk/python/eksamen/1t/2022_h/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.752710 matematikk-0.0.98/src/matematikk/python/eksamen/1t/2022_h/del_1/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.762807 matematikk-0.0.98/src/matematikk/python/eksamen/1t/2022_h/del_1/03/
--rw-r--r--   0 krj        (502) staff       (20)      254 2024-02-02 14:11:29.000000 matematikk-0.0.98/src/matematikk/python/eksamen/1t/2022_h/del_1/03/oppg_3_a_rasjonal_funksjon_bug.py
--rw-r--r--   0 krj        (502) staff       (20)      310 2024-02-02 14:11:30.000000 matematikk-0.0.98/src/matematikk/python/eksamen/1t/2022_h/del_1/03/oppg_3_b_rasjonal_funksjon_if.py
--rw-r--r--   0 krj        (502) staff       (20)      298 2024-02-02 14:11:29.000000 matematikk-0.0.98/src/matematikk/python/eksamen/1t/2022_h/del_1/03/oppg_3_b_rasjonal_funksjon_if_else.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.752834 matematikk-0.0.98/src/matematikk/python/eksamen/1t/2022_v/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.752885 matematikk-0.0.98/src/matematikk/python/eksamen/1t/2022_v/del_1/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.762980 matematikk-0.0.98/src/matematikk/python/eksamen/1t/2022_v/del_1/04/
--rw-r--r--   0 krj        (502) staff       (20)      273 2024-02-02 14:11:30.000000 matematikk-0.0.98/src/matematikk/python/eksamen/1t/2022_v/del_1/04/oppg_4_kvadrattall.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.753676 matematikk-0.0.98/src/matematikk/python/eksamen/s1/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.753155 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.753089 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_1/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.763182 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_1/05/
--rw-r--r--   0 krj        (502) staff       (20)      262 2024-02-02 14:11:30.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_1/05/oppg_5_grensekostnad.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.753584 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.766427 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/
--rw-r--r--   0 krj        (502) staff       (20)     2856 2024-02-02 14:11:30.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_1_sofa_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     3564 2024-02-02 14:11:30.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_2_sofa_def_reggis_str_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     3497 2024-02-02 14:11:30.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_3_sofa_def_reggis_cas_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     1935 2024-02-02 14:11:30.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_4_sofa_matematikk_mas.py
--rw-r--r--   0 krj        (502) staff       (20)      577 2024-02-02 14:11:30.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_5_sofa_matematikk_speedrun_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     4672 2024-02-02 14:11:30.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_1_sofa_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     8632 2024-02-02 14:11:30.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_2_sofa_def_superlos_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     2883 2024-02-02 14:11:31.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_3_sofa_matematikk_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     3276 2024-02-02 14:11:31.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_4_sofa_def_overskudd_max_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     3798 2024-02-02 14:11:31.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_5_sofa_abstrahering_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     2759 2024-02-02 14:11:31.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_6_sofa_matematikk_mas.py
--rw-r--r--   0 krj        (502) staff       (20)      806 2024-02-02 14:11:31.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_7_sofa_matematikk_speedrun_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     7323 2024-02-02 14:11:31.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_c_sofa_mas.py
--rw-r--r--   0 krj        (502) staff       (20)      436 2024-02-02 14:11:31.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/02_oppg_1_a_sofa_torodd.py
--rw-r--r--   0 krj        (502) staff       (20)      483 2024-02-02 14:11:31.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/02_oppg_1_b_sofa_torodd.py
--rw-r--r--   0 krj        (502) staff       (20)     1211 2024-02-02 14:11:31.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/02_oppg_1_c_sofa_torodd.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.768159 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/02/
--rw-r--r--   0 krj        (502) staff       (20)     1885 2024-02-02 14:11:31.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/02/01_oppg_2_a_venstrehendte_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     4382 2024-02-02 14:11:31.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/02/01_oppg_2_b_1_venstrehendte_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     5738 2024-02-02 14:11:31.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/02/01_oppg_2_b_2_venstrehendte_relasjoner_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     3936 2024-02-02 14:11:31.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/02/01_oppg_2_c_venstrehendte_mas.py
--rw-r--r--   0 krj        (502) staff       (20)      486 2024-02-02 14:11:32.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/02/02_oppg_2_a_venstrehendte_torodd.py
--rw-r--r--   0 krj        (502) staff       (20)      603 2024-02-02 14:11:32.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/02/02_oppg_2_b_venstrehendte_torodd.py
--rw-r--r--   0 krj        (502) staff       (20)      644 2024-02-02 14:11:32.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/02/02_oppg_2_c_venstrehendte_torodd.py
--rw-r--r--   0 krj        (502) staff       (20)    17344 2024-02-02 14:11:31.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/02/mal_sannsynlighets_relasjoner_mas.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.769894 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/03/
--rw-r--r--   0 krj        (502) staff       (20)     2846 2024-02-02 14:11:32.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_a_sparekonto_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     4982 2024-02-02 14:11:32.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_b_sparekonto_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     6361 2024-02-02 14:11:32.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_c_1_sparekonto_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     9428 2024-02-02 14:11:32.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_c_2_sparekonto_superlos_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     5275 2024-02-02 14:11:32.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_c_3_sparekonto_matematikk_mas.py
--rw-r--r--   0 krj        (502) staff       (20)      383 2024-02-02 14:11:32.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/03/02_oppg_3_a_sparekonto_torodd.py
--rw-r--r--   0 krj        (502) staff       (20)      549 2024-02-02 14:11:32.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/03/02_oppg_3_b_sparekonto_torodd.py
--rw-r--r--   0 krj        (502) staff       (20)      385 2024-02-02 14:11:32.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/03/02_oppg_3_c_sparekonto_torodd.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.771404 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/04/
--rw-r--r--   0 krj        (502) staff       (20)     2399 2024-02-02 14:11:32.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/04/01_oppg_4_a_terninger_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     4765 2024-02-02 14:11:32.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/04/01_oppg_4_b_terninger_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     6243 2024-02-02 14:11:32.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/04/01_oppg_4_c_terninger_mas.py
--rw-r--r--   0 krj        (502) staff       (20)      327 2024-02-02 14:11:32.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/04/02_oppg_4_a_terninger_torodd.py
--rw-r--r--   0 krj        (502) staff       (20)      600 2024-02-02 14:11:33.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/04/02_oppg_4_b_terninger_torodd.py
--rw-r--r--   0 krj        (502) staff       (20)      518 2024-02-02 14:11:33.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/04/02_oppg_4_c_terninger_torodd.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.772975 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/05/
--rw-r--r--   0 krj        (502) staff       (20)     2060 2024-02-02 14:11:33.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_a_1_prisme_geometrisk_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     2835 2024-02-02 14:11:33.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_a_2_prisme_likning_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     6114 2024-02-02 14:11:33.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_a_3_prisme_likning_superlos_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     8802 2024-02-02 14:11:33.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_b_prisme_likning_mas.py
--rw-r--r--   0 krj        (502) staff       (20)    11004 2024-02-02 14:11:33.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_c_prisme_likning_mas.py
--rw-r--r--   0 krj        (502) staff       (20)      460 2024-02-02 14:11:33.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/05/02_oppg_5_a_prisme_likning_torodd.py
--rw-r--r--   0 krj        (502) staff       (20)      460 2024-02-02 14:11:33.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/05/02_oppg_5_b_prisme_likning_torodd.py
--rw-r--r--   0 krj        (502) staff       (20)      460 2024-02-02 14:11:33.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/05/02_oppg_5_c_prisme_likning_torodd.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.774154 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/06/
--rw-r--r--   0 krj        (502) staff       (20)     8905 2024-02-02 14:11:33.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/06/01_oppg_6_a_tredjegradsfunksjon_mas.py
--rw-r--r--   0 krj        (502) staff       (20)    11517 2024-02-02 14:11:33.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/06/01_oppg_6_b_tredjegradsfunksjon_mas.py
--rw-r--r--   0 krj        (502) staff       (20)    13330 2024-02-02 14:11:33.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/06/01_oppg_6_c_tredjegradsfunksjon_mas.py
--rw-r--r--   0 krj        (502) staff       (20)      579 2024-02-02 14:11:33.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/06/02_oppg_6_a_tredjegradsfunksjon_torodd.py
--rw-r--r--   0 krj        (502) staff       (20)      422 2024-02-02 14:11:34.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/06/02_oppg_6_b_tredjegradsfunksjon_torodd.py
--rw-r--r--   0 krj        (502) staff       (20)      669 2024-02-02 14:11:34.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/06/02_oppg_6_c_tredjegradsfunksjon_torodd.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.753737 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_v/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.753816 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_v/del_2/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.774600 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_v/del_2/01/
--rw-r--r--   0 krj        (502) staff       (20)     6795 2024-02-02 14:11:30.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_v/del_2/01/01_oppg_1_a_timelonn_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     6792 2024-02-02 14:11:30.000000 matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_v/del_2/01/01_oppg_1_b_timelonn_mas.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.753992 matematikk-0.0.98/src/matematikk/python/funksjoner/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.754401 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.754113 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/funksjoner/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.754176 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.775387 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/
--rw-r--r--   0 krj        (502) staff       (20)      840 2024-02-02 14:11:34.000000 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/def_ekstremalpunkt_max_mas.py
--rw-r--r--   0 krj        (502) staff       (20)      840 2024-02-02 14:11:34.000000 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/def_ekstremalpunkt_max_matematikk_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     1005 2024-02-02 14:11:34.000000 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/def_overskudd_max_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     1008 2024-02-02 14:11:34.000000 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/def_overskudd_max_matematikk_mas.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.754319 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/likninger/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.775813 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/likninger/superlos/
--rw-r--r--   0 krj        (502) staff       (20)     4251 2024-02-02 14:11:34.000000 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/likninger/superlos/def_superlos_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     4622 2024-02-02 14:11:34.000000 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/likninger/superlos/def_superlos_matematikk_mas.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.754455 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/regresjon/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.754505 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/regresjon/polynom/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.776188 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/regresjon/polynom/reggis/
--rw-r--r--   0 krj        (502) staff       (20)     1641 2024-02-02 14:11:34.000000 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/regresjon/polynom/reggis/def_reggis_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     1963 2024-02-02 14:11:34.000000 matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/regresjon/polynom/reggis/def_reggis_matematikk_mas.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.754673 matematikk-0.0.98/src/matematikk/python/oppgaver/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.754741 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.755240 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.776580 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_55/
--rw-r--r--   0 krj        (502) staff       (20)     4045 2024-02-02 14:11:35.000000 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_55/01_oppg_1_55_vanjas_scooter_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     4023 2024-02-02 14:11:35.000000 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_55/02_oppg_1_55_vanjas_scooter_input_mas.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.776779 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_56/
--rw-r--r--   0 krj        (502) staff       (20)     3765 2024-02-02 14:11:35.000000 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_56/oppg_1_56_elbiler_mas.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.776976 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_57/
--rw-r--r--   0 krj        (502) staff       (20)     3850 2024-02-02 14:11:35.000000 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_57/oppg_1_57_hus_og_elbiler_mas.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.777974 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/
--rw-r--r--   0 krj        (502) staff       (20)      342 2024-02-02 14:11:34.000000 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/01_eks_1_5_a_b_vindpark_bok.py
--rw-r--r--   0 krj        (502) staff       (20)     1749 2024-02-02 14:11:34.000000 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/02_eks_1_5_a_b_vindpark_mas.py
--rw-r--r--   0 krj        (502) staff       (20)      474 2024-02-02 14:11:34.000000 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/03_eks_1_5_a_b_vindpark_input_bok.py
--rw-r--r--   0 krj        (502) staff       (20)     2109 2024-02-02 14:11:34.000000 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/04_eks_1_5_a_b_vindpark_input_mas.py
--rw-r--r--   0 krj        (502) staff       (20)     3485 2024-02-02 14:11:35.000000 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/05_oppg_1_59_vindpark_mas.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.778180 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/9/
--rw-r--r--   0 krj        (502) staff       (20)     3657 2024-02-02 14:11:35.000000 matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/9/oppg_k_1_9_pythagoras_mas.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.756983 matematikk-0.0.98/src/matematikk/python/programmer/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.756622 matematikk-0.0.98/src/matematikk/python/programmer/datatype/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.756539 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.779080 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/antall/
--rw-r--r--   0 krj        (502) staff       (20)      363 2024-02-02 14:11:35.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/antall/liste_count_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1156 2024-02-02 14:11:35.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/antall/liste_count_2_input_str.py
--rw-r--r--   0 krj        (502) staff       (20)      296 2024-02-02 14:11:35.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/antall/liste_length_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1056 2024-02-02 14:11:35.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/antall/liste_length_2_input_str.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.779285 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/change/
--rw-r--r--   0 krj        (502) staff       (20)      394 2024-02-02 14:11:35.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/change/liste_bytt_el.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.780653 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/copy/
--rw-r--r--   0 krj        (502) staff       (20)      234 2024-02-02 14:11:36.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/copy/liste_copy.py
--rw-r--r--   0 krj        (502) staff       (20)      236 2024-02-02 14:11:35.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/copy/liste_copy_assignment.py
--rw-r--r--   0 krj        (502) staff       (20)      247 2024-02-02 14:11:35.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/copy/liste_copy_comprehension.py
--rw-r--r--   0 krj        (502) staff       (20)      754 2024-02-02 14:11:35.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/copy/liste_copy_deepcopy.py
--rw-r--r--   0 krj        (502) staff       (20)      431 2024-02-02 14:11:36.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/copy/liste_copy_extend.py
--rw-r--r--   0 krj        (502) staff       (20)      268 2024-02-02 14:11:35.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/copy/liste_copy_extend_kort.py
--rw-r--r--   0 krj        (502) staff       (20)      429 2024-02-02 14:11:36.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/copy/liste_copy_slice.py
--rw-r--r--   0 krj        (502) staff       (20)      242 2024-02-02 14:11:36.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/copy/liste_copy_slice_kort.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.781410 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/delete/
--rw-r--r--   0 krj        (502) staff       (20)      235 2024-02-02 14:11:36.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/delete/liste_delete.py
--rw-r--r--   0 krj        (502) staff       (20)      644 2024-02-02 14:11:36.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/delete/liste_remove_negative_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1250 2024-02-02 14:11:36.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/delete/liste_remove_negative_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)      644 2024-02-02 14:11:36.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/delete/liste_remove_positive_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1250 2024-02-02 14:11:36.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/delete/liste_remove_positive_2_input.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.782142 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/eksisterer/
--rw-r--r--   0 krj        (502) staff       (20)      327 2024-02-02 14:11:36.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/eksisterer/liste_eksisterer_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1119 2024-02-02 14:11:36.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/eksisterer/liste_eksisterer_2_input_str.py
--rw-r--r--   0 krj        (502) staff       (20)      352 2024-02-02 14:11:36.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/eksisterer/liste_eksisterer_for_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1404 2024-02-02 14:11:36.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/eksisterer/liste_eksisterer_for_2_input_str.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.782891 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/max/
--rw-r--r--   0 krj        (502) staff       (20)      579 2024-02-02 14:11:36.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/max/liste_max_for_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1195 2024-02-02 14:11:37.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/max/liste_max_for_2_input_int.py
--rw-r--r--   0 krj        (502) staff       (20)      473 2024-02-02 14:11:37.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/max/liste_max_sort_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1086 2024-02-02 14:11:37.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/max/liste_max_sort_2_input_int.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.783541 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/min/
--rw-r--r--   0 krj        (502) staff       (20)      568 2024-02-02 14:11:37.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/min/liste_min_for_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1185 2024-02-02 14:11:37.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/min/liste_min_for_2_input_int.py
--rw-r--r--   0 krj        (502) staff       (20)      507 2024-02-02 14:11:37.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/min/liste_min_sort_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1121 2024-02-02 14:11:37.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/min/liste_min_sort_2_input_int.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.784691 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/monotonic/
--rw-r--r--   0 krj        (502) staff       (20)      702 2024-02-02 14:11:37.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_all_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1274 2024-02-02 14:11:37.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_all_2_input_int.py
--rw-r--r--   0 krj        (502) staff       (20)      995 2024-02-02 14:11:37.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_sort_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1569 2024-02-02 14:11:37.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_sort_2_input_int.py
--rw-r--r--   0 krj        (502) staff       (20)     1251 2024-02-02 14:11:37.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_sort_3_to.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.786358 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/
--rw-r--r--   0 krj        (502) staff       (20)      849 2024-02-02 14:11:37.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_comprehension_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1524 2024-02-02 14:11:37.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_comprehension_2_input_str.py
--rw-r--r--   0 krj        (502) staff       (20)      871 2024-02-02 14:11:37.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_for_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1525 2024-02-02 14:11:38.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_for_2_input_str.py
--rw-r--r--   0 krj        (502) staff       (20)      760 2024-02-02 14:11:38.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_numpy_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1409 2024-02-02 14:11:38.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_numpy_2_input_str.py
--rw-r--r--   0 krj        (502) staff       (20)      801 2024-02-02 14:11:38.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_yield_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1444 2024-02-02 14:11:38.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_yield_2_input_str.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.787879 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/product/
--rw-r--r--   0 krj        (502) staff       (20)      463 2024-02-02 14:11:38.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/product/liste_produkt_for_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1094 2024-02-02 14:11:38.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/product/liste_produkt_for_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)      299 2024-02-02 14:11:38.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/product/liste_produkt_math_1.py
--rw-r--r--   0 krj        (502) staff       (20)      930 2024-02-02 14:11:38.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/product/liste_produkt_math_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)      303 2024-02-02 14:11:38.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/product/liste_produkt_numpy_1.py
--rw-r--r--   0 krj        (502) staff       (20)      934 2024-02-02 14:11:38.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/product/liste_produkt_numpy_2_input.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.788834 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/reversert/
--rw-r--r--   0 krj        (502) staff       (20)      322 2024-02-02 14:11:38.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/reversert/liste_reversert_1.py
--rw-r--r--   0 krj        (502) staff       (20)      942 2024-02-02 14:11:38.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/reversert/liste_reversert_2_input_int.py
--rw-r--r--   0 krj        (502) staff       (20)      465 2024-02-02 14:11:38.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/reversert/liste_reversert_copy_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1032 2024-02-02 14:11:39.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/reversert/liste_reversert_copy_2_input_int.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.789354 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/rotate/
--rw-r--r--   0 krj        (502) staff       (20)     1835 2024-02-02 14:11:39.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/rotate/liste_rotasjon_int_1.py
--rw-r--r--   0 krj        (502) staff       (20)     2450 2024-02-02 14:11:39.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/rotate/liste_rotasjon_int_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)     1860 2024-02-02 14:11:39.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/rotate/liste_rotasjon_str_1.py
--rw-r--r--   0 krj        (502) staff       (20)     2629 2024-02-02 14:11:39.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/rotate/liste_rotasjon_str_2_input.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.790081 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/sum/
--rw-r--r--   0 krj        (502) staff       (20)      242 2024-02-02 14:11:39.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/sum/liste_sum_1_int.py
--rw-r--r--   0 krj        (502) staff       (20)      864 2024-02-02 14:11:39.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/sum/liste_sum_2_input_int.py
--rw-r--r--   0 krj        (502) staff       (20)      417 2024-02-02 14:11:39.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/sum/liste_sum_for_1_int.py
--rw-r--r--   0 krj        (502) staff       (20)     1039 2024-02-02 14:11:39.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/sum/liste_sum_for_2_input_int.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.756674 matematikk-0.0.98/src/matematikk/python/programmer/datatype/str/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.790364 matematikk-0.0.98/src/matematikk/python/programmer/datatype/str/ascii/
--rw-r--r--   0 krj        (502) staff       (20)      477 2024-02-02 14:11:39.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/str/ascii/ascii_1.py
--rw-r--r--   0 krj        (502) staff       (20)      485 2024-02-02 14:11:39.000000 matematikk-0.0.98/src/matematikk/python/programmer/datatype/str/ascii/ascii_2_input.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.756836 matematikk-0.0.98/src/matematikk/python/programmer/economics/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.790622 matematikk-0.0.98/src/matematikk/python/programmer/economics/rente/
--rw-r--r--   0 krj        (502) staff       (20)      607 2024-02-02 14:11:39.000000 matematikk-0.0.98/src/matematikk/python/programmer/economics/rente/rente_opptjent_1.py
--rw-r--r--   0 krj        (502) staff       (20)      694 2024-02-02 14:11:39.000000 matematikk-0.0.98/src/matematikk/python/programmer/economics/rente/rente_opptjent_2_input.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.758115 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.757256 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/aritmetikk/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.757170 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/aritmetikk/addisjon/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.791190 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/aritmetikk/addisjon/to_tall/
--rw-r--r--   0 krj        (502) staff       (20)      289 2024-02-02 14:11:39.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/aritmetikk/addisjon/to_tall/addisjon_to_tall_1.py
--rw-r--r--   0 krj        (502) staff       (20)      318 2024-02-02 14:11:39.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/aritmetikk/addisjon/to_tall/addisjon_to_tall_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)      172 2024-02-02 14:11:40.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/aritmetikk/addisjon/to_tall/addisjon_to_tall_enkel_1.py
--rw-r--r--   0 krj        (502) staff       (20)      247 2024-02-02 14:11:40.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/aritmetikk/addisjon/to_tall/addisjon_to_tall_enkel_2_input.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.791729 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/aritmetikk/siffer/
--rw-r--r--   0 krj        (502) staff       (20)      689 2024-02-02 14:11:40.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/aritmetikk/siffer/siffer_antall_divisjon_1.py
--rw-r--r--   0 krj        (502) staff       (20)      679 2024-02-02 14:11:40.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/aritmetikk/siffer/siffer_antall_divisjon_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)      397 2024-02-02 14:11:40.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/aritmetikk/siffer/siffer_antall_len_1.py
--rw-r--r--   0 krj        (502) staff       (20)      407 2024-02-02 14:11:40.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/aritmetikk/siffer/siffer_antall_len_2_input.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.757431 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/geometri/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.792729 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/geometri/sirkel/
--rw-r--r--   0 krj        (502) staff       (20)      314 2024-02-02 14:11:40.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/geometri/sirkel/sirkel_areal_r_eksponent_1.py
--rw-r--r--   0 krj        (502) staff       (20)      349 2024-02-02 14:11:40.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/geometri/sirkel/sirkel_areal_r_eksponent_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)      351 2024-02-02 14:11:40.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/geometri/sirkel/sirkel_areal_r_enhet_eksponent_1.py
--rw-r--r--   0 krj        (502) staff       (20)      399 2024-02-02 14:11:40.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/geometri/sirkel/sirkel_areal_r_enhet_eksponent_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)      370 2024-02-02 14:11:40.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/geometri/sirkel/sirkel_areal_r_enhet_math_1.py
--rw-r--r--   0 krj        (502) staff       (20)      411 2024-02-02 14:11:40.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/geometri/sirkel/sirkel_areal_r_enhet_math_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)      334 2024-02-02 14:11:40.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/geometri/sirkel/sirkel_areal_r_math_1.py
--rw-r--r--   0 krj        (502) staff       (20)      361 2024-02-02 14:11:40.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/geometri/sirkel/sirkel_areal_r_math_2_input.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.757859 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/matrise/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.792852 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/matrise/produkt/
--rw-r--r--   0 krj        (502) staff       (20)      570 2024-02-02 14:11:41.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/matrise/produkt/matrise_produkt.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.792962 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/matrise/subtraksjon/
--rw-r--r--   0 krj        (502) staff       (20)      446 2024-02-02 14:11:41.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/matrise/subtraksjon/matrise_subtraksjon.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.793066 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/matrise/sum/
--rw-r--r--   0 krj        (502) staff       (20)      431 2024-02-02 14:11:41.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/matrise/sum/matrise_sum.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.793298 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/matrise/transpose/
--rw-r--r--   0 krj        (502) staff       (20)      322 2024-02-02 14:11:41.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/matrise/transpose/matrise_transponering.py
--rw-r--r--   0 krj        (502) staff       (20)      444 2024-02-02 14:11:41.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/matrise/transpose/matrise_transponering_array.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.758047 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/rekke/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.793717 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/rekke/kube/
--rw-r--r--   0 krj        (502) staff       (20)      433 2024-02-02 14:11:41.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/rekke/kube/rekke_n_kuber_for_1.py
--rw-r--r--   0 krj        (502) staff       (20)      457 2024-02-02 14:11:41.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/rekke/kube/rekke_n_kuber_for_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)      359 2024-02-02 14:11:41.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/rekke/kube/rekke_n_kuber_formel_1.py
--rw-r--r--   0 krj        (502) staff       (20)      429 2024-02-02 14:11:41.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/rekke/kube/rekke_n_kuber_formel_2_input.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.794265 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/rekke/kvadrat/
--rw-r--r--   0 krj        (502) staff       (20)      457 2024-02-02 14:11:41.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/rekke/kvadrat/rekke_n_kvadrater_for_1.py
--rw-r--r--   0 krj        (502) staff       (20)      485 2024-02-02 14:11:41.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/rekke/kvadrat/rekke_n_kvadrater_for_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)      445 2024-02-02 14:11:41.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/rekke/kvadrat/rekke_n_kvadrater_formel_1.py
--rw-r--r--   0 krj        (502) staff       (20)      472 2024-02-02 14:11:41.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/rekke/kvadrat/rekke_n_kvadrater_formel_2_input.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.758678 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.794959 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/
--rw-r--r--   0 krj        (502) staff       (20)     1479 2024-02-02 14:11:41.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_ja_nei_intervall_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1511 2024-02-02 14:11:42.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_ja_nei_intervall_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)     1350 2024-02-02 14:11:42.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_ja_nei_n_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1389 2024-02-02 14:11:42.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_ja_nei_n_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)     1523 2024-02-02 14:11:42.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_liste_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1555 2024-02-02 14:11:42.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_liste_2_input.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.796740 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/
--rw-r--r--   0 krj        (502) staff       (20)     1081 2024-02-02 14:11:42.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_for_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1126 2024-02-02 14:11:42.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_for_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)     1152 2024-02-02 14:11:42.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_newton_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1197 2024-02-02 14:11:42.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_newton_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)      927 2024-02-02 14:11:42.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_rekursiv_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1040 2024-02-02 14:11:42.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_rekursiv_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)     1816 2024-02-02 14:11:42.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_ja_nei_intervall_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1825 2024-02-02 14:11:42.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_ja_nei_intervall_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)     1560 2024-02-02 14:11:42.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_ja_nei_n_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1599 2024-02-02 14:11:42.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_ja_nei_n_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)     1162 2024-02-02 14:11:43.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_liste_rekursiv_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1179 2024-02-02 14:11:43.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_liste_rekursiv_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)     1352 2024-02-02 14:11:43.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_lister_rekursiv_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1371 2024-02-02 14:11:43.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_lister_rekursiv_2_input.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.758345 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/figurtall/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.796860 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/figurtall/pyramide/
--rw-r--r--   0 krj        (502) staff       (20)      943 2024-02-02 14:11:43.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/figurtall/pyramide/pyramide.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.797092 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/negative_tall/
--rw-r--r--   0 krj        (502) staff       (20)      612 2024-02-02 14:11:43.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/negative_tall/negative_tall_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1222 2024-02-02 14:11:43.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/negative_tall/negative_tall_2_input_int.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.797317 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/oddetall/
--rw-r--r--   0 krj        (502) staff       (20)      599 2024-02-02 14:11:43.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/oddetall/oddetall_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1202 2024-02-02 14:11:43.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/oddetall/oddetall_2_input.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.797523 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/partall/
--rw-r--r--   0 krj        (502) staff       (20)      589 2024-02-02 14:11:43.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/partall/partall_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1191 2024-02-02 14:11:43.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/partall/partall_2_input.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.797734 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/positive_tall/
--rw-r--r--   0 krj        (502) staff       (20)      612 2024-02-02 14:11:43.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/positive_tall/positive_tall_1.py
--rw-r--r--   0 krj        (502) staff       (20)     1222 2024-02-02 14:11:43.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/positive_tall/positive_tall_2_input_int.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.799191 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/
--rw-r--r--   0 krj        (502) staff       (20)      847 2024-02-02 14:11:43.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_intervall_1.py
--rw-r--r--   0 krj        (502) staff       (20)      883 2024-02-02 14:11:43.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_intervall_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)      808 2024-02-02 14:11:44.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_math_intervall_1.py
--rw-r--r--   0 krj        (502) staff       (20)      844 2024-02-02 14:11:44.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_math_intervall_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)      801 2024-02-02 14:11:44.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_math_n_1.py
--rw-r--r--   0 krj        (502) staff       (20)      823 2024-02-02 14:11:44.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_math_n_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)      835 2024-02-02 14:11:44.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_n_1.py
--rw-r--r--   0 krj        (502) staff       (20)      865 2024-02-02 14:11:44.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_n_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)      937 2024-02-02 14:11:44.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_liste_intervall_1.py
--rw-r--r--   0 krj        (502) staff       (20)      972 2024-02-02 14:11:44.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_liste_intervall_2_input.py
--rw-r--r--   0 krj        (502) staff       (20)      895 2024-02-02 14:11:44.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_liste_math_1.py
--rw-r--r--   0 krj        (502) staff       (20)      930 2024-02-02 14:11:44.000000 matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_liste_math_2_input.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.758811 matematikk-0.0.98/src/matematikk/python/tutorial/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.760047 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.799311 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/_def/
--rw-r--r--   0 krj        (502) staff       (20)      129 2024-02-02 14:11:44.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/_def/variabel_def.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.759977 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.799785 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/_def/
--rw-r--r--   0 krj        (502) staff       (20)      139 2024-02-02 14:11:44.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/_def/datatype_def.py
--rw-r--r--   0 krj        (502) staff       (20)      242 2024-02-02 14:11:46.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/_def/datatype_int_type_cast.py
--rw-r--r--   0 krj        (502) staff       (20)      998 2024-02-02 14:11:45.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/_def/datatype_oversikt.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.800180 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/bool/
--rw-r--r--   0 krj        (502) staff       (20)      167 2024-02-02 14:11:45.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/bool/datatype_bool_def.py
--rw-r--r--   0 krj        (502) staff       (20)      161 2024-02-02 14:11:45.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/bool/datatype_bool_none.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.800355 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/bytearray/
--rw-r--r--   0 krj        (502) staff       (20)      106 2024-02-02 14:11:45.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/bytearray/datatype_bytearray_def.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.800525 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/bytes/
--rw-r--r--   0 krj        (502) staff       (20)       98 2024-02-02 14:11:45.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/bytes/datatype_bytes_def.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.800661 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/complex/
--rw-r--r--   0 krj        (502) staff       (20)      281 2024-02-02 14:11:45.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/complex/datatype_complex_def.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.801286 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/dict/
--rw-r--r--   0 krj        (502) staff       (20)      293 2024-02-02 14:11:45.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/dict/datatype_dict_change.py
--rw-r--r--   0 krj        (502) staff       (20)      113 2024-02-02 14:11:45.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/dict/datatype_dict_def.py
--rw-r--r--   0 krj        (502) staff       (20)      303 2024-02-02 14:11:45.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/dict/datatype_dict_felt.py
--rw-r--r--   0 krj        (502) staff       (20)      201 2024-02-02 14:11:45.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/dict/datatype_dict_key_value.py
--rw-r--r--   0 krj        (502) staff       (20)      453 2024-02-02 14:11:45.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/dict/datatype_dict_multi.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.801413 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/float/
--rw-r--r--   0 krj        (502) staff       (20)      110 2024-02-02 14:11:45.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/float/datatype_float_def.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.801527 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/frozenset/
--rw-r--r--   0 krj        (502) staff       (20)      338 2024-02-02 14:11:46.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/frozenset/datatype_frozenset_add.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.801642 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/int/
--rw-r--r--   0 krj        (502) staff       (20)      110 2024-02-02 14:11:46.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/int/datatype_int_def.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.802239 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/list/
--rw-r--r--   0 krj        (502) staff       (20)      134 2024-02-02 14:11:46.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/list/datatype_list_def.py
--rw-r--r--   0 krj        (502) staff       (20)      222 2024-02-02 14:11:46.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/list/datatype_list_for_1_indeks.py
--rw-r--r--   0 krj        (502) staff       (20)      215 2024-02-02 14:11:46.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/list/datatype_list_for_2_el.py
--rw-r--r--   0 krj        (502) staff       (20)      184 2024-02-02 14:11:46.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/list/datatype_list_indeks.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.802353 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/memoryview/
--rw-r--r--   0 krj        (502) staff       (20)      101 2024-02-02 14:11:46.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/memoryview/datatype_memoryview_def.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.802476 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/nonetype/
--rw-r--r--   0 krj        (502) staff       (20)      322 2024-02-02 14:11:46.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/nonetype/datatype_nonetype_def.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.802923 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/range/
--rw-r--r--   0 krj        (502) staff       (20)      202 2024-02-02 14:11:46.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/range/datatype_range_1.py
--rw-r--r--   0 krj        (502) staff       (20)      220 2024-02-02 14:11:46.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/range/datatype_range_2_kort.py
--rw-r--r--   0 krj        (502) staff       (20)      234 2024-02-02 14:11:46.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/range/datatype_range_inkludert.py
--rw-r--r--   0 krj        (502) staff       (20)      265 2024-02-02 14:11:46.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/range/datatype_range_steg.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.803243 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/set/
--rw-r--r--   0 krj        (502) staff       (20)      285 2024-02-02 14:11:47.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/set/datatype_set_add.py
--rw-r--r--   0 krj        (502) staff       (20)      133 2024-02-02 14:11:47.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/set/datatype_set_def.py
--rw-r--r--   0 krj        (502) staff       (20)      291 2024-02-02 14:11:47.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/set/datatype_set_remove.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.804328 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/str/
--rw-r--r--   0 krj        (502) staff       (20)      259 2024-02-02 14:11:47.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_bokstav_1.py
--rw-r--r--   0 krj        (502) staff       (20)      248 2024-02-02 14:11:47.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_bokstav_2_for_indeks.py
--rw-r--r--   0 krj        (502) staff       (20)      237 2024-02-02 14:11:47.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_bokstav_3_for.py
--rw-r--r--   0 krj        (502) staff       (20)       98 2024-02-02 14:11:47.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_def.py
--rw-r--r--   0 krj        (502) staff       (20)      153 2024-02-02 14:11:47.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_emoji.py
--rw-r--r--   0 krj        (502) staff       (20)      134 2024-02-02 14:11:47.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_escape_char.py
--rw-r--r--   0 krj        (502) staff       (20)      191 2024-02-02 14:11:47.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_escape_char_oversikt.py
--rw-r--r--   0 krj        (502) staff       (20)      451 2024-02-02 14:11:47.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_hermetegn.py
--rw-r--r--   0 krj        (502) staff       (20)      219 2024-02-02 14:11:47.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_len.py
--rw-r--r--   0 krj        (502) staff       (20)      124 2024-02-02 14:11:47.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_unicode.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.804436 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/tuple/
--rw-r--r--   0 krj        (502) staff       (20)      219 2024-02-02 14:11:48.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/tuple/datatype_tuple_def.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.804754 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/variabelnavn/
--rw-r--r--   0 krj        (502) staff       (20)      289 2024-02-02 14:11:48.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/variabelnavn/variabelnavn_case.py
--rw-r--r--   0 krj        (502) staff       (20)      212 2024-02-02 14:11:48.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/variabelnavn/variabelnavn_gyldig.py
--rw-r--r--   0 krj        (502) staff       (20)      220 2024-02-02 14:11:48.000000 matematikk-0.0.98/src/matematikk/python/tutorial/variabel/variabelnavn/variabelnavn_ugyldig.py
--rw-r--r--   0 krj        (502) staff       (20)     4661 2024-02-02 14:11:29.000000 matematikk-0.0.98/src/matematikk/superløs_fil.py
-drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:12:14.804967 matematikk-0.0.98/src/matematikk.egg-info/
--rw-r--r--   0 krj        (502) staff       (20)      625 2024-02-02 14:12:14.000000 matematikk-0.0.98/src/matematikk.egg-info/PKG-INFO
--rw-r--r--   0 krj        (502) staff       (20)    22140 2024-02-02 14:12:14.000000 matematikk-0.0.98/src/matematikk.egg-info/SOURCES.txt
--rw-r--r--   0 krj        (502) staff       (20)        1 2024-02-02 14:12:14.000000 matematikk-0.0.98/src/matematikk.egg-info/dependency_links.txt
--rw-r--r--   0 krj        (502) staff       (20)       11 2024-02-02 14:12:14.000000 matematikk-0.0.98/src/matematikk.egg-info/top_level.txt
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.601415 matematikk-0.0.99/
+-rw-r--r--   0 krj        (502) staff       (20)     1073 2024-02-02 07:00:53.000000 matematikk-0.0.99/LICENCE
+-rw-r--r--   0 krj        (502) staff       (20)      625 2024-02-02 14:17:18.601144 matematikk-0.0.99/PKG-INFO
+-rw-r--r--   0 krj        (502) staff       (20)      170 2024-02-02 07:00:53.000000 matematikk-0.0.99/README.md
+-rw-r--r--   0 krj        (502) staff       (20)      435 2024-02-02 14:17:03.000000 matematikk-0.0.99/pyproject.toml
+-rw-r--r--   0 krj        (502) staff       (20)       38 2024-02-02 14:17:18.601458 matematikk-0.0.99/setup.cfg
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.541843 matematikk-0.0.99/src/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.550751 matematikk-0.0.99/src/matematikk/
+-rw-r--r--   0 krj        (502) staff       (20)     1632 2024-02-02 14:16:41.000000 matematikk-0.0.99/src/matematikk/__init__.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.541961 matematikk-0.0.99/src/matematikk/_ch_1/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.542006 matematikk-0.0.99/src/matematikk/_ch_1/ch_2/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.551625 matematikk-0.0.99/src/matematikk/_ch_1/ch_2/ch_3/
+-rw-r--r--   0 krj        (502) staff       (20)      252 2024-02-02 14:16:41.000000 matematikk-0.0.99/src/matematikk/_ch_1/ch_2/ch_3/ch_4_fil.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.551734 matematikk-0.0.99/src/matematikk/eksamen/
+-rw-r--r--   0 krj        (502) staff       (20)      861 2024-02-02 14:16:41.000000 matematikk-0.0.99/src/matematikk/eksamen/oppg_test.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.548465 matematikk-0.0.99/src/matematikk/python/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.542629 matematikk-0.0.99/src/matematikk/python/eksamen/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.542454 matematikk-0.0.99/src/matematikk/python/eksamen/1t/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.542336 matematikk-0.0.99/src/matematikk/python/eksamen/1t/2022_h/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.542381 matematikk-0.0.99/src/matematikk/python/eksamen/1t/2022_h/del_1/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.552561 matematikk-0.0.99/src/matematikk/python/eksamen/1t/2022_h/del_1/03/
+-rw-r--r--   0 krj        (502) staff       (20)      254 2024-02-02 14:16:41.000000 matematikk-0.0.99/src/matematikk/python/eksamen/1t/2022_h/del_1/03/oppg_3_a_rasjonal_funksjon_bug.py
+-rw-r--r--   0 krj        (502) staff       (20)      310 2024-02-02 14:16:42.000000 matematikk-0.0.99/src/matematikk/python/eksamen/1t/2022_h/del_1/03/oppg_3_b_rasjonal_funksjon_if.py
+-rw-r--r--   0 krj        (502) staff       (20)      298 2024-02-02 14:16:42.000000 matematikk-0.0.99/src/matematikk/python/eksamen/1t/2022_h/del_1/03/oppg_3_b_rasjonal_funksjon_if_else.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.542509 matematikk-0.0.99/src/matematikk/python/eksamen/1t/2022_v/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.542558 matematikk-0.0.99/src/matematikk/python/eksamen/1t/2022_v/del_1/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.552714 matematikk-0.0.99/src/matematikk/python/eksamen/1t/2022_v/del_1/04/
+-rw-r--r--   0 krj        (502) staff       (20)      273 2024-02-02 14:16:42.000000 matematikk-0.0.99/src/matematikk/python/eksamen/1t/2022_v/del_1/04/oppg_4_kvadrattall.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.543602 matematikk-0.0.99/src/matematikk/python/eksamen/s1/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.542960 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.542836 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_1/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.552960 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_1/05/
+-rw-r--r--   0 krj        (502) staff       (20)      262 2024-02-02 14:16:42.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_1/05/oppg_5_grensekostnad.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.543505 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.556222 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/
+-rw-r--r--   0 krj        (502) staff       (20)     2856 2024-02-02 14:16:42.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_1_sofa_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     3564 2024-02-02 14:16:42.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_2_sofa_def_reggis_str_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     3497 2024-02-02 14:16:42.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_3_sofa_def_reggis_cas_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     1935 2024-02-02 14:16:42.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_4_sofa_matematikk_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)      577 2024-02-02 14:16:42.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_5_sofa_matematikk_speedrun_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     4672 2024-02-02 14:16:42.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_1_sofa_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     8632 2024-02-02 14:16:42.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_2_sofa_def_superlos_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     2883 2024-02-02 14:16:43.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_3_sofa_matematikk_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     3276 2024-02-02 14:16:43.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_4_sofa_def_overskudd_max_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     3798 2024-02-02 14:16:43.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_5_sofa_abstrahering_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     2759 2024-02-02 14:16:43.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_6_sofa_matematikk_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)      806 2024-02-02 14:16:43.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_7_sofa_matematikk_speedrun_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     7323 2024-02-02 14:16:43.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_c_sofa_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)      436 2024-02-02 14:16:43.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/02_oppg_1_a_sofa_torodd.py
+-rw-r--r--   0 krj        (502) staff       (20)      483 2024-02-02 14:16:43.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/02_oppg_1_b_sofa_torodd.py
+-rw-r--r--   0 krj        (502) staff       (20)     1211 2024-02-02 14:16:43.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/02_oppg_1_c_sofa_torodd.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.557754 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/02/
+-rw-r--r--   0 krj        (502) staff       (20)     1885 2024-02-02 14:16:43.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/02/01_oppg_2_a_venstrehendte_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     4382 2024-02-02 14:16:43.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/02/01_oppg_2_b_1_venstrehendte_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     5738 2024-02-02 14:16:43.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/02/01_oppg_2_b_2_venstrehendte_relasjoner_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     3936 2024-02-02 14:16:44.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/02/01_oppg_2_c_venstrehendte_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)      486 2024-02-02 14:16:44.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/02/02_oppg_2_a_venstrehendte_torodd.py
+-rw-r--r--   0 krj        (502) staff       (20)      603 2024-02-02 14:16:44.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/02/02_oppg_2_b_venstrehendte_torodd.py
+-rw-r--r--   0 krj        (502) staff       (20)      644 2024-02-02 14:16:44.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/02/02_oppg_2_c_venstrehendte_torodd.py
+-rw-r--r--   0 krj        (502) staff       (20)    17344 2024-02-02 14:16:43.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/02/mal_sannsynlighets_relasjoner_mas.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.559634 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/03/
+-rw-r--r--   0 krj        (502) staff       (20)     2846 2024-02-02 14:16:44.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_a_sparekonto_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     4982 2024-02-02 14:16:44.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_b_sparekonto_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     6361 2024-02-02 14:16:44.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_c_1_sparekonto_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     9428 2024-02-02 14:16:44.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_c_2_sparekonto_superlos_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     5275 2024-02-02 14:16:44.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_c_3_sparekonto_matematikk_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)      383 2024-02-02 14:16:44.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/03/02_oppg_3_a_sparekonto_torodd.py
+-rw-r--r--   0 krj        (502) staff       (20)      549 2024-02-02 14:16:44.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/03/02_oppg_3_b_sparekonto_torodd.py
+-rw-r--r--   0 krj        (502) staff       (20)      385 2024-02-02 14:16:44.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/03/02_oppg_3_c_sparekonto_torodd.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.560841 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/04/
+-rw-r--r--   0 krj        (502) staff       (20)     2399 2024-02-02 14:16:44.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/04/01_oppg_4_a_terninger_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     4765 2024-02-02 14:16:45.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/04/01_oppg_4_b_terninger_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     6243 2024-02-02 14:16:45.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/04/01_oppg_4_c_terninger_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)      327 2024-02-02 14:16:45.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/04/02_oppg_4_a_terninger_torodd.py
+-rw-r--r--   0 krj        (502) staff       (20)      600 2024-02-02 14:16:45.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/04/02_oppg_4_b_terninger_torodd.py
+-rw-r--r--   0 krj        (502) staff       (20)      518 2024-02-02 14:16:45.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/04/02_oppg_4_c_terninger_torodd.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.563258 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/05/
+-rw-r--r--   0 krj        (502) staff       (20)     2060 2024-02-02 14:16:45.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_a_1_prisme_geometrisk_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     2835 2024-02-02 14:16:45.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_a_2_prisme_likning_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     6114 2024-02-02 14:16:45.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_a_3_prisme_likning_superlos_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     8802 2024-02-02 14:16:45.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_b_prisme_likning_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)    11004 2024-02-02 14:16:45.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_c_prisme_likning_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)      460 2024-02-02 14:16:45.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/05/02_oppg_5_a_prisme_likning_torodd.py
+-rw-r--r--   0 krj        (502) staff       (20)      460 2024-02-02 14:16:45.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/05/02_oppg_5_b_prisme_likning_torodd.py
+-rw-r--r--   0 krj        (502) staff       (20)      460 2024-02-02 14:16:45.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/05/02_oppg_5_c_prisme_likning_torodd.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.564548 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/06/
+-rw-r--r--   0 krj        (502) staff       (20)     8905 2024-02-02 14:16:45.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/06/01_oppg_6_a_tredjegradsfunksjon_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)    11517 2024-02-02 14:16:46.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/06/01_oppg_6_b_tredjegradsfunksjon_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)    13330 2024-02-02 14:16:46.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/06/01_oppg_6_c_tredjegradsfunksjon_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)      579 2024-02-02 14:16:46.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/06/02_oppg_6_a_tredjegradsfunksjon_torodd.py
+-rw-r--r--   0 krj        (502) staff       (20)      422 2024-02-02 14:16:46.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/06/02_oppg_6_b_tredjegradsfunksjon_torodd.py
+-rw-r--r--   0 krj        (502) staff       (20)      669 2024-02-02 14:16:46.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/06/02_oppg_6_c_tredjegradsfunksjon_torodd.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.543662 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_v/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.543712 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_v/del_2/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.564926 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_v/del_2/01/
+-rw-r--r--   0 krj        (502) staff       (20)     6795 2024-02-02 14:16:42.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_v/del_2/01/01_oppg_1_a_timelonn_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     6792 2024-02-02 14:16:42.000000 matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_v/del_2/01/01_oppg_1_b_timelonn_mas.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.543870 matematikk-0.0.99/src/matematikk/python/funksjoner/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.544219 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.543974 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/funksjoner/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.544023 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.565602 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/
+-rw-r--r--   0 krj        (502) staff       (20)      840 2024-02-02 14:16:46.000000 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/def_ekstremalpunkt_max_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)      840 2024-02-02 14:16:46.000000 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/def_ekstremalpunkt_max_matematikk_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     1005 2024-02-02 14:16:46.000000 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/def_overskudd_max_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     1008 2024-02-02 14:16:46.000000 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/def_overskudd_max_matematikk_mas.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.544140 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/likninger/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.566002 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/likninger/superlos/
+-rw-r--r--   0 krj        (502) staff       (20)     4251 2024-02-02 14:16:46.000000 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/likninger/superlos/def_superlos_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     4624 2024-02-02 14:16:46.000000 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/likninger/superlos/def_superlos_matematikk_mas.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.544271 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/regresjon/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.544326 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/regresjon/polynom/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.566365 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/regresjon/polynom/reggis/
+-rw-r--r--   0 krj        (502) staff       (20)     1641 2024-02-02 14:16:46.000000 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/regresjon/polynom/reggis/def_reggis_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     1963 2024-02-02 14:16:46.000000 matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/regresjon/polynom/reggis/def_reggis_matematikk_mas.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.544481 matematikk-0.0.99/src/matematikk/python/oppgaver/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.544541 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.544908 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.566809 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_55/
+-rw-r--r--   0 krj        (502) staff       (20)     4045 2024-02-02 14:16:47.000000 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_55/01_oppg_1_55_vanjas_scooter_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     4023 2024-02-02 14:16:47.000000 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_55/02_oppg_1_55_vanjas_scooter_input_mas.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.566980 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_56/
+-rw-r--r--   0 krj        (502) staff       (20)     3765 2024-02-02 14:16:47.000000 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_56/oppg_1_56_elbiler_mas.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.567190 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_57/
+-rw-r--r--   0 krj        (502) staff       (20)     3850 2024-02-02 14:16:47.000000 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_57/oppg_1_57_hus_og_elbiler_mas.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.568026 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/
+-rw-r--r--   0 krj        (502) staff       (20)      342 2024-02-02 14:16:46.000000 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/01_eks_1_5_a_b_vindpark_bok.py
+-rw-r--r--   0 krj        (502) staff       (20)     1749 2024-02-02 14:16:47.000000 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/02_eks_1_5_a_b_vindpark_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)      474 2024-02-02 14:16:47.000000 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/03_eks_1_5_a_b_vindpark_input_bok.py
+-rw-r--r--   0 krj        (502) staff       (20)     2109 2024-02-02 14:16:47.000000 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/04_eks_1_5_a_b_vindpark_input_mas.py
+-rw-r--r--   0 krj        (502) staff       (20)     3485 2024-02-02 14:16:47.000000 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/05_oppg_1_59_vindpark_mas.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.568183 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/9/
+-rw-r--r--   0 krj        (502) staff       (20)     3657 2024-02-02 14:16:47.000000 matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/9/oppg_k_1_9_pythagoras_mas.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.546663 matematikk-0.0.99/src/matematikk/python/programmer/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.546413 matematikk-0.0.99/src/matematikk/python/programmer/datatype/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.546332 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.568960 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/antall/
+-rw-r--r--   0 krj        (502) staff       (20)      363 2024-02-02 14:16:47.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/antall/liste_count_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1156 2024-02-02 14:16:47.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/antall/liste_count_2_input_str.py
+-rw-r--r--   0 krj        (502) staff       (20)      296 2024-02-02 14:16:47.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/antall/liste_length_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1056 2024-02-02 14:16:47.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/antall/liste_length_2_input_str.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.569104 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/change/
+-rw-r--r--   0 krj        (502) staff       (20)      394 2024-02-02 14:16:47.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/change/liste_bytt_el.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.570541 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/copy/
+-rw-r--r--   0 krj        (502) staff       (20)      234 2024-02-02 14:16:48.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/copy/liste_copy.py
+-rw-r--r--   0 krj        (502) staff       (20)      236 2024-02-02 14:16:48.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/copy/liste_copy_assignment.py
+-rw-r--r--   0 krj        (502) staff       (20)      247 2024-02-02 14:16:48.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/copy/liste_copy_comprehension.py
+-rw-r--r--   0 krj        (502) staff       (20)      754 2024-02-02 14:16:48.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/copy/liste_copy_deepcopy.py
+-rw-r--r--   0 krj        (502) staff       (20)      431 2024-02-02 14:16:48.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/copy/liste_copy_extend.py
+-rw-r--r--   0 krj        (502) staff       (20)      268 2024-02-02 14:16:48.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/copy/liste_copy_extend_kort.py
+-rw-r--r--   0 krj        (502) staff       (20)      429 2024-02-02 14:16:48.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/copy/liste_copy_slice.py
+-rw-r--r--   0 krj        (502) staff       (20)      242 2024-02-02 14:16:48.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/copy/liste_copy_slice_kort.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.571344 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/delete/
+-rw-r--r--   0 krj        (502) staff       (20)      235 2024-02-02 14:16:48.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/delete/liste_delete.py
+-rw-r--r--   0 krj        (502) staff       (20)      644 2024-02-02 14:16:48.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/delete/liste_remove_negative_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1250 2024-02-02 14:16:48.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/delete/liste_remove_negative_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)      644 2024-02-02 14:16:48.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/delete/liste_remove_positive_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1250 2024-02-02 14:16:48.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/delete/liste_remove_positive_2_input.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.572124 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/eksisterer/
+-rw-r--r--   0 krj        (502) staff       (20)      327 2024-02-02 14:16:48.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/eksisterer/liste_eksisterer_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1119 2024-02-02 14:16:49.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/eksisterer/liste_eksisterer_2_input_str.py
+-rw-r--r--   0 krj        (502) staff       (20)      352 2024-02-02 14:16:49.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/eksisterer/liste_eksisterer_for_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1404 2024-02-02 14:16:49.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/eksisterer/liste_eksisterer_for_2_input_str.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.572872 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/max/
+-rw-r--r--   0 krj        (502) staff       (20)      579 2024-02-02 14:16:49.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/max/liste_max_for_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1195 2024-02-02 14:16:49.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/max/liste_max_for_2_input_int.py
+-rw-r--r--   0 krj        (502) staff       (20)      473 2024-02-02 14:16:49.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/max/liste_max_sort_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1086 2024-02-02 14:16:49.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/max/liste_max_sort_2_input_int.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.573608 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/min/
+-rw-r--r--   0 krj        (502) staff       (20)      568 2024-02-02 14:16:49.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/min/liste_min_for_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1185 2024-02-02 14:16:49.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/min/liste_min_for_2_input_int.py
+-rw-r--r--   0 krj        (502) staff       (20)      507 2024-02-02 14:16:49.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/min/liste_min_sort_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1121 2024-02-02 14:16:49.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/min/liste_min_sort_2_input_int.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.574621 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/monotonic/
+-rw-r--r--   0 krj        (502) staff       (20)      702 2024-02-02 14:16:49.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_all_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1274 2024-02-02 14:16:49.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_all_2_input_int.py
+-rw-r--r--   0 krj        (502) staff       (20)      995 2024-02-02 14:16:49.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_sort_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1569 2024-02-02 14:16:49.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_sort_2_input_int.py
+-rw-r--r--   0 krj        (502) staff       (20)     1251 2024-02-02 14:16:50.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_sort_3_to.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.576359 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/
+-rw-r--r--   0 krj        (502) staff       (20)      849 2024-02-02 14:16:50.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_comprehension_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1524 2024-02-02 14:16:50.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_comprehension_2_input_str.py
+-rw-r--r--   0 krj        (502) staff       (20)      871 2024-02-02 14:16:50.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_for_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1525 2024-02-02 14:16:50.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_for_2_input_str.py
+-rw-r--r--   0 krj        (502) staff       (20)      760 2024-02-02 14:16:50.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_numpy_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1409 2024-02-02 14:16:50.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_numpy_2_input_str.py
+-rw-r--r--   0 krj        (502) staff       (20)      801 2024-02-02 14:16:50.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_yield_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1444 2024-02-02 14:16:50.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_yield_2_input_str.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.577567 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/product/
+-rw-r--r--   0 krj        (502) staff       (20)      463 2024-02-02 14:16:50.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/product/liste_produkt_for_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1094 2024-02-02 14:16:50.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/product/liste_produkt_for_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)      299 2024-02-02 14:16:50.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/product/liste_produkt_math_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      930 2024-02-02 14:16:50.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/product/liste_produkt_math_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)      303 2024-02-02 14:16:51.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/product/liste_produkt_numpy_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      934 2024-02-02 14:16:51.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/product/liste_produkt_numpy_2_input.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.578307 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/reversert/
+-rw-r--r--   0 krj        (502) staff       (20)      322 2024-02-02 14:16:51.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/reversert/liste_reversert_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      942 2024-02-02 14:16:51.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/reversert/liste_reversert_2_input_int.py
+-rw-r--r--   0 krj        (502) staff       (20)      465 2024-02-02 14:16:51.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/reversert/liste_reversert_copy_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1032 2024-02-02 14:16:51.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/reversert/liste_reversert_copy_2_input_int.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.579140 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/rotate/
+-rw-r--r--   0 krj        (502) staff       (20)     1835 2024-02-02 14:16:51.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/rotate/liste_rotasjon_int_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     2450 2024-02-02 14:16:51.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/rotate/liste_rotasjon_int_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)     1860 2024-02-02 14:16:51.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/rotate/liste_rotasjon_str_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     2629 2024-02-02 14:16:51.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/rotate/liste_rotasjon_str_2_input.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.579783 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/sum/
+-rw-r--r--   0 krj        (502) staff       (20)      242 2024-02-02 14:16:51.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/sum/liste_sum_1_int.py
+-rw-r--r--   0 krj        (502) staff       (20)      864 2024-02-02 14:16:51.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/sum/liste_sum_2_input_int.py
+-rw-r--r--   0 krj        (502) staff       (20)      417 2024-02-02 14:16:51.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/sum/liste_sum_for_1_int.py
+-rw-r--r--   0 krj        (502) staff       (20)     1039 2024-02-02 14:16:51.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/sum/liste_sum_for_2_input_int.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.546470 matematikk-0.0.99/src/matematikk/python/programmer/datatype/str/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.580173 matematikk-0.0.99/src/matematikk/python/programmer/datatype/str/ascii/
+-rw-r--r--   0 krj        (502) staff       (20)      477 2024-02-02 14:16:51.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/str/ascii/ascii_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      485 2024-02-02 14:16:52.000000 matematikk-0.0.99/src/matematikk/python/programmer/datatype/str/ascii/ascii_2_input.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.546588 matematikk-0.0.99/src/matematikk/python/programmer/economics/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.580557 matematikk-0.0.99/src/matematikk/python/programmer/economics/rente/
+-rw-r--r--   0 krj        (502) staff       (20)      607 2024-02-02 14:16:52.000000 matematikk-0.0.99/src/matematikk/python/programmer/economics/rente/rente_opptjent_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      694 2024-02-02 14:16:52.000000 matematikk-0.0.99/src/matematikk/python/programmer/economics/rente/rente_opptjent_2_input.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.547704 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.546870 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/aritmetikk/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.546804 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/aritmetikk/addisjon/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.581190 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/aritmetikk/addisjon/to_tall/
+-rw-r--r--   0 krj        (502) staff       (20)      289 2024-02-02 14:16:52.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/aritmetikk/addisjon/to_tall/addisjon_to_tall_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      318 2024-02-02 14:16:52.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/aritmetikk/addisjon/to_tall/addisjon_to_tall_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)      172 2024-02-02 14:16:52.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/aritmetikk/addisjon/to_tall/addisjon_to_tall_enkel_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      247 2024-02-02 14:16:52.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/aritmetikk/addisjon/to_tall/addisjon_to_tall_enkel_2_input.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.581983 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/aritmetikk/siffer/
+-rw-r--r--   0 krj        (502) staff       (20)      689 2024-02-02 14:16:52.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/aritmetikk/siffer/siffer_antall_divisjon_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      679 2024-02-02 14:16:52.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/aritmetikk/siffer/siffer_antall_divisjon_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)      397 2024-02-02 14:16:52.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/aritmetikk/siffer/siffer_antall_len_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      407 2024-02-02 14:16:52.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/aritmetikk/siffer/siffer_antall_len_2_input.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.547001 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/geometri/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.583462 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/geometri/sirkel/
+-rw-r--r--   0 krj        (502) staff       (20)      314 2024-02-02 14:16:52.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/geometri/sirkel/sirkel_areal_r_eksponent_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      349 2024-02-02 14:16:52.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/geometri/sirkel/sirkel_areal_r_eksponent_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)      351 2024-02-02 14:16:53.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/geometri/sirkel/sirkel_areal_r_enhet_eksponent_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      399 2024-02-02 14:16:53.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/geometri/sirkel/sirkel_areal_r_enhet_eksponent_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)      370 2024-02-02 14:16:53.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/geometri/sirkel/sirkel_areal_r_enhet_math_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      411 2024-02-02 14:16:53.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/geometri/sirkel/sirkel_areal_r_enhet_math_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)      334 2024-02-02 14:16:53.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/geometri/sirkel/sirkel_areal_r_math_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      361 2024-02-02 14:16:53.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/geometri/sirkel/sirkel_areal_r_math_2_input.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.547402 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/matrise/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.583684 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/matrise/produkt/
+-rw-r--r--   0 krj        (502) staff       (20)      570 2024-02-02 14:16:53.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/matrise/produkt/matrise_produkt.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.583857 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/matrise/subtraksjon/
+-rw-r--r--   0 krj        (502) staff       (20)      446 2024-02-02 14:16:53.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/matrise/subtraksjon/matrise_subtraksjon.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.584042 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/matrise/sum/
+-rw-r--r--   0 krj        (502) staff       (20)      431 2024-02-02 14:16:53.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/matrise/sum/matrise_sum.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.584448 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/matrise/transpose/
+-rw-r--r--   0 krj        (502) staff       (20)      322 2024-02-02 14:16:53.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/matrise/transpose/matrise_transponering.py
+-rw-r--r--   0 krj        (502) staff       (20)      444 2024-02-02 14:16:53.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/matrise/transpose/matrise_transponering_array.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.547623 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/rekke/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.585142 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/rekke/kube/
+-rw-r--r--   0 krj        (502) staff       (20)      433 2024-02-02 14:16:53.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/rekke/kube/rekke_n_kuber_for_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      457 2024-02-02 14:16:53.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/rekke/kube/rekke_n_kuber_for_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)      359 2024-02-02 14:16:54.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/rekke/kube/rekke_n_kuber_formel_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      429 2024-02-02 14:16:54.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/rekke/kube/rekke_n_kuber_formel_2_input.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.585836 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/rekke/kvadrat/
+-rw-r--r--   0 krj        (502) staff       (20)      457 2024-02-02 14:16:54.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/rekke/kvadrat/rekke_n_kvadrater_for_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      485 2024-02-02 14:16:54.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/rekke/kvadrat/rekke_n_kvadrater_for_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)      445 2024-02-02 14:16:54.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/rekke/kvadrat/rekke_n_kvadrater_formel_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      472 2024-02-02 14:16:54.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/rekke/kvadrat/rekke_n_kvadrater_formel_2_input.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.548375 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.586858 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/
+-rw-r--r--   0 krj        (502) staff       (20)     1479 2024-02-02 14:16:54.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_ja_nei_intervall_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1511 2024-02-02 14:16:54.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_ja_nei_intervall_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)     1350 2024-02-02 14:16:54.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_ja_nei_n_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1389 2024-02-02 14:16:54.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_ja_nei_n_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)     1523 2024-02-02 14:16:54.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_liste_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1555 2024-02-02 14:16:54.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_liste_2_input.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.589276 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/
+-rw-r--r--   0 krj        (502) staff       (20)     1081 2024-02-02 14:16:55.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_for_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1126 2024-02-02 14:16:55.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_for_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)     1152 2024-02-02 14:16:55.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_newton_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1197 2024-02-02 14:16:55.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_newton_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)      927 2024-02-02 14:16:55.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_rekursiv_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1040 2024-02-02 14:16:55.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_rekursiv_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)     1816 2024-02-02 14:16:55.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_ja_nei_intervall_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1825 2024-02-02 14:16:55.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_ja_nei_intervall_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)     1560 2024-02-02 14:16:55.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_ja_nei_n_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1599 2024-02-02 14:16:55.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_ja_nei_n_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)     1162 2024-02-02 14:16:55.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_liste_rekursiv_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1179 2024-02-02 14:16:55.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_liste_rekursiv_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)     1352 2024-02-02 14:16:55.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_lister_rekursiv_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1371 2024-02-02 14:16:56.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_lister_rekursiv_2_input.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.547982 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/figurtall/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.589456 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/figurtall/pyramide/
+-rw-r--r--   0 krj        (502) staff       (20)      943 2024-02-02 14:16:56.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/figurtall/pyramide/pyramide.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.589792 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/negative_tall/
+-rw-r--r--   0 krj        (502) staff       (20)      612 2024-02-02 14:16:56.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/negative_tall/negative_tall_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1222 2024-02-02 14:16:56.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/negative_tall/negative_tall_2_input_int.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.590101 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/oddetall/
+-rw-r--r--   0 krj        (502) staff       (20)      599 2024-02-02 14:16:56.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/oddetall/oddetall_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1202 2024-02-02 14:16:56.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/oddetall/oddetall_2_input.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.590453 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/partall/
+-rw-r--r--   0 krj        (502) staff       (20)      589 2024-02-02 14:16:56.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/partall/partall_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1191 2024-02-02 14:16:56.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/partall/partall_2_input.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.590894 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/positive_tall/
+-rw-r--r--   0 krj        (502) staff       (20)      612 2024-02-02 14:16:56.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/positive_tall/positive_tall_1.py
+-rw-r--r--   0 krj        (502) staff       (20)     1222 2024-02-02 14:16:56.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/positive_tall/positive_tall_2_input_int.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.593025 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/
+-rw-r--r--   0 krj        (502) staff       (20)      847 2024-02-02 14:16:56.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_intervall_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      883 2024-02-02 14:16:56.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_intervall_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)      808 2024-02-02 14:16:56.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_math_intervall_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      844 2024-02-02 14:16:56.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_math_intervall_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)      801 2024-02-02 14:16:57.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_math_n_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      823 2024-02-02 14:16:57.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_math_n_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)      835 2024-02-02 14:16:57.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_n_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      865 2024-02-02 14:16:57.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_n_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)      937 2024-02-02 14:16:57.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_liste_intervall_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      972 2024-02-02 14:16:57.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_liste_intervall_2_input.py
+-rw-r--r--   0 krj        (502) staff       (20)      895 2024-02-02 14:16:57.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_liste_math_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      930 2024-02-02 14:16:57.000000 matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_liste_math_2_input.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.548529 matematikk-0.0.99/src/matematikk/python/tutorial/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.549926 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.593203 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/_def/
+-rw-r--r--   0 krj        (502) staff       (20)      129 2024-02-02 14:16:57.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/_def/variabel_def.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.549861 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.593746 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/_def/
+-rw-r--r--   0 krj        (502) staff       (20)      139 2024-02-02 14:16:57.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/_def/datatype_def.py
+-rw-r--r--   0 krj        (502) staff       (20)      242 2024-02-02 14:16:58.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/_def/datatype_int_type_cast.py
+-rw-r--r--   0 krj        (502) staff       (20)      998 2024-02-02 14:16:57.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/_def/datatype_oversikt.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.594092 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/bool/
+-rw-r--r--   0 krj        (502) staff       (20)      167 2024-02-02 14:16:57.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/bool/datatype_bool_def.py
+-rw-r--r--   0 krj        (502) staff       (20)      161 2024-02-02 14:16:57.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/bool/datatype_bool_none.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.594338 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/bytearray/
+-rw-r--r--   0 krj        (502) staff       (20)      106 2024-02-02 14:16:57.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/bytearray/datatype_bytearray_def.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.594569 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/bytes/
+-rw-r--r--   0 krj        (502) staff       (20)       98 2024-02-02 14:16:58.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/bytes/datatype_bytes_def.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.594752 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/complex/
+-rw-r--r--   0 krj        (502) staff       (20)      281 2024-02-02 14:16:58.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/complex/datatype_complex_def.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.595557 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/dict/
+-rw-r--r--   0 krj        (502) staff       (20)      293 2024-02-02 14:16:58.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/dict/datatype_dict_change.py
+-rw-r--r--   0 krj        (502) staff       (20)      113 2024-02-02 14:16:58.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/dict/datatype_dict_def.py
+-rw-r--r--   0 krj        (502) staff       (20)      303 2024-02-02 14:16:58.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/dict/datatype_dict_felt.py
+-rw-r--r--   0 krj        (502) staff       (20)      201 2024-02-02 14:16:58.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/dict/datatype_dict_key_value.py
+-rw-r--r--   0 krj        (502) staff       (20)      453 2024-02-02 14:16:58.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/dict/datatype_dict_multi.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.595712 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/float/
+-rw-r--r--   0 krj        (502) staff       (20)      110 2024-02-02 14:16:58.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/float/datatype_float_def.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.595952 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/frozenset/
+-rw-r--r--   0 krj        (502) staff       (20)      338 2024-02-02 14:16:58.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/frozenset/datatype_frozenset_add.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.596169 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/int/
+-rw-r--r--   0 krj        (502) staff       (20)      110 2024-02-02 14:16:58.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/int/datatype_int_def.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.596813 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/list/
+-rw-r--r--   0 krj        (502) staff       (20)      134 2024-02-02 14:16:58.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/list/datatype_list_def.py
+-rw-r--r--   0 krj        (502) staff       (20)      222 2024-02-02 14:16:59.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/list/datatype_list_for_1_indeks.py
+-rw-r--r--   0 krj        (502) staff       (20)      215 2024-02-02 14:16:59.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/list/datatype_list_for_2_el.py
+-rw-r--r--   0 krj        (502) staff       (20)      184 2024-02-02 14:16:59.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/list/datatype_list_indeks.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.596990 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/memoryview/
+-rw-r--r--   0 krj        (502) staff       (20)      101 2024-02-02 14:16:59.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/memoryview/datatype_memoryview_def.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.597165 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/nonetype/
+-rw-r--r--   0 krj        (502) staff       (20)      322 2024-02-02 14:16:59.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/nonetype/datatype_nonetype_def.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.597809 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/range/
+-rw-r--r--   0 krj        (502) staff       (20)      202 2024-02-02 14:16:59.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/range/datatype_range_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      220 2024-02-02 14:16:59.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/range/datatype_range_2_kort.py
+-rw-r--r--   0 krj        (502) staff       (20)      234 2024-02-02 14:16:59.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/range/datatype_range_inkludert.py
+-rw-r--r--   0 krj        (502) staff       (20)      265 2024-02-02 14:16:59.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/range/datatype_range_steg.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.598250 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/set/
+-rw-r--r--   0 krj        (502) staff       (20)      285 2024-02-02 14:16:59.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/set/datatype_set_add.py
+-rw-r--r--   0 krj        (502) staff       (20)      133 2024-02-02 14:16:59.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/set/datatype_set_def.py
+-rw-r--r--   0 krj        (502) staff       (20)      291 2024-02-02 14:16:59.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/set/datatype_set_remove.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.599759 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/str/
+-rw-r--r--   0 krj        (502) staff       (20)      259 2024-02-02 14:16:59.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_bokstav_1.py
+-rw-r--r--   0 krj        (502) staff       (20)      248 2024-02-02 14:16:59.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_bokstav_2_for_indeks.py
+-rw-r--r--   0 krj        (502) staff       (20)      237 2024-02-02 14:17:00.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_bokstav_3_for.py
+-rw-r--r--   0 krj        (502) staff       (20)       98 2024-02-02 14:17:00.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_def.py
+-rw-r--r--   0 krj        (502) staff       (20)      153 2024-02-02 14:17:00.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_emoji.py
+-rw-r--r--   0 krj        (502) staff       (20)      134 2024-02-02 14:17:00.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_escape_char.py
+-rw-r--r--   0 krj        (502) staff       (20)      191 2024-02-02 14:17:00.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_escape_char_oversikt.py
+-rw-r--r--   0 krj        (502) staff       (20)      451 2024-02-02 14:17:00.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_hermetegn.py
+-rw-r--r--   0 krj        (502) staff       (20)      219 2024-02-02 14:17:00.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_len.py
+-rw-r--r--   0 krj        (502) staff       (20)      124 2024-02-02 14:17:00.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/str/datatype_str_unicode.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.599965 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/tuple/
+-rw-r--r--   0 krj        (502) staff       (20)      219 2024-02-02 14:17:00.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/tuple/datatype_tuple_def.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.600575 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/variabelnavn/
+-rw-r--r--   0 krj        (502) staff       (20)      289 2024-02-02 14:17:00.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/variabelnavn/variabelnavn_case.py
+-rw-r--r--   0 krj        (502) staff       (20)      212 2024-02-02 14:17:00.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/variabelnavn/variabelnavn_gyldig.py
+-rw-r--r--   0 krj        (502) staff       (20)      220 2024-02-02 14:17:00.000000 matematikk-0.0.99/src/matematikk/python/tutorial/variabel/variabelnavn/variabelnavn_ugyldig.py
+drwxr-xr-x   0 krj        (502) staff       (20)        0 2024-02-02 14:17:18.600826 matematikk-0.0.99/src/matematikk.egg-info/
+-rw-r--r--   0 krj        (502) staff       (20)      625 2024-02-02 14:17:18.000000 matematikk-0.0.99/src/matematikk.egg-info/PKG-INFO
+-rw-r--r--   0 krj        (502) staff       (20)    22108 2024-02-02 14:17:18.000000 matematikk-0.0.99/src/matematikk.egg-info/SOURCES.txt
+-rw-r--r--   0 krj        (502) staff       (20)        1 2024-02-02 14:17:18.000000 matematikk-0.0.99/src/matematikk.egg-info/dependency_links.txt
+-rw-r--r--   0 krj        (502) staff       (20)       11 2024-02-02 14:17:18.000000 matematikk-0.0.99/src/matematikk.egg-info/top_level.txt
```

### Comparing `matematikk-0.0.98/LICENCE` & `matematikk-0.0.99/LICENCE`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/PKG-INFO` & `matematikk-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matematikk
-Version: 0.0.98
+Version: 0.0.99
 Summary: Matematikk-bibliotek
 Author-email: matematikk <kontakt@matematikk.as>
 Project-URL: Homepage, https://matematikk.as
 Project-URL: Issues, https://matematikk.as
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `matematikk-0.0.98/src/matematikk/__init__.py` & `matematikk-0.0.99/src/matematikk/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Versjon: 0.0.97
+# Versjon: 0.0.98
 
 # Chain mal
 from ._ch_1.ch_2.ch_3.ch_4_fil import ch_5_fn
 
 # numpy()
 from numpy import(
     polyfit
@@ -37,15 +37,15 @@
     # Alias > Reversed
     cas_regresjon,
     cas_regresjon_polynom,
     regresjon_polynom_cas
     )
 
 # superlos()
-from .superløs_fil import (
+from .python.funksjoner.matematikk.likninger.superlos.def_superlos_matematikk_mas import (
     superløs,
 
     # Alias > Right
     los,
     losning,
     løs,
     løsning,
```

### Comparing `matematikk-0.0.98/src/matematikk/eksamen/oppg_test.py` & `matematikk-0.0.99/src/matematikk/eksamen/oppg_test.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_1_sofa_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_1_sofa_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_2_sofa_def_reggis_str_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_2_sofa_def_reggis_str_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_3_sofa_def_reggis_cas_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_3_sofa_def_reggis_cas_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_4_sofa_matematikk_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_4_sofa_matematikk_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_5_sofa_matematikk_speedrun_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_a_5_sofa_matematikk_speedrun_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_1_sofa_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_1_sofa_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_2_sofa_def_superlos_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_2_sofa_def_superlos_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_3_sofa_matematikk_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_3_sofa_matematikk_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_4_sofa_def_overskudd_max_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_4_sofa_def_overskudd_max_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_5_sofa_abstrahering_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_5_sofa_abstrahering_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_6_sofa_matematikk_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_6_sofa_matematikk_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_7_sofa_matematikk_speedrun_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_b_7_sofa_matematikk_speedrun_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_c_sofa_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/01_oppg_1_c_sofa_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/01/02_oppg_1_c_sofa_torodd.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/01/02_oppg_1_c_sofa_torodd.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/02/01_oppg_2_a_venstrehendte_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/02/01_oppg_2_a_venstrehendte_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/02/01_oppg_2_b_1_venstrehendte_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/02/01_oppg_2_b_1_venstrehendte_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/02/01_oppg_2_b_2_venstrehendte_relasjoner_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/02/01_oppg_2_b_2_venstrehendte_relasjoner_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/02/01_oppg_2_c_venstrehendte_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/02/01_oppg_2_c_venstrehendte_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/02/02_oppg_2_b_venstrehendte_torodd.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/02/02_oppg_2_b_venstrehendte_torodd.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/02/02_oppg_2_c_venstrehendte_torodd.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/02/02_oppg_2_c_venstrehendte_torodd.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/02/mal_sannsynlighets_relasjoner_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/02/mal_sannsynlighets_relasjoner_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_a_sparekonto_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_a_sparekonto_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_b_sparekonto_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_b_sparekonto_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_c_1_sparekonto_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_c_1_sparekonto_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_c_2_sparekonto_superlos_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_c_2_sparekonto_superlos_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_c_3_sparekonto_matematikk_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/03/01_oppg_3_c_3_sparekonto_matematikk_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/03/02_oppg_3_b_sparekonto_torodd.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/03/02_oppg_3_b_sparekonto_torodd.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/04/01_oppg_4_a_terninger_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/04/01_oppg_4_a_terninger_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/04/01_oppg_4_b_terninger_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/04/01_oppg_4_b_terninger_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/04/01_oppg_4_c_terninger_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/04/01_oppg_4_c_terninger_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/04/02_oppg_4_b_terninger_torodd.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/04/02_oppg_4_b_terninger_torodd.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/04/02_oppg_4_c_terninger_torodd.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/04/02_oppg_4_c_terninger_torodd.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_a_1_prisme_geometrisk_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_a_1_prisme_geometrisk_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_a_2_prisme_likning_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_a_2_prisme_likning_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_a_3_prisme_likning_superlos_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_a_3_prisme_likning_superlos_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_b_prisme_likning_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_b_prisme_likning_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_c_prisme_likning_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/05/01_oppg_5_c_prisme_likning_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/06/01_oppg_6_a_tredjegradsfunksjon_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/06/01_oppg_6_a_tredjegradsfunksjon_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/06/01_oppg_6_b_tredjegradsfunksjon_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/06/01_oppg_6_b_tredjegradsfunksjon_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/06/01_oppg_6_c_tredjegradsfunksjon_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/06/01_oppg_6_c_tredjegradsfunksjon_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/06/02_oppg_6_a_tredjegradsfunksjon_torodd.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/06/02_oppg_6_a_tredjegradsfunksjon_torodd.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_h/del_2/06/02_oppg_6_c_tredjegradsfunksjon_torodd.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_h/del_2/06/02_oppg_6_c_tredjegradsfunksjon_torodd.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_v/del_2/01/01_oppg_1_a_timelonn_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_v/del_2/01/01_oppg_1_a_timelonn_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/eksamen/s1/2023_v/del_2/01/01_oppg_1_b_timelonn_mas.py` & `matematikk-0.0.99/src/matematikk/python/eksamen/s1/2023_v/del_2/01/01_oppg_1_b_timelonn_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/def_ekstremalpunkt_max_mas.py` & `matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/def_ekstremalpunkt_max_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/def_ekstremalpunkt_max_matematikk_mas.py` & `matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/def_ekstremalpunkt_max_matematikk_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/def_overskudd_max_mas.py` & `matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/def_overskudd_max_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/def_overskudd_max_matematikk_mas.py` & `matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/funksjoner/_drøfting/ekstremalpunkt/def_overskudd_max_matematikk_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/likninger/superlos/def_superlos_mas.py` & `matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/likninger/superlos/def_superlos_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/likninger/superlos/def_superlos_matematikk_mas.py` & `matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/likninger/superlos/def_superlos_matematikk_mas.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         print(f"Løsnings-elemente(er) avrundet   :: {losning_rund_liste}")
         print(f"-----------------------------------")
         print(f"Løsning ut (returnert) -----------> {losning_ut}")
         print(f"-----------------------------------")
 
     return losning_ut
 
-
+  
 # Alias > Right
 los                     = superløs
 losning                 = superløs
 løs                     = superløs
 løsning                 = superløs
 superlos                = superløs
 super_los               = superløs
```

### Comparing `matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/regresjon/polynom/reggis/def_reggis_mas.py` & `matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/regresjon/polynom/reggis/def_reggis_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/funksjoner/matematikk/regresjon/polynom/reggis/def_reggis_matematikk_mas.py` & `matematikk-0.0.99/src/matematikk/python/funksjoner/matematikk/regresjon/polynom/reggis/def_reggis_matematikk_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_55/01_oppg_1_55_vanjas_scooter_mas.py` & `matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_55/01_oppg_1_55_vanjas_scooter_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_55/02_oppg_1_55_vanjas_scooter_input_mas.py` & `matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_55/02_oppg_1_55_vanjas_scooter_input_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_56/oppg_1_56_elbiler_mas.py` & `matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_56/oppg_1_56_elbiler_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_57/oppg_1_57_hus_og_elbiler_mas.py` & `matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_57/oppg_1_57_hus_og_elbiler_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/02_eks_1_5_a_b_vindpark_mas.py` & `matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/02_eks_1_5_a_b_vindpark_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/04_eks_1_5_a_b_vindpark_input_mas.py` & `matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/04_eks_1_5_a_b_vindpark_input_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/05_oppg_1_59_vindpark_mas.py` & `matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/1_5_eks/05_oppg_1_59_vindpark_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/oppgaver/1t/brettboka/9/oppg_k_1_9_pythagoras_mas.py` & `matematikk-0.0.99/src/matematikk/python/oppgaver/1t/brettboka/9/oppg_k_1_9_pythagoras_mas.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/antall/liste_count_2_input_str.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/antall/liste_count_2_input_str.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/antall/liste_length_2_input_str.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/antall/liste_length_2_input_str.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/copy/liste_copy_deepcopy.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/copy/liste_copy_deepcopy.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/delete/liste_remove_negative_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/delete/liste_remove_negative_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/delete/liste_remove_negative_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/delete/liste_remove_negative_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/delete/liste_remove_positive_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/delete/liste_remove_positive_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/delete/liste_remove_positive_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/delete/liste_remove_positive_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/eksisterer/liste_eksisterer_2_input_str.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/eksisterer/liste_eksisterer_2_input_str.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/eksisterer/liste_eksisterer_for_2_input_str.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/eksisterer/liste_eksisterer_for_2_input_str.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/max/liste_max_for_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/max/liste_max_for_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/max/liste_max_for_2_input_int.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/max/liste_max_for_2_input_int.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/max/liste_max_sort_2_input_int.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/max/liste_max_sort_2_input_int.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/min/liste_min_for_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/min/liste_min_for_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/min/liste_min_for_2_input_int.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/min/liste_min_for_2_input_int.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/min/liste_min_sort_2_input_int.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/min/liste_min_sort_2_input_int.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_all_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_all_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_all_2_input_int.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_all_2_input_int.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_sort_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_sort_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_sort_2_input_int.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_sort_2_input_int.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_sort_3_to.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/monotonic/liste_sortert_ja_nei_sort_3_to.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_comprehension_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_comprehension_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_comprehension_2_input_str.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_comprehension_2_input_str.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_for_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_for_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_for_2_input_str.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_for_2_input_str.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_numpy_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_numpy_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_numpy_2_input_str.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_numpy_2_input_str.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_yield_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_yield_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_yield_2_input_str.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/oppdeling/liste_oppdeling_yield_2_input_str.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/product/liste_produkt_for_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/product/liste_produkt_for_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/product/liste_produkt_math_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/product/liste_produkt_math_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/product/liste_produkt_numpy_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/product/liste_produkt_numpy_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/reversert/liste_reversert_2_input_int.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/reversert/liste_reversert_2_input_int.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/reversert/liste_reversert_copy_2_input_int.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/reversert/liste_reversert_copy_2_input_int.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/rotate/liste_rotasjon_int_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/rotate/liste_rotasjon_int_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/rotate/liste_rotasjon_int_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/rotate/liste_rotasjon_int_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/rotate/liste_rotasjon_str_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/rotate/liste_rotasjon_str_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/rotate/liste_rotasjon_str_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/rotate/liste_rotasjon_str_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/sum/liste_sum_2_input_int.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/sum/liste_sum_2_input_int.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/datatype/list/sum/liste_sum_for_2_input_int.py` & `matematikk-0.0.99/src/matematikk/python/programmer/datatype/list/sum/liste_sum_for_2_input_int.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/economics/rente/rente_opptjent_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/economics/rente/rente_opptjent_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/economics/rente/rente_opptjent_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/economics/rente/rente_opptjent_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/aritmetikk/siffer/siffer_antall_divisjon_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/aritmetikk/siffer/siffer_antall_divisjon_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/aritmetikk/siffer/siffer_antall_divisjon_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/aritmetikk/siffer/siffer_antall_divisjon_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/matrise/produkt/matrise_produkt.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/matrise/produkt/matrise_produkt.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_ja_nei_intervall_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_ja_nei_intervall_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_ja_nei_intervall_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_ja_nei_intervall_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_ja_nei_n_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_ja_nei_n_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_ja_nei_n_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_ja_nei_n_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_liste_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_liste_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_liste_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/armstrong_tall/armstrong_liste_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_for_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_for_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_for_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_for_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_newton_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_newton_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_newton_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_newton_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_rekursiv_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_rekursiv_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_rekursiv_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_formel_n_rekursiv_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_ja_nei_intervall_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_ja_nei_intervall_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_ja_nei_intervall_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_ja_nei_intervall_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_ja_nei_n_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_ja_nei_n_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_ja_nei_n_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_ja_nei_n_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_liste_rekursiv_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_liste_rekursiv_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_liste_rekursiv_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_liste_rekursiv_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_lister_rekursiv_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_lister_rekursiv_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_lister_rekursiv_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/fibonacci_tall/fibonacci_lister_rekursiv_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/figurtall/pyramide/pyramide.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/figurtall/pyramide/pyramide.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/negative_tall/negative_tall_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/negative_tall/negative_tall_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/negative_tall/negative_tall_2_input_int.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/negative_tall/negative_tall_2_input_int.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/oddetall/oddetall_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/oddetall/oddetall_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/oddetall/oddetall_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/oddetall/oddetall_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/partall/partall_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/partall/partall_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/partall/partall_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/partall/partall_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/positive_tall/positive_tall_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/positive_tall/positive_tall_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/positive_tall/positive_tall_2_input_int.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/positive_tall/positive_tall_2_input_int.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_intervall_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_intervall_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_intervall_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_intervall_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_math_intervall_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_math_intervall_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_math_intervall_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_math_intervall_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_math_n_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_math_n_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_math_n_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_math_n_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_n_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_n_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_n_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_ja_nei_n_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_liste_intervall_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_liste_intervall_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_liste_intervall_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_liste_intervall_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_liste_math_1.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_liste_math_1.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_liste_math_2_input.py` & `matematikk-0.0.99/src/matematikk/python/programmer/matematikk/tallteori/primtall/primtall_liste_math_2_input.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk/python/tutorial/variabel/datatype/_def/datatype_oversikt.py` & `matematikk-0.0.99/src/matematikk/python/tutorial/variabel/datatype/_def/datatype_oversikt.py`

 * *Files identical despite different names*

### Comparing `matematikk-0.0.98/src/matematikk.egg-info/PKG-INFO` & `matematikk-0.0.99/src/matematikk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matematikk
-Version: 0.0.98
+Version: 0.0.99
 Summary: Matematikk-bibliotek
 Author-email: matematikk <kontakt@matematikk.as>
 Project-URL: Homepage, https://matematikk.as
 Project-URL: Issues, https://matematikk.as
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `matematikk-0.0.98/src/matematikk.egg-info/SOURCES.txt` & `matematikk-0.0.99/src/matematikk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENCE
 README.md
 pyproject.toml
 src/matematikk/__init__.py
-src/matematikk/superløs_fil.py
 src/matematikk.egg-info/PKG-INFO
 src/matematikk.egg-info/SOURCES.txt
 src/matematikk.egg-info/dependency_links.txt
 src/matematikk.egg-info/top_level.txt
 src/matematikk/_ch_1/ch_2/ch_3/ch_4_fil.py
 src/matematikk/eksamen/oppg_test.py
 src/matematikk/python/eksamen/1t/2022_h/del_1/03/oppg_3_a_rasjonal_funksjon_bug.py
```

