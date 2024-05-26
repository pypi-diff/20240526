# Comparing `tmp/TB2J-0.9.0.tar.gz` & `tmp/TB2J-0.9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TB2J-0.9.0.tar", last modified: Wed May 22 13:11:16 2024, max compression
+gzip compressed data, was "TB2J-0.9.0.1.tar", last modified: Sun May 26 15:02:03 2024, max compression
```

## Comparing `TB2J-0.9.0.tar` & `TB2J-0.9.0.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.087083 TB2J-0.9.0/
--rw-r--r--   0 hexu      (1032) phythema   (500)     1332 2024-02-28 11:18:04.000000 TB2J-0.9.0/LICENSE
--rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2024-05-22 13:11:16.087083 TB2J-0.9.0/PKG-INFO
--rw-r--r--   0 hexu      (1032) phythema   (500)     2089 2024-03-08 15:04:05.000000 TB2J-0.9.0/README.md
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.083083 TB2J-0.9.0/TB2J/
--rw-r--r--   0 hexu      (1032) phythema   (500)     6980 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/Jdownfolder.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3179 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/Jtensor.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3383 2024-04-07 10:46:54.000000 TB2J-0.9.0/TB2J/Oiju.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6809 2024-04-07 10:46:54.000000 TB2J-0.9.0/TB2J/Oiju_epc.py
--rw-r--r--   0 hexu      (1032) phythema   (500)       22 2024-05-22 12:10:06.000000 TB2J-0.9.0/TB2J/__init__.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.083083 TB2J-0.9.0/TB2J/abacus/
--rw-r--r--   0 hexu      (1032) phythema   (500)       56 2024-03-04 09:41:08.000000 TB2J-0.9.0/TB2J/abacus/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     7267 2024-03-04 09:41:08.000000 TB2J-0.9.0/TB2J/abacus/abacus_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8461 2024-05-22 12:05:11.000000 TB2J-0.9.0/TB2J/abacus/abacus_wrapper.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2973 2024-03-04 09:41:08.000000 TB2J-0.9.0/TB2J/abacus/gen_exchange_abacus.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1562 2024-03-04 09:41:08.000000 TB2J-0.9.0/TB2J/abacus/orbital_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    67888 2024-03-08 12:59:31.000000 TB2J-0.9.0/TB2J/abacus/stru_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2024-03-04 09:41:08.000000 TB2J-0.9.0/TB2J/abacus/test_read_HRSR.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      785 2024-03-04 09:41:08.000000 TB2J-0.9.0/TB2J/abacus/test_read_stru.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1558 2024-03-04 09:41:08.000000 TB2J-0.9.0/TB2J/basis.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2891 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/citation.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2633 2024-04-18 09:51:34.000000 TB2J-0.9.0/TB2J/contour.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1514 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/density_matrix.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3474 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/epc.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    29586 2024-05-22 12:05:11.000000 TB2J-0.9.0/TB2J/exchange.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    10985 2024-05-22 12:05:07.000000 TB2J-0.9.0/TB2J/exchangeCL2.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8523 2024-04-07 10:46:54.000000 TB2J-0.9.0/TB2J/exchange_pert.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8436 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/exchange_qspace.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.083083 TB2J-0.9.0/TB2J/external/
--rw-r--r--   0 hexu      (1032) phythema   (500)      137 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/external/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     5831 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/external/p_tqdm.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6890 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/gpaw_wrapper.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    13377 2024-05-22 12:05:07.000000 TB2J-0.9.0/TB2J/green.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1603 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/greentest.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.087083 TB2J-0.9.0/TB2J/io_exchange/
--rw-r--r--   0 hexu      (1032) phythema   (500)       32 2024-02-28 11:09:31.000000 TB2J-0.9.0/TB2J/io_exchange/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    19354 2024-04-13 21:06:36.000000 TB2J-0.9.0/TB2J/io_exchange/io_exchange.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6739 2024-05-22 12:05:07.000000 TB2J-0.9.0/TB2J/io_exchange/io_multibinit.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4173 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/io_exchange/io_tomsasd.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    10547 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/io_exchange/io_txt.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3301 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/io_exchange/io_uppasd.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     5583 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/io_exchange/io_vampire.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6825 2024-05-22 12:05:11.000000 TB2J-0.9.0/TB2J/io_merge.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      532 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/kpoints.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    15372 2024-04-07 10:46:54.000000 TB2J-0.9.0/TB2J/manager.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      300 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/mathutils.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    17659 2024-05-22 12:05:11.000000 TB2J-0.9.0/TB2J/myTB.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6669 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/orbmap.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4120 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/pauli.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1192 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/pert.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4104 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/plot.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     3277 2024-05-22 12:05:11.000000 TB2J-0.9.0/TB2J/rotate_atoms.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1070 2024-05-22 12:05:11.000000 TB2J-0.9.0/TB2J/rotate_siestaDM.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    14792 2024-05-22 12:05:11.000000 TB2J-0.9.0/TB2J/sisl_wrapper.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.087083 TB2J-0.9.0/TB2J/spinham/
--rw-rw-r--   0 hexu      (1032) phythema   (500)        0 2020-07-08 14:12:19.000000 TB2J-0.9.0/TB2J/spinham/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2196 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/base_parser.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      762 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/constants.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    16607 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/hamiltonian.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     9714 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/hamiltonian_terms.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6599 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/plot.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4986 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/qsolver.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2219 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/spin_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    11033 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/spin_xml.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    12217 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/supercell.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8083 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/tensor_rotate.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3897 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/utest.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     9880 2024-05-22 12:05:07.000000 TB2J-0.9.0/TB2J/utils.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      337 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/versioninfo.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.087083 TB2J-0.9.0/TB2J/wannier/
--rw-r--r--   0 hexu      (1032) phythema   (500)       80 2024-03-04 10:09:47.000000 TB2J-0.9.0/TB2J/wannier/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4620 2024-03-14 08:56:01.000000 TB2J-0.9.0/TB2J/wannier/w90_parser.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4610 2024-03-04 10:09:47.000000 TB2J-0.9.0/TB2J/wannier/w90_tb_parser.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.083083 TB2J-0.9.0/TB2J.egg-info/
--rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2024-05-22 13:11:16.000000 TB2J-0.9.0/TB2J.egg-info/PKG-INFO
--rw-r--r--   0 hexu      (1032) phythema   (500)     1796 2024-05-22 13:11:16.000000 TB2J-0.9.0/TB2J.egg-info/SOURCES.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)        1 2024-05-22 13:11:16.000000 TB2J-0.9.0/TB2J.egg-info/dependency_links.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)       79 2024-05-22 13:11:16.000000 TB2J-0.9.0/TB2J.egg-info/requires.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)        5 2024-05-22 13:11:16.000000 TB2J-0.9.0/TB2J.egg-info/top_level.txt
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.087083 TB2J-0.9.0/scripts/
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     1868 2024-02-28 11:18:04.000000 TB2J-0.9.0/scripts/TB2J_downfold.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     1142 2024-02-28 11:18:04.000000 TB2J-0.9.0/scripts/TB2J_eigen.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     3115 2024-02-28 11:18:04.000000 TB2J-0.9.0/scripts/TB2J_magnon.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)      124 2024-02-28 11:18:04.000000 TB2J-0.9.0/scripts/TB2J_magnon_dos.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     1868 2024-05-22 12:05:11.000000 TB2J-0.9.0/scripts/TB2J_merge.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)      887 2024-05-22 12:05:11.000000 TB2J-0.9.0/scripts/TB2J_rotate.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      581 2024-05-22 12:05:11.000000 TB2J-0.9.0/scripts/TB2J_rotateDM.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     4422 2024-03-04 09:41:08.000000 TB2J-0.9.0/scripts/abacus2J.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     4317 2024-04-07 10:46:54.000000 TB2J-0.9.0/scripts/siesta2J.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     5728 2024-04-07 10:46:54.000000 TB2J-0.9.0/scripts/wann2J.py
--rw-r--r--   0 hexu      (1032) phythema   (500)       38 2024-05-22 13:11:16.087083 TB2J-0.9.0/setup.cfg
--rw-r--r--   0 hexu      (1032) phythema   (500)     1986 2024-05-22 12:09:56.000000 TB2J-0.9.0/setup.py
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-05-26 15:02:03.335851 TB2J-0.9.0.1/
+-rw-r--r--   0 hexu       (501) staff       (20)     1332 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/LICENSE
+-rw-r--r--   0 hexu       (501) staff       (20)     1417 2024-05-26 15:02:03.335666 TB2J-0.9.0.1/PKG-INFO
+-rw-r--r--   0 hexu       (501) staff       (20)     2184 2024-05-26 14:59:17.000000 TB2J-0.9.0.1/README.md
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-05-26 15:02:03.330440 TB2J-0.9.0.1/TB2J/
+-rw-r--r--   0 hexu       (501) staff       (20)     6980 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/Jdownfolder.py
+-rw-r--r--   0 hexu       (501) staff       (20)     3179 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/Jtensor.py
+-rw-r--r--   0 hexu       (501) staff       (20)     3383 2024-04-07 08:49:33.000000 TB2J-0.9.0.1/TB2J/Oiju.py
+-rw-r--r--   0 hexu       (501) staff       (20)     6809 2024-04-07 08:49:33.000000 TB2J-0.9.0.1/TB2J/Oiju_epc.py
+-rw-r--r--   0 hexu       (501) staff       (20)       24 2024-05-26 15:01:26.000000 TB2J-0.9.0.1/TB2J/__init__.py
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-05-26 15:02:03.331897 TB2J-0.9.0.1/TB2J/abacus/
+-rw-r--r--   0 hexu       (501) staff       (20)       56 2024-02-18 22:38:09.000000 TB2J-0.9.0.1/TB2J/abacus/__init__.py
+-rw-r--r--   0 hexu       (501) staff       (20)     7267 2024-02-25 13:06:00.000000 TB2J-0.9.0.1/TB2J/abacus/abacus_api.py
+-rw-r--r--   0 hexu       (501) staff       (20)     8461 2024-05-26 14:59:12.000000 TB2J-0.9.0.1/TB2J/abacus/abacus_wrapper.py
+-rw-r--r--   0 hexu       (501) staff       (20)     2973 2024-05-23 20:25:31.000000 TB2J-0.9.0.1/TB2J/abacus/gen_exchange_abacus.py
+-rw-r--r--   0 hexu       (501) staff       (20)     1562 2024-02-18 22:38:09.000000 TB2J-0.9.0.1/TB2J/abacus/orbital_api.py
+-rw-r--r--   0 hexu       (501) staff       (20)    67888 2024-03-19 22:14:36.000000 TB2J-0.9.0.1/TB2J/abacus/stru_api.py
+-rw-r--r--   0 hexu       (501) staff       (20)     1254 2024-02-18 22:38:09.000000 TB2J-0.9.0.1/TB2J/abacus/test_read_HRSR.py
+-rw-r--r--   0 hexu       (501) staff       (20)      785 2024-02-18 22:38:09.000000 TB2J-0.9.0.1/TB2J/abacus/test_read_stru.py
+-rw-r--r--   0 hexu       (501) staff       (20)     1558 2024-02-18 22:38:09.000000 TB2J-0.9.0.1/TB2J/basis.py
+-rw-r--r--   0 hexu       (501) staff       (20)     2891 2024-05-01 11:00:03.000000 TB2J-0.9.0.1/TB2J/citation.py
+-rw-r--r--   0 hexu       (501) staff       (20)     2633 2024-05-22 21:42:05.000000 TB2J-0.9.0.1/TB2J/contour.py
+-rw-r--r--   0 hexu       (501) staff       (20)     1514 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/density_matrix.py
+-rw-r--r--   0 hexu       (501) staff       (20)     3474 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/epc.py
+-rw-r--r--   0 hexu       (501) staff       (20)    29581 2024-05-26 15:01:08.000000 TB2J-0.9.0.1/TB2J/exchange.py
+-rw-r--r--   0 hexu       (501) staff       (20)    10985 2024-04-27 13:01:59.000000 TB2J-0.9.0.1/TB2J/exchangeCL2.py
+-rw-r--r--   0 hexu       (501) staff       (20)     8523 2024-04-07 08:49:33.000000 TB2J-0.9.0.1/TB2J/exchange_pert.py
+-rw-r--r--   0 hexu       (501) staff       (20)     8436 2023-10-22 10:20:37.000000 TB2J-0.9.0.1/TB2J/exchange_qspace.py
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-05-26 15:02:03.332103 TB2J-0.9.0.1/TB2J/external/
+-rw-r--r--   0 hexu       (501) staff       (20)      137 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/external/__init__.py
+-rw-r--r--   0 hexu       (501) staff       (20)     5831 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/external/p_tqdm.py
+-rw-r--r--   0 hexu       (501) staff       (20)     6890 2023-10-22 10:21:30.000000 TB2J-0.9.0.1/TB2J/gpaw_wrapper.py
+-rw-r--r--   0 hexu       (501) staff       (20)    13377 2024-05-26 14:59:12.000000 TB2J-0.9.0.1/TB2J/green.py
+-rw-r--r--   0 hexu       (501) staff       (20)     1603 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/greentest.py
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-05-26 15:02:03.332895 TB2J-0.9.0.1/TB2J/io_exchange/
+-rw-r--r--   0 hexu       (501) staff       (20)       32 2023-05-13 20:57:02.000000 TB2J-0.9.0.1/TB2J/io_exchange/__init__.py
+-rw-r--r--   0 hexu       (501) staff       (20)    19354 2024-03-19 22:14:36.000000 TB2J-0.9.0.1/TB2J/io_exchange/io_exchange.py
+-rw-r--r--   0 hexu       (501) staff       (20)     6739 2024-05-22 20:20:12.000000 TB2J-0.9.0.1/TB2J/io_exchange/io_multibinit.py
+-rw-r--r--   0 hexu       (501) staff       (20)     4173 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/io_exchange/io_tomsasd.py
+-rw-r--r--   0 hexu       (501) staff       (20)    10547 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/io_exchange/io_txt.py
+-rw-r--r--   0 hexu       (501) staff       (20)     3301 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/io_exchange/io_uppasd.py
+-rw-r--r--   0 hexu       (501) staff       (20)     5583 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/io_exchange/io_vampire.py
+-rw-r--r--   0 hexu       (501) staff       (20)     6825 2024-05-22 20:20:12.000000 TB2J-0.9.0.1/TB2J/io_merge.py
+-rw-r--r--   0 hexu       (501) staff       (20)      532 2024-05-22 21:20:38.000000 TB2J-0.9.0.1/TB2J/kpoints.py
+-rw-r--r--   0 hexu       (501) staff       (20)    15372 2024-04-07 08:49:33.000000 TB2J-0.9.0.1/TB2J/manager.py
+-rw-r--r--   0 hexu       (501) staff       (20)      300 2023-10-22 10:47:10.000000 TB2J-0.9.0.1/TB2J/mathutils.py
+-rw-r--r--   0 hexu       (501) staff       (20)    17659 2024-05-22 20:20:12.000000 TB2J-0.9.0.1/TB2J/myTB.py
+-rw-r--r--   0 hexu       (501) staff       (20)     6669 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/orbmap.py
+-rw-r--r--   0 hexu       (501) staff       (20)     4120 2024-05-26 14:59:12.000000 TB2J-0.9.0.1/TB2J/pauli.py
+-rw-r--r--   0 hexu       (501) staff       (20)     1192 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/pert.py
+-rw-r--r--   0 hexu       (501) staff       (20)     4104 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/plot.py
+-rwxr-xr-x   0 hexu       (501) staff       (20)     3277 2024-05-22 20:20:12.000000 TB2J-0.9.0.1/TB2J/rotate_atoms.py
+-rw-r--r--   0 hexu       (501) staff       (20)     1070 2024-05-22 20:20:12.000000 TB2J-0.9.0.1/TB2J/rotate_siestaDM.py
+-rw-r--r--   0 hexu       (501) staff       (20)    14792 2024-05-22 20:20:12.000000 TB2J-0.9.0.1/TB2J/sisl_wrapper.py
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-05-26 15:02:03.333973 TB2J-0.9.0.1/TB2J/spinham/
+-rw-r--r--   0 hexu       (501) staff       (20)        0 2023-05-13 20:57:02.000000 TB2J-0.9.0.1/TB2J/spinham/__init__.py
+-rw-r--r--   0 hexu       (501) staff       (20)     2196 2024-05-05 08:53:18.000000 TB2J-0.9.0.1/TB2J/spinham/base_parser.py
+-rw-r--r--   0 hexu       (501) staff       (20)      762 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/spinham/constants.py
+-rw-r--r--   0 hexu       (501) staff       (20)    16607 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/spinham/hamiltonian.py
+-rw-r--r--   0 hexu       (501) staff       (20)     9714 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/spinham/hamiltonian_terms.py
+-rw-r--r--   0 hexu       (501) staff       (20)     6599 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/spinham/plot.py
+-rw-r--r--   0 hexu       (501) staff       (20)     4986 2024-05-05 08:53:01.000000 TB2J-0.9.0.1/TB2J/spinham/qsolver.py
+-rw-r--r--   0 hexu       (501) staff       (20)     2219 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/spinham/spin_api.py
+-rw-r--r--   0 hexu       (501) staff       (20)    11033 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/spinham/spin_xml.py
+-rw-r--r--   0 hexu       (501) staff       (20)    12217 2023-10-22 10:18:47.000000 TB2J-0.9.0.1/TB2J/spinham/supercell.py
+-rw-r--r--   0 hexu       (501) staff       (20)     8083 2024-05-23 08:54:20.000000 TB2J-0.9.0.1/TB2J/tensor_rotate.py
+-rw-r--r--   0 hexu       (501) staff       (20)     3897 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/utest.py
+-rw-r--r--   0 hexu       (501) staff       (20)     9880 2024-03-19 22:14:36.000000 TB2J-0.9.0.1/TB2J/utils.py
+-rw-r--r--   0 hexu       (501) staff       (20)      337 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/TB2J/versioninfo.py
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-05-26 15:02:03.334317 TB2J-0.9.0.1/TB2J/wannier/
+-rw-r--r--   0 hexu       (501) staff       (20)       80 2024-03-19 22:14:36.000000 TB2J-0.9.0.1/TB2J/wannier/__init__.py
+-rw-r--r--   0 hexu       (501) staff       (20)     4620 2024-03-19 22:14:36.000000 TB2J-0.9.0.1/TB2J/wannier/w90_parser.py
+-rw-r--r--   0 hexu       (501) staff       (20)     4610 2024-03-19 22:14:36.000000 TB2J-0.9.0.1/TB2J/wannier/w90_tb_parser.py
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-05-26 15:02:03.335463 TB2J-0.9.0.1/TB2J.egg-info/
+-rw-r--r--   0 hexu       (501) staff       (20)     1417 2024-05-26 15:02:03.000000 TB2J-0.9.0.1/TB2J.egg-info/PKG-INFO
+-rw-r--r--   0 hexu       (501) staff       (20)     1796 2024-05-26 15:02:03.000000 TB2J-0.9.0.1/TB2J.egg-info/SOURCES.txt
+-rw-r--r--   0 hexu       (501) staff       (20)        1 2024-05-26 15:02:03.000000 TB2J-0.9.0.1/TB2J.egg-info/dependency_links.txt
+-rw-r--r--   0 hexu       (501) staff       (20)       79 2024-05-26 15:02:03.000000 TB2J-0.9.0.1/TB2J.egg-info/requires.txt
+-rw-r--r--   0 hexu       (501) staff       (20)        5 2024-05-26 15:02:03.000000 TB2J-0.9.0.1/TB2J.egg-info/top_level.txt
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-05-26 15:02:03.335324 TB2J-0.9.0.1/scripts/
+-rwxr-xr-x   0 hexu       (501) staff       (20)     1868 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/scripts/TB2J_downfold.py
+-rwxr-xr-x   0 hexu       (501) staff       (20)     1142 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/scripts/TB2J_eigen.py
+-rwxr-xr-x   0 hexu       (501) staff       (20)     3115 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/scripts/TB2J_magnon.py
+-rwxr-xr-x   0 hexu       (501) staff       (20)      124 2023-10-22 07:17:59.000000 TB2J-0.9.0.1/scripts/TB2J_magnon_dos.py
+-rwxr-xr-x   0 hexu       (501) staff       (20)     1868 2024-05-22 20:20:12.000000 TB2J-0.9.0.1/scripts/TB2J_merge.py
+-rwxr-xr-x   0 hexu       (501) staff       (20)      887 2024-05-22 20:20:12.000000 TB2J-0.9.0.1/scripts/TB2J_rotate.py
+-rw-r--r--   0 hexu       (501) staff       (20)      581 2024-05-22 20:20:12.000000 TB2J-0.9.0.1/scripts/TB2J_rotateDM.py
+-rwxr-xr-x   0 hexu       (501) staff       (20)     4422 2024-02-18 22:38:09.000000 TB2J-0.9.0.1/scripts/abacus2J.py
+-rwxr-xr-x   0 hexu       (501) staff       (20)     4317 2024-04-07 08:49:33.000000 TB2J-0.9.0.1/scripts/siesta2J.py
+-rwxr-xr-x   0 hexu       (501) staff       (20)     5728 2024-04-07 08:49:33.000000 TB2J-0.9.0.1/scripts/wann2J.py
+-rw-r--r--   0 hexu       (501) staff       (20)       38 2024-05-26 15:02:03.335888 TB2J-0.9.0.1/setup.cfg
+-rw-r--r--   0 hexu       (501) staff       (20)     1988 2024-05-26 15:01:37.000000 TB2J-0.9.0.1/setup.py
```

### Comparing `TB2J-0.9.0/LICENSE` & `TB2J-0.9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/PKG-INFO` & `TB2J-0.9.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: TB2J
-Version: 0.9.0
+Version: 0.9.0.1
 Summary: TB2J: First principle to Heisenberg exchange J using tight-binding Green function method
-Home-page: UNKNOWN
 Author: Xu He
 Author-email: mailhexu@gmail.com
 License: BSD-2-clause
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.6
 License-File: LICENSE
+Requires-Dist: numpy>1.16.5
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: ase>=3.19
+Requires-Dist: tqdm
+Requires-Dist: pathos
+Requires-Dist: packaging>=20.0
+Requires-Dist: pre-commit
 
 TB2J is a Python package aimed to compute automatically the magnetic interactions (superexchange  and Dzyaloshinskii-Moriya) between atoms of magnetic crystals from DFT Hamiltonian based on Wannier functions or Linear combination of atomic orbitals. It uses the Green's function method and take the local rigid spin rotation as a perturbation. The package can take the output from Wannier90, which is interfaced with many density functional theory codes or from codes based on localised orbitals. A minimal user input is needed, which allows for an easily integration into a high-throughput workflows. 
-
```

### Comparing `TB2J-0.9.0/README.md` & `TB2J-0.9.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 [![Build Status](https://app.travis-ci.com/mailhexu/TB2J.svg?branch=master)](https://app.travis-ci.com/mailhexu/TB2J)
 [![Downloads](https://pepy.tech/badge/tb2j)](https://pepy.tech/project/tb2j)
 
 ## Description
 
 TB2J is a open source python package for calculating the magnetic interaction parameters in Heisenberg models from DFT. It use the magnetic force theorem and take the local rigid spin rotation as a perturbation in the Green's function method. 
 
+The TB2J project is initialized in the PhyTheMa and Nanomat teams in the University of Liege.
+
 The features include:
  - Calculates  parameters in Heisenberg model, including isotropic exchange, anisotropic exchange, Dyzanoshinskii-Moriya interaction.
  - Can use the input from many DFT codes with Wannier90, e.g. Abinit, Quantum Espresso, Siesta, VASP, etc.
  - Can use input from DFT codes with numerical orbitals from Siesta, OpenMX and ABACUS.
  - Calculate magnon band structure from the Heisenberg Hamiltonian.
  - Generate input for spin dynamics/Monte Carlo codes MULTIBINIT.
  - Require only ground state DFT calculation.
```

### Comparing `TB2J-0.9.0/TB2J/Jdownfolder.py` & `TB2J-0.9.0.1/TB2J/Jdownfolder.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/Jtensor.py` & `TB2J-0.9.0.1/TB2J/Jtensor.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/Oiju.py` & `TB2J-0.9.0.1/TB2J/Oiju.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/Oiju_epc.py` & `TB2J-0.9.0.1/TB2J/Oiju_epc.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/abacus/abacus_api.py` & `TB2J-0.9.0.1/TB2J/abacus/abacus_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/abacus/abacus_wrapper.py` & `TB2J-0.9.0.1/TB2J/abacus/abacus_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/abacus/gen_exchange_abacus.py` & `TB2J-0.9.0.1/TB2J/abacus/gen_exchange_abacus.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/abacus/orbital_api.py` & `TB2J-0.9.0.1/TB2J/abacus/orbital_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/abacus/stru_api.py` & `TB2J-0.9.0.1/TB2J/abacus/stru_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/abacus/test_read_HRSR.py` & `TB2J-0.9.0.1/TB2J/abacus/test_read_HRSR.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/abacus/test_read_stru.py` & `TB2J-0.9.0.1/TB2J/abacus/test_read_stru.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/basis.py` & `TB2J-0.9.0.1/TB2J/basis.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/citation.py` & `TB2J-0.9.0.1/TB2J/citation.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/contour.py` & `TB2J-0.9.0.1/TB2J/contour.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/density_matrix.py` & `TB2J-0.9.0.1/TB2J/density_matrix.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/epc.py` & `TB2J-0.9.0.1/TB2J/epc.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/exchange.py` & `TB2J-0.9.0.1/TB2J/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,15 +341,15 @@
             self.efermi,
             use_cache=self._use_cache,
             nproc=self.np,
         )
         self.norb = self.G.norb
         self.nbasis = self.G.nbasis
         # self.rho = np.zeros((self.nbasis, self.nbasis), dtype=complex)
-        self.rho = self.G.get_density_matrix().real
+        self.rho = self.G.get_density_matrix()
         self.A_ijR_list = defaultdict(lambda: [])
         self.A_ijR = defaultdict(lambda: np.zeros((4, 4), dtype=complex))
         self.A_ijR_orb = dict()
         self.HR0 = self.G.H0
         self._is_collinear = False
         self.Pdict = {}
         if self.write_density_matrix:
```

### Comparing `TB2J-0.9.0/TB2J/exchangeCL2.py` & `TB2J-0.9.0.1/TB2J/exchangeCL2.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/exchange_pert.py` & `TB2J-0.9.0.1/TB2J/exchange_pert.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/exchange_qspace.py` & `TB2J-0.9.0.1/TB2J/exchange_qspace.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/external/p_tqdm.py` & `TB2J-0.9.0.1/TB2J/external/p_tqdm.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/gpaw_wrapper.py` & `TB2J-0.9.0.1/TB2J/gpaw_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/green.py` & `TB2J-0.9.0.1/TB2J/green.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/greentest.py` & `TB2J-0.9.0.1/TB2J/greentest.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/io_exchange/io_exchange.py` & `TB2J-0.9.0.1/TB2J/io_exchange/io_exchange.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/io_exchange/io_multibinit.py` & `TB2J-0.9.0.1/TB2J/io_exchange/io_multibinit.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/io_exchange/io_tomsasd.py` & `TB2J-0.9.0.1/TB2J/io_exchange/io_tomsasd.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/io_exchange/io_txt.py` & `TB2J-0.9.0.1/TB2J/io_exchange/io_txt.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/io_exchange/io_uppasd.py` & `TB2J-0.9.0.1/TB2J/io_exchange/io_uppasd.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/io_exchange/io_vampire.py` & `TB2J-0.9.0.1/TB2J/io_exchange/io_vampire.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/io_merge.py` & `TB2J-0.9.0.1/TB2J/io_merge.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/kpoints.py` & `TB2J-0.9.0.1/TB2J/kpoints.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/manager.py` & `TB2J-0.9.0.1/TB2J/manager.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/myTB.py` & `TB2J-0.9.0.1/TB2J/myTB.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/orbmap.py` & `TB2J-0.9.0.1/TB2J/orbmap.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/pauli.py` & `TB2J-0.9.0.1/TB2J/pauli.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/pert.py` & `TB2J-0.9.0.1/TB2J/pert.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/plot.py` & `TB2J-0.9.0.1/TB2J/plot.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/rotate_atoms.py` & `TB2J-0.9.0.1/TB2J/rotate_atoms.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/rotate_siestaDM.py` & `TB2J-0.9.0.1/TB2J/rotate_siestaDM.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/sisl_wrapper.py` & `TB2J-0.9.0.1/TB2J/sisl_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/spinham/base_parser.py` & `TB2J-0.9.0.1/TB2J/spinham/base_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/spinham/constants.py` & `TB2J-0.9.0.1/TB2J/spinham/constants.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/spinham/hamiltonian.py` & `TB2J-0.9.0.1/TB2J/spinham/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/spinham/hamiltonian_terms.py` & `TB2J-0.9.0.1/TB2J/spinham/hamiltonian_terms.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/spinham/plot.py` & `TB2J-0.9.0.1/TB2J/spinham/plot.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/spinham/qsolver.py` & `TB2J-0.9.0.1/TB2J/spinham/qsolver.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/spinham/spin_api.py` & `TB2J-0.9.0.1/TB2J/spinham/spin_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/spinham/spin_xml.py` & `TB2J-0.9.0.1/TB2J/spinham/spin_xml.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/spinham/supercell.py` & `TB2J-0.9.0.1/TB2J/spinham/supercell.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/tensor_rotate.py` & `TB2J-0.9.0.1/TB2J/tensor_rotate.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/utest.py` & `TB2J-0.9.0.1/TB2J/utest.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/utils.py` & `TB2J-0.9.0.1/TB2J/utils.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/wannier/w90_parser.py` & `TB2J-0.9.0.1/TB2J/wannier/w90_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J/wannier/w90_tb_parser.py` & `TB2J-0.9.0.1/TB2J/wannier/w90_tb_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/TB2J.egg-info/PKG-INFO` & `TB2J-0.9.0.1/TB2J.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: TB2J
-Version: 0.9.0
+Version: 0.9.0.1
 Summary: TB2J: First principle to Heisenberg exchange J using tight-binding Green function method
-Home-page: UNKNOWN
 Author: Xu He
 Author-email: mailhexu@gmail.com
 License: BSD-2-clause
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.6
 License-File: LICENSE
+Requires-Dist: numpy>1.16.5
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: ase>=3.19
+Requires-Dist: tqdm
+Requires-Dist: pathos
+Requires-Dist: packaging>=20.0
+Requires-Dist: pre-commit
 
 TB2J is a Python package aimed to compute automatically the magnetic interactions (superexchange  and Dzyaloshinskii-Moriya) between atoms of magnetic crystals from DFT Hamiltonian based on Wannier functions or Linear combination of atomic orbitals. It uses the Green's function method and take the local rigid spin rotation as a perturbation. The package can take the output from Wannier90, which is interfaced with many density functional theory codes or from codes based on localised orbitals. A minimal user input is needed, which allows for an easily integration into a high-throughput workflows. 
-
```

### Comparing `TB2J-0.9.0/TB2J.egg-info/SOURCES.txt` & `TB2J-0.9.0.1/TB2J.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/scripts/TB2J_downfold.py` & `TB2J-0.9.0.1/scripts/TB2J_downfold.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/scripts/TB2J_eigen.py` & `TB2J-0.9.0.1/scripts/TB2J_eigen.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/scripts/TB2J_magnon.py` & `TB2J-0.9.0.1/scripts/TB2J_magnon.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/scripts/TB2J_merge.py` & `TB2J-0.9.0.1/scripts/TB2J_merge.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/scripts/TB2J_rotate.py` & `TB2J-0.9.0.1/scripts/TB2J_rotate.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/scripts/TB2J_rotateDM.py` & `TB2J-0.9.0.1/scripts/TB2J_rotateDM.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/scripts/abacus2J.py` & `TB2J-0.9.0.1/scripts/abacus2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/scripts/siesta2J.py` & `TB2J-0.9.0.1/scripts/siesta2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/scripts/wann2J.py` & `TB2J-0.9.0.1/scripts/wann2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.9.0/setup.py` & `TB2J-0.9.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
-__version__ = "0.9.0"
+__version__ = "0.9.0.1"
 
 long_description = """TB2J is a Python package aimed to compute automatically the magnetic interactions (superexchange  and Dzyaloshinskii-Moriya) between atoms of magnetic crystals from DFT Hamiltonian based on Wannier functions or Linear combination of atomic orbitals. It uses the Green's function method and take the local rigid spin rotation as a perturbation. The package can take the output from Wannier90, which is interfaced with many density functional theory codes or from codes based on localised orbitals. A minimal user input is needed, which allows for an easily integration into a high-throughput workflows. """
 
 setup(
     name="TB2J",
     version=__version__,
     description="TB2J: First principle to Heisenberg exchange J using tight-binding Green function method",
```

