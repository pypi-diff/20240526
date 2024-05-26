# Comparing `tmp/ambit_fe-1.2.7.tar.gz` & `tmp/ambit_fe-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambit_fe-1.2.7.tar", last modified: Mon May 20 08:45:07 2024, max compression
+gzip compressed data, was "ambit_fe-1.2.8.tar", last modified: Sun May 26 14:05:05 2024, max compression
```

## Comparing `ambit_fe-1.2.7.tar` & `ambit_fe-1.2.8.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-20 08:45:07.922971 ambit_fe-1.2.7/
--rw-rw-r--   0 mh        (1001) mh        (1001)     1073 2024-01-13 20:57:23.000000 ambit_fe-1.2.7/LICENSE
--rw-r--r--   0 mh        (1001) mh        (1001)     6223 2024-05-20 08:45:07.922971 ambit_fe-1.2.7/PKG-INFO
--rw-rw-r--   0 mh        (1001) mh        (1001)     4368 2024-03-06 11:21:34.000000 ambit_fe-1.2.7/README.md
--rw-rw-r--   0 mh        (1001) mh        (1001)      849 2024-05-20 08:38:02.000000 ambit_fe-1.2.7/pyproject.toml
--rw-rw-r--   0 mh        (1001) mh        (1001)       38 2024-05-20 08:45:07.922971 ambit_fe-1.2.7/setup.cfg
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-20 08:45:07.902971 ambit_fe-1.2.7/src/
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-20 08:45:07.906971 ambit_fe-1.2.7/src/ambit_fe/
--rw-rw-r--   0 mh        (1001) mh        (1001)      283 2024-01-13 19:07:42.000000 ambit_fe-1.2.7/src/ambit_fe/__init__.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-20 08:45:07.906971 ambit_fe-1.2.7/src/ambit_fe/ale/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:09.000000 ambit_fe-1.2.7/src/ambit_fe/ale/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     1860 2024-05-20 07:43:12.000000 ambit_fe-1.2.7/src/ambit_fe/ale/ale_kinematics_constitutive.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    14183 2024-05-15 09:27:26.000000 ambit_fe-1.2.7/src/ambit_fe/ale/ale_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     1834 2024-05-20 07:42:57.000000 ambit_fe-1.2.7/src/ambit_fe/ale/ale_material.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     1920 2024-05-14 15:10:21.000000 ambit_fe-1.2.7/src/ambit_fe/ale/ale_variationalform.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    15484 2024-03-21 20:03:07.000000 ambit_fe-1.2.7/src/ambit_fe/ambit_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    12464 2024-04-27 18:55:05.000000 ambit_fe-1.2.7/src/ambit_fe/base.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    32967 2024-05-17 21:14:28.000000 ambit_fe-1.2.7/src/ambit_fe/boundaryconditions.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-20 08:45:07.906971 ambit_fe-1.2.7/src/ambit_fe/coupling/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:12.000000 ambit_fe-1.2.7/src/ambit_fe/coupling/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    22475 2024-05-15 09:14:23.000000 ambit_fe-1.2.7/src/ambit_fe/coupling/fluid_ale_flow0d_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    26806 2024-05-16 10:26:46.000000 ambit_fe-1.2.7/src/ambit_fe/coupling/fluid_ale_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    36543 2024-05-06 17:50:28.000000 ambit_fe-1.2.7/src/ambit_fe/coupling/fluid_flow0d_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    18048 2024-05-15 09:11:38.000000 ambit_fe-1.2.7/src/ambit_fe/coupling/fsi_flow0d_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    17262 2024-05-15 09:09:51.000000 ambit_fe-1.2.7/src/ambit_fe/coupling/fsi_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    21754 2024-05-05 16:54:53.000000 ambit_fe-1.2.7/src/ambit_fe/coupling/solid_constraint_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    38541 2024-05-05 16:54:41.000000 ambit_fe-1.2.7/src/ambit_fe/coupling/solid_flow0d_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     5219 2024-03-09 22:52:23.000000 ambit_fe-1.2.7/src/ambit_fe/coupling/solid_flow0d_periodicref_main.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-20 08:45:07.906971 ambit_fe-1.2.7/src/ambit_fe/electrophysiology/
--rw-rw-r--   0 mh        (1001) mh        (1001)     1480 2024-02-12 18:01:07.000000 ambit_fe-1.2.7/src/ambit_fe/electrophysiology/electrophysiology_constitutive.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    14716 2024-04-11 19:20:57.000000 ambit_fe-1.2.7/src/ambit_fe/electrophysiology/electrophysiology_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)      947 2024-02-14 11:55:11.000000 ambit_fe-1.2.7/src/ambit_fe/electrophysiology/electrophysiology_variationalform.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     1242 2024-01-21 16:56:18.000000 ambit_fe-1.2.7/src/ambit_fe/expression.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-20 08:45:07.910971 ambit_fe-1.2.7/src/ambit_fe/flow0d/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:17.000000 ambit_fe-1.2.7/src/ambit_fe/flow0d/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    18497 2024-01-13 19:08:17.000000 ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     5113 2024-05-20 08:33:06.000000 ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_2elwindkessel.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     7236 2024-05-20 08:33:04.000000 ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_4elwindkesselLpZ.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     6719 2024-05-20 08:33:56.000000 ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_4elwindkesselLsZ.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     3939 2024-01-13 19:08:16.000000 ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_CRLinoutlink.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    15029 2024-01-13 19:08:16.000000 ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_coronary.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    30594 2024-01-13 19:08:17.000000 ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_syspul.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    78326 2024-01-13 19:08:17.000000 ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_syspulcap.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    54451 2024-01-13 19:08:17.000000 ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_syspulcaprespir.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     1666 2024-01-13 19:08:17.000000 ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_vad.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    22555 2024-05-16 14:10:39.000000 ambit_fe-1.2.7/src/ambit_fe/flow0d/flow0d_main.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-20 08:45:07.910971 ambit_fe-1.2.7/src/ambit_fe/fluid/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:05.000000 ambit_fe-1.2.7/src/ambit_fe/fluid/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     2990 2024-04-09 07:24:44.000000 ambit_fe-1.2.7/src/ambit_fe/fluid/fluid_kinematics_constitutive.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    89969 2024-05-13 12:15:01.000000 ambit_fe-1.2.7/src/ambit_fe/fluid/fluid_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)      581 2024-01-13 19:08:05.000000 ambit_fe-1.2.7/src/ambit_fe/fluid/fluid_material.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    17383 2024-05-14 15:22:01.000000 ambit_fe-1.2.7/src/ambit_fe/fluid/fluid_variationalform.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     8457 2024-05-07 06:21:03.000000 ambit_fe-1.2.7/src/ambit_fe/ioparams.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    65866 2024-04-04 12:42:34.000000 ambit_fe-1.2.7/src/ambit_fe/ioroutines.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     3372 2024-01-13 19:07:42.000000 ambit_fe-1.2.7/src/ambit_fe/mathutils.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     5319 2024-01-13 19:07:42.000000 ambit_fe-1.2.7/src/ambit_fe/meshutils.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-20 08:45:07.910971 ambit_fe-1.2.7/src/ambit_fe/mor/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:53.000000 ambit_fe-1.2.7/src/ambit_fe/mor/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    31475 2024-04-26 12:41:43.000000 ambit_fe-1.2.7/src/ambit_fe/mor/mor_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     1667 2024-01-13 19:07:42.000000 ambit_fe-1.2.7/src/ambit_fe/mpiroutines.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-20 08:45:07.910971 ambit_fe-1.2.7/src/ambit_fe/multiscale/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:48.000000 ambit_fe-1.2.7/src/ambit_fe/multiscale/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    15481 2024-01-21 16:15:11.000000 ambit_fe-1.2.7/src/ambit_fe/multiscale/solid_flow0d_growthremodel_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     9642 2024-05-20 08:34:19.000000 ambit_fe-1.2.7/src/ambit_fe/oderoutines.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-20 08:45:07.910971 ambit_fe-1.2.7/src/ambit_fe/postprocess/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:38.000000 ambit_fe-1.2.7/src/ambit_fe/postprocess/__init__.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    72147 2024-01-29 08:41:01.000000 ambit_fe-1.2.7/src/ambit_fe/postprocess/flow0d_plot.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     4022 2024-03-04 18:00:59.000000 ambit_fe-1.2.7/src/ambit_fe/resultcheck.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-20 08:45:07.910971 ambit_fe-1.2.7/src/ambit_fe/signet/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:26.000000 ambit_fe-1.2.7/src/ambit_fe/signet/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    37626 2024-01-13 19:08:26.000000 ambit_fe-1.2.7/src/ambit_fe/signet/signet_hypertrophy.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    10380 2024-03-08 08:28:58.000000 ambit_fe-1.2.7/src/ambit_fe/signet/signet_main.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-20 08:45:07.910971 ambit_fe-1.2.7/src/ambit_fe/solid/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:01.000000 ambit_fe-1.2.7/src/ambit_fe/solid/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    26329 2024-03-15 14:40:16.000000 ambit_fe-1.2.7/src/ambit_fe/solid/solid_kinematics_constitutive.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    69021 2024-05-05 16:53:25.000000 ambit_fe-1.2.7/src/ambit_fe/solid/solid_main.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    14578 2024-03-15 14:39:57.000000 ambit_fe-1.2.7/src/ambit_fe/solid/solid_material.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     5572 2024-01-13 19:08:01.000000 ambit_fe-1.2.7/src/ambit_fe/solid/solid_variationalform.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-20 08:45:07.914970 ambit_fe-1.2.7/src/ambit_fe/solver/
--rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:07:57.000000 ambit_fe-1.2.7/src/ambit_fe/solver/__init__.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    45093 2024-05-07 14:58:01.000000 ambit_fe-1.2.7/src/ambit_fe/solver/preconditioner.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     1904 2024-01-13 19:07:57.000000 ambit_fe-1.2.7/src/ambit_fe/solver/projection.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    48647 2024-05-07 06:54:00.000000 ambit_fe-1.2.7/src/ambit_fe/solver/solver_nonlin.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    27453 2024-05-04 09:02:14.000000 ambit_fe-1.2.7/src/ambit_fe/solver/solver_utils.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    31969 2024-05-17 21:17:57.000000 ambit_fe-1.2.7/src/ambit_fe/timeintegration.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     5823 2024-03-27 07:11:03.000000 ambit_fe-1.2.7/src/ambit_fe/utilities.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    12381 2024-03-19 17:33:23.000000 ambit_fe-1.2.7/src/ambit_fe/variationalform.py
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-20 08:45:07.918971 ambit_fe-1.2.7/src/ambit_fe.egg-info/
--rw-r--r--   0 mh        (1001) mh        (1001)     6223 2024-05-20 08:45:07.000000 ambit_fe-1.2.7/src/ambit_fe.egg-info/PKG-INFO
--rw-rw-r--   0 mh        (1001) mh        (1001)     5548 2024-05-20 08:45:07.000000 ambit_fe-1.2.7/src/ambit_fe.egg-info/SOURCES.txt
--rw-rw-r--   0 mh        (1001) mh        (1001)        1 2024-05-20 08:45:07.000000 ambit_fe-1.2.7/src/ambit_fe.egg-info/dependency_links.txt
--rw-rw-r--   0 mh        (1001) mh        (1001)       13 2024-05-20 08:45:07.000000 ambit_fe-1.2.7/src/ambit_fe.egg-info/requires.txt
--rw-rw-r--   0 mh        (1001) mh        (1001)        9 2024-05-20 08:45:07.000000 ambit_fe-1.2.7/src/ambit_fe.egg-info/top_level.txt
-drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-20 08:45:07.918971 ambit_fe-1.2.7/tests/
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3042 2024-02-23 10:07:29.000000 ambit_fe-1.2.7/tests/test_ale_linelast.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     2937 2024-02-13 18:57:20.000000 ambit_fe-1.2.7/tests/test_electrophysiology.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     7081 2024-02-23 10:07:26.000000 ambit_fe-1.2.7/tests/test_flow0d_0dheart_syspul.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    15443 2024-02-23 10:07:22.000000 ambit_fe-1.2.7/tests/test_flow0d_0dheart_syspulcap.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    15626 2024-02-23 10:07:19.000000 ambit_fe-1.2.7/tests/test_flow0d_0dheart_syspulcapcor.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    22686 2024-02-23 10:07:15.000000 ambit_fe-1.2.7/tests/test_flow0d_0dheart_syspulcaprespir_periodic.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     7490 2024-02-23 10:07:09.000000 ambit_fe-1.2.7/tests/test_flow0d_0dheart_syspulcor.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     8426 2024-02-23 10:07:05.000000 ambit_fe-1.2.7/tests/test_flow0d_0dheart_syspulcorvad.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     2531 2024-05-16 14:24:57.000000 ambit_fe-1.2.7/tests/test_flow0d_0dvol_2elwindkessel_n3.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     2426 2024-05-20 08:09:42.000000 ambit_fe-1.2.7/tests/test_flow0d_0dvol_4elwindkesselLpZ.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     2360 2024-05-20 08:09:39.000000 ambit_fe-1.2.7/tests/test_flow0d_0dvol_4elwindkesselLsZ.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    10709 2024-05-08 14:19:38.000000 ambit_fe-1.2.7/tests/test_fluid_ale_flow0d_lalv_syspul_prescribed.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4535 2024-05-05 15:25:38.000000 ambit_fe-1.2.7/tests/test_fluid_flow0d_monolagr_taylorhood_cylinder.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4675 2024-05-05 15:34:51.000000 ambit_fe-1.2.7/tests/test_fluid_flow0d_monolagr_taylorhood_cylinder_condensed.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3937 2024-04-09 06:48:19.000000 ambit_fe-1.2.7/tests/test_fluid_p1p1_stab_cylinder.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4356 2024-04-09 06:47:16.000000 ambit_fe-1.2.7/tests/test_fluid_p1p1_stab_cylinder_schur2x2.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4875 2024-05-20 07:12:17.000000 ambit_fe-1.2.7/tests/test_fluid_p1p1_stab_cylinder_valve.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3640 2024-02-23 10:06:18.000000 ambit_fe-1.2.7/tests/test_fluid_taylorhood_cylinder.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     6058 2024-05-16 14:16:49.000000 ambit_fe-1.2.7/tests/test_frsi_artseg_modepartitionunity.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4804 2024-03-25 09:01:11.000000 ambit_fe-1.2.7/tests/test_frsi_artseg_prefile.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     5868 2024-04-13 08:29:00.000000 ambit_fe-1.2.7/tests/test_frsi_artseg_prefile_bgsschur4x4.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     6016 2024-03-25 09:01:16.000000 ambit_fe-1.2.7/tests/test_frsi_artseg_prefile_partitioned_schur3x3.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     5358 2024-05-15 09:21:51.000000 ambit_fe-1.2.7/tests/test_frsi_artseg_prestress.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     7766 2024-04-09 06:52:03.000000 ambit_fe-1.2.7/tests/test_fsi_flow0d_p1p1_stab_artseg.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     6638 2024-04-09 06:51:31.000000 ambit_fe-1.2.7/tests/test_fsi_p1p1_stab_artseg.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     5667 2024-02-23 10:06:33.000000 ambit_fe-1.2.7/tests/test_fsi_taylorhood_artseg.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     2329 2024-05-16 14:11:50.000000 ambit_fe-1.2.7/tests/test_signet_0d_hypertrophy.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     2815 2024-03-15 14:39:36.000000 ambit_fe-1.2.7/tests/test_solid_2d_pres.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4995 2024-03-07 06:30:09.000000 ambit_fe-1.2.7/tests/test_solid_2dheart_frankstarling.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3769 2024-02-23 10:05:10.000000 ambit_fe-1.2.7/tests/test_solid_bodyforce_gravity.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3390 2024-02-23 10:05:06.000000 ambit_fe-1.2.7/tests/test_solid_constraint_volume_chamber.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3036 2024-02-23 10:05:02.000000 ambit_fe-1.2.7/tests/test_solid_divcont_ptc.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4079 2024-02-23 10:04:58.000000 ambit_fe-1.2.7/tests/test_solid_flow0d_monodir2field_4elwindkesselLpZ_chamber.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    18369 2024-04-13 14:32:00.000000 ambit_fe-1.2.7/tests/test_solid_flow0d_monodir2field_flux_syspulcap_3Dheart_schur3x3.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3997 2024-02-23 10:04:50.000000 ambit_fe-1.2.7/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4444 2024-05-07 06:45:16.000000 ambit_fe-1.2.7/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4619 2024-02-23 10:04:42.000000 ambit_fe-1.2.7/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2fieldsplit.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    18252 2024-04-13 08:32:04.000000 ambit_fe-1.2.7/tests/test_solid_flow0d_monodir_flux_syspulcap_3Dheart_schur2x2.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    10261 2024-03-05 08:28:49.000000 ambit_fe-1.2.7/tests/test_solid_flow0d_monodir_syspul_2dheart_prestress.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    10378 2024-03-25 08:40:46.000000 ambit_fe-1.2.7/tests/test_solid_flow0d_monodir_syspulcor_2dheart_rom.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4196 2024-03-05 18:14:14.000000 ambit_fe-1.2.7/tests/test_solid_flow0d_monolagr2field_2elwindkessel_chamber.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4969 2024-02-23 10:04:20.000000 ambit_fe-1.2.7/tests/test_solid_flow0d_monolagr_CRLinoutlink_chambers.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    19455 2024-02-23 10:04:16.000000 ambit_fe-1.2.7/tests/test_solid_flow0d_multiscalegrowthremodeling_concentric.py
--rw-rw-r--   0 mh        (1001) mh        (1001)    19437 2024-02-23 10:04:11.000000 ambit_fe-1.2.7/tests/test_solid_flow0d_multiscalegrowthremodeling_eccentric.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)    11399 2024-03-09 22:53:35.000000 ambit_fe-1.2.7/tests/test_solid_flow0d_periodicref_syspul_lvchamber.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3302 2024-02-23 10:03:13.000000 ambit_fe-1.2.7/tests/test_solid_growth_prescribed_iso_lv.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3859 2024-02-23 10:04:01.000000 ambit_fe-1.2.7/tests/test_solid_growth_volstressmandel.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4034 2024-02-23 10:03:58.000000 ambit_fe-1.2.7/tests/test_solid_growth_volstressmandel_incomp.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4595 2024-02-23 10:03:55.000000 ambit_fe-1.2.7/tests/test_solid_growthremodeling_fiberstretch.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     7304 2024-02-23 10:03:51.000000 ambit_fe-1.2.7/tests/test_solid_mat_uniax_hex_2field.py
--rwxr-xr-x   0 mh        (1001) mh        (1001)     7538 2024-01-21 17:16:25.000000 ambit_fe-1.2.7/tests/test_solid_membrane.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4541 2024-05-20 07:14:36.000000 ambit_fe-1.2.7/tests/test_solid_ost_dbc_ramp.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3710 2024-02-23 10:03:41.000000 ambit_fe-1.2.7/tests/test_solid_pinch_edge.py
--rw-rw-r--   0 mh        (1001) mh        (1001)     3171 2024-02-23 10:03:37.000000 ambit_fe-1.2.7/tests/test_solid_plasticity_vonmises.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3523 2024-02-23 10:03:34.000000 ambit_fe-1.2.7/tests/test_solid_robin_genalpha.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     4037 2024-05-07 06:44:22.000000 ambit_fe-1.2.7/tests/test_solid_robin_genalpha_amg.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3108 2024-02-23 10:03:26.000000 ambit_fe-1.2.7/tests/test_solid_robin_static_prestress.py
--rwxrwxr-x   0 mh        (1001) mh        (1001)     3114 2024-02-23 10:03:22.000000 ambit_fe-1.2.7/tests/test_solid_robin_visco.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-26 14:05:05.579576 ambit_fe-1.2.8/
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1073 2024-01-13 20:57:23.000000 ambit_fe-1.2.8/LICENSE
+-rw-r--r--   0 mh        (1001) mh        (1001)     6224 2024-05-26 14:05:05.579576 ambit_fe-1.2.8/PKG-INFO
+-rw-rw-r--   0 mh        (1001) mh        (1001)     4369 2024-05-26 13:59:00.000000 ambit_fe-1.2.8/README.md
+-rw-rw-r--   0 mh        (1001) mh        (1001)      849 2024-05-26 13:59:25.000000 ambit_fe-1.2.8/pyproject.toml
+-rw-rw-r--   0 mh        (1001) mh        (1001)       38 2024-05-26 14:05:05.579576 ambit_fe-1.2.8/setup.cfg
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-26 14:05:05.559576 ambit_fe-1.2.8/src/
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-26 14:05:05.563576 ambit_fe-1.2.8/src/ambit_fe/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      283 2024-01-13 19:07:42.000000 ambit_fe-1.2.8/src/ambit_fe/__init__.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-26 14:05:05.563576 ambit_fe-1.2.8/src/ambit_fe/ale/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:09.000000 ambit_fe-1.2.8/src/ambit_fe/ale/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1945 2024-05-26 13:54:27.000000 ambit_fe-1.2.8/src/ambit_fe/ale/ale_kinematics_constitutive.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    14225 2024-05-24 18:02:55.000000 ambit_fe-1.2.8/src/ambit_fe/ale/ale_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     2702 2024-05-26 13:53:57.000000 ambit_fe-1.2.8/src/ambit_fe/ale/ale_material.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1920 2024-05-14 15:10:21.000000 ambit_fe-1.2.8/src/ambit_fe/ale/ale_variationalform.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    15484 2024-03-21 20:03:07.000000 ambit_fe-1.2.8/src/ambit_fe/ambit_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    12464 2024-04-27 18:55:05.000000 ambit_fe-1.2.8/src/ambit_fe/base.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    32729 2024-05-23 17:10:09.000000 ambit_fe-1.2.8/src/ambit_fe/boundaryconditions.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-26 14:05:05.563576 ambit_fe-1.2.8/src/ambit_fe/coupling/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:12.000000 ambit_fe-1.2.8/src/ambit_fe/coupling/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    22269 2024-05-23 17:50:14.000000 ambit_fe-1.2.8/src/ambit_fe/coupling/fluid_ale_flow0d_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    27713 2024-05-23 17:54:00.000000 ambit_fe-1.2.8/src/ambit_fe/coupling/fluid_ale_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    36124 2024-05-23 17:47:57.000000 ambit_fe-1.2.8/src/ambit_fe/coupling/fluid_flow0d_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    17711 2024-05-21 13:30:22.000000 ambit_fe-1.2.8/src/ambit_fe/coupling/fsi_flow0d_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    17262 2024-05-15 09:09:51.000000 ambit_fe-1.2.8/src/ambit_fe/coupling/fsi_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    21547 2024-05-23 17:55:55.000000 ambit_fe-1.2.8/src/ambit_fe/coupling/solid_constraint_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    38122 2024-05-24 17:37:27.000000 ambit_fe-1.2.8/src/ambit_fe/coupling/solid_flow0d_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     5219 2024-03-09 22:52:23.000000 ambit_fe-1.2.8/src/ambit_fe/coupling/solid_flow0d_periodicref_main.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-26 14:05:05.563576 ambit_fe-1.2.8/src/ambit_fe/electrophysiology/
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1480 2024-02-12 18:01:07.000000 ambit_fe-1.2.8/src/ambit_fe/electrophysiology/electrophysiology_constitutive.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    14716 2024-04-11 19:20:57.000000 ambit_fe-1.2.8/src/ambit_fe/electrophysiology/electrophysiology_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)      947 2024-02-14 11:55:11.000000 ambit_fe-1.2.8/src/ambit_fe/electrophysiology/electrophysiology_variationalform.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1242 2024-01-21 16:56:18.000000 ambit_fe-1.2.8/src/ambit_fe/expression.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-26 14:05:05.563576 ambit_fe-1.2.8/src/ambit_fe/flow0d/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:17.000000 ambit_fe-1.2.8/src/ambit_fe/flow0d/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    18497 2024-01-13 19:08:17.000000 ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     5113 2024-05-20 08:33:06.000000 ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_2elwindkessel.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     7119 2024-05-22 21:38:26.000000 ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_4elwindkesselLpZ.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     6611 2024-05-22 21:38:31.000000 ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_4elwindkesselLsZ.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     3939 2024-01-13 19:08:16.000000 ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_CRLinoutlink.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    15029 2024-01-13 19:08:16.000000 ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_coronary.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    30594 2024-01-13 19:08:17.000000 ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_syspul.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    78326 2024-01-13 19:08:17.000000 ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_syspulcap.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    54451 2024-01-13 19:08:17.000000 ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_syspulcaprespir.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1666 2024-01-13 19:08:17.000000 ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_vad.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    22555 2024-05-16 14:10:39.000000 ambit_fe-1.2.8/src/ambit_fe/flow0d/flow0d_main.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-26 14:05:05.563576 ambit_fe-1.2.8/src/ambit_fe/fluid/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:05.000000 ambit_fe-1.2.8/src/ambit_fe/fluid/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     2990 2024-04-09 07:24:44.000000 ambit_fe-1.2.8/src/ambit_fe/fluid/fluid_kinematics_constitutive.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    89546 2024-05-24 18:10:50.000000 ambit_fe-1.2.8/src/ambit_fe/fluid/fluid_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)      581 2024-01-13 19:08:05.000000 ambit_fe-1.2.8/src/ambit_fe/fluid/fluid_material.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    17383 2024-05-14 15:22:01.000000 ambit_fe-1.2.8/src/ambit_fe/fluid/fluid_variationalform.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     8457 2024-05-07 06:21:03.000000 ambit_fe-1.2.8/src/ambit_fe/ioparams.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    65919 2024-05-23 17:44:19.000000 ambit_fe-1.2.8/src/ambit_fe/ioroutines.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     3372 2024-01-13 19:07:42.000000 ambit_fe-1.2.8/src/ambit_fe/mathutils.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     5319 2024-01-13 19:07:42.000000 ambit_fe-1.2.8/src/ambit_fe/meshutils.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-26 14:05:05.563576 ambit_fe-1.2.8/src/ambit_fe/mor/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:53.000000 ambit_fe-1.2.8/src/ambit_fe/mor/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    31195 2024-05-22 17:59:56.000000 ambit_fe-1.2.8/src/ambit_fe/mor/mor_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1667 2024-01-13 19:07:42.000000 ambit_fe-1.2.8/src/ambit_fe/mpiroutines.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-26 14:05:05.563576 ambit_fe-1.2.8/src/ambit_fe/multiscale/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:48.000000 ambit_fe-1.2.8/src/ambit_fe/multiscale/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    15481 2024-01-21 16:15:11.000000 ambit_fe-1.2.8/src/ambit_fe/multiscale/solid_flow0d_growthremodel_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     9642 2024-05-20 08:34:19.000000 ambit_fe-1.2.8/src/ambit_fe/oderoutines.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-26 14:05:05.563576 ambit_fe-1.2.8/src/ambit_fe/postprocess/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:38.000000 ambit_fe-1.2.8/src/ambit_fe/postprocess/__init__.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    72147 2024-01-29 08:41:01.000000 ambit_fe-1.2.8/src/ambit_fe/postprocess/flow0d_plot.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     4022 2024-03-04 18:00:59.000000 ambit_fe-1.2.8/src/ambit_fe/resultcheck.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-26 14:05:05.563576 ambit_fe-1.2.8/src/ambit_fe/signet/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:26.000000 ambit_fe-1.2.8/src/ambit_fe/signet/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    37626 2024-01-13 19:08:26.000000 ambit_fe-1.2.8/src/ambit_fe/signet/signet_hypertrophy.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    10380 2024-03-08 08:28:58.000000 ambit_fe-1.2.8/src/ambit_fe/signet/signet_main.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-26 14:05:05.567576 ambit_fe-1.2.8/src/ambit_fe/solid/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:08:01.000000 ambit_fe-1.2.8/src/ambit_fe/solid/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    26329 2024-03-15 14:40:16.000000 ambit_fe-1.2.8/src/ambit_fe/solid/solid_kinematics_constitutive.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    69025 2024-05-23 17:19:23.000000 ambit_fe-1.2.8/src/ambit_fe/solid/solid_main.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    14578 2024-03-15 14:39:57.000000 ambit_fe-1.2.8/src/ambit_fe/solid/solid_material.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     5572 2024-01-13 19:08:01.000000 ambit_fe-1.2.8/src/ambit_fe/solid/solid_variationalform.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-26 14:05:05.567576 ambit_fe-1.2.8/src/ambit_fe/solver/
+-rw-rw-r--   0 mh        (1001) mh        (1001)      231 2024-01-13 19:07:57.000000 ambit_fe-1.2.8/src/ambit_fe/solver/__init__.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    45093 2024-05-07 14:58:01.000000 ambit_fe-1.2.8/src/ambit_fe/solver/preconditioner.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     1904 2024-01-13 19:07:57.000000 ambit_fe-1.2.8/src/ambit_fe/solver/projection.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    48647 2024-05-07 06:54:00.000000 ambit_fe-1.2.8/src/ambit_fe/solver/solver_nonlin.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    27453 2024-05-04 09:02:14.000000 ambit_fe-1.2.8/src/ambit_fe/solver/solver_utils.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    31969 2024-05-17 21:17:57.000000 ambit_fe-1.2.8/src/ambit_fe/timeintegration.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     5823 2024-03-27 07:11:03.000000 ambit_fe-1.2.8/src/ambit_fe/utilities.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    12381 2024-03-19 17:33:23.000000 ambit_fe-1.2.8/src/ambit_fe/variationalform.py
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-26 14:05:05.579576 ambit_fe-1.2.8/src/ambit_fe.egg-info/
+-rw-r--r--   0 mh        (1001) mh        (1001)     6224 2024-05-26 14:05:05.000000 ambit_fe-1.2.8/src/ambit_fe.egg-info/PKG-INFO
+-rw-rw-r--   0 mh        (1001) mh        (1001)     5548 2024-05-26 14:05:05.000000 ambit_fe-1.2.8/src/ambit_fe.egg-info/SOURCES.txt
+-rw-rw-r--   0 mh        (1001) mh        (1001)        1 2024-05-26 14:05:05.000000 ambit_fe-1.2.8/src/ambit_fe.egg-info/dependency_links.txt
+-rw-rw-r--   0 mh        (1001) mh        (1001)       13 2024-05-26 14:05:05.000000 ambit_fe-1.2.8/src/ambit_fe.egg-info/requires.txt
+-rw-rw-r--   0 mh        (1001) mh        (1001)        9 2024-05-26 14:05:05.000000 ambit_fe-1.2.8/src/ambit_fe.egg-info/top_level.txt
+drwxrwxr-x   0 mh        (1001) mh        (1001)        0 2024-05-26 14:05:05.579576 ambit_fe-1.2.8/tests/
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3042 2024-02-23 10:07:29.000000 ambit_fe-1.2.8/tests/test_ale_linelast.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     2937 2024-02-13 18:57:20.000000 ambit_fe-1.2.8/tests/test_electrophysiology.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     7081 2024-02-23 10:07:26.000000 ambit_fe-1.2.8/tests/test_flow0d_0dheart_syspul.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    15443 2024-02-23 10:07:22.000000 ambit_fe-1.2.8/tests/test_flow0d_0dheart_syspulcap.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    15626 2024-02-23 10:07:19.000000 ambit_fe-1.2.8/tests/test_flow0d_0dheart_syspulcapcor.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    22686 2024-02-23 10:07:15.000000 ambit_fe-1.2.8/tests/test_flow0d_0dheart_syspulcaprespir_periodic.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     7490 2024-02-23 10:07:09.000000 ambit_fe-1.2.8/tests/test_flow0d_0dheart_syspulcor.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     8426 2024-02-23 10:07:05.000000 ambit_fe-1.2.8/tests/test_flow0d_0dheart_syspulcorvad.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     2531 2024-05-16 14:24:57.000000 ambit_fe-1.2.8/tests/test_flow0d_0dvol_2elwindkessel_n3.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     2426 2024-05-20 08:09:42.000000 ambit_fe-1.2.8/tests/test_flow0d_0dvol_4elwindkesselLpZ.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     2360 2024-05-20 08:09:39.000000 ambit_fe-1.2.8/tests/test_flow0d_0dvol_4elwindkesselLsZ.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    10713 2024-05-23 17:45:25.000000 ambit_fe-1.2.8/tests/test_fluid_ale_flow0d_lalv_syspul_prescribed.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4535 2024-05-05 15:25:38.000000 ambit_fe-1.2.8/tests/test_fluid_flow0d_monolagr_taylorhood_cylinder.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4675 2024-05-05 15:34:51.000000 ambit_fe-1.2.8/tests/test_fluid_flow0d_monolagr_taylorhood_cylinder_condensed.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3937 2024-04-09 06:48:19.000000 ambit_fe-1.2.8/tests/test_fluid_p1p1_stab_cylinder.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4356 2024-04-09 06:47:16.000000 ambit_fe-1.2.8/tests/test_fluid_p1p1_stab_cylinder_schur2x2.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4879 2024-05-23 18:04:54.000000 ambit_fe-1.2.8/tests/test_fluid_p1p1_stab_cylinder_valve.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3640 2024-02-23 10:06:18.000000 ambit_fe-1.2.8/tests/test_fluid_taylorhood_cylinder.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     5955 2024-05-21 13:26:08.000000 ambit_fe-1.2.8/tests/test_frsi_artseg_modepartitionunity.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4804 2024-03-25 09:01:11.000000 ambit_fe-1.2.8/tests/test_frsi_artseg_prefile.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     5868 2024-04-13 08:29:00.000000 ambit_fe-1.2.8/tests/test_frsi_artseg_prefile_bgsschur4x4.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     6016 2024-03-25 09:01:16.000000 ambit_fe-1.2.8/tests/test_frsi_artseg_prefile_partitioned_schur3x3.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     5378 2024-05-24 18:03:04.000000 ambit_fe-1.2.8/tests/test_frsi_artseg_prestress.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     7766 2024-04-09 06:52:03.000000 ambit_fe-1.2.8/tests/test_fsi_flow0d_p1p1_stab_artseg.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     6638 2024-04-09 06:51:31.000000 ambit_fe-1.2.8/tests/test_fsi_p1p1_stab_artseg.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     5667 2024-02-23 10:06:33.000000 ambit_fe-1.2.8/tests/test_fsi_taylorhood_artseg.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     2329 2024-05-16 14:11:50.000000 ambit_fe-1.2.8/tests/test_signet_0d_hypertrophy.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     2815 2024-03-15 14:39:36.000000 ambit_fe-1.2.8/tests/test_solid_2d_pres.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4995 2024-03-07 06:30:09.000000 ambit_fe-1.2.8/tests/test_solid_2dheart_frankstarling.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3769 2024-02-23 10:05:10.000000 ambit_fe-1.2.8/tests/test_solid_bodyforce_gravity.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3390 2024-02-23 10:05:06.000000 ambit_fe-1.2.8/tests/test_solid_constraint_volume_chamber.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3036 2024-02-23 10:05:02.000000 ambit_fe-1.2.8/tests/test_solid_divcont_ptc.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4079 2024-02-23 10:04:58.000000 ambit_fe-1.2.8/tests/test_solid_flow0d_monodir2field_4elwindkesselLpZ_chamber.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    18369 2024-04-13 14:32:00.000000 ambit_fe-1.2.8/tests/test_solid_flow0d_monodir2field_flux_syspulcap_3Dheart_schur3x3.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3997 2024-02-23 10:04:50.000000 ambit_fe-1.2.8/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4444 2024-05-07 06:45:16.000000 ambit_fe-1.2.8/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4619 2024-02-23 10:04:42.000000 ambit_fe-1.2.8/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2fieldsplit.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    18252 2024-04-13 08:32:04.000000 ambit_fe-1.2.8/tests/test_solid_flow0d_monodir_flux_syspulcap_3Dheart_schur2x2.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    10261 2024-03-05 08:28:49.000000 ambit_fe-1.2.8/tests/test_solid_flow0d_monodir_syspul_2dheart_prestress.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    10378 2024-03-25 08:40:46.000000 ambit_fe-1.2.8/tests/test_solid_flow0d_monodir_syspulcor_2dheart_rom.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4196 2024-03-05 18:14:14.000000 ambit_fe-1.2.8/tests/test_solid_flow0d_monolagr2field_2elwindkessel_chamber.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4969 2024-02-23 10:04:20.000000 ambit_fe-1.2.8/tests/test_solid_flow0d_monolagr_CRLinoutlink_chambers.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    19455 2024-02-23 10:04:16.000000 ambit_fe-1.2.8/tests/test_solid_flow0d_multiscalegrowthremodeling_concentric.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)    19437 2024-02-23 10:04:11.000000 ambit_fe-1.2.8/tests/test_solid_flow0d_multiscalegrowthremodeling_eccentric.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)    11399 2024-03-09 22:53:35.000000 ambit_fe-1.2.8/tests/test_solid_flow0d_periodicref_syspul_lvchamber.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3302 2024-02-23 10:03:13.000000 ambit_fe-1.2.8/tests/test_solid_growth_prescribed_iso_lv.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3859 2024-02-23 10:04:01.000000 ambit_fe-1.2.8/tests/test_solid_growth_volstressmandel.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4034 2024-02-23 10:03:58.000000 ambit_fe-1.2.8/tests/test_solid_growth_volstressmandel_incomp.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4595 2024-02-23 10:03:55.000000 ambit_fe-1.2.8/tests/test_solid_growthremodeling_fiberstretch.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     7304 2024-02-23 10:03:51.000000 ambit_fe-1.2.8/tests/test_solid_mat_uniax_hex_2field.py
+-rwxr-xr-x   0 mh        (1001) mh        (1001)     7538 2024-01-21 17:16:25.000000 ambit_fe-1.2.8/tests/test_solid_membrane.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4541 2024-05-20 07:14:36.000000 ambit_fe-1.2.8/tests/test_solid_ost_dbc_ramp.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3710 2024-02-23 10:03:41.000000 ambit_fe-1.2.8/tests/test_solid_pinch_edge.py
+-rw-rw-r--   0 mh        (1001) mh        (1001)     3171 2024-02-23 10:03:37.000000 ambit_fe-1.2.8/tests/test_solid_plasticity_vonmises.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3523 2024-02-23 10:03:34.000000 ambit_fe-1.2.8/tests/test_solid_robin_genalpha.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     4037 2024-05-07 06:44:22.000000 ambit_fe-1.2.8/tests/test_solid_robin_genalpha_amg.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3108 2024-02-23 10:03:26.000000 ambit_fe-1.2.8/tests/test_solid_robin_static_prestress.py
+-rwxrwxr-x   0 mh        (1001) mh        (1001)     3114 2024-02-23 10:03:22.000000 ambit_fe-1.2.8/tests/test_solid_robin_visco.py
```

### Comparing `ambit_fe-1.2.7/LICENSE` & `ambit_fe-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/PKG-INFO` & `ambit_fe-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambit-fe
-Version: 1.2.7
+Version: 1.2.8
 Summary: A FEniCS-based cardiovascular multi-physics solver
 Author-email: Marc Hirschvogel <marc.hirschvogel@ambit.net>
 License: MIT License
         
         Copyright (c) 2024 Marc Hirschvogel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,15 +34,15 @@
 Requires-Dist: sympy
 
 # README #
 
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05744/status.svg)](https://doi.org/10.21105/joss.05744)
 
 Ambit is an open-source multi-physics finite element solver written in Python, supporting solid and fluid mechanics, fluid-structure interaction (FSI), and lumped-parameter models.
-It is tailored towards solving problems in cardiac mechanics, but may also be used for more general nonlinear finite element analysis. It uses the finite element backend FEniCS and
+It is tailored towards solving problems in cardiac mechanics, but may also be used for more general nonlinear finite element analysis. It uses the finite element backend FEniCSx and
 linear algebra library PETSc.
 
 https://github.com/marchirschvogel/ambit/assets/52761273/a438ff55-9b37-4572-a1c5-499dd3cfba73
 
 **Heart cycle simulation of a generic bi-ventricular heart model coupled to a closed-loop circulation model.**
 
 https://github.com/marchirschvogel/ambit/assets/52761273/8e681cb6-7a4f-4d1f-b34a-cefb642f44b7
```

### Comparing `ambit_fe-1.2.7/README.md` & `ambit_fe-1.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # README #
 
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05744/status.svg)](https://doi.org/10.21105/joss.05744)
 
 Ambit is an open-source multi-physics finite element solver written in Python, supporting solid and fluid mechanics, fluid-structure interaction (FSI), and lumped-parameter models.
-It is tailored towards solving problems in cardiac mechanics, but may also be used for more general nonlinear finite element analysis. It uses the finite element backend FEniCS and
+It is tailored towards solving problems in cardiac mechanics, but may also be used for more general nonlinear finite element analysis. It uses the finite element backend FEniCSx and
 linear algebra library PETSc.
 
 https://github.com/marchirschvogel/ambit/assets/52761273/a438ff55-9b37-4572-a1c5-499dd3cfba73
 
 **Heart cycle simulation of a generic bi-ventricular heart model coupled to a closed-loop circulation model.**
 
 https://github.com/marchirschvogel/ambit/assets/52761273/8e681cb6-7a4f-4d1f-b34a-cefb642f44b7
```

### Comparing `ambit_fe-1.2.7/pyproject.toml` & `ambit_fe-1.2.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=61.0.0", "wheel"]
 
 [project]
 name = "ambit-fe"
-version = "v1.2.7"
+version = "v1.2.8"
 description = "A FEniCS-based cardiovascular multi-physics solver"
 authors = [{name = "Marc Hirschvogel", email = "marc.hirschvogel@ambit.net"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 keywords = [
     "finite elements",
     "solid mechanics",
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe/ale/ale_kinematics_constitutive.py` & `ambit_fe-1.2.8/src/ambit_fe/ale/ale_kinematics_constitutive.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,57 +32,59 @@
 
         F_ = ufl.variable(self.kin.F(d_))
 
         dim = len(d_)
 
         stress = ufl.constantvalue.zero((dim,dim))
 
-        mat = materiallaw(d_,F_)
+        mat = materiallaw(d_, F_, self.kin.elem_metrics)
 
         m = 0
         for matlaw in self.matmodels:
 
             # extract associated material parameters
             matparams_m = self.matparams[m]
 
-            if matlaw == 'linelast':
+            if matlaw == 'diffusion':
+
+                stress += mat.diffusion(matparams_m)
+
+            elif matlaw == 'diffusion_sym':
+
+                stress += mat.diffusion_sym(matparams_m)
+
+            elif matlaw == 'linelast':
 
                 stress += mat.linelast(matparams_m)
 
             elif matlaw == 'neohooke':
 
                 stress += mat.neohooke(matparams_m)
 
             elif matlaw == 'exponential':
 
                 stress += mat.exponential(matparams_m)
 
-            elif matlaw == 'diffusion':
-
-                stress += mat.diffusion(matparams_m)
-
-            elif matlaw == 'diffusion_sym':
-
-                stress += mat.diffusion_sym(matparams_m)
-
             else:
 
                 raise NameError('Unknown ALE material law!')
 
             m += 1
 
         return stress
 
 
 class kinematics:
 
-    def __init__(self, dim):
+    def __init__(self, dim, elem_metrics=None):
 
         self.dim = dim
 
         # identity tensor
         self.I = ufl.Identity(self.dim)
 
+        self.elem_metrics = elem_metrics
+
 
     # ALE deformation gradient
     def F(self, d_):
         return self.I + ufl.grad(d_)
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe/ale/ale_main.py` & `ambit_fe-1.2.8/src/ambit_fe/ale/ale_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 
         self.numdof = self.d.vector.getSize()
 
         # initialize ALE time-integration class
         self.ti = timeintegration.timeintegration_ale(time_params, self.pbase.dt, self.pbase.numstep, fem_params, time_curves=time_curves, t_init=self.pbase.t_init, dim=self.dim, comm=self.comm)
 
         # initialize kinematics_constitutive class
-        self.ki = ale_kinematics_constitutive.kinematics(self.dim)
+        self.ki = ale_kinematics_constitutive.kinematics(self.dim, elem_metrics={'jac_det' : self.io.detj0})
 
         # initialize material/constitutive classes (one per domain)
         self.ma = []
         for n in range(self.num_domains):
             self.ma.append(ale_kinematics_constitutive.constitutive(self.ki, self.constitutive_models['MAT'+str(n+1)]))
 
         # initialize ALE variational form class
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe/ale/ale_variationalform.py` & `ambit_fe-1.2.8/src/ambit_fe/ale/ale_variationalform.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/ambit_main.py` & `ambit_fe-1.2.8/src/ambit_fe/ambit_main.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/base.py` & `ambit_fe-1.2.8/src/ambit_fe/base.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/boundaryconditions.py` & `ambit_fe-1.2.8/src/ambit_fe/boundaryconditions.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,31 +101,27 @@
                 else:
                     # read file into function
                     self.io.readfunction(func, fle, filetype=ftype)
             else:
                 raise RuntimeError("Need to have 'curve', 'val', 'expression', or 'file' specified!")
 
             if d['dir'] == 'all':
-                for i in range(len(d['id'])):
-                    self.dbcs.append( fem.dirichletbc(func, fem.locate_dofs_topological(V, codim, mdata.indices[mdata.values == d['id'][i]])) )
+                self.dbcs.append( fem.dirichletbc(func, fem.locate_dofs_topological(V, codim, mdata.indices[np.isin(mdata.values, d['id'])])) )
 
             elif d['dir'] == 'x':
-                for i in range(len(d['id'])):
-                    dofs_x = fem.locate_dofs_topological(V.sub(0), codim, mdata.indices[mdata.values == d['id'][i]])
-                    self.dbcs.append( fem.dirichletbc(func.sub(0), dofs_x) )
+                dofs_x = fem.locate_dofs_topological(V.sub(0), codim, mdata.indices[np.isin(mdata.values, d['id'])])
+                self.dbcs.append( fem.dirichletbc(func.sub(0), dofs_x) )
 
             elif d['dir'] == 'y':
-                for i in range(len(d['id'])):
-                    dofs_y = fem.locate_dofs_topological(V.sub(1), codim, mdata.indices[mdata.values == d['id'][i]])
-                    self.dbcs.append( fem.dirichletbc(func.sub(1), dofs_y) )
+                dofs_y = fem.locate_dofs_topological(V.sub(1), codim, mdata.indices[np.isin(mdata.values, d['id'])])
+                self.dbcs.append( fem.dirichletbc(func.sub(1), dofs_y) )
 
             elif d['dir'] == 'z':
-                for i in range(len(d['id'])):
-                    dofs_z = fem.locate_dofs_topological(V.sub(2), codim, mdata.indices[mdata.values == d['id'][i]])
-                    self.dbcs.append( fem.dirichletbc(func.sub(2), dofs_z) )
+                dofs_z = fem.locate_dofs_topological(V.sub(2), codim, mdata.indices[np.isin(mdata.values, d['id'])])
+                self.dbcs.append( fem.dirichletbc(func.sub(2), dofs_z) )
 
             elif d['dir'] == '2dimX':
                 dofs_x = fem.locate_dofs_topological(V.sub(0), codim, mesh.locate_entities_boundary(self.io.mesh, codim, self.twodimX))
                 self.dbcs.append( fem.dirichletbc(func.sub(0), dofs_x) )
 
             elif d['dir'] == '2dimY':
                 dofs_y = fem.locate_dofs_topological(V.sub(1), codim, mesh.locate_entities_boundary(self.io.mesh, codim, self.twodimY))
@@ -163,16 +159,15 @@
                 try: scale = d['scale']
                 except: scale = 1.0
                 self.ti.funcs_data.append({func : d['file'], 'scale' : scale})
                 self.have_dirichlet_file = True
             else:
                 raise RuntimeError("Need to have 'curve', 'val', or 'file' specified!")
 
-            for i in range(len(d['id'])):
-                self.dbcs.append( fem.dirichletbc(func, fem.locate_dofs_topological(V, self.dim, self.io.mt_d.indices[self.io.mt_d.values == d['id'][i]])) )
+            self.dbcs.append( fem.dirichletbc(func, fem.locate_dofs_topological(V, self.dim, self.io.mt_d.indices[np.isin(self.io.mt_d.values, d['id'])])) )
 
 
     # function to mark x=0
     def twodimX(self, x):
         return np.isclose(x[0], 0.0)
 
     # function to mark y=0
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe/coupling/fluid_ale_flow0d_main.py` & `ambit_fe-1.2.8/src/ambit_fe/coupling/fluid_ale_flow0d_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,19 +158,16 @@
 
             self.dofs_coupling_vq = [[]]*self.pbf0.num_coupling_surf
 
             self.k_sd_subvec, sze_sd = [], []
 
             for n in range(self.pbf0.num_coupling_surf):
 
-                nds_vq_local = [[]]*len(self.pbf0.surface_vq_ids[n])
-                for i in range(len(self.pbf0.surface_vq_ids[n])):
-                    nds_vq_local[i] = fem.locate_dofs_topological(self.pba.V_d, self.pba.io.mesh.topology.dim-1, self.pba.io.mt_b1.indices[self.pba.io.mt_b1.values == self.pbf0.surface_vq_ids[n][i]])
-                nds_vq_local_flat = [item for sublist in nds_vq_local for item in sublist]
-                nds_vq = np.array( self.pbf.V_v.dofmap.index_map.local_to_global(np.asarray(nds_vq_local_flat, dtype=np.int32)), dtype=np.int32 )
+                nds_vq_local = fem.locate_dofs_topological(self.pba.V_d, self.pba.io.mesh.topology.dim-1, self.pba.io.mt_b1.indices[np.isin(self.pba.io.mt_b1.values, self.pbf0.surface_vq_ids[n])])
+                nds_vq = np.array( self.pbf.V_v.dofmap.index_map.local_to_global(np.asarray(nds_vq_local, dtype=np.int32)), dtype=np.int32 )
                 self.dofs_coupling_vq[n] = PETSc.IS().createBlock(self.pba.V_d.dofmap.index_map_bs, nds_vq, comm=self.comm)
 
                 self.k_sd_subvec.append( self.k_sd_vec[n].getSubVector(self.dofs_coupling_vq[n]) )
 
                 sze_sd.append(self.k_sd_subvec[-1].getSize())
 
             # derivative of multiplier constraint w.r.t. fluid velocities
@@ -197,26 +194,25 @@
 
     def assemble_stiffness(self, t, subsolver=None):
 
         if self.have_weak_dirichlet_fluid_ale:
             self.K_dv.zeroEntries()
             fem.petsc.assemble_matrix(self.K_dv, self.jac_dv, self.pba.bc.dbcs)
             self.K_dv.assemble()
-
-        elif self.have_dbc_fluid_ale: # TODO: Does not seem to yield quadratic convergence yet! Why?
-            self.K_dv.zeroEntries()
-            fem.petsc.assemble_matrix(self.K_dv, self.pba.jac_dd, self.pba.bc.dbcs)
-            # fem.petsc.assemble_matrix(self.K_dv, self.pba.jac_dd, [])
-            self.K_dv.assemble()
-
-            # self.K_dv.zeroRowsColumns(self.iset_d_0, diag=0.)
-            self.K_dv.zeroRows(self.iset_d_0, diag=0.)
+        elif self.have_dbc_fluid_ale:
+            self.K_dv_.zeroEntries()
+            fem.petsc.assemble_matrix(self.K_dv_, self.pba.jac_dd, self.pba.bc.dbcs_nofluid) # need DBCs w/o fluid here
+            self.K_dv_.assemble()
+            # multiply to get the relevant columns only
+            self.K_dv_.matMult(self.Diag_ale, result=self.K_dv)
+            # zero rows where DBC is applied and set diagonal entry to -1
+            self.K_dv.zeroRows(self.fdofs, diag=-1.)
             # we apply u_fluid to ALE, hence get du_fluid/dv
             fac = self.pbf.ti.get_factor_deriv_varint(self.pbase.dt)
-            self.K_dv.scale(-fac)
+            self.K_dv.scale(fac)
 
         self.K_list[3][0] = self.K_dv
 
         self.pbf0.assemble_stiffness(t, subsolver=subsolver)
         self.pba.assemble_stiffness(t)
 
         self.K_list[0][0] = self.pbf0.K_list[0][0]
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe/coupling/fluid_ale_main.py` & `ambit_fe-1.2.8/src/ambit_fe/coupling/fluid_ale_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,27 +115,20 @@
 
             for j in range(len(self.coupling_fluid_ale)):
 
                 ids_fluid_ale = self.coupling_fluid_ale[j]['surface_ids']
 
                 if self.coupling_fluid_ale[j]['type'] == 'strong_dirichlet':
 
-                    for i in range(len(ids_fluid_ale)):
-                        dbcs_coup_fluid_ale.append( fem.dirichletbc(self.ufa, fem.locate_dofs_topological(self.pba.V_d, self.io.mesh.topology.dim-1, self.io.mt_b1.indices[self.io.mt_b1.values == ids_fluid_ale[i]])) )
+                    dbcs_coup_fluid_ale.append( fem.dirichletbc(self.ufa, fem.locate_dofs_topological(self.pba.V_d, self.io.mesh.topology.dim-1, self.io.mt_b1.indices[np.isin(self.io.mt_b1.values, ids_fluid_ale)])) )
 
                     # get surface dofs for dr_ALE/dv matrix entry
-                    fnode_indices_local = [[]]*len(ids_fluid_ale)
-                    for i in range(len(ids_fluid_ale)):
-                        fnode_indices_local[i] = fem.locate_dofs_topological(self.pba.V_d, self.pba.io.mesh.topology.dim-1, self.pba.io.mt_b1.indices[self.pba.io.mt_b1.values == ids_fluid_ale[i]])
-                    fnode_indices_local_flat = [item for sublist in fnode_indices_local for item in sublist]
-                    fnode_indices_all = np.array( self.pba.V_d.dofmap.index_map.local_to_global(np.asarray(fnode_indices_local_flat, dtype=np.int32)), dtype=np.int32 )
-                    fdofs = PETSc.IS().createBlock(self.pba.V_d.dofmap.index_map_bs, fnode_indices_all, comm=self.comm)
-                    # all indices
-                    iset_d_0 = PETSc.IS().createStride(self.pba.d.vector.getLocalSize(), first=self.pba.d.vector.getOwnershipRange()[0], step=1, comm=self.comm)
-                    self.iset_d_0 = iset_d_0.difference(fdofs) # subtract
+                    fnode_indices_local = fem.locate_dofs_topological(self.pba.V_d, self.pba.io.mesh.topology.dim-1, self.pba.io.mt_b1.indices[np.isin(self.pba.io.mt_b1.values, ids_fluid_ale)])
+                    fnode_indices_all = np.array( self.pba.V_d.dofmap.index_map.local_to_global(np.asarray(fnode_indices_local, dtype=np.int32)), dtype=np.int32 )
+                    self.fdofs = PETSc.IS().createBlock(self.pba.V_d.dofmap.index_map_bs, fnode_indices_all, comm=self.comm)
 
                 elif self.coupling_fluid_ale[j]['type'] == 'weak_dirichlet':
 
                     beta = self.coupling_fluid_ale[j]['beta']
                     try: hscale = self.coupling_fluid_ale[j]['hscale']
                     except: hscale = False
 
@@ -146,14 +139,18 @@
                             work_weak_dirichlet_fluid_ale += self.pba.vf.deltaW_int_nitsche_dirichlet(self.pba.d, self.pbf.ufluid, self.pba.ma[n].stress(self.pba.var_d), beta, db_, hscale=hscale) # here, ufluid as form is used!
 
                 else:
                     raise ValueError("Unknown coupling_fluid_ale option for fluid to ALE!")
 
             # now add the DBCs: pay attention to order... first u=uf, then the others... hence re-set!
             if bool(dbcs_coup_fluid_ale):
+                # store DBCs without those from fluid
+                self.pba.bc.dbcs_nofluid = []
+                for k in self.pba.bc.dbcs:
+                    self.pba.bc.dbcs_nofluid.append(k)
                 self.pba.bc.dbcs = []
                 self.pba.bc.dbcs += dbcs_coup_fluid_ale
                 # Dirichlet boundary conditions
                 if 'dirichlet' in self.pba.bc_dict.keys():
                     self.pba.bc.dirichlet_bcs(self.pba.bc_dict['dirichlet'], self.pba.V_d)
                 self.have_dbc_fluid_ale = True
 
@@ -172,16 +169,15 @@
 
             for j in range(len(self.coupling_ale_fluid)):
 
                 ids_ale_fluid = self.coupling_ale_fluid[j]['surface_ids']
 
                 if self.coupling_ale_fluid[j]['type'] == 'strong_dirichlet':
 
-                    for i in range(len(ids_ale_fluid)):
-                        dbcs_coup_ale_fluid.append( fem.dirichletbc(self.wf, fem.locate_dofs_topological(self.pbf.V_v, self.io.mesh.topology.dim-1, self.io.mt_b1.indices[self.io.mt_b1.values == ids_ale_fluid[i]])) )
+                    dbcs_coup_ale_fluid.append( fem.dirichletbc(self.wf, fem.locate_dofs_topological(self.pbf.V_v, self.io.mesh.topology.dim-1, self.io.mt_b1.indices[np.isin(self.io.mt_b1.values, ids_ale_fluid)])) )
 
                     #NOTE: linearization entries due to strong DBCs of ALE on fluid are currently not considered in the monolithic block matrix!
 
                 elif self.coupling_ale_fluid[j]['type'] == 'robin':
 
                     for i in range(len(ids_ale_fluid)):
                         if self.coupling_ale_fluid[j]['type'] == 'robin':
@@ -266,15 +262,34 @@
 
         if self.coupling_strategy=='monolithic':
 
             self.K_vd = fem.petsc.create_matrix(self.jac_vd)
             if self.have_weak_dirichlet_fluid_ale:
                 self.K_dv = fem.petsc.create_matrix(self.jac_dv)
             elif self.have_dbc_fluid_ale:
-                self.K_dv = fem.petsc.create_matrix(self.pba.jac_dd)
+                # create unity vector with 1's on surface dofs and zeros elsewhere
+                self.Iale = self.pba.K_dd.createVecLeft()
+                self.Iale.setValues(self.fdofs, np.ones(self.fdofs.getLocalSize()), addv=PETSc.InsertMode.INSERT)
+                self.Iale.assemble()
+                # create diagonal matrix
+                self.Diag_ale = PETSc.Mat().createAIJ(self.pba.K_dd.getSizes(), bsize=None, nnz=(1,1), csr=None, comm=self.comm)
+                self.Diag_ale.setUp()
+                self.Diag_ale.assemble()
+                # set 1's to get correct allocation pattern
+                self.Diag_ale.shift(1.)
+                # now only set the 1's at surface dofs
+                self.Diag_ale.setDiagonal(self.Iale, addv=PETSc.InsertMode.INSERT)
+                self.Diag_ale.assemble()
+                # create from ALE matrix and only keep the necessary columns
+                # need to assemble here to get correct sparsity pattern when doing the column product
+                self.K_dv_ = fem.petsc.assemble_matrix(self.pba.jac_dd, [])
+                self.K_dv_.assemble()
+                # now multiply to grep out the correct columns
+                self.K_dv = self.K_dv_.matMult(self.Diag_ale)
+                self.K_dv.setOption(PETSc.Mat.Option.KEEP_NONZERO_PATTERN, True) # needed so that zeroRows does not change it!
             else:
                 self.K_dv = None
 
             if self.pbf.num_dupl > 1:
                 self.K_pd = fem.petsc.create_matrix_block(self.jac_pd_)
             else:
                 self.K_pd = fem.petsc.create_matrix(self.jac_pd)
@@ -294,26 +309,25 @@
 
     def assemble_stiffness(self, t, subsolver=None):
 
         if self.have_weak_dirichlet_fluid_ale:
             self.K_dv.zeroEntries()
             fem.petsc.assemble_matrix(self.K_dv, self.jac_dv, self.pba.bc.dbcs)
             self.K_dv.assemble()
-
-        elif self.have_dbc_fluid_ale: # TODO: Does not seem to yield quadratic convergence yet! Why?
-            self.K_dv.zeroEntries()
-            fem.petsc.assemble_matrix(self.K_dv, self.pba.jac_dd, self.pba.bc.dbcs)
-            # fem.petsc.assemble_matrix(self.K_dv, self.pba.jac_dd, [])
-            self.K_dv.assemble()
-
-            # self.K_dv.zeroRowsColumns(self.iset_d_0, diag=0.)
-            self.K_dv.zeroRows(self.iset_d_0, diag=0.)
+        elif self.have_dbc_fluid_ale:
+            self.K_dv_.zeroEntries()
+            fem.petsc.assemble_matrix(self.K_dv_, self.pba.jac_dd, self.pba.bc.dbcs_nofluid) # need DBCs w/o fluid here
+            self.K_dv_.assemble()
+            # multiply to get the relevant columns only
+            self.K_dv_.matMult(self.Diag_ale, result=self.K_dv)
+            # zero rows where DBC is applied and set diagonal entry to -1
+            self.K_dv.zeroRows(self.fdofs, diag=-1.)
             # we apply u_fluid to ALE, hence get du_fluid/dv
             fac = self.pbf.ti.get_factor_deriv_varint(self.pbase.dt)
-            self.K_dv.scale(-fac)
+            self.K_dv.scale(fac)
 
         self.K_list[2][0] = self.K_dv
 
         self.pbf.assemble_stiffness(t)
         self.pba.assemble_stiffness(t)
 
         self.K_list[0][0] = self.pbf.K_list[0][0]
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe/coupling/fluid_flow0d_main.py` & `ambit_fe-1.2.8/src/ambit_fe/coupling/fluid_flow0d_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,30 +250,24 @@
 
         self.dofs_coupling_vq, self.dofs_coupling_p = [[]]*self.num_coupling_surf, [[]]*self.num_coupling_surf
 
         self.k_vs_subvec, self.k_sv_subvec, sze_vs, sze_sv = [], [], [], []
 
         for n in range(self.num_coupling_surf):
 
-            nds_vq_local = [[]]*len(self.surface_vq_ids[n])
-            for i in range(len(self.surface_vq_ids[n])):
-                nds_vq_local[i] = fem.locate_dofs_topological(self.pbf.V_v, self.pbf.io.mesh.topology.dim-1, self.pbf.io.mt_b1.indices[self.pbf.io.mt_b1.values == self.surface_vq_ids[n][i]])
-            nds_vq_local_flat = [item for sublist in nds_vq_local for item in sublist]
-            nds_vq = np.array( self.pbf.V_v.dofmap.index_map.local_to_global(np.asarray(nds_vq_local_flat, dtype=np.int32)), dtype=np.int32 )
+            nds_vq_local = fem.locate_dofs_topological(self.pbf.V_v, self.pbf.io.mesh.topology.dim-1, self.pbf.io.mt_b1.indices[np.isin(self.pbf.io.mt_b1.values, self.surface_vq_ids[n])])
+            nds_vq = np.array( self.pbf.V_v.dofmap.index_map.local_to_global(np.asarray(nds_vq_local, dtype=np.int32)), dtype=np.int32 )
             self.dofs_coupling_vq[n] = PETSc.IS().createBlock(self.pbf.V_v.dofmap.index_map_bs, nds_vq, comm=self.comm)
 
             self.k_sv_subvec.append( self.k_sv_vec[n].getSubVector(self.dofs_coupling_vq[n]) )
 
             sze_sv.append(self.k_sv_subvec[-1].getSize())
 
-            nds_p_local = [[]]*len(self.surface_p_ids[n])
-            for i in range(len(self.surface_p_ids[n])):
-                nds_p_local[i] = fem.locate_dofs_topological(self.pbf.V_v, self.pbf.io.mesh.topology.dim-1, self.pbf.io.mt_b1.indices[self.pbf.io.mt_b1.values == self.surface_p_ids[n][i]])
-            nds_p_local_flat = [item for sublist in nds_p_local for item in sublist]
-            nds_p = np.array( self.pbf.V_v.dofmap.index_map.local_to_global(np.asarray(nds_p_local_flat, dtype=np.int32)), dtype=np.int32 )
+            nds_p_local = fem.locate_dofs_topological(self.pbf.V_v, self.pbf.io.mesh.topology.dim-1, self.pbf.io.mt_b1.indices[np.isin(self.pbf.io.mt_b1.values, self.surface_p_ids[n])])
+            nds_p = np.array( self.pbf.V_v.dofmap.index_map.local_to_global(np.asarray(nds_p_local, dtype=np.int32)), dtype=np.int32 )
             self.dofs_coupling_p[n] = PETSc.IS().createBlock(self.pbf.V_v.dofmap.index_map_bs, nds_p, comm=self.comm)
 
             self.k_vs_subvec.append( self.k_vs_vec[n].getSubVector(self.dofs_coupling_p[n]) )
 
             sze_vs.append(self.k_vs_subvec[-1].getSize())
 
         # derivative of fluid residual w.r.t. multipliers
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe/coupling/fsi_flow0d_main.py` & `ambit_fe-1.2.8/src/ambit_fe/coupling/fsi_flow0d_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,22 +216,14 @@
 
 
     def assemble_stiffness(self, t, subsolver=None):
 
         if self.pbs.incompressible_2field: off = 1
         else: off = 0
 
-        # if self.have_dbc_fluid_ale:
-            # self.K_list[5+off][1+off] = self.K_dv
-        if self.have_weak_dirichlet_fluid_ale:
-            self.K_dv.zeroEntries()
-            fem.petsc.assemble_matrix(self.K_dv, self.jac_dv, self.pba.bc.dbcs)
-            self.K_dv.assemble()
-            self.K_list[5+off][1+off] = self.K_dv
-
         self.pbs.assemble_stiffness(t)
         self.pbfa0.assemble_stiffness(t, subsolver=subsolver)
 
         # solid displacement
         self.K_list[0][0] = self.pbs.K_list[0][0]
         if self.pbs.incompressible_2field:
             self.K_list[0][1] = self.pbs.K_list[0][1]
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe/coupling/fsi_main.py` & `ambit_fe-1.2.8/src/ambit_fe/coupling/fsi_main.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/coupling/solid_constraint_main.py` & `ambit_fe-1.2.8/src/ambit_fe/coupling/solid_constraint_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,19 +218,16 @@
 
         self.dofs_coupling = [[]]*self.num_coupling_surf
 
         self.k_us_subvec, self.k_su_subvec, sze_us, sze_su = [], [], [], []
 
         for n in range(self.num_coupling_surf):
 
-            nds_c_local = [[]]*len(self.surface_c_ids[n])
-            for i in range(len(self.surface_c_ids[n])):
-                nds_c_local[i] = fem.locate_dofs_topological(self.pbs.V_u, self.pbs.io.mesh.topology.dim-1, self.pbs.io.mt_b1.indices[self.pbs.io.mt_b1.values == self.surface_c_ids[n][i]])
-            nds_c_local_flat = [item for sublist in nds_c_local for item in sublist]
-            nds_c = np.array( self.pbs.V_u.dofmap.index_map.local_to_global(np.asarray(nds_c_local_flat, dtype=np.int32)), dtype=np.int32 )
+            nds_c_local = fem.locate_dofs_topological(self.pbs.V_u, self.pbs.io.mesh.topology.dim-1, self.pbs.io.mt_b1.indices[np.isin(self.pbs.io.mt_b1.values, self.surface_c_ids[n])])
+            nds_c = np.array( self.pbs.V_u.dofmap.index_map.local_to_global(np.asarray(nds_c_local, dtype=np.int32)), dtype=np.int32 )
             self.dofs_coupling[n] = PETSc.IS().createBlock(self.pbs.V_u.dofmap.index_map_bs, nds_c, comm=self.comm)
 
             self.k_su_subvec.append( self.k_su_vec[n].getSubVector(self.dofs_coupling[n]) )
 
             sze_su.append(self.k_su_subvec[-1].getSize())
 
             self.k_us_subvec.append( self.k_us_vec[n].getSubVector(self.dofs_coupling[n]) )
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe/coupling/solid_flow0d_main.py` & `ambit_fe-1.2.8/src/ambit_fe/coupling/solid_flow0d_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,30 +350,24 @@
 
         self.dofs_coupling_vq, self.dofs_coupling_p = [[]]*self.num_coupling_surf, [[]]*self.num_coupling_surf
 
         self.k_us_subvec, self.k_su_subvec, sze_us, sze_su = [], [], [], []
 
         for n in range(self.num_coupling_surf):
 
-            nds_vq_local = [[]]*len(self.surface_vq_ids[n])
-            for i in range(len(self.surface_vq_ids[n])):
-                nds_vq_local[i] = fem.locate_dofs_topological(self.pbs.V_u, self.pbs.io.mesh.topology.dim-1, self.pbs.io.mt_b1.indices[self.pbs.io.mt_b1.values == self.surface_vq_ids[n][i]])
-            nds_vq_local_flat = [item for sublist in nds_vq_local for item in sublist]
-            nds_vq = np.array( self.pbs.V_u.dofmap.index_map.local_to_global(np.asarray(nds_vq_local_flat, dtype=np.int32)), dtype=np.int32 )
+            nds_vq_local = fem.locate_dofs_topological(self.pbs.V_u, self.pbs.io.mesh.topology.dim-1, self.pbs.io.mt_b1.indices[np.isin(self.pbs.io.mt_b1.values, self.surface_vq_ids[n])])
+            nds_vq = np.array( self.pbs.V_u.dofmap.index_map.local_to_global(np.asarray(nds_vq_local, dtype=np.int32)), dtype=np.int32 )
             self.dofs_coupling_vq[n] = PETSc.IS().createBlock(self.pbs.V_u.dofmap.index_map_bs, nds_vq, comm=self.comm)
 
             self.k_su_subvec.append( self.k_su_vec[n].getSubVector(self.dofs_coupling_vq[n]) )
 
             sze_su.append(self.k_su_subvec[-1].getSize())
 
-            nds_p_local = [[]]*len(self.surface_p_ids[n])
-            for i in range(len(self.surface_p_ids[n])):
-                nds_p_local[i] = fem.locate_dofs_topological(self.pbs.V_u, self.pbs.io.mesh.topology.dim-1, self.pbs.io.mt_b1.indices[self.pbs.io.mt_b1.values == self.surface_p_ids[n][i]])
-            nds_p_local_flat = [item for sublist in nds_p_local for item in sublist]
-            nds_p = np.array( self.pbs.V_u.dofmap.index_map.local_to_global(np.asarray(nds_p_local_flat, dtype=np.int32)), dtype=np.int32 )
+            nds_p_local = fem.locate_dofs_topological(self.pbs.V_u, self.pbs.io.mesh.topology.dim-1, self.pbs.io.mt_b1.indices[np.isin(self.pbs.io.mt_b1.values, self.surface_p_ids[n])])
+            nds_p = np.array( self.pbs.V_u.dofmap.index_map.local_to_global(np.asarray(nds_p_local, dtype=np.int32)), dtype=np.int32 )
             self.dofs_coupling_p[n] = PETSc.IS().createBlock(self.pbs.V_u.dofmap.index_map_bs, nds_p, comm=self.comm)
 
             self.k_us_subvec.append( self.k_us_vec[n].getSubVector(self.dofs_coupling_p[n]) )
 
             sze_us.append(self.k_us_subvec[-1].getSize())
 
         # derivative of solid residual w.r.t. 0D pressures/multipliers
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe/coupling/solid_flow0d_periodicref_main.py` & `ambit_fe-1.2.8/src/ambit_fe/coupling/solid_flow0d_periodicref_main.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/electrophysiology/electrophysiology_constitutive.py` & `ambit_fe-1.2.8/src/ambit_fe/electrophysiology/electrophysiology_constitutive.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/electrophysiology/electrophysiology_main.py` & `ambit_fe-1.2.8/src/ambit_fe/electrophysiology/electrophysiology_main.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/electrophysiology/electrophysiology_variationalform.py` & `ambit_fe-1.2.8/src/ambit_fe/electrophysiology/electrophysiology_variationalform.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/expression.py` & `ambit_fe-1.2.8/src/ambit_fe/expression.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D.py` & `ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_2elwindkessel.py` & `ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_2elwindkessel.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_4elwindkesselLpZ.py` & `ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_4elwindkesselLpZ.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,14 @@
         self.set_solve_arrays()
 
 
     def equation_map(self):
 
         self.varmap, self.auxmap = {}, {}
         for n in range(self.num_models):
-            # self.varmap = {self.vname : 0, 'g' : 1, 'q' : 2, 's' : 3}
-            # self.auxmap = {self.cname : 2}
             self.varmap[self.vname[n]] = 4*n+0
             self.varmap['g'] = 4*n+1
             self.varmap['q'] = 4*n+2
             self.varmap['s'] = 4*n+3
             self.auxmap[self.cname[n]] = 4*n+2
 
         self.t_ = sp.Symbol('t_')
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_4elwindkesselLsZ.py` & `ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_4elwindkesselLsZ.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,16 +103,14 @@
         self.set_solve_arrays()
 
 
     def equation_map(self):
 
         self.varmap, self.auxmap = {}, {}
         for n in range(self.num_models):
-            # self.varmap = {self.vname : 0, 'q' : 1, 's' : 2}
-            # self.auxmap = {self.cname : 1}
             self.varmap[self.vname[n]] = 3*n+0
             self.varmap['q'] = 3*n+1
             self.varmap['s'] = 3*n+2
             self.auxmap[self.cname[n]] = 3*n+1
 
         self.t_ = sp.Symbol('t_')
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_CRLinoutlink.py` & `ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_CRLinoutlink.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_coronary.py` & `ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_coronary.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_syspul.py` & `ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_syspul.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_syspulcap.py` & `ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_syspulcap.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_syspulcaprespir.py` & `ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_syspulcaprespir.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/flow0d/cardiovascular0D_vad.py` & `ambit_fe-1.2.8/src/ambit_fe/flow0d/cardiovascular0D_vad.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/flow0d/flow0d_main.py` & `ambit_fe-1.2.8/src/ambit_fe/flow0d/flow0d_main.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/fluid/fluid_kinematics_constitutive.py` & `ambit_fe-1.2.8/src/ambit_fe/fluid/fluid_kinematics_constitutive.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/fluid/fluid_main.py` & `ambit_fe-1.2.8/src/ambit_fe/fluid/fluid_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,33 +159,33 @@
             assert(self.io.USE_MIXED_DOLFINX_BRANCH or self.io.USE_NEW_DOLFINX)
             assert(self.num_domains>1)
 
             self.num_dupl = self.num_domains
 
             self.io.submshes_emap, inv_emap, self.io.sub_mt_b1 = {}, {}, {}
 
-            for mp in self.io.duplicate_mesh_domains:
-                self.io.submshes_emap[mp] = mesh.create_submesh(self.io.mesh, self.io.mesh.topology.dim, self.io.mt_d.indices[self.io.mt_d.values == mp])[0:2]
+            for m, mp in enumerate(self.io.duplicate_mesh_domains):
+                self.io.submshes_emap[m+1] = mesh.create_submesh(self.io.mesh, self.io.mesh.topology.dim, self.io.mt_d.indices[np.isin(self.io.mt_d.values, mp)])[0:2]
 
             cell_imap = self.io.mesh.topology.index_map(self.io.mesh.topology.dim)
             num_cells = cell_imap.size_local + cell_imap.num_ghosts
 
-            for mp in self.io.duplicate_mesh_domains:
+            for m, mp in enumerate(self.io.duplicate_mesh_domains):
                 if self.io.USE_NEW_DOLFINX:
-                    self.V_p__[mp] = fem.functionspace(self.io.submshes_emap[mp][0], ("Lagrange", self.order_pres))
+                    self.V_p__[m+1] = fem.functionspace(self.io.submshes_emap[m+1][0], ("Lagrange", self.order_pres))
                 else:
-                    self.V_p__[mp] = fem.FunctionSpace(self.io.submshes_emap[mp][0], P_p)
+                    self.V_p__[m+1] = fem.FunctionSpace(self.io.submshes_emap[m+1][0], P_p)
 
-                inv_emap[mp] = np.full(num_cells, -1)
+                inv_emap[m+1] = np.full(num_cells, -1)
 
-            for mp in self.io.duplicate_mesh_domains:
-                inv_emap[mp][self.io.submshes_emap[mp][1]] = np.arange(len(self.io.submshes_emap[mp][1]))
-                self.io.entity_maps[self.io.submshes_emap[mp][0]] = inv_emap[mp]
+            for m, mp in enumerate(self.io.duplicate_mesh_domains):
+                inv_emap[m+1][self.io.submshes_emap[m+1][1]] = np.arange(len(self.io.submshes_emap[m+1][1]))
+                self.io.entity_maps[self.io.submshes_emap[m+1][0]] = inv_emap[m+1]
                 # transfer boundary meshtags to submesh
-                self.io.sub_mt_b1[mp] = meshutils.meshtags_parent_to_child(self.io.mt_b1, self.io.submshes_emap[mp][0], self.io.submshes_emap[mp][1], self.io.mesh, 'boundary')
+                self.io.sub_mt_b1[m+1] = meshutils.meshtags_parent_to_child(self.io.mt_b1, self.io.submshes_emap[m+1][0], self.io.submshes_emap[m+1][1], self.io.mesh, 'boundary')
 
         else:
             self.num_dupl = 1
             if self.io.USE_NEW_DOLFINX:
                 self.V_p_ = [ fem.functionspace(self.io.mesh, ("Lagrange", self.order_pres)) ]
             else:
                 self.V_p_ = [ fem.FunctionSpace(self.io.mesh, P_p) ]
@@ -234,20 +234,20 @@
         self.dv     = ufl.TrialFunction(self.V_v)            # Incremental velocity
         self.var_v  = ufl.TestFunction(self.V_v)             # Test function
         self.v      = fem.Function(self.V_v, name="Velocity")
 
         # pressure can have duplicate nodes (one variable per domain)
         self.p__, self.p_old__, self.var_p__, self.dp__ = {}, {}, {}, {}
         if self.num_dupl > 1:
-            for mp in self.io.duplicate_mesh_domains:
-                self.p__[mp] = fem.Function(self.V_p__[mp], name="Pressure"+str(mp))
-                self.dp__[mp] = ufl.TrialFunction(self.V_p__[mp])            # Incremental pressure
-                self.var_p__[mp] = ufl.TestFunction(self.V_p__[mp])          # Test function
+            for m, mp in enumerate(self.io.duplicate_mesh_domains):
+                self.p__[m+1] = fem.Function(self.V_p__[m+1], name="Pressure"+str(m+1))
+                self.dp__[m+1] = ufl.TrialFunction(self.V_p__[m+1])            # Incremental pressure
+                self.var_p__[m+1] = ufl.TestFunction(self.V_p__[m+1])          # Test function
                 # values of previous time step
-                self.p_old__[mp] = fem.Function(self.V_p__[mp])
+                self.p_old__[m+1] = fem.Function(self.V_p__[m+1])
             # make lists
             self.V_p_ = list(self.V_p__.values())
             self.p_, self.dp_, self.var_p_, self.p_old_ = list(self.p__.values()), list(self.dp__.values()), list(self.var_p__.values()), list(self.p_old__.values())
         else:
             self.p_ = [ fem.Function(self.V_p_[0], name="Pressure") ]
             self.dp_ = [ ufl.TrialFunction(self.V_p_[0]) ]            # Incremental pressure
             self.var_p_ = [ ufl.TestFunction(self.V_p_[0]) ]          # Test function
@@ -279,44 +279,42 @@
         if self.pbase.have_rom:
             self.xr_, self.xr_old_, self.xrpre_ = self.v, self.v_old, None
             self.xdtr_old_, self.xintr_old_, self.xintrpre_ = self.a_old, self.uf_old, self.uf_pre
 
         # collect references to pressure vectors
         self.pvecs_, self.pvecs_old_ = [], []
         if self.num_dupl > 1:
-            for mp in range(self.num_dupl):
-                self.pvecs_.append(self.p_[mp].vector)
-                self.pvecs_old_.append(self.p_old_[mp].vector)
+            for m in range(self.num_dupl):
+                self.pvecs_.append(self.p_[m].vector)
+                self.pvecs_old_.append(self.p_old_[m].vector)
                 # full pressure vectors - dummy function that holds a class variable "vector"
                 self.p = expression.function_dummy(self.pvecs_,self.comm)
                 self.p_old = expression.function_dummy(self.pvecs_old_,self.comm)
         else:
             self.V_p, self.p, self.p_old = self.V_p_[0], self.p_[0], self.p_old_[0] # pointer to first p's...
 
         # if we want to initialize the pressure (domain wise) with a scalar value
         if self.pbase.restart_step==0:
             if bool(self.initial_fluid_pressure):
-                for mp in range(self.num_dupl):
-                    val = self.initial_fluid_pressure[mp]
-                    self.p_[mp].vector.set(val)
-                    self.p_[mp].vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
-                    self.p_old_[mp].vector.set(val)
-                    self.p_old_[mp].vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
+                for m in range(self.num_dupl):
+                    val = self.initial_fluid_pressure[m]
+                    self.p_[m].vector.set(val)
+                    self.p_[m].vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
+                    self.p_old_[m].vector.set(val)
+                    self.p_old_[m].vector.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
 
         # own read function: requires plain txt format of type "node-id val-x val-y val-z" (or one value in case of a scalar)
         if bool(self.prestress_from_file):
             self.io.readfunction(self.uf_pre, self.prestress_from_file[0])
             # if available, we might want to read in the pressure field, too
             if len(self.prestress_from_file)>1:
                 if bool(self.duplicate_mesh_domains):
-                    m=0
-                    for j in self.duplicate_mesh_domains:
+                    for m, mp in enumerate(self.io.duplicate_mesh_domains):
                         self.io.readfunction(self.p_[m], self.prestress_from_file[1].replace('*',str(m+1)))
                         self.io.readfunction(self.p_old_[m], self.prestress_from_file[1].replace('*',str(m+1)))
-                        m+=1
                 else:
                     self.io.readfunction(self.p_[0], self.prestress_from_file[1])
                     self.io.readfunction(self.p_old_[0], self.prestress_from_file[1])
 
         # dictionaries of internal variables
         self.internalvars, self.internalvars_old, self.internalvars_mid = {}, {}, {}
 
@@ -419,16 +417,16 @@
         # set mid-point representations
         self.acc_mid     = self.timefac_m * self.acc    + (1.-self.timefac_m) * self.a_old
         self.vel_mid     = self.timefac   * self.v      + (1.-self.timefac)   * self.v_old
         self.ufluid_mid  = self.timefac   * self.ufluid + (1.-self.timefac)   * self.uf_old
 
         self.pf_mid__ = {}
         if self.num_dupl > 1:
-            for mp in self.io.duplicate_mesh_domains:
-                self.pf_mid__[mp] = self.timefac * self.p__[mp] + (1.-self.timefac) * self.p_old__[mp]
+            for m, mp in enumerate(self.io.duplicate_mesh_domains):
+                self.pf_mid__[m+1] = self.timefac * self.p__[m+1] + (1.-self.timefac) * self.p_old__[m+1]
             # make list
             self.pf_mid_ = list(self.pf_mid__.values())
         else:
             self.pf_mid_ = [ self.timefac * self.p_[0] + (1.-self.timefac) * self.p_old_[0] ]
 
         # kinetic, internal, and pressure virtual power
         self.deltaW_kin, self.deltaW_kin_old, self.deltaW_kin_mid = ufl.as_ufl(0), ufl.as_ufl(0), ufl.as_ufl(0)
@@ -1019,30 +1017,24 @@
 
             self.dofs_coupling_v = [[]]*self.num_valve_coupling_surf
 
             self.k_vz_subvec, self.k_zp_subvec, sze_vz, sze_zp = [], [], [], []
 
             for n in range(self.num_valve_coupling_surf):
 
-                # nds_p_local = [[]]*len(self.surface_vlv_ids[n])
-                # for i in range(len(self.surface_vlv_ids[n])):
-                #     nds_p_local[i] = fem.locate_dofs_topological(self.V_p, self.io.mesh.topology.dim-1, self.io.mt_b1.indices[self.io.mt_b1.values == self.surface_vlv_ids[n][i]])
-                # nds_p_local_flat = [item for sublist in nds_p_local for item in sublist]
-                # nds_p = np.array( self.V_v.dofmap.index_map.local_to_global(np.asarray(nds_p_local_flat, dtype=np.int32)), dtype=np.int32 )
+                # nds_p_local = fem.locate_dofs_topological(self.V_p, self.io.mesh.topology.dim-1, self.io.mt_b1.indices[np.isin(self.io.mt_b1.values, self.surface_vlv_ids[n])])
+                # nds_p = np.array( self.V_v.dofmap.index_map.local_to_global(np.asarray(nds_p_local, dtype=np.int32)), dtype=np.int32 )
                 # self.dofs_coupling_p[n] = PETSc.IS().createBlock(self.V_p.dofmap.index_map_bs, nds_p, comm=self.comm)
                 #
                 # self.k_zp_subvec.append( self.k_zp_vec[n].getSubVector(self.dofs_coupling_p[n]) )
                 #
                 # sze_zp.append(self.k_zp_subvec[-1].getSize())
 
-                nds_v_local = [[]]*len(self.surface_vlv_ids[n])
-                for i in range(len(self.surface_vlv_ids[n])):
-                    nds_v_local[i] = fem.locate_dofs_topological(self.V_v, self.io.mesh.topology.dim-1, self.io.mt_b1.indices[self.io.mt_b1.values == self.surface_vlv_ids[n][i]])
-                nds_v_local_flat = [item for sublist in nds_v_local for item in sublist]
-                nds_v = np.array( self.V_v.dofmap.index_map.local_to_global(np.asarray(nds_v_local_flat, dtype=np.int32)), dtype=np.int32 )
+                nds_v_local = fem.locate_dofs_topological(self.V_v, self.io.mesh.topology.dim-1, self.io.mt_b1.indices[np.isin(self.io.mt_b1.values, self.surface_vlv_ids[n])])
+                nds_v = np.array( self.V_v.dofmap.index_map.local_to_global(np.asarray(nds_v_local, dtype=np.int32)), dtype=np.int32 )
                 self.dofs_coupling_v[n] = PETSc.IS().createBlock(self.V_v.dofmap.index_map_bs, nds_v, comm=self.comm)
 
                 self.k_vz_subvec.append( self.k_vz_vec[n].getSubVector(self.dofs_coupling_v[n]) )
 
                 sze_vz.append(self.k_vz_subvec[-1].getSize())
 
             # derivative of fluid residual w.r.t. valve state variables
@@ -1498,19 +1490,17 @@
         if 'fluiddisplacement' in self.pb.results_to_write and self.pb.io.write_results_every > 0:
             self.pb.io.write_output_pre(self.pb, self.pb.uf_pre, 0, 'fluiddisplacement_pre')
 
         if self.pb.prestress_initial_only:
             # it may be convenient to write the prestress displacement field to a file for later read-in
             self.pb.io.writefunction(self.pb.uf_pre, self.pb.io.output_path_pre+'/results_'+self.pb.pbase.simname+'_fluiddisplacement_pre')
             if bool(self.pb.io.duplicate_mesh_domains):
-                m=0
-                for j in self.pb.io.duplicate_mesh_domains:
+                for m, mp in enumerate(self.pb.io.duplicate_mesh_domains):
                      # TODO: Might not work for duplicate mesh, since we do not have the input node indices (do we...?)
                     self.pb.io.writefunction(self.pb.p_[m], self.pb.io.output_path_pre+'/results_'+self.pb.pbase.simname+'_pressure'+str(m+1)+'_pre')
-                    m+=1
             else:
                 self.pb.io.writefunction(self.pb.p_[0], self.pb.io.output_path_pre+'/results_'+self.pb.pbase.simname+'_pressure_pre')
             utilities.print_status("Prestress only done. To resume, set file path(s) in 'prestress_from_file' and read in uf_pre.", self.pb.comm)
             os._exit(0)
 
         # reset state
         self.pb.v.vector.set(0.0)
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe/fluid/fluid_material.py` & `ambit_fe-1.2.8/src/ambit_fe/fluid/fluid_material.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/fluid/fluid_variationalform.py` & `ambit_fe-1.2.8/src/ambit_fe/fluid/fluid_variationalform.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/ioparams.py` & `ambit_fe-1.2.8/src/ambit_fe/ioparams.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/ioroutines.py` & `ambit_fe-1.2.8/src/ambit_fe/ioroutines.py`

 * *Files 2% similar despite different names*

```diff
@@ -807,18 +807,18 @@
         if writemesh:
 
             if self.write_results_every > 0:
 
                 for res in pb.results_to_write:
                     if res not in self.results_pre:
                         if res=='pressure' and bool(self.duplicate_mesh_domains):
-                            for j in self.duplicate_mesh_domains:
-                                outfile = io.XDMFFile(self.comm, self.output_path+'/results_'+pb.pbase.simname+'_'+pb.problem_physics+'_'+res+str(j)+'.xdmf', 'w')
-                                outfile.write_mesh(self.submshes_emap[j][0])
-                                self.resultsfiles[res+str(j)] = outfile
+                            for m, mp in enumerate(self.duplicate_mesh_domains):
+                                outfile = io.XDMFFile(self.comm, self.output_path+'/results_'+pb.pbase.simname+'_'+pb.problem_physics+'_'+res+str(m+1)+'.xdmf', 'w')
+                                outfile.write_mesh(self.submshes_emap[m+1][0])
+                                self.resultsfiles[res+str(m+1)] = outfile
                         else:
                             outfile = io.XDMFFile(self.comm, self.output_path+'/results_'+pb.pbase.simname+'_'+pb.problem_physics+'_'+res+'.xdmf', 'w')
                             outfile.write_mesh(self.mesh)
                             self.resultsfiles[res] = outfile
 
             return
 
@@ -837,21 +837,19 @@
                     elif res=='acceleration': # passed in a is not a function but form, so we have to project
                         a_proj = project(pb.acc, pb.V_v, self.dx, domids=pb.domain_ids, nm="Acceleration", comm=self.comm, entity_maps=self.entity_maps)
                         a_out = fem.Function(pb.V_out_vector, name=a_proj.name)
                         a_out.interpolate(a_proj)
                         self.resultsfiles[res].write_function(a_out, indicator)
                     elif res=='pressure':
                         if bool(self.duplicate_mesh_domains):
-                            m=0
-                            for j in self.duplicate_mesh_domains:
-                                V_out_scalar_sub = fem.FunctionSpace(self.submshes_emap[j][0], ("CG", pb.mesh_degree))
+                            for m, mp in enumerate(self.duplicate_mesh_domains):
+                                V_out_scalar_sub = fem.FunctionSpace(self.submshes_emap[m+1][0], ("CG", pb.mesh_degree))
                                 p_out = fem.Function(V_out_scalar_sub, name=pb.p_[m].name)
                                 p_out.interpolate(pb.p_[m])
-                                self.resultsfiles[res+str(j)].write_function(p_out, indicator)
-                                m+=1
+                                self.resultsfiles[res+str(m+1)].write_function(p_out, indicator)
                         else:
                             p_out = fem.Function(pb.V_out_scalar, name=pb.p_[0].name)
                             p_out.interpolate(pb.p_[0])
                             self.resultsfiles[res].write_function(p_out, indicator)
                     elif res=='cauchystress':
                         stressfuncs=[]
                         for n in range(pb.num_domains):
@@ -916,17 +914,17 @@
         vecs_to_read[pb.uf_old] = 'uf_old' # needed for ALE fluid / FSI / FrSI
         if pb.have_active_stress: # for active membrane model (FrSI)
             vecs_to_read[pb.tau_a] = 'tau_a'
             vecs_to_read[pb.tau_a_old] = 'tau_a'
 
         # pressure may be discontinuous across domains
         if bool(self.duplicate_mesh_domains):
-            for mp in self.duplicate_mesh_domains:
-                vecs_to_read[pb.p__[mp]] = 'p'+str(mp)
-                vecs_to_read[pb.p_old__[mp]] = 'p_old'+str(mp)
+            for m, mp in enumerate(self.duplicate_mesh_domains):
+                vecs_to_read[pb.p__[m+1]] = 'p'+str(m+1)
+                vecs_to_read[pb.p_old__[m+1]] = 'p_old'+str(m+1)
         else:
             vecs_to_read[pb.p] = 'p'
             vecs_to_read[pb.p_old] = 'p_old'
 
         for key in vecs_to_read:
 
             if self.restart_io_type=='petscvector':
@@ -950,17 +948,17 @@
         vecs_to_write[pb.a_old] = 'a_old'
         vecs_to_write[pb.uf_old] = 'uf_old' # needed for ALE fluid / FSI / FrSI
         if pb.have_active_stress:
             vecs_to_write[pb.tau_a] = 'tau_a'
 
         # pressure may be discontinuous across domains
         if bool(self.duplicate_mesh_domains):
-            for mp in self.duplicate_mesh_domains:
-                vecs_to_write[pb.p__[mp]] = 'p'+str(mp)
-                vecs_to_write[pb.p_old__[mp]] = 'p_old'+str(mp)
+            for m, mp in enumerate(self.duplicate_mesh_domains):
+                vecs_to_write[pb.p__[m+1]] = 'p'+str(m+1)
+                vecs_to_write[pb.p_old__[m+1]] = 'p_old'+str(m+1)
         else:
             vecs_to_write[pb.p] = 'p'
             vecs_to_write[pb.p_old] = 'p_old'
 
         for key in vecs_to_write:
 
             if self.restart_io_type=='petscvector':
@@ -979,16 +977,16 @@
 
         if self.write_results_every > 0:
 
             for res in pb.results_to_write:
                 if res not in self.results_pre:
 
                     if res=='pressure' and bool(self.duplicate_mesh_domains):
-                        for j in self.duplicate_mesh_domains:
-                            self.resultsfiles[res+str(j)].close()
+                        for m, mp in enumerate(self.duplicate_mesh_domains):
+                            self.resultsfiles[res+str(m+1)].close()
                     else:
                         self.resultsfiles[res].close()
 
 
 
 class IO_ale(IO):
 
@@ -1166,25 +1164,25 @@
                     raise ValueError("Unknown restart_io_type!")
 
 
     def create_submeshes(self):
 
         self.dom_solid, self.dom_fluid, self.surf_interf = self.io_params['domain_ids_solid'], self.io_params['domain_ids_fluid'], self.io_params['surface_ids_interface']
 
-        self.msh_emap_solid = mesh.create_submesh(self.mesh, self.mesh.topology.dim, self.mt_d.indices[self.mt_d.values == self.dom_solid])[0:2]
-        self.msh_emap_fluid = mesh.create_submesh(self.mesh, self.mesh.topology.dim, self.mt_d.indices[self.mt_d.values == self.dom_fluid])[0:2]
+        self.msh_emap_solid = mesh.create_submesh(self.mesh, self.mesh.topology.dim, self.mt_d.indices[np.isin(self.mt_d.values, self.dom_solid)])[0:2]
+        self.msh_emap_fluid = mesh.create_submesh(self.mesh, self.mesh.topology.dim, self.mt_d.indices[np.isin(self.mt_d.values, self.dom_fluid)])[0:2]
 
         # TODO: Assert that meshtags start actually from 1 when transferred!
         self.mt_d_solid = meshutils.meshtags_parent_to_child(self.mt_d, self.msh_emap_solid[0], self.msh_emap_solid[1], self.mesh, 'domain')
         self.mt_d_fluid = meshutils.meshtags_parent_to_child(self.mt_d, self.msh_emap_fluid[0], self.msh_emap_fluid[1], self.mesh, 'domain')
 
         self.mt_b1_solid = meshutils.meshtags_parent_to_child(self.mt_b1, self.msh_emap_solid[0], self.msh_emap_solid[1], self.mesh, 'boundary')
         self.mt_b1_fluid = meshutils.meshtags_parent_to_child(self.mt_b1, self.msh_emap_fluid[0], self.msh_emap_fluid[1], self.mesh, 'boundary')
 
-        self.msh_emap_lm = mesh.create_submesh(self.mesh, self.mesh.topology.dim-1, self.mt_b1.indices[self.mt_b1.values == self.surf_interf])[0:2]
+        self.msh_emap_lm = mesh.create_submesh(self.mesh, self.mesh.topology.dim-1, self.mt_b1.indices[np.isin(self.mt_b1.values, self.surf_interf)])[0:2]
 
         cell_imap = self.mesh.topology.index_map(self.mesh.topology.dim)
         facet_imap = self.mesh.topology.index_map(self.mesh.topology.dim-1)
 
         num_facets = facet_imap.size_local + facet_imap.num_ghosts
         num_cells = cell_imap.size_local + cell_imap.num_ghosts
 
@@ -1208,16 +1206,16 @@
         if self.mt_d_master is not None:
             self.dx = ufl.Measure("dx", domain=msh, subdomain_data=self.mt_d_master, metadata={'quadrature_degree': self.quad_degree})
         else:
             self.dx_ = ufl.Measure("dx", domain=msh, metadata={'quadrature_degree': self.quad_degree})
             self.dx = lambda a : self.dx_ # so that we can call dx(1) even without domain meshtags
 
         # now the boundary ones
-        interface_facets = self.mt_b1.indices[self.mt_b1.values == self.surf_interf[0]]
-        solid_cells = self.mt_d.indices[self.mt_d.values == self.dom_solid[0]]
+        interface_facets = self.mt_b1.indices[np.isin(self.mt_b1.values, self.surf_interf)]
+        solid_cells = self.mt_d.indices[np.isin(self.mt_d.values, self.dom_solid)]
 
         integration_entities = []
 
         # we need one global "master" ds measure, so need to append all other facets from mesh tags
         # using the format (cell, local_facet_index)
 
         # first, get all mesh tags
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe/mathutils.py` & `ambit_fe-1.2.8/src/ambit_fe/mathutils.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/meshutils.py` & `ambit_fe-1.2.8/src/ambit_fe/meshutils.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/mor/mor_main.py` & `ambit_fe-1.2.8/src/ambit_fe/mor/mor_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -364,53 +364,53 @@
 
     def build_reduced_basis(self):
 
         ts = time.time()
         utilities.print_status("ROM: Building reduced basis operator...", self.pb.comm, e=" ")
 
         # create aij matrix - important to specify an approximation for nnz (number of non-zeros per row) for efficient value setting
-        self.V = PETSc.Mat().createAIJ(size=((self.locmatsize_u,self.matsize_u),(PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions)), bsize=None, nnz=(self.numredbasisvec_true*self.num_partitions,self.locmatsize_u), csr=None, comm=self.pb.comm)
+        self.V = PETSc.Mat().createAIJ(size=((self.locmatsize_u,self.matsize_u),(PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions)), bsize=None, nnz=(self.numredbasisvec_true*self.num_partitions+1), csr=None, comm=self.pb.comm)
         self.V.setUp()
 
         vrs, vre = self.V.getOwnershipRange()
 
         # set Phi columns
         self.V[vrs:vre,:] = self.Phi[vrs:vre,:]
 
         self.V.assemble()
 
         # set regularizations terms on reduced variable
         if bool(self.regularizations):
             assert(len(self.regularizations)==self.numredbasisvec_true*self.num_partitions)
 
-            self.Cpen = PETSc.Mat().createAIJ(size=((PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions),(PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions)), bsize=None, nnz=(self.numredbasisvec_true*self.num_partitions), csr=None, comm=self.pb.comm)
+            self.Cpen = PETSc.Mat().createAIJ(size=((PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions),(PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions)), bsize=None, nnz=(1,1), csr=None, comm=self.pb.comm)
             self.Cpen.setUp()
 
             for i in range(len(self.regularizations)):
                 self.Cpen[i,i] = self.regularizations[i]
 
             self.Cpen.assemble()
 
         # set regularizations terms on integration of reduced variable
         if bool(self.regularizations_integ):
             assert(len(self.regularizations_integ)==self.numredbasisvec_true*self.num_partitions)
 
-            self.Cpeninteg = PETSc.Mat().createAIJ(size=((PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions),(PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions)), bsize=None, nnz=(self.numredbasisvec_true*self.num_partitions), csr=None, comm=self.pb.comm)
+            self.Cpeninteg = PETSc.Mat().createAIJ(size=((PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions),(PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions)), bsize=None, nnz=(1,1), csr=None, comm=self.pb.comm)
             self.Cpeninteg.setUp()
 
             for i in range(len(self.regularizations_integ)):
                 self.Cpeninteg[i,i] = self.regularizations_integ[i]
 
             self.Cpeninteg.assemble()
 
         # set regularizations terms on derivative of reduced variable
         if bool(self.regularizations_deriv):
             assert(len(self.regularizations_deriv)==self.numredbasisvec_true*self.num_partitions)
 
-            self.Cpenderiv = PETSc.Mat().createAIJ(size=((PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions),(PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions)), bsize=None, nnz=(self.numredbasisvec_true*self.num_partitions), csr=None, comm=self.pb.comm)
+            self.Cpenderiv = PETSc.Mat().createAIJ(size=((PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions),(PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions)), bsize=None, nnz=(1,1), csr=None, comm=self.pb.comm)
             self.Cpenderiv.setUp()
 
             for i in range(len(self.regularizations_deriv)):
                 self.Cpenderiv[i,i] = self.regularizations_deriv[i]
 
             self.Cpenderiv.assemble()
 
@@ -453,15 +453,15 @@
                 row_1.append(row)
                 col_1.append(col_id)
 
         # make set for faster checking
         col_fd_set = set(col_fd)
 
         # create aij matrix - important to specify an approximation for nnz (number of non-zeros per row) for efficient value setting
-        self.V = PETSc.Mat().createAIJ(size=((self.locmatsize_u,self.matsize_u),(PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions+ndof_bulk)), bsize=None, nnz=(self.numredbasisvec_true*self.num_partitions+1,self.locmatsize_u), csr=None, comm=self.pb.comm)
+        self.V = PETSc.Mat().createAIJ(size=((self.locmatsize_u,self.matsize_u),(PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions+ndof_bulk)), bsize=None, nnz=(self.numredbasisvec_true*self.num_partitions+1), csr=None, comm=self.pb.comm)
         self.V.setUp()
 
         vrs, vre = self.V.getOwnershipRange()
         vcs, vce = self.V.getOwnershipRangeColumn()
 
         # Phi should not have any non-zero rows that do not belong to a surface dof which is reduced
         for i in range(vrs, vre):
@@ -488,45 +488,45 @@
 
         self.V.assemble()
 
         # set regularizations terms on reduced variable
         if bool(self.regularizations):
             assert(len(self.regularizations)==self.numredbasisvec_true*self.num_partitions)
 
-            self.Cpen = PETSc.Mat().createAIJ(size=((PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions+ndof_bulk),(PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions+ndof_bulk)), bsize=None, nnz=(self.numredbasisvec_true*self.num_partitions), csr=None, comm=self.pb.comm)
+            self.Cpen = PETSc.Mat().createAIJ(size=((PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions+ndof_bulk),(PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions+ndof_bulk)), bsize=None, nnz=(1,1), csr=None, comm=self.pb.comm)
             self.Cpen.setUp()
 
             n=0
             for col in range(self.numredbasisvec_true*self.num_partitions+ndof_bulk):
                 if col in col_fd_set:
                     self.Cpen[col,col] = self.regularizations[n]
                     n += 1
 
             self.Cpen.assemble()
 
         # set regularizations terms on integration of reduced variable
         if bool(self.regularizations_integ):
             assert(len(self.regularizations_integ)==self.numredbasisvec_true*self.num_partitions)
 
-            self.Cpeninteg = PETSc.Mat().createAIJ(size=((PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions+ndof_bulk),(PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions+ndof_bulk)), bsize=None, nnz=(self.numredbasisvec_true*self.num_partitions), csr=None, comm=self.pb.comm)
+            self.Cpeninteg = PETSc.Mat().createAIJ(size=((PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions+ndof_bulk),(PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions+ndof_bulk)), bsize=None, nnz=(1,1), csr=None, comm=self.pb.comm)
             self.Cpeninteg.setUp()
 
             n=0
             for col in range(self.numredbasisvec_true*self.num_partitions+ndof_bulk):
                 if col in col_fd_set:
                     self.Cpeninteg[col,col] = self.regularizations_integ[n]
                     n += 1
 
             self.Cpeninteg.assemble()
 
         # set regularizations terms on derivative of reduced variable
         if bool(self.regularizations_deriv):
             assert(len(self.regularizations_deriv)==self.numredbasisvec_true*self.num_partitions)
 
-            self.Cpenderiv = PETSc.Mat().createAIJ(size=((PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions+ndof_bulk),(PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions+ndof_bulk)), bsize=None, nnz=(self.numredbasisvec_true*self.num_partitions), csr=None, comm=self.pb.comm)
+            self.Cpenderiv = PETSc.Mat().createAIJ(size=((PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions+ndof_bulk),(PETSc.DECIDE,self.numredbasisvec_true*self.num_partitions+ndof_bulk)), bsize=None, nnz=(1,1), csr=None, comm=self.pb.comm)
             self.Cpenderiv.setUp()
 
             n=0
             for col in range(self.numredbasisvec_true*self.num_partitions+ndof_bulk):
                 if col in col_fd_set:
                     self.Cpenderiv[col,col] = self.regularizations_deriv[n]
                     n += 1
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe/mpiroutines.py` & `ambit_fe-1.2.8/src/ambit_fe/mpiroutines.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/multiscale/solid_flow0d_growthremodel_main.py` & `ambit_fe-1.2.8/src/ambit_fe/multiscale/solid_flow0d_growthremodel_main.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/oderoutines.py` & `ambit_fe-1.2.8/src/ambit_fe/oderoutines.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/postprocess/flow0d_plot.py` & `ambit_fe-1.2.8/src/ambit_fe/postprocess/flow0d_plot.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/resultcheck.py` & `ambit_fe-1.2.8/src/ambit_fe/resultcheck.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/signet/signet_hypertrophy.py` & `ambit_fe-1.2.8/src/ambit_fe/signet/signet_hypertrophy.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/signet/signet_main.py` & `ambit_fe-1.2.8/src/ambit_fe/signet/signet_main.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/solid/solid_kinematics_constitutive.py` & `ambit_fe-1.2.8/src/ambit_fe/solid/solid_kinematics_constitutive.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/solid/solid_main.py` & `ambit_fe-1.2.8/src/ambit_fe/solid/solid_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -872,15 +872,15 @@
         for n, M in enumerate(self.domain_ids):
             a += ufl.inner(ufl.grad(uf), ufl.grad(vf))*self.io.dx(M)
             L += ufl.dot(f,vf)*self.io.dx(M)
 
         uf = fem.Function(self.V_u, name="uf")
 
         dbcs_laplace=[]
-        dbcs_laplace.append( fem.dirichletbc(self.u, fem.locate_dofs_topological(self.V_u, 2, self.io.mt_b1.indices[self.io.mt_b1.values == self.volume_laplace[0]])) )
+        dbcs_laplace.append( fem.dirichletbc(self.u, fem.locate_dofs_topological(self.V_u, 2, self.io.mt_b1.indices[np.isin(self.io.mt_b1.values, self.volume_laplace)])) )
 
         # solve linear Laplace problem
         lp = fem.petsc.LinearProblem(a, L, bcs=dbcs_laplace, u=uf)
         lp.solve()
 
         vol_all = ufl.as_ufl(0)
         for n, M in enumerate(self.domain_ids):
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe/solid/solid_material.py` & `ambit_fe-1.2.8/src/ambit_fe/solid/solid_material.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/solid/solid_variationalform.py` & `ambit_fe-1.2.8/src/ambit_fe/solid/solid_variationalform.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/solver/preconditioner.py` & `ambit_fe-1.2.8/src/ambit_fe/solver/preconditioner.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/solver/projection.py` & `ambit_fe-1.2.8/src/ambit_fe/solver/projection.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/solver/solver_nonlin.py` & `ambit_fe-1.2.8/src/ambit_fe/solver/solver_nonlin.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/solver/solver_utils.py` & `ambit_fe-1.2.8/src/ambit_fe/solver/solver_utils.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/timeintegration.py` & `ambit_fe-1.2.8/src/ambit_fe/timeintegration.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/utilities.py` & `ambit_fe-1.2.8/src/ambit_fe/utilities.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe/variationalform.py` & `ambit_fe-1.2.8/src/ambit_fe/variationalform.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/src/ambit_fe.egg-info/PKG-INFO` & `ambit_fe-1.2.8/src/ambit_fe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambit-fe
-Version: 1.2.7
+Version: 1.2.8
 Summary: A FEniCS-based cardiovascular multi-physics solver
 Author-email: Marc Hirschvogel <marc.hirschvogel@ambit.net>
 License: MIT License
         
         Copyright (c) 2024 Marc Hirschvogel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,15 +34,15 @@
 Requires-Dist: sympy
 
 # README #
 
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05744/status.svg)](https://doi.org/10.21105/joss.05744)
 
 Ambit is an open-source multi-physics finite element solver written in Python, supporting solid and fluid mechanics, fluid-structure interaction (FSI), and lumped-parameter models.
-It is tailored towards solving problems in cardiac mechanics, but may also be used for more general nonlinear finite element analysis. It uses the finite element backend FEniCS and
+It is tailored towards solving problems in cardiac mechanics, but may also be used for more general nonlinear finite element analysis. It uses the finite element backend FEniCSx and
 linear algebra library PETSc.
 
 https://github.com/marchirschvogel/ambit/assets/52761273/a438ff55-9b37-4572-a1c5-499dd3cfba73
 
 **Heart cycle simulation of a generic bi-ventricular heart model coupled to a closed-loop circulation model.**
 
 https://github.com/marchirschvogel/ambit/assets/52761273/8e681cb6-7a4f-4d1f-b34a-cefb642f44b7
```

### Comparing `ambit_fe-1.2.7/src/ambit_fe.egg-info/SOURCES.txt` & `ambit_fe-1.2.8/src/ambit_fe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_ale_linelast.py` & `ambit_fe-1.2.8/tests/test_ale_linelast.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_electrophysiology.py` & `ambit_fe-1.2.8/tests/test_electrophysiology.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_flow0d_0dheart_syspul.py` & `ambit_fe-1.2.8/tests/test_flow0d_0dheart_syspul.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_flow0d_0dheart_syspulcap.py` & `ambit_fe-1.2.8/tests/test_flow0d_0dheart_syspulcap.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_flow0d_0dheart_syspulcapcor.py` & `ambit_fe-1.2.8/tests/test_flow0d_0dheart_syspulcapcor.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_flow0d_0dheart_syspulcaprespir_periodic.py` & `ambit_fe-1.2.8/tests/test_flow0d_0dheart_syspulcaprespir_periodic.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_flow0d_0dheart_syspulcor.py` & `ambit_fe-1.2.8/tests/test_flow0d_0dheart_syspulcor.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_flow0d_0dheart_syspulcorvad.py` & `ambit_fe-1.2.8/tests/test_flow0d_0dheart_syspulcorvad.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_flow0d_0dvol_2elwindkessel_n3.py` & `ambit_fe-1.2.8/tests/test_flow0d_0dvol_2elwindkessel_n3.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_flow0d_0dvol_4elwindkesselLpZ.py` & `ambit_fe-1.2.8/tests/test_flow0d_0dvol_4elwindkesselLpZ.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_flow0d_0dvol_4elwindkesselLsZ.py` & `ambit_fe-1.2.8/tests/test_flow0d_0dvol_4elwindkesselLsZ.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_fluid_ale_flow0d_lalv_syspul_prescribed.py` & `ambit_fe-1.2.8/tests/test_fluid_ale_flow0d_lalv_syspul_prescribed.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     # reads in restart step from the command line
     try: restart_step = int(sys.argv[1])
     except: restart_step = 0
 
     IO_PARAMS            = {'problem_type'          : 'fluid_ale_flow0d',
                             'USE_MIXED_DOLFINX_BRANCH' : True,
-                            'duplicate_mesh_domains': [1,2],
+                            'duplicate_mesh_domains': [[1],[2]],
                             'write_results_every'   : 1,
                             'write_restart_every'   : 1,
                             'indicate_results_by'   : 'step',
                             'restart_step'          : restart_step,
                             'output_path'           : basepath+'/tmp/',
                             'mesh_domain'           : basepath+'/input/lalv_domain.xdmf',
                             'mesh_boundary'         : basepath+'/input/lalv_boundary.xdmf',
```

### Comparing `ambit_fe-1.2.7/tests/test_fluid_flow0d_monolagr_taylorhood_cylinder.py` & `ambit_fe-1.2.8/tests/test_fluid_flow0d_monolagr_taylorhood_cylinder.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_fluid_flow0d_monolagr_taylorhood_cylinder_condensed.py` & `ambit_fe-1.2.8/tests/test_fluid_flow0d_monolagr_taylorhood_cylinder_condensed.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_fluid_p1p1_stab_cylinder.py` & `ambit_fe-1.2.8/tests/test_fluid_p1p1_stab_cylinder.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_fluid_p1p1_stab_cylinder_schur2x2.py` & `ambit_fe-1.2.8/tests/test_fluid_p1p1_stab_cylinder_schur2x2.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_fluid_p1p1_stab_cylinder_valve.py` & `ambit_fe-1.2.8/tests/test_fluid_p1p1_stab_cylinder_valve.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     # reads in restart step from the command line
     try: restart_step = int(sys.argv[1])
     except: restart_step = 0
 
     IO_PARAMS           = {'problem_type'          : 'fluid',
                            'USE_MIXED_DOLFINX_BRANCH' : True,
-                           'duplicate_mesh_domains': [1,2],
+                           'duplicate_mesh_domains': [[1],[2]],
                            'mesh_domain'           : basepath+'/input/cylinder_domain.xdmf',
                            'mesh_boundary'         : basepath+'/input/cylinder_boundary.xdmf',
                            'write_results_every'   : 1,
                            'write_restart_every'   : 9,
                            'restart_step'          : restart_step,
                            'output_path'           : basepath+'/tmp/',
                            'results_to_write'      : ['velocity','pressure'],
```

### Comparing `ambit_fe-1.2.7/tests/test_fluid_taylorhood_cylinder.py` & `ambit_fe-1.2.8/tests/test_fluid_taylorhood_cylinder.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_frsi_artseg_modepartitionunity.py` & `ambit_fe-1.2.8/tests/test_frsi_artseg_modepartitionunity.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                             'order_pres'            : 1,
                             'quad_degree'           : 6,
                             'fluid_formulation'     : 'nonconservative'}
 
     FEM_PARAMS_ALE       = {'order_disp'            : 2,
                             'quad_degree'           : 6}
 
-    COUPLING_PARAMS      = {'coupling_fluid_ale'    : [{'surface_ids' : [1,6], 'type' : 'weak_dirichlet', 'beta' : 1e6, 'hscale' : False}]} # use of cell circumradius (hscale) not working for non-simplex cells...
+    COUPLING_PARAMS      = {'coupling_fluid_ale'    : [{'surface_ids' : [1,6], 'type' : 'strong_dirichlet'}]}
 
     MATERIALS_FLUID      = { 'MAT1' : {'newtonian' : {'mu' : 4.0e-6},
                                        'inertia'   : {'rho' : 1.025e-6}} }
 
     MATERIALS_ALE        = { 'MAT1' : {'linelast' : {'Emod' : 15.0, 'nu' : 0.1}} }
```

### Comparing `ambit_fe-1.2.7/tests/test_frsi_artseg_prefile.py` & `ambit_fe-1.2.8/tests/test_frsi_artseg_prefile.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_frsi_artseg_prefile_bgsschur4x4.py` & `ambit_fe-1.2.8/tests/test_frsi_artseg_prefile_bgsschur4x4.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_frsi_artseg_prefile_partitioned_schur3x3.py` & `ambit_fe-1.2.8/tests/test_frsi_artseg_prefile_partitioned_schur3x3.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_frsi_artseg_prestress.py` & `ambit_fe-1.2.8/tests/test_frsi_artseg_prestress.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                             'quad_degree'           : 6}
 
     COUPLING_PARAMS      = {'coupling_fluid_ale'    : [{'surface_ids' : [1,6], 'type' : 'strong_dirichlet'}]}
 
     MATERIALS_FLUID      = { 'MAT1' : {'newtonian' : {'mu' : 4.0e-6},
                                        'inertia'   : {'rho' : 1.025e-6}} }
 
-    MATERIALS_ALE        = { 'MAT1' : {'diffusion' : {'D' : 1.0}} }
+    MATERIALS_ALE        = { 'MAT1' : {'diffusion' : {'D' : 1.0, 'scale_det' : True}} }
 
 
     class expression1: # prestress
         def __init__(self):
             self.t = 0.0
         def evaluate(self, x):
             pmax = 0.01
```

### Comparing `ambit_fe-1.2.7/tests/test_fsi_flow0d_p1p1_stab_artseg.py` & `ambit_fe-1.2.8/tests/test_fsi_flow0d_p1p1_stab_artseg.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_fsi_p1p1_stab_artseg.py` & `ambit_fe-1.2.8/tests/test_fsi_p1p1_stab_artseg.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_fsi_taylorhood_artseg.py` & `ambit_fe-1.2.8/tests/test_fsi_taylorhood_artseg.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_signet_0d_hypertrophy.py` & `ambit_fe-1.2.8/tests/test_signet_0d_hypertrophy.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_2d_pres.py` & `ambit_fe-1.2.8/tests/test_solid_2d_pres.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_2dheart_frankstarling.py` & `ambit_fe-1.2.8/tests/test_solid_2dheart_frankstarling.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_bodyforce_gravity.py` & `ambit_fe-1.2.8/tests/test_solid_bodyforce_gravity.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_constraint_volume_chamber.py` & `ambit_fe-1.2.8/tests/test_solid_constraint_volume_chamber.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_divcont_ptc.py` & `ambit_fe-1.2.8/tests/test_solid_divcont_ptc.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_flow0d_monodir2field_4elwindkesselLpZ_chamber.py` & `ambit_fe-1.2.8/tests/test_solid_flow0d_monodir2field_4elwindkesselLpZ_chamber.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_flow0d_monodir2field_flux_syspulcap_3Dheart_schur3x3.py` & `ambit_fe-1.2.8/tests/test_solid_flow0d_monodir2field_flux_syspulcap_3Dheart_schur3x3.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber.py` & `ambit_fe-1.2.8/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2.py` & `ambit_fe-1.2.8/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2fieldsplit.py` & `ambit_fe-1.2.8/tests/test_solid_flow0d_monodir_4elwindkesselLsZ_chamber_bgs2x2fieldsplit.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_flow0d_monodir_flux_syspulcap_3Dheart_schur2x2.py` & `ambit_fe-1.2.8/tests/test_solid_flow0d_monodir_flux_syspulcap_3Dheart_schur2x2.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_flow0d_monodir_syspul_2dheart_prestress.py` & `ambit_fe-1.2.8/tests/test_solid_flow0d_monodir_syspul_2dheart_prestress.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_flow0d_monodir_syspulcor_2dheart_rom.py` & `ambit_fe-1.2.8/tests/test_solid_flow0d_monodir_syspulcor_2dheart_rom.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_flow0d_monolagr2field_2elwindkessel_chamber.py` & `ambit_fe-1.2.8/tests/test_solid_flow0d_monolagr2field_2elwindkessel_chamber.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_flow0d_monolagr_CRLinoutlink_chambers.py` & `ambit_fe-1.2.8/tests/test_solid_flow0d_monolagr_CRLinoutlink_chambers.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_flow0d_multiscalegrowthremodeling_concentric.py` & `ambit_fe-1.2.8/tests/test_solid_flow0d_multiscalegrowthremodeling_concentric.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_flow0d_multiscalegrowthremodeling_eccentric.py` & `ambit_fe-1.2.8/tests/test_solid_flow0d_multiscalegrowthremodeling_eccentric.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_flow0d_periodicref_syspul_lvchamber.py` & `ambit_fe-1.2.8/tests/test_solid_flow0d_periodicref_syspul_lvchamber.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_growth_prescribed_iso_lv.py` & `ambit_fe-1.2.8/tests/test_solid_growth_prescribed_iso_lv.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_growth_volstressmandel.py` & `ambit_fe-1.2.8/tests/test_solid_growth_volstressmandel.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_growth_volstressmandel_incomp.py` & `ambit_fe-1.2.8/tests/test_solid_growth_volstressmandel_incomp.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_growthremodeling_fiberstretch.py` & `ambit_fe-1.2.8/tests/test_solid_growthremodeling_fiberstretch.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_mat_uniax_hex_2field.py` & `ambit_fe-1.2.8/tests/test_solid_mat_uniax_hex_2field.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_membrane.py` & `ambit_fe-1.2.8/tests/test_solid_membrane.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_ost_dbc_ramp.py` & `ambit_fe-1.2.8/tests/test_solid_ost_dbc_ramp.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_pinch_edge.py` & `ambit_fe-1.2.8/tests/test_solid_pinch_edge.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_plasticity_vonmises.py` & `ambit_fe-1.2.8/tests/test_solid_plasticity_vonmises.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_robin_genalpha.py` & `ambit_fe-1.2.8/tests/test_solid_robin_genalpha.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_robin_genalpha_amg.py` & `ambit_fe-1.2.8/tests/test_solid_robin_genalpha_amg.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_robin_static_prestress.py` & `ambit_fe-1.2.8/tests/test_solid_robin_static_prestress.py`

 * *Files identical despite different names*

### Comparing `ambit_fe-1.2.7/tests/test_solid_robin_visco.py` & `ambit_fe-1.2.8/tests/test_solid_robin_visco.py`

 * *Files identical despite different names*

