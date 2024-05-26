# Comparing `tmp/riskparityportfolio-0.5.1.tar.gz` & `tmp/riskparityportfolio-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riskparityportfolio-0.5.1.tar", last modified: Sat Mar  2 00:03:46 2024, max compression
+gzip compressed data, was "riskparityportfolio-0.6.0.tar", last modified: Sun May 26 09:54:46 2024, max compression
```

## Comparing `riskparityportfolio-0.5.1.tar` & `riskparityportfolio-0.6.0.tar`

### file list

```diff
@@ -1,1760 +1,1783 @@
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.398855 riskparityportfolio-0.5.1/
--rw-r--r--   0 mirca      (501) staff       (20)     1068 2021-04-16 02:33:45.000000 riskparityportfolio-0.5.1/LICENSE
--rw-r--r--   0 mirca      (501) staff       (20)       80 2024-03-01 23:53:59.000000 riskparityportfolio-0.5.1/MANIFEST.in
--rw-r--r--   0 mirca      (501) staff       (20)      534 2024-03-02 00:03:46.398313 riskparityportfolio-0.5.1/PKG-INFO
--rw-r--r--   0 mirca      (501) staff       (20)     3854 2023-01-17 03:31:11.000000 riskparityportfolio-0.5.1/README.md
--rw-r--r--   0 mirca      (501) staff       (20)      371 2024-03-01 14:32:22.000000 riskparityportfolio-0.5.1/pyproject.toml
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:43.939602 riskparityportfolio-0.5.1/riskparityportfolio.egg-info/
--rw-r--r--   0 mirca      (501) staff       (20)      534 2024-03-02 00:03:43.000000 riskparityportfolio-0.5.1/riskparityportfolio.egg-info/PKG-INFO
--rw-r--r--   0 mirca      (501) staff       (20)    96229 2024-03-02 00:03:43.000000 riskparityportfolio-0.5.1/riskparityportfolio.egg-info/SOURCES.txt
--rw-r--r--   0 mirca      (501) staff       (20)        1 2024-03-02 00:03:43.000000 riskparityportfolio-0.5.1/riskparityportfolio.egg-info/dependency_links.txt
--rw-r--r--   0 mirca      (501) staff       (20)        1 2024-03-01 23:56:19.000000 riskparityportfolio-0.5.1/riskparityportfolio.egg-info/not-zip-safe
--rw-r--r--   0 mirca      (501) staff       (20)       20 2024-03-02 00:03:43.000000 riskparityportfolio-0.5.1/riskparityportfolio.egg-info/top_level.txt
--rw-r--r--   0 mirca      (501) staff       (20)       38 2024-03-02 00:03:46.399033 riskparityportfolio-0.5.1/setup.cfg
--rw-r--r--   0 mirca      (501) staff       (20)     4806 2024-03-01 23:58:16.000000 riskparityportfolio-0.5.1/setup.py
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:43.861074 riskparityportfolio-0.5.1/src/
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:43.945415 riskparityportfolio-0.5.1/src/riskparityportfolio/
--rw-r--r--   0 mirca      (501) staff       (20)      230 2021-06-10 12:21:49.000000 riskparityportfolio-0.5.1/src/riskparityportfolio/__init__.py
--rw-r--r--   0 mirca      (501) staff       (20)     1477 2021-06-10 12:21:49.000000 riskparityportfolio-0.5.1/src/riskparityportfolio/riskfunctions.py
--rw-r--r--   0 mirca      (501) staff       (20)     5358 2022-09-26 03:47:31.000000 riskparityportfolio-0.5.1/src/riskparityportfolio/rpp.py
--rw-r--r--   0 mirca      (501) staff       (20)     7668 2021-06-10 12:21:49.000000 riskparityportfolio-0.5.1/src/riskparityportfolio/sca.py
--rw-r--r--   0 mirca      (501) staff       (20)     3206 2023-01-17 02:45:04.000000 riskparityportfolio-0.5.1/src/riskparityportfolio/vanilla.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2770 2022-11-10 09:38:13.000000 riskparityportfolio-0.5.1/src/riskparityportfolio/vanilla.h
--rw-r--r--   0 mirca      (501) staff       (20)       22 2024-03-01 23:55:26.000000 riskparityportfolio-0.5.1/src/riskparityportfolio/version.py
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:43.861720 riskparityportfolio-0.5.1/third-party/
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:43.990300 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/
--rw-r--r--   0 mirca      (501) staff       (20)      117 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/.hg_archival.txt
--rw-r--r--   0 mirca      (501) staff       (20)      180 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/.hgeol
--rw-r--r--   0 mirca      (501) staff       (20)      244 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/.hgignore
--rw-r--r--   0 mirca      (501) staff       (20)     1844 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/.hgtags
--rw-r--r--   0 mirca      (501) staff       (20)    24308 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     1516 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/COPYING.BSD
--rw-r--r--   0 mirca      (501) staff       (20)    35147 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/COPYING.GPL
--rw-r--r--   0 mirca      (501) staff       (20)    26530 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/COPYING.LGPL
--rw-r--r--   0 mirca      (501) staff       (20)     2246 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/COPYING.MINPACK
--rw-r--r--   0 mirca      (501) staff       (20)    16726 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/COPYING.MPL2
--rw-r--r--   0 mirca      (501) staff       (20)      779 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/COPYING.README
--rw-r--r--   0 mirca      (501) staff       (20)      543 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/CTestConfig.cmake
--rw-r--r--   0 mirca      (501) staff       (20)      180 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/CTestCustom.cmake.in
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.058152 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/
--rw-r--r--   0 mirca      (501) staff       (20)      694 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     1206 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/Cholesky
--rw-r--r--   0 mirca      (501) staff       (20)     1900 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/CholmodSupport
--rw-r--r--   0 mirca      (501) staff       (20)    17961 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/Core
--rw-r--r--   0 mirca      (501) staff       (20)      122 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/Dense
--rw-r--r--   0 mirca      (501) staff       (20)       35 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/Eigen
--rw-r--r--   0 mirca      (501) staff       (20)     1822 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/Eigenvalues
--rw-r--r--   0 mirca      (501) staff       (20)     2050 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/Geometry
--rw-r--r--   0 mirca      (501) staff       (20)      874 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/Householder
--rw-r--r--   0 mirca      (501) staff       (20)     2083 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/IterativeLinearSolvers
--rw-r--r--   0 mirca      (501) staff       (20)      939 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/Jacobi
--rw-r--r--   0 mirca      (501) staff       (20)     1433 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/LU
--rw-r--r--   0 mirca      (501) staff       (20)      991 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/MetisSupport
--rw-r--r--   0 mirca      (501) staff       (20)     2483 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/OrderingMethods
--rw-r--r--   0 mirca      (501) staff       (20)     1676 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/PaStiXSupport
--rwxr-xr-x   0 mirca      (501) staff       (20)     1116 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/PardisoSupport
--rw-r--r--   0 mirca      (501) staff       (20)     1317 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/QR
--rw-r--r--   0 mirca      (501) staff       (20)      945 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/QtAlignedMalloc
--rw-r--r--   0 mirca      (501) staff       (20)     1162 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/SPQRSupport
--rw-r--r--   0 mirca      (501) staff       (20)     1629 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/SVD
--rw-r--r--   0 mirca      (501) staff       (20)      919 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/Sparse
--rw-r--r--   0 mirca      (501) staff       (20)     1371 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/SparseCholesky
--rw-r--r--   0 mirca      (501) staff       (20)     2240 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/SparseCore
--rw-r--r--   0 mirca      (501) staff       (20)     1713 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/SparseLU
--rw-r--r--   0 mirca      (501) staff       (20)     1222 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/SparseQR
--rw-r--r--   0 mirca      (501) staff       (20)      797 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/StdDeque
--rw-r--r--   0 mirca      (501) staff       (20)      726 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/StdList
--rw-r--r--   0 mirca      (501) staff       (20)      803 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/StdVector
--rw-r--r--   0 mirca      (501) staff       (20)     2243 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/SuperLUSupport
--rw-r--r--   0 mirca      (501) staff       (20)     1382 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/UmfPackSupport
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:43.899399 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.060402 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Cholesky/
--rw-r--r--   0 mirca      (501) staff       (20)    24480 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 mirca      (501) staff       (20)    18395 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 mirca      (501) staff       (20)     3974 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.061119 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/CholmodSupport/
--rw-r--r--   0 mirca      (501) staff       (20)    22307 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.195518 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/
--rw-r--r--   0 mirca      (501) staff       (20)    12115 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Array.h
--rw-r--r--   0 mirca      (501) staff       (20)     8179 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 mirca      (501) staff       (20)     6775 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 mirca      (501) staff       (20)     2720 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Assign.h
--rw-r--r--   0 mirca      (501) staff       (20)    38153 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/AssignEvaluator.h
--rwxr-xr-x   0 mirca      (501) staff       (20)    12479 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 mirca      (501) staff       (20)    13910 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 mirca      (501) staff       (20)    18064 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Block.h
--rw-r--r--   0 mirca      (501) staff       (20)     4249 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 mirca      (501) staff       (20)     5689 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 mirca      (501) staff       (20)     6990 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 mirca      (501) staff       (20)    62197 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 mirca      (501) staff       (20)     4525 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 mirca      (501) staff       (20)     7593 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 mirca      (501) staff       (20)    31424 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 mirca      (501) staff       (20)     8256 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 mirca      (501) staff       (20)     3877 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 mirca      (501) staff       (20)     5282 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 mirca      (501) staff       (20)    27420 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 mirca      (501) staff       (20)    24212 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 mirca      (501) staff       (20)    21959 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 mirca      (501) staff       (20)     9597 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 mirca      (501) staff       (20)    12666 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 mirca      (501) staff       (20)      970 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 mirca      (501) staff       (20)    11507 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Dot.h
--rw-r--r--   0 mirca      (501) staff       (20)     5619 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 mirca      (501) staff       (20)     4769 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 mirca      (501) staff       (20)     5705 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 mirca      (501) staff       (20)    21123 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 mirca      (501) staff       (20)    22185 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 mirca      (501) staff       (20)    10222 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 mirca      (501) staff       (20)     7076 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/IO.h
--rw-r--r--   0 mirca      (501) staff       (20)     3519 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Inverse.h
--rw-r--r--   0 mirca      (501) staff       (20)     7239 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Map.h
--rw-r--r--   0 mirca      (501) staff       (20)    10991 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/MapBase.h
--rw-r--r--   0 mirca      (501) staff       (20)    40865 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 mirca      (501) staff       (20)     3369 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 mirca      (501) staff       (20)    19067 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Matrix.h
--rw-r--r--   0 mirca      (501) staff       (20)    23213 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 mirca      (501) staff       (20)     3400 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 mirca      (501) staff       (20)     3582 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 mirca      (501) staff       (20)     9234 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 mirca      (501) staff       (20)    21646 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 mirca      (501) staff       (20)    45180 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 mirca      (501) staff       (20)     7235 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Product.h
--rw-r--r--   0 mirca      (501) staff       (20)    49497 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 mirca      (501) staff       (20)     6379 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Random.h
--rw-r--r--   0 mirca      (501) staff       (20)    17852 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Redux.h
--rw-r--r--   0 mirca      (501) staff       (20)    12800 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Ref.h
--rw-r--r--   0 mirca      (501) staff       (20)     5595 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Replicate.h
--rw-r--r--   0 mirca      (501) staff       (20)     4200 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 mirca      (501) staff       (20)     7073 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Reverse.h
--rw-r--r--   0 mirca      (501) staff       (20)     6020 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Select.h
--rw-r--r--   0 mirca      (501) staff       (20)    14245 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 mirca      (501) staff       (20)     1697 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 mirca      (501) staff       (20)     6795 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Solve.h
--rw-r--r--   0 mirca      (501) staff       (20)     9136 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 mirca      (501) staff       (20)     4365 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 mirca      (501) staff       (20)     7692 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 mirca      (501) staff       (20)     3865 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Stride.h
--rw-r--r--   0 mirca      (501) staff       (20)     2683 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Swap.h
--rw-r--r--   0 mirca      (501) staff       (20)    14777 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Transpose.h
--rw-r--r--   0 mirca      (501) staff       (20)    14386 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 mirca      (501) staff       (20)    37234 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 mirca      (501) staff       (20)     3462 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 mirca      (501) staff       (20)    29441 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 mirca      (501) staff       (20)     8074 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:43.865840 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.199791 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 mirca      (501) staff       (20)    18037 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 mirca      (501) staff       (20)    17776 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 mirca      (501) staff       (20)    27841 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 mirca      (501) staff       (20)     1194 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.201252 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 mirca      (501) staff       (20)    15733 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 mirca      (501) staff       (20)    50985 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX512/PacketMath.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.204038 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 mirca      (501) staff       (20)    16443 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 mirca      (501) staff       (20)    10797 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rwxr-xr-x   0 mirca      (501) staff       (20)    37671 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.239524 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 mirca      (501) staff       (20)     4240 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/Complex.h
--rw-r--r--   0 mirca      (501) staff       (20)    23528 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/Half.h
--rw-r--r--   0 mirca      (501) staff       (20)     2387 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/MathFunctions.h
--rw-r--r--   0 mirca      (501) staff       (20)    10744 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/PacketMath.h
--rw-r--r--   0 mirca      (501) staff       (20)    35538 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
--rw-r--r--   0 mirca      (501) staff       (20)     5509 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/TypeCasting.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.241812 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/Default/
--rw-r--r--   0 mirca      (501) staff       (20)     1989 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 mirca      (501) staff       (20)     1746 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/Default/Settings.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.244902 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 mirca      (501) staff       (20)    17706 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 mirca      (501) staff       (20)     2846 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 mirca      (501) staff       (20)    28726 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/NEON/PacketMath.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.248803 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 mirca      (501) staff       (20)    19426 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 mirca      (501) staff       (20)    18888 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxr-xr-x   0 mirca      (501) staff       (20)    35843 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 mirca      (501) staff       (20)     1759 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.250896 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 mirca      (501) staff       (20)    15366 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 mirca      (501) staff       (20)     4418 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxr-xr-x   0 mirca      (501) staff       (20)    32283 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.255307 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/functors/
--rw-r--r--   0 mirca      (501) staff       (20)     6284 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 mirca      (501) staff       (20)    18263 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 mirca      (501) staff       (20)     8229 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 mirca      (501) staff       (20)     4400 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 mirca      (501) staff       (20)      607 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 mirca      (501) staff       (20)    27944 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.272088 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/
--rw-r--r--   0 mirca      (501) staff       (20)    81534 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 mirca      (501) staff       (20)    18478 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 mirca      (501) staff       (20)    15188 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 mirca      (501) staff       (20)     6907 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 mirca      (501) staff       (20)     5017 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 mirca      (501) staff       (20)    26808 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 mirca      (501) staff       (20)     6368 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 mirca      (501) staff       (20)     4905 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 mirca      (501) staff       (20)    19632 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 mirca      (501) staff       (20)    11198 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 mirca      (501) staff       (20)     9901 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 mirca      (501) staff       (20)     5209 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 mirca      (501) staff       (20)     6105 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 mirca      (501) staff       (20)     4066 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 mirca      (501) staff       (20)    20403 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 mirca      (501) staff       (20)    13743 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 mirca      (501) staff       (20)    14722 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 mirca      (501) staff       (20)    10571 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 mirca      (501) staff       (20)    13979 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 mirca      (501) staff       (20)     6513 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 mirca      (501) staff       (20)     5741 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.324907 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/
--rwxr-xr-x   0 mirca      (501) staff       (20)    15722 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 mirca      (501) staff       (20)    21579 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/Constants.h
--rwxr-xr-x   0 mirca      (501) staff       (20)     3981 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 mirca      (501) staff       (20)    14150 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/ForwardDeclarations.h
--rwxr-xr-x   0 mirca      (501) staff       (20)     4026 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 mirca      (501) staff       (20)    36570 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 mirca      (501) staff       (20)    40579 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/Memory.h
--rwxr-xr-x   0 mirca      (501) staff       (20)    20586 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 mirca      (501) staff       (20)       85 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 mirca      (501) staff       (20)      856 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 mirca      (501) staff       (20)    10518 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 mirca      (501) staff       (20)    34198 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.337890 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/
--rw-r--r--   0 mirca      (501) staff       (20)    12558 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 mirca      (501) staff       (20)    17021 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 mirca      (501) staff       (20)     4178 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 mirca      (501) staff       (20)    22944 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 mirca      (501) staff       (20)    17176 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 mirca      (501) staff       (20)     9715 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 mirca      (501) staff       (20)    14351 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 mirca      (501) staff       (20)     5539 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 mirca      (501) staff       (20)    23586 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 mirca      (501) staff       (20)    20288 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 mirca      (501) staff       (20)     3650 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 mirca      (501) staff       (20)    33674 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 mirca      (501) staff       (20)     4104 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0 mirca      (501) staff       (20)    22444 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.349485 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/
--rw-r--r--   0 mirca      (501) staff       (20)    14815 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 mirca      (501) staff       (20)     8423 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 mirca      (501) staff       (20)     3639 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 mirca      (501) staff       (20)    20539 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0 mirca      (501) staff       (20)    11961 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 mirca      (501) staff       (20)     8949 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 mirca      (501) staff       (20)     8308 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0 mirca      (501) staff       (20)    32152 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 mirca      (501) staff       (20)     6877 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 mirca      (501) staff       (20)     8063 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/RotationBase.h
--rwxr-xr-x   0 mirca      (501) staff       (20)     6324 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 mirca      (501) staff       (20)    60514 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/Transform.h
--rw-r--r--   0 mirca      (501) staff       (20)     7773 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 mirca      (501) staff       (20)     6191 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/Umeyama.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.350142 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/arch/
--rw-r--r--   0 mirca      (501) staff       (20)     5387 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/arch/Geometry_SSE.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.386185 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Householder/
--rw-r--r--   0 mirca      (501) staff       (20)     4481 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 mirca      (501) staff       (20)     5345 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Householder/Householder.h
--rw-r--r--   0 mirca      (501) staff       (20)    20603 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.394323 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 mirca      (501) staff       (20)     6755 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 mirca      (501) staff       (20)     7253 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 mirca      (501) staff       (20)     9289 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 mirca      (501) staff       (20)    15062 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 mirca      (501) staff       (20)    15234 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 mirca      (501) staff       (20)    11527 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0 mirca      (501) staff       (20)     7762 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 mirca      (501) staff       (20)     4158 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.395058 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Jacobi/
--rw-r--r--   0 mirca      (501) staff       (20)    15902 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.399997 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/LU/
--rw-r--r--   0 mirca      (501) staff       (20)     3057 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/LU/Determinant.h
--rw-r--r--   0 mirca      (501) staff       (20)    32803 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 mirca      (501) staff       (20)    15064 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 mirca      (501) staff       (20)    21478 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0 mirca      (501) staff       (20)     3555 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.400733 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/LU/arch/
--rw-r--r--   0 mirca      (501) staff       (20)    13669 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/LU/arch/Inverse_SSE.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.401744 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/MetisSupport/
--rw-r--r--   0 mirca      (501) staff       (20)     4588 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.404684 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/OrderingMethods/
--rw-r--r--   0 mirca      (501) staff       (20)    16396 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 mirca      (501) staff       (20)    62266 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 mirca      (501) staff       (20)     5229 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.405426 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/PaStiXSupport/
--rw-r--r--   0 mirca      (501) staff       (20)    22248 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.406272 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/PardisoSupport/
--rw-r--r--   0 mirca      (501) staff       (20)    20032 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.447817 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/QR/
--rw-r--r--   0 mirca      (501) staff       (20)    24881 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 mirca      (501) staff       (20)     4662 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 mirca      (501) staff       (20)    20805 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 mirca      (501) staff       (20)    25478 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0 mirca      (501) staff       (20)    14022 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 mirca      (501) staff       (20)     2993 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.449434 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SPQRSupport/
--rw-r--r--   0 mirca      (501) staff       (20)    11405 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.454414 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SVD/
--rw-r--r--   0 mirca      (501) staff       (20)    48778 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 mirca      (501) staff       (20)    32949 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 mirca      (501) staff       (20)     5099 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0 mirca      (501) staff       (20)    12740 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 mirca      (501) staff       (20)    15957 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SVD/UpperBidiagonalization.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.455990 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCholesky/
--rw-r--r--   0 mirca      (501) staff       (20)    24010 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 mirca      (501) staff       (20)     6898 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.520520 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/
--rw-r--r--   0 mirca      (501) staff       (20)    10537 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 mirca      (501) staff       (20)     8164 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 mirca      (501) staff       (20)    13178 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 mirca      (501) staff       (20)     2191 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 mirca      (501) staff       (20)     8080 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 mirca      (501) staff       (20)    25592 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 mirca      (501) staff       (20)     6485 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 mirca      (501) staff       (20)    12720 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 mirca      (501) staff       (20)    25840 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 mirca      (501) staff       (20)     4711 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 mirca      (501) staff       (20)    12487 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 mirca      (501) staff       (20)     5808 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 mirca      (501) staff       (20)     3080 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 mirca      (501) staff       (20)     1107 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0 mirca      (501) staff       (20)    12589 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 mirca      (501) staff       (20)    52373 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 mirca      (501) staff       (20)    17923 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 mirca      (501) staff       (20)     7329 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 mirca      (501) staff       (20)     7049 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 mirca      (501) staff       (20)     1699 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 mirca      (501) staff       (20)    15492 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 mirca      (501) staff       (20)    25715 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 mirca      (501) staff       (20)     4424 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 mirca      (501) staff       (20)     8704 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 mirca      (501) staff       (20)     3175 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 mirca      (501) staff       (20)     6437 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 mirca      (501) staff       (20)     6602 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 mirca      (501) staff       (20)    14831 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 mirca      (501) staff       (20)     8110 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 mirca      (501) staff       (20)     9657 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/TriangularSolver.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.533053 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/
--rw-r--r--   0 mirca      (501) staff       (20)    27866 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0 mirca      (501) staff       (20)     4303 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 mirca      (501) staff       (20)     7601 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 mirca      (501) staff       (20)     4974 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 mirca      (501) staff       (20)    10022 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 mirca      (501) staff       (20)     2049 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 mirca      (501) staff       (20)     6712 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 mirca      (501) staff       (20)     6582 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 mirca      (501) staff       (20)     3681 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 mirca      (501) staff       (20)    10216 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 mirca      (501) staff       (20)     4181 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 mirca      (501) staff       (20)     5723 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 mirca      (501) staff       (20)     8486 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 mirca      (501) staff       (20)     9028 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 mirca      (501) staff       (20)     4979 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 mirca      (501) staff       (20)     4545 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 mirca      (501) staff       (20)     2889 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.533860 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseQR/
--rw-r--r--   0 mirca      (501) staff       (20)    28373 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseQR/SparseQR.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.536651 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/StlSupport/
--rw-r--r--   0 mirca      (501) staff       (20)     5117 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 mirca      (501) staff       (20)     4147 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0 mirca      (501) staff       (20)     5330 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 mirca      (501) staff       (20)     2809 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/StlSupport/details.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.537298 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SuperLUSupport/
--rw-r--r--   0 mirca      (501) staff       (20)    34345 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.537975 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/UmfPackSupport/
--rw-r--r--   0 mirca      (501) staff       (20)    17202 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.566831 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/misc/
--rw-r--r--   0 mirca      (501) staff       (20)     2913 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/misc/Image.h
--rw-r--r--   0 mirca      (501) staff       (20)     2742 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/misc/Kernel.h
--rw-r--r--   0 mirca      (501) staff       (20)     1748 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 mirca      (501) staff       (20)    30560 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/misc/blas.h
--rw-r--r--   0 mirca      (501) staff       (20)     7834 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/misc/lapack.h
--rwxr-xr-x   0 mirca      (501) staff       (20)  1058368 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/misc/lapacke.h
--rw-r--r--   0 mirca      (501) staff       (20)      474 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.571766 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/plugins/
--rw-r--r--   0 mirca      (501) staff       (20)    13132 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 mirca      (501) staff       (20)    16929 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 mirca      (501) staff       (20)    37403 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 mirca      (501) staff       (20)     4828 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 mirca      (501) staff       (20)     5621 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 mirca      (501) staff       (20)     6375 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 mirca      (501) staff       (20)     2937 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-r--r--   0 mirca      (501) staff       (20)     1145 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/INSTALL
--rw-r--r--   0 mirca      (501) staff       (20)      175 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/README.md
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.599835 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/
--rw-r--r--   0 mirca      (501) staff       (20)     3932 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/BenchSparseUtil.h
--rw-r--r--   0 mirca      (501) staff       (20)     4392 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/BenchTimer.h
--rw-r--r--   0 mirca      (501) staff       (20)     2529 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/BenchUtil.h
--rw-r--r--   0 mirca      (501) staff       (20)     2008 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/README.txt
--rw-r--r--   0 mirca      (501) staff       (20)    28983 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/analyze-blocking-sizes.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1421 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/basicbench.cxxlist
--rw-r--r--   0 mirca      (501) staff       (20)     1107 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/basicbenchmark.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1669 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/basicbenchmark.h
--rw-r--r--   0 mirca      (501) staff       (20)     6313 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchBlasGemm.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3534 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchCholesky.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5788 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchEigenSolver.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2806 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchFFT.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3598 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchGeometry.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5193 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchVecAdd.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    10821 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/bench_gemm.cpp
--rwxr-xr-x   0 mirca      (501) staff       (20)      618 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/bench_multi_compilers.sh
--rw-r--r--   0 mirca      (501) staff       (20)    11652 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/bench_norm.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2159 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/bench_reverse.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      320 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/bench_sum.cpp
--rwxr-xr-x   0 mirca      (501) staff       (20)      651 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/bench_unrolling
--rw-r--r--   0 mirca      (501) staff       (20)    22259 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchmark-blocking-sizes.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      790 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchmark.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      835 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchmarkSlice.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      640 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchmarkX.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      605 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchmarkXcwise.cpp
--rwxr-xr-x   0 mirca      (501) staff       (20)     1209 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchmark_suite
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.601552 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/
--rw-r--r--   0 mirca      (501) staff       (20)     2869 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)    18109 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/COPYING
--rw-r--r--   0 mirca      (501) staff       (20)     6447 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/README
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.647964 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/
--rw-r--r--   0 mirca      (501) staff       (20)     3374 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_aat_product.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3354 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_ata_product.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3670 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_atv_product.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3371 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_axpby.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3340 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_axpy.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3202 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_cholesky.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3460 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_ger.hh
--rw-r--r--   0 mirca      (501) staff       (20)     5598 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_hessenberg.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3151 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_lu_decomp.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3598 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_lu_solve.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3886 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_matrix_matrix_product.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3982 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_matrix_matrix_product_bis.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3989 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_matrix_vector_product.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3188 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_partial_lu.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3019 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_rot.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3691 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_symv.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3664 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_syr2.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3425 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_trisolve.hh
--rw-r--r--   0 mirca      (501) staff       (20)     4061 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_trisolve_matrix.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3907 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_trmm.hh
--rw-r--r--   0 mirca      (501) staff       (20)      467 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/basic_actions.hh
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.657160 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/
--rw-r--r--   0 mirca      (501) staff       (20)      932 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindACML.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     1365 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindATLAS.cmake
--rw-r--r--   0 mirca      (501) staff       (20)      815 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindBLAZE.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     1092 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindBlitz.cmake
--rw-r--r--   0 mirca      (501) staff       (20)      668 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindCBLAS.cmake
--rw-r--r--   0 mirca      (501) staff       (20)      366 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindGMM.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     1370 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindMKL.cmake
--rw-r--r--   0 mirca      (501) staff       (20)      819 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindMTL4.cmake
--rw-r--r--   0 mirca      (501) staff       (20)      622 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindOPENBLAS.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     2372 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0 mirca      (501) staff       (20)      832 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindTvmet.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     1315 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.669161 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/
--rw-r--r--   0 mirca      (501) staff       (20)      869 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     1368 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/action_settings.txt
--rw-r--r--   0 mirca      (501) staff       (20)     2224 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/gnuplot_common_settings.hh
--rwxr-xr-x   0 mirca      (501) staff       (20)     2065 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/go_mean
--rw-r--r--   0 mirca      (501) staff       (20)     5306 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/mean.cxx
--rw-r--r--   0 mirca      (501) staff       (20)     1850 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/mk_gnuplot_script.sh
--rw-r--r--   0 mirca      (501) staff       (20)      929 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/mk_mean_script.sh
--rwxr-xr-x   0 mirca      (501) staff       (20)     1742 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/mk_new_gnuplot.sh
--rw-r--r--   0 mirca      (501) staff       (20)      974 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/perlib_plot_settings.txt
--rw-r--r--   0 mirca      (501) staff       (20)     3425 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/regularize.cxx
--rw-r--r--   0 mirca      (501) staff       (20)     5112 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/smooth.cxx
--rwxr-xr-x   0 mirca      (501) staff       (20)     1687 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/smooth_all.sh
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.671486 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/
--rw-r--r--   0 mirca      (501) staff       (20)     4827 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/bench.hh
--rw-r--r--   0 mirca      (501) staff       (20)     1916 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/bench_parameter.hh
--rw-r--r--   0 mirca      (501) staff       (20)     6748 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/btl.hh
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.703592 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/init/
--rw-r--r--   0 mirca      (501) staff       (20)     1478 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/init/init_function.hh
--rw-r--r--   0 mirca      (501) staff       (20)     2295 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/init/init_matrix.hh
--rw-r--r--   0 mirca      (501) staff       (20)     1416 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/init/init_vector.hh
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.705846 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/static/
--rw-r--r--   0 mirca      (501) staff       (20)     2278 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/static/bench_static.hh
--rw-r--r--   0 mirca      (501) staff       (20)     1948 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/static/intel_bench_fixed_size.hh
--rw-r--r--   0 mirca      (501) staff       (20)     2222 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/static/static_size_generator.hh
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.711072 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/
--rw-r--r--   0 mirca      (501) staff       (20)     2305 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/STL_perf_analyzer.hh
--rw-r--r--   0 mirca      (501) staff       (20)     2522 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/STL_timer.hh
--rw-r--r--   0 mirca      (501) staff       (20)     1994 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh
--rw-r--r--   0 mirca      (501) staff       (20)     2938 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/portable_perf_analyzer.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3534 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh
--rwxr-xr-x   0 mirca      (501) staff       (20)     3534 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/portable_timer.hh
--rw-r--r--   0 mirca      (501) staff       (20)     2927 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/x86_perf_analyzer.hh
--rw-r--r--   0 mirca      (501) staff       (20)     5294 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/x86_timer.hh
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.714077 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/
--rw-r--r--   0 mirca      (501) staff       (20)     1658 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/size_lin_log.hh
--rw-r--r--   0 mirca      (501) staff       (20)     1645 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/size_log.hh
--rw-r--r--   0 mirca      (501) staff       (20)     2745 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/utilities.h
--rw-r--r--   0 mirca      (501) staff       (20)     2213 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/xy_file.hh
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:43.908090 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.718236 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/BLAS/
--rw-r--r--   0 mirca      (501) staff       (20)     1572 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/BLAS/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)    35158 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/BLAS/blas.h
--rw-r--r--   0 mirca      (501) staff       (20)     2891 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/BLAS/blas_interface.hh
--rw-r--r--   0 mirca      (501) staff       (20)     4811 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/BLAS/blas_interface_impl.hh
--rw-r--r--   0 mirca      (501) staff       (20)     1634 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/BLAS/c_interface_base.h
--rw-r--r--   0 mirca      (501) staff       (20)     2963 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/BLAS/main.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.720333 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/STL/
--rw-r--r--   0 mirca      (501) staff       (20)       37 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/STL/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     5838 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/STL/STL_interface.hh
--rw-r--r--   0 mirca      (501) staff       (20)     1828 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/STL/main.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.722422 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blaze/
--rw-r--r--   0 mirca      (501) staff       (20)      475 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blaze/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     4012 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blaze/blaze_interface.hh
--rw-r--r--   0 mirca      (501) staff       (20)     1645 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blaze/main.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.726600 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blitz/
--rw-r--r--   0 mirca      (501) staff       (20)      424 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blitz/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     5364 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blitz/blitz_LU_solve_interface.hh
--rw-r--r--   0 mirca      (501) staff       (20)     4129 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blitz/blitz_interface.hh
--rw-r--r--   0 mirca      (501) staff       (20)     1962 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blitz/btl_blitz.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1393 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blitz/btl_tiny_blitz.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3100 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blitz/tiny_blitz_interface.hh
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.732047 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen2/
--rw-r--r--   0 mirca      (501) staff       (20)      768 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen2/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     1664 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5151 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen2/eigen2_interface.hh
--rw-r--r--   0 mirca      (501) staff       (20)     1799 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen2/main_adv.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1205 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen2/main_linear.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1384 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen2/main_matmat.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1456 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen2/main_vecmat.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.737028 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen3/
--rw-r--r--   0 mirca      (501) staff       (20)     3292 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen3/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     1664 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     8077 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen3/eigen3_interface.hh
--rw-r--r--   0 mirca      (501) staff       (20)     1799 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen3/main_adv.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1285 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen3/main_linear.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1381 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen3/main_matmat.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1447 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen3/main_vecmat.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.739688 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/gmm/
--rw-r--r--   0 mirca      (501) staff       (20)      125 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/gmm/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     5364 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/gmm/gmm_LU_solve_interface.hh
--rw-r--r--   0 mirca      (501) staff       (20)     4174 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/gmm/gmm_interface.hh
--rw-r--r--   0 mirca      (501) staff       (20)     2113 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/gmm/main.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.778198 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/mtl4/
--rw-r--r--   0 mirca      (501) staff       (20)      153 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/mtl4/.kdbgrc.main
--rw-r--r--   0 mirca      (501) staff       (20)      133 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/mtl4/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     1943 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/mtl4/main.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5364 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh
--rw-r--r--   0 mirca      (501) staff       (20)     4210 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/mtl4/mtl4_interface.hh
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.782020 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tensors/
--rw-r--r--   0 mirca      (501) staff       (20)     2155 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tensors/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)      671 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tensors/main_linear.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      624 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tensors/main_matmat.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      624 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tensors/main_vecmat.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3190 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tensors/tensor_interface.hh
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.784013 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tvmet/
--rw-r--r--   0 mirca      (501) staff       (20)      142 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tvmet/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     1460 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tvmet/main.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3017 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tvmet/tvmet_interface.hh
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.786236 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/ublas/
--rw-r--r--   0 mirca      (501) staff       (20)      180 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/ublas/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     1785 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/ublas/main.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4342 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/ublas/ublas_interface.hh
--rw-r--r--   0 mirca      (501) staff       (20)     3269 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/check_cache_queries.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6416 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/dense_solvers.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     7244 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/eig33.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3307 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/geometry.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:43.908727 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/perf_monitoring/
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.790327 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/
--rw-r--r--   0 mirca      (501) staff       (20)     3786 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/changesets.txt
--rw-r--r--   0 mirca      (501) staff       (20)     1269 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/gemm.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      169 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/gemm_settings.txt
--rw-r--r--   0 mirca      (501) staff       (20)     2368 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/lazy_gemm.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      132 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/lazy_gemm_settings.txt
--rwxr-xr-x   0 mirca      (501) staff       (20)      991 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/make_plot.sh
--rwxr-xr-x   0 mirca      (501) staff       (20)     3290 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/run.sh
--rw-r--r--   0 mirca      (501) staff       (20)     3232 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/product_threshold.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6006 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/quat_slerp.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1097 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/quatmul.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6260 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/sparse_cholesky.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5101 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/sparse_dense_product.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3011 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/sparse_lu.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     8999 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/sparse_product.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3358 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/sparse_randomsetter.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    13761 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/sparse_setter.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2347 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/sparse_transpose.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6114 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/sparse_trisolver.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.795169 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spbench/
--rw-r--r--   0 mirca      (501) staff       (20)     2939 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spbench/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     3974 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spbench/sp_solver.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1856 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spbench/spbench.dtd
--rw-r--r--   0 mirca      (501) staff       (20)     3302 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spbench/spbenchsolver.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    17717 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spbench/spbenchsolver.h
--rw-r--r--   0 mirca      (501) staff       (20)     3825 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spbench/spbenchstyle.h
--rw-r--r--   0 mirca      (501) staff       (20)     2830 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spbench/test_sparseLU.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6096 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spmv.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.801668 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/
--rw-r--r--   0 mirca      (501) staff       (20)     2220 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/README
--rw-r--r--   0 mirca      (501) staff       (20)     1585 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/benchmark.h
--rw-r--r--   0 mirca      (501) staff       (20)     6834 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/benchmark_main.cc
--rw-r--r--   0 mirca      (501) staff       (20)     1389 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/contraction_benchmarks_cpu.cc
--rw-r--r--   0 mirca      (501) staff       (20)    16193 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks.h
--rw-r--r--   0 mirca      (501) staff       (20)     6264 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks_cpu.cc
--rw-r--r--   0 mirca      (501) staff       (20)     3381 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks_fp16_gpu.cu
--rw-r--r--   0 mirca      (501) staff       (20)     3373 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks_gpu.cu
--rw-r--r--   0 mirca      (501) staff       (20)     1153 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks_sycl.cc
--rw-r--r--   0 mirca      (501) staff       (20)     1203 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/vdw_new.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.847748 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/
--rw-r--r--   0 mirca      (501) staff       (20)     3614 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/BandTriangularSolver.h
--rw-r--r--   0 mirca      (501) staff       (20)     1687 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     1608 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/GeneralRank1Update.h
--rw-r--r--   0 mirca      (501) staff       (20)     2036 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/PackedSelfadjointProduct.h
--rw-r--r--   0 mirca      (501) staff       (20)     3165 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/PackedTriangularMatrixVector.h
--rw-r--r--   0 mirca      (501) staff       (20)     3191 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/PackedTriangularSolverVector.h
--rw-r--r--   0 mirca      (501) staff       (20)      183 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/README.txt
--rw-r--r--   0 mirca      (501) staff       (20)     2168 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/Rank2Update.h
--rw-r--r--   0 mirca      (501) staff       (20)     4361 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/common.h
--rw-r--r--   0 mirca      (501) staff       (20)      647 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/complex_double.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      646 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/complex_single.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1501 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/double.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.862664 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/
--rw-r--r--   0 mirca      (501) staff       (20)    15108 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/chbmv.c
--rw-r--r--   0 mirca      (501) staff       (20)    13026 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/chpmv.c
--rw-r--r--   0 mirca      (501) staff       (20)     2310 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/complexdots.c
--rw-r--r--   0 mirca      (501) staff       (20)    18944 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/ctbmv.c
--rw-r--r--   0 mirca      (501) staff       (20)      117 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/d_cnjg.c
--rw-r--r--   0 mirca      (501) staff       (20)      657 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/datatypes.h
--rw-r--r--   0 mirca      (501) staff       (20)     4968 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/drotm.c
--rw-r--r--   0 mirca      (501) staff       (20)     6193 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/drotmg.c
--rw-r--r--   0 mirca      (501) staff       (20)    10188 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/dsbmv.c
--rw-r--r--   0 mirca      (501) staff       (20)     8075 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/dspmv.c
--rw-r--r--   0 mirca      (501) staff       (20)    11656 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/dtbmv.c
--rw-r--r--   0 mirca      (501) staff       (20)     2976 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/lsame.c
--rw-r--r--   0 mirca      (501) staff       (20)      105 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/r_cnjg.c
--rw-r--r--   0 mirca      (501) staff       (20)     4902 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/srotm.c
--rw-r--r--   0 mirca      (501) staff       (20)     6056 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/srotmg.c
--rw-r--r--   0 mirca      (501) staff       (20)    10210 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/ssbmv.c
--rw-r--r--   0 mirca      (501) staff       (20)     8051 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/sspmv.c
--rw-r--r--   0 mirca      (501) staff       (20)    11642 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/stbmv.c
--rw-r--r--   0 mirca      (501) staff       (20)    15144 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/zhbmv.c
--rw-r--r--   0 mirca      (501) staff       (20)    13060 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/zhpmv.c
--rw-r--r--   0 mirca      (501) staff       (20)    18972 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/ztbmv.c
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.863510 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/fortran/
--rw-r--r--   0 mirca      (501) staff       (20)      979 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/fortran/complexdots.f
--rw-r--r--   0 mirca      (501) staff       (20)     4956 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/level1_cplx_impl.h
--rw-r--r--   0 mirca      (501) staff       (20)     4559 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/level1_impl.h
--rw-r--r--   0 mirca      (501) staff       (20)     3617 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/level1_real_impl.h
--rw-r--r--   0 mirca      (501) staff       (20)    12223 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/level2_cplx_impl.h
--rw-r--r--   0 mirca      (501) staff       (20)    25172 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/level2_impl.h
--rw-r--r--   0 mirca      (501) staff       (20)    10499 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/level2_real_impl.h
--rw-r--r--   0 mirca      (501) staff       (20)    37780 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/level3_impl.h
--rw-r--r--   0 mirca      (501) staff       (20)      757 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/single.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.922255 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/
--rw-r--r--   0 mirca      (501) staff       (20)      964 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)    32109 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/cblat1.f
--rw-r--r--   0 mirca      (501) staff       (20)     1546 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/cblat2.dat
--rw-r--r--   0 mirca      (501) staff       (20)   116657 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/cblat2.f
--rw-r--r--   0 mirca      (501) staff       (20)     1046 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/cblat3.dat
--rw-r--r--   0 mirca      (501) staff       (20)   131550 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/cblat3.f
--rw-r--r--   0 mirca      (501) staff       (20)    44819 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/dblat1.f
--rw-r--r--   0 mirca      (501) staff       (20)     1466 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/dblat2.dat
--rw-r--r--   0 mirca      (501) staff       (20)   112335 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/dblat2.f
--rw-r--r--   0 mirca      (501) staff       (20)      882 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/dblat3.dat
--rw-r--r--   0 mirca      (501) staff       (20)   104262 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/dblat3.f
--rwxr-xr-x   0 mirca      (501) staff       (20)     1016 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/runblastest.sh
--rw-r--r--   0 mirca      (501) staff       (20)    43388 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/sblat1.f
--rw-r--r--   0 mirca      (501) staff       (20)     1466 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/sblat2.dat
--rw-r--r--   0 mirca      (501) staff       (20)   112251 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/sblat2.f
--rw-r--r--   0 mirca      (501) staff       (20)      882 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/sblat3.dat
--rw-r--r--   0 mirca      (501) staff       (20)   104172 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/sblat3.f
--rw-r--r--   0 mirca      (501) staff       (20)    32114 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/zblat1.f
--rw-r--r--   0 mirca      (501) staff       (20)     1546 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/zblat2.dat
--rw-r--r--   0 mirca      (501) staff       (20)   117003 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/zblat2.f
--rw-r--r--   0 mirca      (501) staff       (20)     1046 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/zblat3.dat
--rw-r--r--   0 mirca      (501) staff       (20)   131995 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/zblat3.f
--rw-r--r--   0 mirca      (501) staff       (20)      389 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/xerbla.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.972600 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/
--rw-r--r--   0 mirca      (501) staff       (20)      769 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/Eigen3Config.cmake.in
--rw-r--r--   0 mirca      (501) staff       (20)     1397 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/Eigen3ConfigLegacy.cmake.in
--rw-r--r--   0 mirca      (501) staff       (20)     2825 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/EigenConfigureTesting.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     1562 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/EigenDetermineOSVersion.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     1814 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/EigenDetermineVSServicePack.cmake
--rw-r--r--   0 mirca      (501) staff       (20)    26743 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/EigenTesting.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     1200 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/EigenUninstall.cmake
--rw-r--r--   0 mirca      (501) staff       (20)      501 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindAdolc.cmake
--rw-r--r--   0 mirca      (501) staff       (20)    43820 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindBLAS.cmake
--rw-r--r--   0 mirca      (501) staff       (20)    13031 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindBLASEXT.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     2572 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindCholmod.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     9003 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindComputeCpp.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     2842 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindEigen2.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     3501 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindEigen3.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     2757 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindFFTW.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     2943 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindGLEW.cmake
--rw-r--r--   0 mirca      (501) staff       (20)      554 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindGMP.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     5035 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindGSL.cmake
--rw-r--r--   0 mirca      (501) staff       (20)      909 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindGoogleHash.cmake
--rw-r--r--   0 mirca      (501) staff       (20)    11857 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindHWLOC.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     9909 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindLAPACK.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     2845 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindMPFR.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     8963 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindMetis.cmake
--rw-r--r--   0 mirca      (501) staff       (20)    14450 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindPTSCOTCH.cmake
--rw-r--r--   0 mirca      (501) staff       (20)    23207 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindPastix.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     1188 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindSPQR.cmake
--rw-r--r--   0 mirca      (501) staff       (20)    12010 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindScotch.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     2194 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindStandardMathLibrary.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     2299 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindSuperLU.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     1735 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindUmfpack.cmake
--rw-r--r--   0 mirca      (501) staff       (20)      936 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/RegexUtils.cmake
--rw-r--r--   0 mirca      (501) staff       (20)      177 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/UseEigen3.cmake
--rw-r--r--   0 mirca      (501) staff       (20)     2413 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/language_support.cmake
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:43.912411 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/debug/
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.973898 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/debug/gdb/
--rw-r--r--   0 mirca      (501) staff       (20)       22 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/debug/gdb/__init__.py
--rw-r--r--   0 mirca      (501) staff       (20)     7548 2021-06-10 12:21:49.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/debug/gdb/printers.py
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.975587 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/debug/msvc/
--rw-r--r--   0 mirca      (501) staff       (20)    11661 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/debug/msvc/eigen.natvis
--rw-r--r--   0 mirca      (501) staff       (20)     7566 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/debug/msvc/eigen_autoexp_part.dat
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.976354 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/
--rw-r--r--   0 mirca      (501) staff       (20)      296 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/CMakeLists.txt
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.979434 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/mandelbrot/
--rw-r--r--   0 mirca      (501) staff       (20)      486 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/mandelbrot/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)      336 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/mandelbrot/README
--rw-r--r--   0 mirca      (501) staff       (20)     7509 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/mandelbrot/mandelbrot.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1888 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/mandelbrot/mandelbrot.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.982444 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/mix_eigen_and_c/
--rw-r--r--   0 mirca      (501) staff       (20)      261 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/mix_eigen_and_c/README
--rw-r--r--   0 mirca      (501) staff       (20)     4158 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/mix_eigen_and_c/binary_library.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3345 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/mix_eigen_and_c/binary_library.h
--rw-r--r--   0 mirca      (501) staff       (20)     1616 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/mix_eigen_and_c/example.c
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:44.990328 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/
--rw-r--r--   0 mirca      (501) staff       (20)      695 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)      403 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/README
--rw-r--r--   0 mirca      (501) staff       (20)     5981 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/camera.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3435 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/camera.h
--rw-r--r--   0 mirca      (501) staff       (20)     3974 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/gpuhelper.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     7177 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/gpuhelper.h
--rw-r--r--   0 mirca      (501) staff       (20)     3927 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/icosphere.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      869 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/icosphere.h
--rw-r--r--   0 mirca      (501) staff       (20)    19192 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/quaternion_demo.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2635 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/quaternion_demo.h
--rw-r--r--   0 mirca      (501) staff       (20)     1756 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/trackball.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      943 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/trackball.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:45.069432 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/
--rw-r--r--   0 mirca      (501) staff       (20)    12377 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/A05_PortingFrom2To3.dox
--rw-r--r--   0 mirca      (501) staff       (20)    10274 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/AsciiQuickReference.txt
--rw-r--r--   0 mirca      (501) staff       (20)     2425 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/B01_Experimental.dox
--rw-r--r--   0 mirca      (501) staff       (20)     4659 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     6332 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/ClassHierarchy.dox
--rw-r--r--   0 mirca      (501) staff       (20)    16511 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/CoeffwiseMathFunctionsTable.dox
--rw-r--r--   0 mirca      (501) staff       (20)     4424 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/CustomizingEigen_CustomScalar.dox
--rw-r--r--   0 mirca      (501) staff       (20)     1337 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/CustomizingEigen_InheritingMatrix.dox
--rw-r--r--   0 mirca      (501) staff       (20)     3658 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/CustomizingEigen_NullaryExpr.dox
--rw-r--r--   0 mirca      (501) staff       (20)     3658 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/CustomizingEigen_Plugins.dox
--rw-r--r--   0 mirca      (501) staff       (20)     5022 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/DenseDecompositionBenchmark.dox
--rw-r--r--   0 mirca      (501) staff       (20)    85220 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/Doxyfile.in
--rw-r--r--   0 mirca      (501) staff       (20)     8355 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/Eigen_Silly_Professor_64x64.png
--rw-r--r--   0 mirca      (501) staff       (20)     1718 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/FixedSizeVectorizable.dox
--rw-r--r--   0 mirca      (501) staff       (20)    13452 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/FunctionsTakingEigenTypes.dox
--rw-r--r--   0 mirca      (501) staff       (20)     5429 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/HiPerformance.dox
--rw-r--r--   0 mirca      (501) staff       (20)     3797 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/InplaceDecomposition.dox
--rw-r--r--   0 mirca      (501) staff       (20)    30239 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/InsideEigenExample.dox
--rw-r--r--   0 mirca      (501) staff       (20)     2791 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/LeastSquares.dox
--rw-r--r--   0 mirca      (501) staff       (20)     6551 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/Manual.dox
--rw-r--r--   0 mirca      (501) staff       (20)      758 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/MatrixfreeSolverExample.dox
--rw-r--r--   0 mirca      (501) staff       (20)     5610 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/NewExpressionType.dox
--rw-r--r--   0 mirca      (501) staff       (20)     2058 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/Overview.dox
--rw-r--r--   0 mirca      (501) staff       (20)     1153 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/PassingByValue.dox
--rw-r--r--   0 mirca      (501) staff       (20)     1984 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/Pitfalls.dox
--rw-r--r--   0 mirca      (501) staff       (20)    13440 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/PreprocessorDirectives.dox
--rw-r--r--   0 mirca      (501) staff       (20)    29069 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/QuickReference.dox
--rw-r--r--   0 mirca      (501) staff       (20)     6577 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/QuickStartGuide.dox
--rw-r--r--   0 mirca      (501) staff       (20)    19614 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/SparseLinearSystems.dox
--rw-r--r--   0 mirca      (501) staff       (20)     8312 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/SparseQuickReference.dox
--rw-r--r--   0 mirca      (501) staff       (20)     3424 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/StlContainers.dox
--rw-r--r--   0 mirca      (501) staff       (20)     4119 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/StorageOrders.dox
--rw-r--r--   0 mirca      (501) staff       (20)     6212 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/StructHavingEigenMembers.dox
--rw-r--r--   0 mirca      (501) staff       (20)     6156 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TemplateKeyword.dox
--rw-r--r--   0 mirca      (501) staff       (20)    10269 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TopicAliasing.dox
--rw-r--r--   0 mirca      (501) staff       (20)     5285 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TopicAssertions.dox
--rw-r--r--   0 mirca      (501) staff       (20)     1642 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TopicCMakeGuide.dox
--rw-r--r--   0 mirca      (501) staff       (20)      173 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TopicEigenExpressionTemplates.dox
--rw-r--r--   0 mirca      (501) staff       (20)     5453 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TopicLazyEvaluation.dox
--rw-r--r--   0 mirca      (501) staff       (20)     8806 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TopicLinearAlgebraDecompositions.dox
--rw-r--r--   0 mirca      (501) staff       (20)     2532 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TopicMultithreading.dox
--rw-r--r--   0 mirca      (501) staff       (20)      137 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TopicResizing.dox
--rw-r--r--   0 mirca      (501) staff       (20)      145 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TopicScalarTypes.dox
--rw-r--r--   0 mirca      (501) staff       (20)       97 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TopicVectorization.dox
--rw-r--r--   0 mirca      (501) staff       (20)     6900 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialAdvancedInitialization.dox
--rw-r--r--   0 mirca      (501) staff       (20)     8523 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialArrayClass.dox
--rw-r--r--   0 mirca      (501) staff       (20)     7823 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialBlockOperations.dox
--rw-r--r--   0 mirca      (501) staff       (20)     9726 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialGeometry.dox
--rw-r--r--   0 mirca      (501) staff       (20)    11202 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialLinearAlgebra.dox
--rw-r--r--   0 mirca      (501) staff       (20)     3986 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialMapClass.dox
--rw-r--r--   0 mirca      (501) staff       (20)     9865 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialMatrixArithmetic.dox
--rw-r--r--   0 mirca      (501) staff       (20)    12421 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialMatrixClass.dox
--rw-r--r--   0 mirca      (501) staff       (20)    12006 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialReductionsVisitorsBroadcasting.dox
--rw-r--r--   0 mirca      (501) staff       (20)     1910 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialReshapeSlicing.dox
--rw-r--r--   0 mirca      (501) staff       (20)    20478 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialSparse.dox
--rw-r--r--   0 mirca      (501) staff       (20)       89 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialSparse_example_details.dox
--rw-r--r--   0 mirca      (501) staff       (20)     6888 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/UnalignedArrayAssert.dox
--rw-r--r--   0 mirca      (501) staff       (20)     6633 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/UsingBlasLapackBackends.dox
--rw-r--r--   0 mirca      (501) staff       (20)     6020 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/UsingIntelMKL.dox
--rw-r--r--   0 mirca      (501) staff       (20)     1437 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/UsingNVCC.dox
--rw-r--r--   0 mirca      (501) staff       (20)     2924 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/WrongStackAlignment.dox
--rw-r--r--   0 mirca      (501) staff       (20)     7960 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/eigen_navtree_hacks.js
--rw-r--r--   0 mirca      (501) staff       (20)     4409 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/eigendoxy.css
--rw-r--r--   0 mirca      (501) staff       (20)     1362 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/eigendoxy_footer.html.in
--rw-r--r--   0 mirca      (501) staff       (20)     2243 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/eigendoxy_header.html.in
--rw-r--r--   0 mirca      (501) staff       (20)     5337 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/eigendoxy_layout.xml.in
--rw-r--r--   0 mirca      (501) staff       (20)     1095 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/eigendoxy_tabs.css
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:45.187462 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/
--rw-r--r--   0 mirca      (501) staff       (20)       34 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/.krazy
--rw-r--r--   0 mirca      (501) staff       (20)      685 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)      766 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/CustomizingEigen_Inheritance.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      189 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Cwise_erf.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      190 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Cwise_erfc.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      192 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Cwise_lgamma.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      282 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/DenseBase_middleCols_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      282 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/DenseBase_middleRows_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      283 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/DenseBase_template_int_middleCols.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      283 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/DenseBase_template_int_middleRows.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      206 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/QuickStart_example.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      305 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/QuickStart_example2_dynamic.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      289 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/QuickStart_example2_fixed.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      677 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TemplateKeyword_flexible.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      508 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TemplateKeyword_simple.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1589 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TutorialInplaceLU.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      622 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgComputeTwice.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      371 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgExComputeSolveError.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      381 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgExSolveColPivHouseholderQR.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      356 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgExSolveLDLT.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      348 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgInverseDeterminant.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      600 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgRankRevealing.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      405 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgSVDSolve.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      534 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      377 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgSetThreshold.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      466 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ArrayClass_accessors.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      400 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ArrayClass_addition.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      410 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ArrayClass_cwise_other.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      444 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ArrayClass_interop.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      591 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      237 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ArrayClass_mult.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      523 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_BlockOperations_block_assignment.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      390 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_BlockOperations_colrow.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      448 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_BlockOperations_corner.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      413 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_BlockOperations_print_block.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      348 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_BlockOperations_vector.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      401 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_PartialLU_solve.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      440 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_1nn.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      356 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      361 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple_rowwise.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      247 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_colwise.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      502 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_maxnorm.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      513 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      675 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      447 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_operatornorm.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      244 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_rowwise.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      531 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      680 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_simple_example_dynamic_size.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      282 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_simple_example_fixed_size.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      737 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/class_Block.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      526 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/class_CwiseBinaryOp.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      561 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/class_CwiseUnaryOp.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      371 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/class_CwiseUnaryOp_ptrfun.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      697 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/class_FixedBlock.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      673 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/class_FixedVectorBlock.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      775 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/class_VectorBlock.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      418 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/function_taking_eigenbase.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      594 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/function_taking_ref.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      366 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      145 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.entry
--rw-r--r--   0 mirca      (501) staff       (20)      948 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.evaluator
--rw-r--r--   0 mirca      (501) staff       (20)      591 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.expression
--rw-r--r--   0 mirca      (501) staff       (20)      146 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.main
--rw-r--r--   0 mirca      (501) staff       (20)       85 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.preamble
--rw-r--r--   0 mirca      (501) staff       (20)      605 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.traits
--rw-r--r--   0 mirca      (501) staff       (20)     1320 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/make_circulant2.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4275 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/matrixfree_cg.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2438 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/nullary_indexing.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      471 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/tut_arithmetic_add_sub.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      393 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/tut_arithmetic_dot_cross.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      612 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/tut_arithmetic_matrix_mul.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      529 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/tut_arithmetic_redux_basic.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      353 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/tut_arithmetic_scalar_mul_div.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      343 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/tut_matrix_coefficient_accessors.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      489 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/tut_matrix_resize.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      229 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/tut_matrix_resize_fixed_size.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       86 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/ftv2node.png
--rw-r--r--   0 mirca      (501) staff       (20)      229 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/ftv2pnode.png
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:45.537925 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/
--rw-r--r--   0 mirca      (501) staff       (20)       34 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/.krazy
--rw-r--r--   0 mirca      (501) staff       (20)      210 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/AngleAxis_mimic_euler.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      393 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/BiCGSTAB_simple.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      406 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/BiCGSTAB_step_by_step.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1114 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)      324 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/ColPivHouseholderQR_solve.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      792 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/ComplexEigenSolver_compute.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      216 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/ComplexEigenSolver_eigenvalues.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      194 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/ComplexEigenSolver_eigenvectors.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      301 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/ComplexSchur_compute.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      263 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/ComplexSchur_matrixT.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      221 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/ComplexSchur_matrixU.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       45 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_abs.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       46 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_abs2.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       55 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_acos.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       85 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_arg.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      232 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_array_power_array.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       55 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_asin.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       65 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_atan.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       64 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_boolean_and.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      105 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_boolean_not.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       64 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_boolean_or.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       63 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_boolean_xor.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       92 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_ceil.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       58 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_cos.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       64 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_cosh.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       44 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_cube.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       52 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_equal_equal.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       43 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_exp.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       93 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_floor.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       51 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_greater.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       52 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_greater_equal.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       47 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_inverse.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      104 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_isFinite.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      101 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_isInf.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      101 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_isNaN.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       51 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_less.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       52 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_less_equal.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       43 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_log.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       47 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_log10.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       54 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_max.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       54 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_min.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       39 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_minus.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       45 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_minus_equal.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       52 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_not_equal.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       39 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_plus.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       45 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_plus_equal.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       53 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_pow.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      141 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_product.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       49 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_quotient.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       93 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_round.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       85 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_scalar_power_array.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       45 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_sign.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       58 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_sin.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       64 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_sinh.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       55 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_slash_equal.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       44 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_sqrt.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       46 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_square.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       58 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_tan.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       64 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_tanh.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       55 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Cwise_times_equal.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      117 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/DenseBase_LinSpaced.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      420 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/DenseBase_LinSpacedInt.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      139 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/DenseBase_LinSpaced_seq.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       60 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/DenseBase_setLinSpaced.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      411 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/DirectionWise_hnormalized.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      186 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/DirectionWise_replicate.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      179 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/DirectionWise_replicate_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      800 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      361 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/EigenSolver_compute.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      176 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/EigenSolver_eigenvalues.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      181 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/EigenSolver_eigenvectors.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      430 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/EigenSolver_pseudoEigenvectors.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      325 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/FullPivHouseholderQR_solve.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      369 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/FullPivLU_image.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      317 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/FullPivLU_kernel.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      413 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/FullPivLU_solve.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      456 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/GeneralizedEigenSolver.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      339 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/HessenbergDecomposition_compute.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      391 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/HessenbergDecomposition_matrixH.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      482 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/HessenbergDecomposition_packedMatrix.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      300 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/HouseholderQR_householderQ.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      357 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/HouseholderQR_solve.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1316 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/HouseholderSequence_HouseholderSequence.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      603 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/IOFormat.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      614 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/JacobiSVD_basic.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      235 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Jacobi_makeGivens.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      292 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Jacobi_makeJacobi.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      519 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/LLT_example.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      456 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/LLT_solve.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      192 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/LeastSquaresNormalEquations.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      177 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/LeastSquaresQR.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      164 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Map_general_stride.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      199 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Map_inner_stride.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      138 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Map_outer_stride.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      182 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Map_placement_new.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       93 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Map_simple.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      169 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_adjoint.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      523 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_all.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      207 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_applyOnTheLeft.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      292 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_applyOnTheRight.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       70 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_array.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      234 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_array_const.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       56 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_asDiagonal.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      244 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_block_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      250 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_block_int_int_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      271 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_bottomLeftCorner_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      274 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_bottomRightCorner_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      242 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_bottomRows_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      119 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cast.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       82 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_col.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      287 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_colwise.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      410 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_computeInverseAndDetWithCheck.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      318 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_computeInverseWithCheck.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       80 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseAbs.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       81 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseAbs2.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      276 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseEqual.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       87 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseInverse.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       60 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseMax.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       60 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseMin.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      286 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseNotEqual.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      153 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseProduct.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       65 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseQuotient.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       80 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseSign.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       50 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseSqrt.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      188 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_diagonal.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      270 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_diagonal_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      274 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_diagonal_template_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      160 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_eigenvalues.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      226 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_end_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      467 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_eval.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      274 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_fixedBlock_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      376 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_hnormalized.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      486 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_homogeneous.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       50 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_identity.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       42 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_identity_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      145 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_inverse.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      241 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_isDiagonal.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      235 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_isIdentity.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      216 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_isOnes.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      293 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_isOrthogonal.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      231 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_isUnitary.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      215 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_isZero.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      236 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_leftCols_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      129 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_noalias.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       75 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_ones.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       77 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_ones_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       37 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_ones_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      132 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_operatorNorm.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      171 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_prod.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       42 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_random.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       37 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_random_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       39 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_random_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      170 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_replicate.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      163 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_replicate_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      407 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_reverse.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      239 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_rightCols_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       82 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_row.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      281 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_rowwise.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      244 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_segment_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      115 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_select.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      361 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_selfadjointView.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      290 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_set.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       83 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_setIdentity.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       72 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_setOnes.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       72 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_setRandom.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       72 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_setZero.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      226 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_start_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      248 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_bottomRows.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      230 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_end.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      264 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_block_int_int_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      274 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      301 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      277 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_bottomRightCorner.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      304 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_bottomRightCorner_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      265 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_topLeftCorner.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      292 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_topLeftCorner_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      268 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_topRightCorner.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      295 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_topRightCorner_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      242 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_leftCols.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      245 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_rightCols.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      244 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_segment.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      230 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_start.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      239 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_topRows.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      262 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_topLeftCorner_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      265 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_topRightCorner_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      233 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_topRows_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      414 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_transpose.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      573 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_triangularView.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       71 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_zero.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       73 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_zero_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       37 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_zero_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      157 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Matrix_Map_stride.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      111 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Matrix_resize_NoChange_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      235 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Matrix_resize_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      111 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Matrix_resize_int_NoChange.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      407 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Matrix_resize_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       52 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Matrix_setConstant_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       55 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Matrix_setConstant_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       52 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Matrix_setIdentity_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       45 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Matrix_setOnes_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       48 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Matrix_setOnes_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       47 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Matrix_setRandom_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       50 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Matrix_setRandom_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       45 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Matrix_setZero_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       48 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Matrix_setZero_int_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      372 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/PartialPivLU_solve.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      263 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/PartialRedux_count.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      176 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/PartialRedux_maxCoeff.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      176 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/PartialRedux_minCoeff.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      169 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/PartialRedux_norm.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      169 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/PartialRedux_prod.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      180 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/PartialRedux_squaredNorm.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      164 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/PartialRedux_sum.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      819 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/RealQZ_compute.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      429 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/RealSchur_RealSchur_MatrixType.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      343 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/RealSchur_compute.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      362 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      816 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      826 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      365 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      396 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType2.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      180 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_eigenvalues.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      193 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_eigenvectors.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      426 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_operatorInverseSqrt.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      363 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_operatorSqrt.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      184 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/SelfAdjointView_eigenvalues.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      157 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/SelfAdjointView_operatorNorm.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      411 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/SparseMatrix_coeffs.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      267 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_block.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      270 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_block_correct.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      591 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_cwise.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       76 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_mult1.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      230 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_mult2.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       86 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_mult3.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      101 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_mult4.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      109 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_mult5.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      525 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/TopicStorageOrders_example.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      520 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Triangular_solve.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      445 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tridiagonalization_Tridiagonalization_MatrixType.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      392 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tridiagonalization_compute.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      475 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tridiagonalization_decomposeInPlace.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      552 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tridiagonalization_diagonal.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      303 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tridiagonalization_householderCoefficients.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      394 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tridiagonalization_packedMatrix.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      132 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_AdvancedInitialization_Block.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      168 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_AdvancedInitialization_CommaTemporary.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      266 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_AdvancedInitialization_Join.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      272 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_AdvancedInitialization_LinSpaced.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      878 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      332 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_AdvancedInitialization_Zero.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      299 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_Map_rowmajor.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      896 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_Map_using.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      170 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_ReshapeMat2Mat.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      298 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_ReshapeMat2Vec.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      610 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_SlicingCol.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      179 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_SlicingVec.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       70 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_commainit_01.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      113 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_commainit_01b.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      215 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_commainit_02.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      146 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_solve_matrix_inverse.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      318 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_solve_multiple_rhs.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      368 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_solve_reuse_decomposition.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      256 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_solve_singular.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      273 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_solve_triangular.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      159 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_solve_triangular_inplace.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      504 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/VectorwiseOp_homogeneous.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      536 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Vectorwise_reverse.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      732 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/class_FullPivLU.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      506 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/compile_snippet.cpp.in
--rw-r--r--   0 mirca      (501) staff       (20)      468 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/tut_arithmetic_redux_minmax.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      187 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/tut_arithmetic_transpose_aliasing.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      277 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/tut_arithmetic_transpose_conjugate.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      173 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/tut_arithmetic_transpose_inplace.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      193 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/tut_matrix_assignment_resizing.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:45.573368 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/special_examples/
--rw-r--r--   0 mirca      (501) staff       (20)     1142 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/special_examples/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     1183 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/special_examples/Tutorial_sparse_example.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1576 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/special_examples/Tutorial_sparse_example_details.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      336 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/special_examples/random_cpp11.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2544 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/tutorial.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      254 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/eigen3.pc.in
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:45.639579 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/
--rw-r--r--   0 mirca      (501) staff       (20)     2791 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)      245 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/bdcsvd_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      233 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/block_nonconst_ctor_on_const_xpr_0.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      233 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/block_nonconst_ctor_on_const_xpr_1.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      261 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/block_nonconst_ctor_on_const_xpr_2.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      262 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/block_on_const_type_actually_const_0.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      262 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/block_on_const_type_actually_const_1.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      257 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/colpivqr_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      245 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/const_qualified_block_method_retval_0.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      240 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/const_qualified_block_method_retval_1.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      239 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/const_qualified_diagonal_method_retval.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      241 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/const_qualified_transpose_method_retval.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      271 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/cwiseunaryview_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      296 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/cwiseunaryview_on_const_type_actually_const.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      228 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/diagonal_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      250 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/diagonal_on_const_type_actually_const.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      276 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/eigensolver_cplx.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      259 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/eigensolver_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      156 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/failtest_sanity_check.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      247 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/fullpivlu_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      258 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/fullpivqr_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      248 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/jacobisvd_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      250 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/ldlt_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      248 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/llt_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      224 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/map_nonconst_ctor_on_const_ptr_0.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      246 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/map_nonconst_ctor_on_const_ptr_1.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      270 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/map_nonconst_ctor_on_const_ptr_2.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      314 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/map_nonconst_ctor_on_const_ptr_3.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      321 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/map_nonconst_ctor_on_const_ptr_4.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      249 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/map_on_const_type_actually_const_0.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      241 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/map_on_const_type_actually_const_1.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      250 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/partialpivlu_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      251 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/qr_int.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      263 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/ref_1.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      213 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/ref_2.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      231 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/ref_3.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      227 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/ref_4.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      238 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/ref_5.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      241 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/selfadjointview_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      266 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/selfadjointview_on_const_type_actually_const.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      302 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/sparse_ref_1.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      238 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/sparse_ref_2.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      271 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/sparse_ref_3.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      235 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/sparse_ref_4.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      285 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/sparse_ref_5.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      290 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/sparse_storage_mismatch.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      217 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/swap_1.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      210 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/swap_2.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      213 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/ternary_1.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      225 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/ternary_2.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      229 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/transpose_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      254 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/transpose_on_const_type_actually_const.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      238 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/triangularview_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      265 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/triangularview_on_const_type_actually_const.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:45.672957 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/
--rw-r--r--   0 mirca      (501) staff       (20)    10884 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     2205 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/cholesky.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2831 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/clacgv.f
--rw-r--r--   0 mirca      (501) staff       (20)     2340 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/cladiv.f
--rw-r--r--   0 mirca      (501) staff       (20)     6295 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/clarf.f
--rw-r--r--   0 mirca      (501) staff       (20)    23424 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/clarfb.f
--rw-r--r--   0 mirca      (501) staff       (20)     5344 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/clarfg.f
--rw-r--r--   0 mirca      (501) staff       (20)    10450 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/clarft.f
--rw-r--r--   0 mirca      (501) staff       (20)      578 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/complex_double.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      577 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/complex_single.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2969 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dladiv.f
--rw-r--r--   0 mirca      (501) staff       (20)     5259 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dlamch.f
--rw-r--r--   0 mirca      (501) staff       (20)     2514 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dlapy2.f
--rw-r--r--   0 mirca      (501) staff       (20)     2737 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dlapy3.f
--rw-r--r--   0 mirca      (501) staff       (20)     6167 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dlarf.f
--rw-r--r--   0 mirca      (501) staff       (20)    22749 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dlarfb.f
--rw-r--r--   0 mirca      (501) staff       (20)     4946 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dlarfg.f
--rw-r--r--   0 mirca      (501) staff       (20)    10222 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dlarft.f
--rw-r--r--   0 mirca      (501) staff       (20)      562 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/double.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1282 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dsecnd_NONE.f
--rw-r--r--   0 mirca      (501) staff       (20)     1826 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/eigenvalues.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2957 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/ilaclc.f
--rw-r--r--   0 mirca      (501) staff       (20)     2997 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/ilaclr.f
--rw-r--r--   0 mirca      (501) staff       (20)     2952 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/iladlc.f
--rw-r--r--   0 mirca      (501) staff       (20)     3000 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/iladlr.f
--rw-r--r--   0 mirca      (501) staff       (20)     2941 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/ilaslc.f
--rw-r--r--   0 mirca      (501) staff       (20)     2988 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/ilaslr.f
--rw-r--r--   0 mirca      (501) staff       (20)     2962 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/ilazlc.f
--rw-r--r--   0 mirca      (501) staff       (20)     3010 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/ilazlr.f
--rw-r--r--   0 mirca      (501) staff       (20)      877 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/lapack_common.h
--rw-r--r--   0 mirca      (501) staff       (20)     2655 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/lu.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1258 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/second_NONE.f
--rw-r--r--   0 mirca      (501) staff       (20)      561 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/single.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2897 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/sladiv.f
--rw-r--r--   0 mirca      (501) staff       (20)     5261 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/slamch.f
--rw-r--r--   0 mirca      (501) staff       (20)     2490 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/slapy2.f
--rw-r--r--   0 mirca      (501) staff       (20)     2701 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/slapy3.f
--rw-r--r--   0 mirca      (501) staff       (20)     6117 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/slarf.f
--rw-r--r--   0 mirca      (501) staff       (20)    22727 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/slarfb.f
--rw-r--r--   0 mirca      (501) staff       (20)     4908 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/slarfg.f
--rw-r--r--   0 mirca      (501) staff       (20)    10183 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/slarft.f
--rw-r--r--   0 mirca      (501) staff       (20)     4891 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/svd.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2839 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/zlacgv.f
--rw-r--r--   0 mirca      (501) staff       (20)     2364 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/zladiv.f
--rw-r--r--   0 mirca      (501) staff       (20)     6278 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/zlarf.f
--rw-r--r--   0 mirca      (501) staff       (20)    23498 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/zlarfb.f
--rw-r--r--   0 mirca      (501) staff       (20)     5359 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/zlarfg.f
--rw-r--r--   0 mirca      (501) staff       (20)    10453 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/zlarft.f
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:45.721735 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/scripts/
--rw-r--r--   0 mirca      (501) staff       (20)      328 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/scripts/CMakeLists.txt
--rwxr-xr-x   0 mirca      (501) staff       (20)      574 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/scripts/buildtests.in
--rw-r--r--   0 mirca      (501) staff       (20)     1566 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/scripts/cdashtesting.cmake.in
--rwxr-xr-x   0 mirca      (501) staff       (20)      670 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/scripts/check.in
--rwxr-xr-x   0 mirca      (501) staff       (20)       44 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/scripts/debug.in
--rw-r--r--   0 mirca      (501) staff       (20)     6384 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/scripts/eigen_gen_credits.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      738 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/scripts/eigen_gen_docs
--rwxr-xr-x   0 mirca      (501) staff       (20)       46 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/scripts/release.in
--rw-r--r--   0 mirca      (501) staff       (20)     2368 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/scripts/relicense.py
--rw-r--r--   0 mirca      (501) staff       (20)      216 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/signature_of_eigen3_matrix_library
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:45.929529 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/
--rw-r--r--   0 mirca      (501) staff       (20)    12197 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     8251 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/adjoint.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    19185 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/array.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    12295 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/array_for_matrix.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      953 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/array_of_string.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2334 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/array_replicate.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4877 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/array_reverse.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2424 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/bandmatrix.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    10604 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/basicstuff.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4234 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/bdcsvd.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1460 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/bicgstab.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    11602 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/block.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5534 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/boostmultiprec.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      174 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/bug1213.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      147 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/bug1213.h
--rw-r--r--   0 mirca      (501) staff       (20)      279 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/bug1213_main.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    17757 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/cholesky.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2686 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/cholmod_support.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2923 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/commainitializer.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1533 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/conjugate_gradient.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4280 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/conservative_resize.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2226 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/constructor.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6440 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/corners.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1749 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/ctorleak.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5345 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/cuda_basic.cu
--rw-r--r--   0 mirca      (501) staff       (20)     3368 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/cuda_common.h
--rw-r--r--   0 mirca      (501) staff       (20)     5054 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/denseLM.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2579 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/dense_storage.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2267 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/determinant.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4107 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/diagonal.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     7157 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/diagonalmatrices.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2221 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/dontalign.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4630 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/dynalloc.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2188 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/eigen2support.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6212 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/eigensolver_complex.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4038 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/eigensolver_generalized_real.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6174 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/eigensolver_generic.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    11023 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/eigensolver_selfadjoint.cpp
--rw-r--r--   0 mirca      (501) staff       (20)        0 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/evaluator_common.h
--rw-r--r--   0 mirca      (501) staff       (20)    19757 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/evaluators.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3629 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/exceptions.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4248 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/fastmath.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1866 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/first_aligned.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5557 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/geo_alignedbox.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3554 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/geo_eulerangles.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5462 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/geo_homogeneous.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     7556 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/geo_hyperplane.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4830 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/geo_orthomethods.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3916 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/geo_parametrizedline.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    10877 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/geo_quaternion.cpp
--rwxr-xr-x   0 mirca      (501) staff       (20)    23509 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/geo_transformations.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    10819 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/half_float.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2396 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/hessenberg.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5940 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/householder.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2572 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/incomplete_cholesky.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3872 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/inplace_decomposition.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5688 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/integer_types.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3849 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/inverse.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1095 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/is_same_dense.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2725 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/jacobi.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5453 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/jacobisvd.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6089 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/linearstructure.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1491 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/lscg.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     9867 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/lu.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    31881 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/main.h
--rw-r--r--   0 mirca      (501) staff       (20)     7940 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/mapped_matrix.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     7300 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/mapstaticmethods.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    10112 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/mapstride.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4715 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/meta.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      743 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/metis_support.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1781 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/miscmatrices.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    17752 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/mixingtypes.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      604 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/mpl2only.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4369 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/nesting_ops.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     8713 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/nomalloc.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    11724 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/nullary.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1692 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/numext.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    24150 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/packetmath.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      947 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/pardiso_support.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1894 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/pastix_support.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6298 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/permutationmatrices.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3196 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/prec_inverse_4x4.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    10790 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product.h
--rw-r--r--   0 mirca      (501) staff       (20)    14544 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_extra.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4252 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_large.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4088 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_mmtr.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     8803 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_notemporary.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3502 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_selfadjoint.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    11857 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_small.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5421 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_symm.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     7355 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_syrk.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6380 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_trmm.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4242 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_trmv.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4989 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_trsolve.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4586 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/qr.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    12543 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/qr_colpivoting.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5242 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/qr_fullpivoting.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4613 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/qtvector.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4365 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/rand.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3094 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/real_qz.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     7906 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/redux.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    11295 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/ref.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1097 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/resize.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2241 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/rvalue_types.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3561 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/schur_complex.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3956 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/schur_real.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2411 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/selfadjoint.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2147 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/simplicial_cholesky.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2051 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sizeof.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2631 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sizeoverflow.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2125 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/smallvectors.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6396 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse.h
--rw-r--r--   0 mirca      (501) staff       (20)     4732 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparseLM.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    25875 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse_basic.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    11867 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse_block.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     9989 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse_permutations.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    25566 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse_product.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6117 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse_ref.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    19059 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse_solver.h
--rw-r--r--   0 mirca      (501) staff       (20)     4691 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse_solvers.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5079 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse_vector.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1783 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparselu.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3815 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparseqr.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1754 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/special_numbers.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1833 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/spqr_support.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     8474 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/stable_norm.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4145 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/stddeque.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4693 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/stddeque_overload.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4115 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/stdlist.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5806 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/stdlist_overload.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5110 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/stdvector.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5008 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/stdvector_overload.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      948 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/superlu_support.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    17971 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/svd_common.h
--rw-r--r--   0 mirca      (501) staff       (20)     4050 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/svd_fill.h
--rw-r--r--   0 mirca      (501) staff       (20)     2974 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/swap.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     9470 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/triangular.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5853 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/umeyama.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      991 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/umfpack_support.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5857 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/unalignedassert.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2134 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/unalignedcount.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1750 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/upperbidiagonalization.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    20171 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/vectorization_logic.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     8627 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/vectorwiseop.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3994 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/visitor.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3384 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/zerosized.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:45.930969 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/
--rw-r--r--   0 mirca      (501) staff       (20)      263 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/CMakeLists.txt
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:45.981622 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/
--rw-r--r--   0 mirca      (501) staff       (20)     4241 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/AdolcForward
--rw-r--r--   0 mirca      (501) staff       (20)     6095 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/AlignedVector3
--rw-r--r--   0 mirca      (501) staff       (20)      905 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/ArpackSupport
--rw-r--r--   0 mirca      (501) staff       (20)     1054 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/AutoDiff
--rw-r--r--   0 mirca      (501) staff       (20)     5505 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/BVH
--rw-r--r--   0 mirca      (501) staff       (20)      603 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CMakeLists.txt
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:45.984277 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/
--rw-r--r--   0 mirca      (501) staff       (20)      307 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     4313 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/Tensor
--rw-r--r--   0 mirca      (501) staff       (20)     1273 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/TensorSymmetry
--rw-r--r--   0 mirca      (501) staff       (20)     1743 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/ThreadPool
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:43.921607 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.111615 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/
--rw-r--r--   0 mirca      (501) staff       (20)    60362 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/README.md
--rw-r--r--   0 mirca      (501) staff       (20)    20561 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
--rw-r--r--   0 mirca      (501) staff       (20)    11022 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
--rw-r--r--   0 mirca      (501) staff       (20)     7676 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
--rw-r--r--   0 mirca      (501) staff       (20)    49692 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
--rw-r--r--   0 mirca      (501) staff       (20)    14286 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
--rw-r--r--   0 mirca      (501) staff       (20)    14755 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
--rw-r--r--   0 mirca      (501) staff       (20)    14653 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
--rw-r--r--   0 mirca      (501) staff       (20)    26680 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
--rw-r--r--   0 mirca      (501) staff       (20)     1594 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
--rw-r--r--   0 mirca      (501) staff       (20)    62023 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
--rw-r--r--   0 mirca      (501) staff       (20)    18564 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
--rw-r--r--   0 mirca      (501) staff       (20)    44052 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
--rw-r--r--   0 mirca      (501) staff       (20)    11006 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
--rw-r--r--   0 mirca      (501) staff       (20)    47585 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
--rw-r--r--   0 mirca      (501) staff       (20)     8443 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
--rw-r--r--   0 mirca      (501) staff       (20)    11445 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
--rw-r--r--   0 mirca      (501) staff       (20)     2570 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
--rw-r--r--   0 mirca      (501) staff       (20)    11080 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
--rw-r--r--   0 mirca      (501) staff       (20)     2474 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
--rw-r--r--   0 mirca      (501) staff       (20)     5196 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
--rw-r--r--   0 mirca      (501) staff       (20)     9931 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
--rw-r--r--   0 mirca      (501) staff       (20)     7674 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
--rw-r--r--   0 mirca      (501) staff       (20)    15529 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
--rw-r--r--   0 mirca      (501) staff       (20)     6560 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
--rw-r--r--   0 mirca      (501) staff       (20)    25305 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
--rw-r--r--   0 mirca      (501) staff       (20)    10248 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
--rw-r--r--   0 mirca      (501) staff       (20)    14694 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
--rw-r--r--   0 mirca      (501) staff       (20)    23299 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
--rw-r--r--   0 mirca      (501) staff       (20)    14916 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
--rw-r--r--   0 mirca      (501) staff       (20)     6595 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
--rw-r--r--   0 mirca      (501) staff       (20)     5412 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
--rw-r--r--   0 mirca      (501) staff       (20)    14625 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
--rw-r--r--   0 mirca      (501) staff       (20)     6341 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
--rw-r--r--   0 mirca      (501) staff       (20)     1316 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
--rw-r--r--   0 mirca      (501) staff       (20)     2560 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
--rw-r--r--   0 mirca      (501) staff       (20)    23098 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
--rw-r--r--   0 mirca      (501) staff       (20)    25810 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
--rw-r--r--   0 mirca      (501) staff       (20)     8430 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
--rw-r--r--   0 mirca      (501) staff       (20)     2716 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
--rw-r--r--   0 mirca      (501) staff       (20)     8527 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
--rw-r--r--   0 mirca      (501) staff       (20)     7354 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
--rw-r--r--   0 mirca      (501) staff       (20)     1310 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
--rw-r--r--   0 mirca      (501) staff       (20)    13527 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
--rw-r--r--   0 mirca      (501) staff       (20)     5309 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
--rw-r--r--   0 mirca      (501) staff       (20)    34277 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
--rw-r--r--   0 mirca      (501) staff       (20)    15746 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
--rw-r--r--   0 mirca      (501) staff       (20)    10687 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
--rw-r--r--   0 mirca      (501) staff       (20)     9298 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
--rw-r--r--   0 mirca      (501) staff       (20)    33938 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
--rw-r--r--   0 mirca      (501) staff       (20)    30324 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h
--rw-r--r--   0 mirca      (501) staff       (20)    14052 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
--rw-r--r--   0 mirca      (501) staff       (20)    13633 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
--rw-r--r--   0 mirca      (501) staff       (20)    10527 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
--rw-r--r--   0 mirca      (501) staff       (20)     9941 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
--rw-r--r--   0 mirca      (501) staff       (20)     9489 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
--rw-r--r--   0 mirca      (501) staff       (20)     5100 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
--rw-r--r--   0 mirca      (501) staff       (20)    13196 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
--rw-r--r--   0 mirca      (501) staff       (20)     2446 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSycl.h
--rw-r--r--   0 mirca      (501) staff       (20)     5046 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclConvertToDeviceExpression.h
--rw-r--r--   0 mirca      (501) staff       (20)    11561 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExprConstructor.h
--rw-r--r--   0 mirca      (501) staff       (20)    12530 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractAccessor.h
--rw-r--r--   0 mirca      (501) staff       (20)     9699 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractFunctors.h
--rw-r--r--   0 mirca      (501) staff       (20)     5288 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclLeafCount.h
--rw-r--r--   0 mirca      (501) staff       (20)     6692 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclPlaceHolderExpr.h
--rw-r--r--   0 mirca      (501) staff       (20)     3090 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclRun.h
--rw-r--r--   0 mirca      (501) staff       (20)     9752 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclTuple.h
--rw-r--r--   0 mirca      (501) staff       (20)     9454 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
--rw-r--r--   0 mirca      (501) staff       (20)     7522 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
--rw-r--r--   0 mirca      (501) staff       (20)    28192 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.114102 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/
--rw-r--r--   0 mirca      (501) staff       (20)    10857 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
--rw-r--r--   0 mirca      (501) staff       (20)     9086 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
--rw-r--r--   0 mirca      (501) staff       (20)    13021 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.114930 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/util/
--rw-r--r--   0 mirca      (501) staff       (20)    21047 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.120421 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/
--rw-r--r--   0 mirca      (501) staff       (20)     8699 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
--rw-r--r--   0 mirca      (501) staff       (20)     9419 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
--rw-r--r--   0 mirca      (501) staff       (20)     8444 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
--rw-r--r--   0 mirca      (501) staff       (20)     4323 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/SimpleThreadPool.h
--rw-r--r--   0 mirca      (501) staff       (20)     1120 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
--rw-r--r--   0 mirca      (501) staff       (20)      801 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
--rw-r--r--   0 mirca      (501) staff       (20)     1084 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
--rw-r--r--   0 mirca      (501) staff       (20)      715 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.123982 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/
--rw-r--r--   0 mirca      (501) staff       (20)    22317 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
--rw-r--r--   0 mirca      (501) staff       (20)     4137 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
--rw-r--r--   0 mirca      (501) staff       (20)     8298 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/EmulateArray.h
--rw-r--r--   0 mirca      (501) staff       (20)     9377 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/EmulateCXX11Meta.h
--rw-r--r--   0 mirca      (501) staff       (20)     3760 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
--rw-r--r--   0 mirca      (501) staff       (20)     1102 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/EulerAngles
--rw-r--r--   0 mirca      (501) staff       (20)    13979 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/FFT
--rw-r--r--   0 mirca      (501) staff       (20)     1295 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/IterativeSolvers
--rw-r--r--   0 mirca      (501) staff       (20)      944 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/KroneckerProduct
--rw-r--r--   0 mirca      (501) staff       (20)     1102 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/LevenbergMarquardt
--rw-r--r--   0 mirca      (501) staff       (20)     7413 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/MPRealSupport
--rw-r--r--   0 mirca      (501) staff       (20)    17776 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/MatrixFunctions
--rw-r--r--   0 mirca      (501) staff       (20)      586 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/MoreVectorization
--rw-r--r--   0 mirca      (501) staff       (20)     5776 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/NonLinearOptimization
--rw-r--r--   0 mirca      (501) staff       (20)     1773 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/NumericalDiff
--rw-r--r--   0 mirca      (501) staff       (20)    19066 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/OpenGLSupport
--rw-r--r--   0 mirca      (501) staff       (20)     4770 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/Polynomials
--rw-r--r--   0 mirca      (501) staff       (20)      912 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/Skyline
--rw-r--r--   0 mirca      (501) staff       (20)     1324 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/SparseExtra
--rw-r--r--   0 mirca      (501) staff       (20)     1574 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/SpecialFunctions
--rw-r--r--   0 mirca      (501) staff       (20)      871 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/Splines
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:43.928880 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.126001 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/AutoDiff/
--rw-r--r--   0 mirca      (501) staff       (20)     3150 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
--rwxr-xr-x   0 mirca      (501) staff       (20)    28169 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
--rw-r--r--   0 mirca      (501) staff       (20)     9029 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.127388 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/BVH/
--rw-r--r--   0 mirca      (501) staff       (20)    12976 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/BVH/BVAlgorithms.h
--rw-r--r--   0 mirca      (501) staff       (20)     9166 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/BVH/KdBVH.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.128096 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Eigenvalues/
--rw-r--r--   0 mirca      (501) staff       (20)    29826 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.130557 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/EulerAngles/
--rw-r--r--   0 mirca      (501) staff       (20)      174 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/EulerAngles/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)    16755 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/EulerAngles/EulerAngles.h
--rw-r--r--   0 mirca      (501) staff       (20)    11467 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/EulerAngles/EulerSystem.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.131981 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/FFT/
--rw-r--r--   0 mirca      (501) staff       (20)     9222 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/FFT/ei_fftw_impl.h
--rw-r--r--   0 mirca      (501) staff       (20)    12275 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.137042 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/
--rw-r--r--   0 mirca      (501) staff       (20)     5379 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
--rw-r--r--   0 mirca      (501) staff       (20)    17769 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
--rw-r--r--   0 mirca      (501) staff       (20)    10442 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/GMRES.h
--rw-r--r--   0 mirca      (501) staff       (20)     2520 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
--rw-r--r--   0 mirca      (501) staff       (20)     5354 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/IterationController.h
--rw-r--r--   0 mirca      (501) staff       (20)    13264 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/MINRES.h
--rw-r--r--   0 mirca      (501) staff       (20)     5739 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/Scaling.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.137755 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/KroneckerProduct/
--rw-r--r--   0 mirca      (501) staff       (20)    10230 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.178309 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/
--rw-r--r--   0 mirca      (501) staff       (20)     2194 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt
--rw-r--r--   0 mirca      (501) staff       (20)     2443 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
--rw-r--r--   0 mirca      (501) staff       (20)     6648 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
--rw-r--r--   0 mirca      (501) staff       (20)     5039 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
--rw-r--r--   0 mirca      (501) staff       (20)     6804 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
--rw-r--r--   0 mirca      (501) staff       (20)    13292 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.183297 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/
--rw-r--r--   0 mirca      (501) staff       (20)    16662 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
--rw-r--r--   0 mirca      (501) staff       (20)    23257 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
--rw-r--r--   0 mirca      (501) staff       (20)    17427 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
--rw-r--r--   0 mirca      (501) staff       (20)    23511 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
--rw-r--r--   0 mirca      (501) staff       (20)    14310 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
--rw-r--r--   0 mirca      (501) staff       (20)     2107 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.183987 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/MoreVectorization/
--rw-r--r--   0 mirca      (501) staff       (20)     3035 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.191105 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/
--rw-r--r--   0 mirca      (501) staff       (20)    19828 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
--rw-r--r--   0 mirca      (501) staff       (20)    22135 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
--rw-r--r--   0 mirca      (501) staff       (20)     1864 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/chkder.h
--rw-r--r--   0 mirca      (501) staff       (20)     1915 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/covar.h
--rw-r--r--   0 mirca      (501) staff       (20)     3297 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
--rw-r--r--   0 mirca      (501) staff       (20)     2225 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
--rw-r--r--   0 mirca      (501) staff       (20)     9111 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
--rw-r--r--   0 mirca      (501) staff       (20)     3263 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
--rw-r--r--   0 mirca      (501) staff       (20)     1081 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
--rw-r--r--   0 mirca      (501) staff       (20)     3082 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
--rw-r--r--   0 mirca      (501) staff       (20)     1362 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.191810 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NumericalDiff/
--rw-r--r--   0 mirca      (501) staff       (20)     4020 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.193941 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Polynomials/
--rw-r--r--   0 mirca      (501) staff       (20)     7745 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Polynomials/Companion.h
--rw-r--r--   0 mirca      (501) staff       (20)    14376 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
--rw-r--r--   0 mirca      (501) staff       (20)     4806 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.198674 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/
--rw-r--r--   0 mirca      (501) staff       (20)    11358 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
--rw-r--r--   0 mirca      (501) staff       (20)    31065 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineMatrix.h
--rw-r--r--   0 mirca      (501) staff       (20)     7745 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
--rw-r--r--   0 mirca      (501) staff       (20)    10853 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineProduct.h
--rw-r--r--   0 mirca      (501) staff       (20)     7969 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineStorage.h
--rw-r--r--   0 mirca      (501) staff       (20)     3153 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineUtil.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.203049 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/
--rw-r--r--   0 mirca      (501) staff       (20)     4260 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h
--rw-r--r--   0 mirca      (501) staff       (20)    40316 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
--rw-r--r--   0 mirca      (501) staff       (20)    13744 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h
--rw-r--r--   0 mirca      (501) staff       (20)     7696 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/MarketIO.h
--rw-r--r--   0 mirca      (501) staff       (20)     7568 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
--rw-r--r--   0 mirca      (501) staff       (20)    11788 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/RandomSetter.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.242785 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/
--rw-r--r--   0 mirca      (501) staff       (20)     5441 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
--rw-r--r--   0 mirca      (501) staff       (20)     7907 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
--rw-r--r--   0 mirca      (501) staff       (20)     2261 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
--rw-r--r--   0 mirca      (501) staff       (20)    42539 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
--rw-r--r--   0 mirca      (501) staff       (20)     2709 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:43.928558 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/arch/
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.243640 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/arch/CUDA/
--rw-r--r--   0 mirca      (501) staff       (20)     4528 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/arch/CUDA/CudaSpecialFunctions.h
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.246464 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Splines/
--rw-r--r--   0 mirca      (501) staff       (20)    18316 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Splines/Spline.h
--rw-r--r--   0 mirca      (501) staff       (20)    16400 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Splines/SplineFitting.h
--rw-r--r--   0 mirca      (501) staff       (20)     4300 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Splines/SplineFwd.h
--rw-r--r--   0 mirca      (501) staff       (20)     1875 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/README.txt
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.247304 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/bench/
--rw-r--r--   0 mirca      (501) staff       (20)     3905 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/bench/bench_svd.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.249220 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/
--rw-r--r--   0 mirca      (501) staff       (20)      114 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)      830 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/Overview.dox
--rw-r--r--   0 mirca      (501) staff       (20)     5283 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/eigendoxy_layout.xml.in
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.258620 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/
--rw-r--r--   0 mirca      (501) staff       (20)     2108 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/BVH_Example.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      667 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     1944 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/EulerAngles.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2522 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/FFT.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      356 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixExponential.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      469 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixFunction.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      375 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixLogarithm.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      364 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixPower.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      424 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixPower_optimal.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      508 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixSine.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      524 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixSinh.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      434 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixSquareRoot.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2392 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/PolynomialSolver1.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      635 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/PolynomialUtils1.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.259284 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/snippets/
--rw-r--r--   0 mirca      (501) staff       (20)     1137 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/snippets/CMakeLists.txt
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.395454 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/
--rw-r--r--   0 mirca      (501) staff       (20)     7182 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/BVH.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     9538 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/CMakeLists.txt
--rw-r--r--   0 mirca      (501) staff       (20)     6481 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/EulerAngles.cpp
--rw-r--r--   0 mirca      (501) staff       (20)       47 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/FFT.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     9225 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/FFTW.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    65493 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/NonLinearOptimization.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2850 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/NumericalDiff.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2300 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/alignedvector3.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    10599 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/autodiff.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2934 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/autodiff_scalar.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3992 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_eventcount.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    18732 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_meta.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3085 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_non_blocking_thread_pool.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     7016 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_runqueue.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     9142 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_argmax.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     8904 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_argmax_cuda.cu
--rw-r--r--   0 mirca      (501) staff       (20)     9699 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_assign.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2538 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_broadcast_sycl.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5296 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_broadcasting.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2470 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_cast_float16_cuda.cu
--rw-r--r--   0 mirca      (501) staff       (20)     2991 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_casts.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    13040 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_chipping.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1983 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_comparisons.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5270 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_complex_cuda.cu
--rw-r--r--   0 mirca      (501) staff       (20)     2758 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_complex_cwise_ops_cuda.cu
--rw-r--r--   0 mirca      (501) staff       (20)     4289 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_concatenation.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1652 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_const.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     7280 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_contract_cuda.cu
--rw-r--r--   0 mirca      (501) staff       (20)    21118 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_contraction.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5362 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_convolution.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    46749 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_cuda.cu
--rw-r--r--   0 mirca      (501) staff       (20)     2510 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_custom_index.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3203 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_custom_op.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    13374 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_device.cu
--rw-r--r--   0 mirca      (501) staff       (20)     1125 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_device_sycl.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2099 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_dimension.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      991 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_empty.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     8407 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_expr.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    12770 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_fft.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     7234 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_fixed_size.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2159 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_forced_eval.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2755 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2250 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_generator.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5934 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_ifft.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    33556 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_image_patch.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    18746 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_index_list.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2101 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_inflation.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4121 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_intdiv.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3269 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_io.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1631 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_layout_swap.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      942 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_lvalue.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6707 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_map.cpp
--rw-r--r--   0 mirca      (501) staff       (20)      985 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_math.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1493 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_mixed_indices.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    15732 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_morphing.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1829 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_notification.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2885 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_of_complex.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2422 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_of_const_values.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    21449 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_of_float16_cuda.cu
--rw-r--r--   0 mirca      (501) staff       (20)     3758 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_of_strings.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2644 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_padding.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5491 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_patch.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2146 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_random.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2354 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_random_cuda.cu
--rw-r--r--   0 mirca      (501) staff       (20)    14383 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_reduction.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5457 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_reduction_cuda.cu
--rw-r--r--   0 mirca      (501) staff       (20)     4935 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_reduction_sycl.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6714 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_ref.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5277 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_reverse.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1478 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_roundings.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2970 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_scan.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2566 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_scan_cuda.cu
--rw-r--r--   0 mirca      (501) staff       (20)     6229 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_shuffling.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     9616 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_simple.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3016 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_striding.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1888 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_sugar.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5799 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_sycl.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    59071 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_symmetry.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    12691 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_thread_pool.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5718 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_uint128.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4599 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_volume_patch.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1272 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/dgmres.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3810 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/forward_adolc.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1237 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/gmres.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     9096 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/kronecker_product.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    55496 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/levenberg_marquardt.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     4409 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/matrix_exponential.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6540 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/matrix_function.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     2106 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/matrix_functions.h
--rw-r--r--   0 mirca      (501) staff       (20)     7150 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/matrix_power.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1042 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/matrix_square_root.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     1650 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/minres.cpp
-drwxr-xr-x   0 mirca      (501) staff       (20)        0 2024-03-02 00:03:46.396213 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/mpreal/
--rw-r--r--   0 mirca      (501) staff       (20)   118239 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/mpreal/mpreal.h
--rw-r--r--   0 mirca      (501) staff       (20)     2375 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/mpreal_support.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    10588 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/openglsupport.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     6626 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/polynomialsolver.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     3574 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/polynomialutils.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     5352 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/sparse_extra.cpp
--rw-r--r--   0 mirca      (501) staff       (20)    16332 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/special_functions.cpp
--rw-r--r--   0 mirca      (501) staff       (20)     8521 2019-10-03 00:55:58.000000 riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/splines.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.184227 riskparityportfolio-0.6.0/
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.270386 riskparityportfolio-0.6.0/.github/
+-rw-r--r--   0 palomar    (501) staff       (20)      119 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/.github/dependabot.yml
+-rw-r--r--   0 palomar    (501) staff       (20)      580 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/.github/issue_template.md
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.271089 riskparityportfolio-0.6.0/.github/workflows/
+-rw-r--r--   0 palomar    (501) staff       (20)      938 2024-05-24 13:30:36.000000 riskparityportfolio-0.6.0/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 palomar    (501) staff       (20)      243 2024-05-26 05:57:28.000000 riskparityportfolio-0.6.0/.gitignore
+-rw-r--r--   0 palomar    (501) staff       (20)     1068 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/LICENSE
+-rw-r--r--   0 palomar    (501) staff       (20)       80 2024-05-24 13:30:36.000000 riskparityportfolio-0.6.0/MANIFEST.in
+-rw-r--r--   0 palomar    (501) staff       (20)      534 2024-05-26 09:54:46.183569 riskparityportfolio-0.6.0/PKG-INFO
+-rw-r--r--   0 palomar    (501) staff       (20)     3854 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/README.md
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.271599 riskparityportfolio-0.6.0/docs/
+-rw-r--r--   0 palomar    (501) staff       (20)      636 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/docs/Makefile
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.272846 riskparityportfolio-0.6.0/docs/source/
+-rw-r--r--   0 palomar    (501) staff       (20)     6355 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/docs/source/conf.py
+-rw-r--r--   0 palomar    (501) staff       (20)     2275 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/docs/source/index.rst
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.275468 riskparityportfolio-0.6.0/docs/source/tutorials/
+-rw-r--r--   0 palomar    (501) staff       (20)    17780 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/docs/source/tutorials/comparison-with-pyrb.ipynb
+-rw-r--r--   0 palomar    (501) staff       (20)   127408 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/docs/source/tutorials/including-mean-return-and-variance.ipynb
+-rw-r--r--   0 palomar    (501) staff       (20)      163 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/docs/source/tutorials/index.rst
+-rw-r--r--   0 palomar    (501) staff       (20)     6751 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/docs/source/tutorials/minimal-usage.ipynb
+-rw-r--r--   0 palomar    (501) staff       (20)      371 2024-05-24 13:30:36.000000 riskparityportfolio-0.6.0/pyproject.toml
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.278499 riskparityportfolio-0.6.0/riskparityportfolio.egg-info/
+-rw-r--r--   0 palomar    (501) staff       (20)      534 2024-05-26 09:54:44.000000 riskparityportfolio-0.6.0/riskparityportfolio.egg-info/PKG-INFO
+-rw-r--r--   0 palomar    (501) staff       (20)    96786 2024-05-26 09:54:44.000000 riskparityportfolio-0.6.0/riskparityportfolio.egg-info/SOURCES.txt
+-rw-r--r--   0 palomar    (501) staff       (20)        1 2024-05-26 09:54:44.000000 riskparityportfolio-0.6.0/riskparityportfolio.egg-info/dependency_links.txt
+-rw-r--r--   0 palomar    (501) staff       (20)        1 2024-05-25 10:54:39.000000 riskparityportfolio-0.6.0/riskparityportfolio.egg-info/not-zip-safe
+-rw-r--r--   0 palomar    (501) staff       (20)       20 2024-05-26 09:54:44.000000 riskparityportfolio-0.6.0/riskparityportfolio.egg-info/top_level.txt
+-rw-r--r--   0 palomar    (501) staff       (20)       38 2024-05-26 09:54:46.184339 riskparityportfolio-0.6.0/setup.cfg
+-rw-r--r--   0 palomar    (501) staff       (20)     4806 2024-05-25 10:27:24.000000 riskparityportfolio-0.6.0/setup.py
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.230223 riskparityportfolio-0.6.0/src/
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.282757 riskparityportfolio-0.6.0/src/riskparityportfolio/
+-rw-r--r--   0 palomar    (501) staff       (20)      230 2024-05-24 13:30:36.000000 riskparityportfolio-0.6.0/src/riskparityportfolio/__init__.py
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.283247 riskparityportfolio-0.6.0/src/riskparityportfolio/examples/
+-rw-r--r--   0 palomar    (501) staff       (20)      387 2024-05-24 13:30:36.000000 riskparityportfolio-0.6.0/src/riskparityportfolio/examples/main.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2460 2024-05-25 10:48:47.000000 riskparityportfolio-0.6.0/src/riskparityportfolio/my_tests.py
+-rw-r--r--   0 palomar    (501) staff       (20)     1477 2024-05-24 13:30:36.000000 riskparityportfolio-0.6.0/src/riskparityportfolio/riskfunctions.py
+-rw-r--r--   0 palomar    (501) staff       (20)     6410 2024-05-25 08:44:04.000000 riskparityportfolio-0.6.0/src/riskparityportfolio/rpp.py
+-rw-r--r--   0 palomar    (501) staff       (20)    11129 2024-05-25 10:46:38.000000 riskparityportfolio-0.6.0/src/riskparityportfolio/sca.py
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.284555 riskparityportfolio-0.6.0/src/riskparityportfolio/tests/
+-rw-r--r--   0 palomar    (501) staff       (20)        0 2024-05-24 13:30:36.000000 riskparityportfolio-0.6.0/src/riskparityportfolio/tests/__init__.py
+-rw-r--r--   0 palomar    (501) staff       (20)     6341 2024-05-25 10:49:52.000000 riskparityportfolio-0.6.0/src/riskparityportfolio/tests/test_modern_rpp.py
+-rw-r--r--   0 palomar    (501) staff       (20)     1462 2024-05-24 13:30:36.000000 riskparityportfolio-0.6.0/src/riskparityportfolio/tests/test_vanilla_rpp.py
+-rw-r--r--   0 palomar    (501) staff       (20)     3206 2024-05-24 13:30:36.000000 riskparityportfolio-0.6.0/src/riskparityportfolio/vanilla.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2770 2024-05-24 13:30:36.000000 riskparityportfolio-0.6.0/src/riskparityportfolio/vanilla.h
+-rw-r--r--   0 palomar    (501) staff       (20)       22 2024-05-24 13:30:36.000000 riskparityportfolio-0.6.0/src/riskparityportfolio/version.py
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.230892 riskparityportfolio-0.6.0/third-party/
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.293120 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/
+-rw-r--r--   0 palomar    (501) staff       (20)      117 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/.hg_archival.txt
+-rw-r--r--   0 palomar    (501) staff       (20)      180 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/.hgeol
+-rw-r--r--   0 palomar    (501) staff       (20)      244 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/.hgignore
+-rw-r--r--   0 palomar    (501) staff       (20)     1844 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/.hgtags
+-rw-r--r--   0 palomar    (501) staff       (20)    24308 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     1516 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/COPYING.BSD
+-rw-r--r--   0 palomar    (501) staff       (20)    35147 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/COPYING.GPL
+-rw-r--r--   0 palomar    (501) staff       (20)    26530 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/COPYING.LGPL
+-rw-r--r--   0 palomar    (501) staff       (20)     2246 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/COPYING.MINPACK
+-rw-r--r--   0 palomar    (501) staff       (20)    16726 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/COPYING.MPL2
+-rw-r--r--   0 palomar    (501) staff       (20)      779 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/COPYING.README
+-rw-r--r--   0 palomar    (501) staff       (20)      543 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/CTestConfig.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)      180 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/CTestCustom.cmake.in
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.313113 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/
+-rw-r--r--   0 palomar    (501) staff       (20)      694 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     1206 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/Cholesky
+-rw-r--r--   0 palomar    (501) staff       (20)     1900 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/CholmodSupport
+-rw-r--r--   0 palomar    (501) staff       (20)    17961 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/Core
+-rw-r--r--   0 palomar    (501) staff       (20)      122 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/Dense
+-rw-r--r--   0 palomar    (501) staff       (20)       35 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/Eigen
+-rw-r--r--   0 palomar    (501) staff       (20)     1822 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/Eigenvalues
+-rw-r--r--   0 palomar    (501) staff       (20)     2050 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/Geometry
+-rw-r--r--   0 palomar    (501) staff       (20)      874 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/Householder
+-rw-r--r--   0 palomar    (501) staff       (20)     2083 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 palomar    (501) staff       (20)      939 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/Jacobi
+-rw-r--r--   0 palomar    (501) staff       (20)     1433 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/LU
+-rw-r--r--   0 palomar    (501) staff       (20)      991 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/MetisSupport
+-rw-r--r--   0 palomar    (501) staff       (20)     2483 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/OrderingMethods
+-rw-r--r--   0 palomar    (501) staff       (20)     1676 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/PaStiXSupport
+-rwxr-xr-x   0 palomar    (501) staff       (20)     1116 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/PardisoSupport
+-rw-r--r--   0 palomar    (501) staff       (20)     1317 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/QR
+-rw-r--r--   0 palomar    (501) staff       (20)      945 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/QtAlignedMalloc
+-rw-r--r--   0 palomar    (501) staff       (20)     1162 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/SPQRSupport
+-rw-r--r--   0 palomar    (501) staff       (20)     1629 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/SVD
+-rw-r--r--   0 palomar    (501) staff       (20)      919 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/Sparse
+-rw-r--r--   0 palomar    (501) staff       (20)     1371 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/SparseCholesky
+-rw-r--r--   0 palomar    (501) staff       (20)     2240 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/SparseCore
+-rw-r--r--   0 palomar    (501) staff       (20)     1713 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/SparseLU
+-rw-r--r--   0 palomar    (501) staff       (20)     1222 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/SparseQR
+-rw-r--r--   0 palomar    (501) staff       (20)      797 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/StdDeque
+-rw-r--r--   0 palomar    (501) staff       (20)      726 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/StdList
+-rw-r--r--   0 palomar    (501) staff       (20)      803 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/StdVector
+-rw-r--r--   0 palomar    (501) staff       (20)     2243 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/SuperLUSupport
+-rw-r--r--   0 palomar    (501) staff       (20)     1382 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/UmfPackSupport
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.239773 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.315225 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Cholesky/
+-rw-r--r--   0 palomar    (501) staff       (20)    24480 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 palomar    (501) staff       (20)    18395 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3974 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.315915 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/CholmodSupport/
+-rw-r--r--   0 palomar    (501) staff       (20)    22307 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.366429 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/
+-rw-r--r--   0 palomar    (501) staff       (20)    12115 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Array.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8179 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6775 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2720 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Assign.h
+-rw-r--r--   0 palomar    (501) staff       (20)    38153 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/AssignEvaluator.h
+-rwxr-xr-x   0 palomar    (501) staff       (20)    12479 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 palomar    (501) staff       (20)    13910 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 palomar    (501) staff       (20)    18064 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Block.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4249 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5689 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6990 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 palomar    (501) staff       (20)    62197 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4525 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7593 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 palomar    (501) staff       (20)    31424 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8256 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3877 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5282 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 palomar    (501) staff       (20)    27420 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 palomar    (501) staff       (20)    24212 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 palomar    (501) staff       (20)    21959 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9597 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 palomar    (501) staff       (20)    12666 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 palomar    (501) staff       (20)      970 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 palomar    (501) staff       (20)    11507 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Dot.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5619 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4769 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5705 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 palomar    (501) staff       (20)    21123 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 palomar    (501) staff       (20)    22185 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 palomar    (501) staff       (20)    10222 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7076 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/IO.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3519 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7239 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Map.h
+-rw-r--r--   0 palomar    (501) staff       (20)    10991 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 palomar    (501) staff       (20)    40865 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3369 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 palomar    (501) staff       (20)    19067 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 palomar    (501) staff       (20)    23213 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3400 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3582 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9234 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 palomar    (501) staff       (20)    21646 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 palomar    (501) staff       (20)    45180 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7235 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Product.h
+-rw-r--r--   0 palomar    (501) staff       (20)    49497 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6379 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Random.h
+-rw-r--r--   0 palomar    (501) staff       (20)    17852 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Redux.h
+-rw-r--r--   0 palomar    (501) staff       (20)    12800 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Ref.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5595 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4200 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7073 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6020 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Select.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14245 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1697 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6795 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Solve.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9136 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4365 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7692 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3865 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Stride.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2683 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Swap.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14777 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14386 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 palomar    (501) staff       (20)    37234 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3462 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 palomar    (501) staff       (20)    29441 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8074 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.233819 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.368630 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 palomar    (501) staff       (20)    18037 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 palomar    (501) staff       (20)    17776 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 palomar    (501) staff       (20)    27841 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1194 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.369754 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 palomar    (501) staff       (20)    15733 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 palomar    (501) staff       (20)    50985 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX512/PacketMath.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.371266 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 palomar    (501) staff       (20)    16443 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 palomar    (501) staff       (20)    10797 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rwxr-xr-x   0 palomar    (501) staff       (20)    37671 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.374133 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 palomar    (501) staff       (20)     4240 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/Complex.h
+-rw-r--r--   0 palomar    (501) staff       (20)    23528 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/Half.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2387 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/MathFunctions.h
+-rw-r--r--   0 palomar    (501) staff       (20)    10744 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/PacketMath.h
+-rw-r--r--   0 palomar    (501) staff       (20)    35538 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5509 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/TypeCasting.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.374856 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 palomar    (501) staff       (20)     1989 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1746 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/Default/Settings.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.376185 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 palomar    (501) staff       (20)    17706 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2846 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 palomar    (501) staff       (20)    28726 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/NEON/PacketMath.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.378385 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 palomar    (501) staff       (20)    19426 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 palomar    (501) staff       (20)    18888 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxr-xr-x   0 palomar    (501) staff       (20)    35843 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1759 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.379809 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 palomar    (501) staff       (20)    15366 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4418 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxr-xr-x   0 palomar    (501) staff       (20)    32283 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.382249 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/functors/
+-rw-r--r--   0 palomar    (501) staff       (20)     6284 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 palomar    (501) staff       (20)    18263 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8229 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4400 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 palomar    (501) staff       (20)      607 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 palomar    (501) staff       (20)    27944 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.458135 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/
+-rw-r--r--   0 palomar    (501) staff       (20)    81534 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 palomar    (501) staff       (20)    18478 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 palomar    (501) staff       (20)    15188 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6907 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5017 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 palomar    (501) staff       (20)    26808 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6368 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4905 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 palomar    (501) staff       (20)    19632 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 palomar    (501) staff       (20)    11198 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9901 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5209 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6105 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4066 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 palomar    (501) staff       (20)    20403 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 palomar    (501) staff       (20)    13743 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14722 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 palomar    (501) staff       (20)    10571 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 palomar    (501) staff       (20)    13979 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6513 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5741 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.469475 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/
+-rwxr-xr-x   0 palomar    (501) staff       (20)    15722 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 palomar    (501) staff       (20)    21579 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/Constants.h
+-rwxr-xr-x   0 palomar    (501) staff       (20)     3981 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14150 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/ForwardDeclarations.h
+-rwxr-xr-x   0 palomar    (501) staff       (20)     4026 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 palomar    (501) staff       (20)    36570 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 palomar    (501) staff       (20)    40579 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/Memory.h
+-rwxr-xr-x   0 palomar    (501) staff       (20)    20586 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 palomar    (501) staff       (20)       85 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 palomar    (501) staff       (20)      856 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 palomar    (501) staff       (20)    10518 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 palomar    (501) staff       (20)    34198 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.479385 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/
+-rw-r--r--   0 palomar    (501) staff       (20)    12558 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 palomar    (501) staff       (20)    17021 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4178 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 palomar    (501) staff       (20)    22944 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 palomar    (501) staff       (20)    17176 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9715 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14351 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5539 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 palomar    (501) staff       (20)    23586 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 palomar    (501) staff       (20)    20288 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3650 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 palomar    (501) staff       (20)    33674 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4104 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 palomar    (501) staff       (20)    22444 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.486759 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/
+-rw-r--r--   0 palomar    (501) staff       (20)    14815 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8423 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3639 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 palomar    (501) staff       (20)    20539 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 palomar    (501) staff       (20)    11961 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8949 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8308 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 palomar    (501) staff       (20)    32152 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6877 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8063 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/RotationBase.h
+-rwxr-xr-x   0 palomar    (501) staff       (20)     6324 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 palomar    (501) staff       (20)    60514 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7773 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6191 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.487291 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/arch/
+-rw-r--r--   0 palomar    (501) staff       (20)     5387 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/arch/Geometry_SSE.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.509729 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Householder/
+-rw-r--r--   0 palomar    (501) staff       (20)     4481 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5345 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 palomar    (501) staff       (20)    20603 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.514377 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 palomar    (501) staff       (20)     6755 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7253 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9289 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 palomar    (501) staff       (20)    15062 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 palomar    (501) staff       (20)    15234 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 palomar    (501) staff       (20)    11527 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7762 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4158 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.514910 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Jacobi/
+-rw-r--r--   0 palomar    (501) staff       (20)    15902 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.517422 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/LU/
+-rw-r--r--   0 palomar    (501) staff       (20)     3057 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 palomar    (501) staff       (20)    32803 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 palomar    (501) staff       (20)    15064 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 palomar    (501) staff       (20)    21478 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3555 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.517923 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/LU/arch/
+-rw-r--r--   0 palomar    (501) staff       (20)    13669 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/LU/arch/Inverse_SSE.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.518414 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/MetisSupport/
+-rw-r--r--   0 palomar    (501) staff       (20)     4588 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.520219 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/OrderingMethods/
+-rw-r--r--   0 palomar    (501) staff       (20)    16396 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 palomar    (501) staff       (20)    62266 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5229 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.520798 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 palomar    (501) staff       (20)    22248 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.521414 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/PardisoSupport/
+-rw-r--r--   0 palomar    (501) staff       (20)    20032 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.524853 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/QR/
+-rw-r--r--   0 palomar    (501) staff       (20)    24881 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4662 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 palomar    (501) staff       (20)    20805 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 palomar    (501) staff       (20)    25478 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14022 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2993 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.525265 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SPQRSupport/
+-rw-r--r--   0 palomar    (501) staff       (20)    11405 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.527968 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SVD/
+-rw-r--r--   0 palomar    (501) staff       (20)    48778 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 palomar    (501) staff       (20)    32949 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5099 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 palomar    (501) staff       (20)    12740 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 palomar    (501) staff       (20)    15957 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.529290 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCholesky/
+-rw-r--r--   0 palomar    (501) staff       (20)    24010 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6898 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.543921 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/
+-rw-r--r--   0 palomar    (501) staff       (20)    10537 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8164 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 palomar    (501) staff       (20)    13178 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2191 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8080 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 palomar    (501) staff       (20)    25592 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6485 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 palomar    (501) staff       (20)    12720 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 palomar    (501) staff       (20)    25840 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4711 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 palomar    (501) staff       (20)    12487 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5808 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3080 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1107 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 palomar    (501) staff       (20)    12589 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 palomar    (501) staff       (20)    52373 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 palomar    (501) staff       (20)    17923 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7329 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7049 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1699 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 palomar    (501) staff       (20)    15492 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 palomar    (501) staff       (20)    25715 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4424 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8704 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3175 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6437 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6602 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14831 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8110 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9657 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.555754 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/
+-rw-r--r--   0 palomar    (501) staff       (20)    27866 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4303 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7601 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4974 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 palomar    (501) staff       (20)    10022 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2049 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6712 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6582 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3681 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 palomar    (501) staff       (20)    10216 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4181 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5723 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8486 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9028 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4979 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4545 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2889 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.556640 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseQR/
+-rw-r--r--   0 palomar    (501) staff       (20)    28373 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.559004 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/StlSupport/
+-rw-r--r--   0 palomar    (501) staff       (20)     5117 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4147 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5330 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2809 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.559559 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 palomar    (501) staff       (20)    34345 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.562081 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 palomar    (501) staff       (20)    17202 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.571396 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/misc/
+-rw-r--r--   0 palomar    (501) staff       (20)     2913 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/misc/Image.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2742 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1748 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 palomar    (501) staff       (20)    30560 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/misc/blas.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7834 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/misc/lapack.h
+-rwxr-xr-x   0 palomar    (501) staff       (20)  1058368 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 palomar    (501) staff       (20)      474 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.579617 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/plugins/
+-rw-r--r--   0 palomar    (501) staff       (20)    13132 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 palomar    (501) staff       (20)    16929 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 palomar    (501) staff       (20)    37403 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4828 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5621 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6375 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2937 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1145 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/INSTALL
+-rw-r--r--   0 palomar    (501) staff       (20)      175 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/README.md
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.604003 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/
+-rw-r--r--   0 palomar    (501) staff       (20)     3932 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/BenchSparseUtil.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4392 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/BenchTimer.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2529 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/BenchUtil.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2008 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/README.txt
+-rw-r--r--   0 palomar    (501) staff       (20)    28983 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/analyze-blocking-sizes.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1421 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/basicbench.cxxlist
+-rw-r--r--   0 palomar    (501) staff       (20)     1107 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/basicbenchmark.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1669 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/basicbenchmark.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6313 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchBlasGemm.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3534 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchCholesky.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5788 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchEigenSolver.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2806 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchFFT.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3598 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchGeometry.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5193 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchVecAdd.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    10821 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/bench_gemm.cpp
+-rwxr-xr-x   0 palomar    (501) staff       (20)      618 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/bench_multi_compilers.sh
+-rw-r--r--   0 palomar    (501) staff       (20)    11652 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/bench_norm.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2159 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/bench_reverse.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      320 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/bench_sum.cpp
+-rwxr-xr-x   0 palomar    (501) staff       (20)      651 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/bench_unrolling
+-rw-r--r--   0 palomar    (501) staff       (20)    22259 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchmark-blocking-sizes.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      790 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchmark.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      835 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchmarkSlice.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      640 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchmarkX.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      605 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchmarkXcwise.cpp
+-rwxr-xr-x   0 palomar    (501) staff       (20)     1209 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchmark_suite
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.606018 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/
+-rw-r--r--   0 palomar    (501) staff       (20)     2869 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)    18109 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/COPYING
+-rw-r--r--   0 palomar    (501) staff       (20)     6447 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/README
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.640982 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/
+-rw-r--r--   0 palomar    (501) staff       (20)     3374 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_aat_product.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3354 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_ata_product.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3670 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_atv_product.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3371 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_axpby.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3340 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_axpy.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3202 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_cholesky.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3460 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_ger.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     5598 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_hessenberg.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3151 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_lu_decomp.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3598 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_lu_solve.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3886 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_matrix_matrix_product.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3982 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_matrix_matrix_product_bis.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3989 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_matrix_vector_product.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3188 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_partial_lu.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3019 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_rot.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3691 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_symv.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3664 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_syr2.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3425 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_trisolve.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     4061 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_trisolve_matrix.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3907 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_trmm.hh
+-rw-r--r--   0 palomar    (501) staff       (20)      467 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/basic_actions.hh
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.646916 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/
+-rw-r--r--   0 palomar    (501) staff       (20)      932 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindACML.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     1365 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindATLAS.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)      815 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindBLAZE.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     1092 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindBlitz.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)      668 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindCBLAS.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)      366 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindGMM.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     1370 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindMKL.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)      819 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindMTL4.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)      622 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindOPENBLAS.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     2372 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)      832 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindTvmet.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     1315 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.653662 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/
+-rw-r--r--   0 palomar    (501) staff       (20)      869 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     1368 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/action_settings.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     2224 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/gnuplot_common_settings.hh
+-rwxr-xr-x   0 palomar    (501) staff       (20)     2065 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/go_mean
+-rw-r--r--   0 palomar    (501) staff       (20)     5306 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/mean.cxx
+-rw-r--r--   0 palomar    (501) staff       (20)     1850 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/mk_gnuplot_script.sh
+-rw-r--r--   0 palomar    (501) staff       (20)      929 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/mk_mean_script.sh
+-rwxr-xr-x   0 palomar    (501) staff       (20)     1742 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/mk_new_gnuplot.sh
+-rw-r--r--   0 palomar    (501) staff       (20)      974 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/perlib_plot_settings.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     3425 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/regularize.cxx
+-rw-r--r--   0 palomar    (501) staff       (20)     5112 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/smooth.cxx
+-rwxr-xr-x   0 palomar    (501) staff       (20)     1687 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/smooth_all.sh
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.655437 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/
+-rw-r--r--   0 palomar    (501) staff       (20)     4827 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/bench.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     1916 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/bench_parameter.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     6748 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/btl.hh
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.658104 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/init/
+-rw-r--r--   0 palomar    (501) staff       (20)     1478 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/init/init_function.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     2295 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/init/init_matrix.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     1416 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/init/init_vector.hh
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.660969 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/static/
+-rw-r--r--   0 palomar    (501) staff       (20)     2278 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/static/bench_static.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     1948 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/static/intel_bench_fixed_size.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     2222 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/static/static_size_generator.hh
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.668825 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/
+-rw-r--r--   0 palomar    (501) staff       (20)     2305 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/STL_perf_analyzer.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     2522 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/STL_timer.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     1994 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     2938 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/portable_perf_analyzer.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3534 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh
+-rwxr-xr-x   0 palomar    (501) staff       (20)     3534 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/portable_timer.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     2927 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/x86_perf_analyzer.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     5294 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/x86_timer.hh
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.672228 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/
+-rw-r--r--   0 palomar    (501) staff       (20)     1658 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/size_lin_log.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     1645 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/size_log.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     2745 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/utilities.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2213 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/xy_file.hh
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.244422 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.677713 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/BLAS/
+-rw-r--r--   0 palomar    (501) staff       (20)     1572 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/BLAS/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)    35158 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/BLAS/blas.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2891 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/BLAS/blas_interface.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     4811 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/BLAS/blas_interface_impl.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     1634 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/BLAS/c_interface_base.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2963 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/BLAS/main.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.679872 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/STL/
+-rw-r--r--   0 palomar    (501) staff       (20)       37 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/STL/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     5838 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/STL/STL_interface.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     1828 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/STL/main.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.682233 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blaze/
+-rw-r--r--   0 palomar    (501) staff       (20)      475 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blaze/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     4012 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blaze/blaze_interface.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     1645 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blaze/main.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.686710 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blitz/
+-rw-r--r--   0 palomar    (501) staff       (20)      424 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blitz/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     5364 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blitz/blitz_LU_solve_interface.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     4129 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blitz/blitz_interface.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     1962 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blitz/btl_blitz.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1393 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blitz/btl_tiny_blitz.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3100 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blitz/tiny_blitz_interface.hh
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.731754 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen2/
+-rw-r--r--   0 palomar    (501) staff       (20)      768 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen2/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     1664 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5151 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen2/eigen2_interface.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     1799 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen2/main_adv.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1205 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen2/main_linear.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1384 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen2/main_matmat.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1456 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen2/main_vecmat.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.736936 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen3/
+-rw-r--r--   0 palomar    (501) staff       (20)     3292 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen3/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     1664 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     8077 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen3/eigen3_interface.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     1799 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen3/main_adv.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1285 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen3/main_linear.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1381 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen3/main_matmat.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1447 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen3/main_vecmat.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.740690 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/gmm/
+-rw-r--r--   0 palomar    (501) staff       (20)      125 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/gmm/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     5364 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/gmm/gmm_LU_solve_interface.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     4174 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/gmm/gmm_interface.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     2113 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/gmm/main.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.744655 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/mtl4/
+-rw-r--r--   0 palomar    (501) staff       (20)      153 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/mtl4/.kdbgrc.main
+-rw-r--r--   0 palomar    (501) staff       (20)      133 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/mtl4/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     1943 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/mtl4/main.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5364 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     4210 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/mtl4/mtl4_interface.hh
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.749338 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tensors/
+-rw-r--r--   0 palomar    (501) staff       (20)     2155 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tensors/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)      671 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tensors/main_linear.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      624 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tensors/main_matmat.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      624 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tensors/main_vecmat.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3190 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tensors/tensor_interface.hh
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.752178 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tvmet/
+-rw-r--r--   0 palomar    (501) staff       (20)      142 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tvmet/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     1460 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tvmet/main.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3017 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tvmet/tvmet_interface.hh
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.754707 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/ublas/
+-rw-r--r--   0 palomar    (501) staff       (20)      180 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/ublas/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     1785 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/ublas/main.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4342 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/ublas/ublas_interface.hh
+-rw-r--r--   0 palomar    (501) staff       (20)     3269 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/check_cache_queries.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6416 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/dense_solvers.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     7244 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/eig33.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3307 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/geometry.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.245011 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/perf_monitoring/
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.760692 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/
+-rw-r--r--   0 palomar    (501) staff       (20)     3786 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/changesets.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     1269 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/gemm.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      169 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/gemm_settings.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     2368 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/lazy_gemm.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      132 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/lazy_gemm_settings.txt
+-rwxr-xr-x   0 palomar    (501) staff       (20)      991 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/make_plot.sh
+-rwxr-xr-x   0 palomar    (501) staff       (20)     3290 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/run.sh
+-rw-r--r--   0 palomar    (501) staff       (20)     3232 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/product_threshold.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6006 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/quat_slerp.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1097 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/quatmul.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6260 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/sparse_cholesky.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5101 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/sparse_dense_product.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3011 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/sparse_lu.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     8999 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/sparse_product.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3358 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/sparse_randomsetter.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    13761 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/sparse_setter.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2347 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/sparse_transpose.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6114 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/sparse_trisolver.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.767346 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spbench/
+-rw-r--r--   0 palomar    (501) staff       (20)     2939 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spbench/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     3974 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spbench/sp_solver.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1856 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spbench/spbench.dtd
+-rw-r--r--   0 palomar    (501) staff       (20)     3302 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spbench/spbenchsolver.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    17717 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spbench/spbenchsolver.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3825 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spbench/spbenchstyle.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2830 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spbench/test_sparseLU.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6096 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spmv.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.775199 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/
+-rw-r--r--   0 palomar    (501) staff       (20)     2220 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/README
+-rw-r--r--   0 palomar    (501) staff       (20)     1585 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/benchmark.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6834 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/benchmark_main.cc
+-rw-r--r--   0 palomar    (501) staff       (20)     1389 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/contraction_benchmarks_cpu.cc
+-rw-r--r--   0 palomar    (501) staff       (20)    16193 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6264 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks_cpu.cc
+-rw-r--r--   0 palomar    (501) staff       (20)     3381 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks_fp16_gpu.cu
+-rw-r--r--   0 palomar    (501) staff       (20)     3373 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks_gpu.cu
+-rw-r--r--   0 palomar    (501) staff       (20)     1153 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks_sycl.cc
+-rw-r--r--   0 palomar    (501) staff       (20)     1203 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/vdw_new.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.845257 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/
+-rw-r--r--   0 palomar    (501) staff       (20)     3614 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/BandTriangularSolver.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1687 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     1608 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/GeneralRank1Update.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2036 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/PackedSelfadjointProduct.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3165 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/PackedTriangularMatrixVector.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3191 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/PackedTriangularSolverVector.h
+-rw-r--r--   0 palomar    (501) staff       (20)      183 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/README.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     2168 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/Rank2Update.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4361 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/common.h
+-rw-r--r--   0 palomar    (501) staff       (20)      647 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/complex_double.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      646 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/complex_single.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1501 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/double.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.865936 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/
+-rw-r--r--   0 palomar    (501) staff       (20)    15108 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/chbmv.c
+-rw-r--r--   0 palomar    (501) staff       (20)    13026 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/chpmv.c
+-rw-r--r--   0 palomar    (501) staff       (20)     2310 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/complexdots.c
+-rw-r--r--   0 palomar    (501) staff       (20)    18944 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/ctbmv.c
+-rw-r--r--   0 palomar    (501) staff       (20)      117 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/d_cnjg.c
+-rw-r--r--   0 palomar    (501) staff       (20)      657 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/datatypes.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4968 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/drotm.c
+-rw-r--r--   0 palomar    (501) staff       (20)     6193 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/drotmg.c
+-rw-r--r--   0 palomar    (501) staff       (20)    10188 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/dsbmv.c
+-rw-r--r--   0 palomar    (501) staff       (20)     8075 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/dspmv.c
+-rw-r--r--   0 palomar    (501) staff       (20)    11656 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/dtbmv.c
+-rw-r--r--   0 palomar    (501) staff       (20)     2976 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/lsame.c
+-rw-r--r--   0 palomar    (501) staff       (20)      105 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/r_cnjg.c
+-rw-r--r--   0 palomar    (501) staff       (20)     4902 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/srotm.c
+-rw-r--r--   0 palomar    (501) staff       (20)     6056 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/srotmg.c
+-rw-r--r--   0 palomar    (501) staff       (20)    10210 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/ssbmv.c
+-rw-r--r--   0 palomar    (501) staff       (20)     8051 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/sspmv.c
+-rw-r--r--   0 palomar    (501) staff       (20)    11642 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/stbmv.c
+-rw-r--r--   0 palomar    (501) staff       (20)    15144 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/zhbmv.c
+-rw-r--r--   0 palomar    (501) staff       (20)    13060 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/zhpmv.c
+-rw-r--r--   0 palomar    (501) staff       (20)    18972 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/ztbmv.c
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.866754 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/fortran/
+-rw-r--r--   0 palomar    (501) staff       (20)      979 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/fortran/complexdots.f
+-rw-r--r--   0 palomar    (501) staff       (20)     4956 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/level1_cplx_impl.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4559 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/level1_impl.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3617 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/level1_real_impl.h
+-rw-r--r--   0 palomar    (501) staff       (20)    12223 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/level2_cplx_impl.h
+-rw-r--r--   0 palomar    (501) staff       (20)    25172 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/level2_impl.h
+-rw-r--r--   0 palomar    (501) staff       (20)    10499 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/level2_real_impl.h
+-rw-r--r--   0 palomar    (501) staff       (20)    37780 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/level3_impl.h
+-rw-r--r--   0 palomar    (501) staff       (20)      757 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/single.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.897046 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/
+-rw-r--r--   0 palomar    (501) staff       (20)      964 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)    32109 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/cblat1.f
+-rw-r--r--   0 palomar    (501) staff       (20)     1546 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/cblat2.dat
+-rw-r--r--   0 palomar    (501) staff       (20)   116657 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/cblat2.f
+-rw-r--r--   0 palomar    (501) staff       (20)     1046 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/cblat3.dat
+-rw-r--r--   0 palomar    (501) staff       (20)   131550 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/cblat3.f
+-rw-r--r--   0 palomar    (501) staff       (20)    44819 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/dblat1.f
+-rw-r--r--   0 palomar    (501) staff       (20)     1466 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/dblat2.dat
+-rw-r--r--   0 palomar    (501) staff       (20)   112335 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/dblat2.f
+-rw-r--r--   0 palomar    (501) staff       (20)      882 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/dblat3.dat
+-rw-r--r--   0 palomar    (501) staff       (20)   104262 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/dblat3.f
+-rwxr-xr-x   0 palomar    (501) staff       (20)     1016 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/runblastest.sh
+-rw-r--r--   0 palomar    (501) staff       (20)    43388 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/sblat1.f
+-rw-r--r--   0 palomar    (501) staff       (20)     1466 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/sblat2.dat
+-rw-r--r--   0 palomar    (501) staff       (20)   112251 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/sblat2.f
+-rw-r--r--   0 palomar    (501) staff       (20)      882 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/sblat3.dat
+-rw-r--r--   0 palomar    (501) staff       (20)   104172 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/sblat3.f
+-rw-r--r--   0 palomar    (501) staff       (20)    32114 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/zblat1.f
+-rw-r--r--   0 palomar    (501) staff       (20)     1546 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/zblat2.dat
+-rw-r--r--   0 palomar    (501) staff       (20)   117003 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/zblat2.f
+-rw-r--r--   0 palomar    (501) staff       (20)     1046 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/zblat3.dat
+-rw-r--r--   0 palomar    (501) staff       (20)   131995 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/zblat3.f
+-rw-r--r--   0 palomar    (501) staff       (20)      389 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/xerbla.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.928428 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/
+-rw-r--r--   0 palomar    (501) staff       (20)      769 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/Eigen3Config.cmake.in
+-rw-r--r--   0 palomar    (501) staff       (20)     1397 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/Eigen3ConfigLegacy.cmake.in
+-rw-r--r--   0 palomar    (501) staff       (20)     2825 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/EigenConfigureTesting.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     1562 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/EigenDetermineOSVersion.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     1814 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/EigenDetermineVSServicePack.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)    26743 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/EigenTesting.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     1200 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/EigenUninstall.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)      501 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindAdolc.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)    43820 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindBLAS.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)    13031 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindBLASEXT.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     2572 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindCholmod.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     9003 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindComputeCpp.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     2842 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindEigen2.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     3501 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindEigen3.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     2757 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindFFTW.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     2943 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindGLEW.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)      554 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindGMP.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     5035 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindGSL.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)      909 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindGoogleHash.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)    11857 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindHWLOC.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     9909 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindLAPACK.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     2845 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindMPFR.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     8963 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindMetis.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)    14450 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindPTSCOTCH.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)    23207 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindPastix.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     1188 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindSPQR.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)    12010 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindScotch.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     2194 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindStandardMathLibrary.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     2299 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindSuperLU.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     1735 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindUmfpack.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)      936 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/RegexUtils.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)      177 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/UseEigen3.cmake
+-rw-r--r--   0 palomar    (501) staff       (20)     2413 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/language_support.cmake
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.248840 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/debug/
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.929918 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/debug/gdb/
+-rw-r--r--   0 palomar    (501) staff       (20)       22 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/debug/gdb/__init__.py
+-rw-r--r--   0 palomar    (501) staff       (20)     7548 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/debug/gdb/printers.py
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.931315 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/debug/msvc/
+-rw-r--r--   0 palomar    (501) staff       (20)    11661 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/debug/msvc/eigen.natvis
+-rw-r--r--   0 palomar    (501) staff       (20)     7566 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/debug/msvc/eigen_autoexp_part.dat
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.932019 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/
+-rw-r--r--   0 palomar    (501) staff       (20)      296 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/CMakeLists.txt
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.934894 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/mandelbrot/
+-rw-r--r--   0 palomar    (501) staff       (20)      486 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/mandelbrot/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)      336 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/mandelbrot/README
+-rw-r--r--   0 palomar    (501) staff       (20)     7509 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/mandelbrot/mandelbrot.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1888 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/mandelbrot/mandelbrot.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.937496 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/mix_eigen_and_c/
+-rw-r--r--   0 palomar    (501) staff       (20)      261 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/mix_eigen_and_c/README
+-rw-r--r--   0 palomar    (501) staff       (20)     4158 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/mix_eigen_and_c/binary_library.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3345 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/mix_eigen_and_c/binary_library.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1616 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/mix_eigen_and_c/example.c
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.961444 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/
+-rw-r--r--   0 palomar    (501) staff       (20)      695 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)      403 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/README
+-rw-r--r--   0 palomar    (501) staff       (20)     5981 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/camera.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3435 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/camera.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3974 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/gpuhelper.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     7177 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/gpuhelper.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3927 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/icosphere.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      869 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/icosphere.h
+-rw-r--r--   0 palomar    (501) staff       (20)    19192 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/quaternion_demo.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2635 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/quaternion_demo.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1756 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/trackball.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      943 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/trackball.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.052069 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/
+-rw-r--r--   0 palomar    (501) staff       (20)    12377 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/A05_PortingFrom2To3.dox
+-rw-r--r--   0 palomar    (501) staff       (20)    10274 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/AsciiQuickReference.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     2425 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/B01_Experimental.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     4659 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     6332 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/ClassHierarchy.dox
+-rw-r--r--   0 palomar    (501) staff       (20)    16511 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/CoeffwiseMathFunctionsTable.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     4424 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/CustomizingEigen_CustomScalar.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     1337 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/CustomizingEigen_InheritingMatrix.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     3658 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/CustomizingEigen_NullaryExpr.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     3658 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/CustomizingEigen_Plugins.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     5022 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/DenseDecompositionBenchmark.dox
+-rw-r--r--   0 palomar    (501) staff       (20)    85220 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/Doxyfile.in
+-rw-r--r--   0 palomar    (501) staff       (20)     8355 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/Eigen_Silly_Professor_64x64.png
+-rw-r--r--   0 palomar    (501) staff       (20)     1718 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/FixedSizeVectorizable.dox
+-rw-r--r--   0 palomar    (501) staff       (20)    13452 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/FunctionsTakingEigenTypes.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     5429 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/HiPerformance.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     3797 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/InplaceDecomposition.dox
+-rw-r--r--   0 palomar    (501) staff       (20)    30239 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/InsideEigenExample.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     2791 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/LeastSquares.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     6551 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/Manual.dox
+-rw-r--r--   0 palomar    (501) staff       (20)      758 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/MatrixfreeSolverExample.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     5610 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/NewExpressionType.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     2058 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/Overview.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     1153 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/PassingByValue.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     1984 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/Pitfalls.dox
+-rw-r--r--   0 palomar    (501) staff       (20)    13440 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/PreprocessorDirectives.dox
+-rw-r--r--   0 palomar    (501) staff       (20)    29069 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/QuickReference.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     6577 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/QuickStartGuide.dox
+-rw-r--r--   0 palomar    (501) staff       (20)    19614 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/SparseLinearSystems.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     8312 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/SparseQuickReference.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     3424 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/StlContainers.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     4119 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/StorageOrders.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     6212 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/StructHavingEigenMembers.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     6156 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TemplateKeyword.dox
+-rw-r--r--   0 palomar    (501) staff       (20)    10269 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TopicAliasing.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     5285 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TopicAssertions.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     1642 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TopicCMakeGuide.dox
+-rw-r--r--   0 palomar    (501) staff       (20)      173 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TopicEigenExpressionTemplates.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     5453 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TopicLazyEvaluation.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     8806 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TopicLinearAlgebraDecompositions.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     2532 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TopicMultithreading.dox
+-rw-r--r--   0 palomar    (501) staff       (20)      137 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TopicResizing.dox
+-rw-r--r--   0 palomar    (501) staff       (20)      145 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TopicScalarTypes.dox
+-rw-r--r--   0 palomar    (501) staff       (20)       97 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TopicVectorization.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     6900 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialAdvancedInitialization.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     8523 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialArrayClass.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     7823 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialBlockOperations.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     9726 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialGeometry.dox
+-rw-r--r--   0 palomar    (501) staff       (20)    11202 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialLinearAlgebra.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     3986 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialMapClass.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     9865 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialMatrixArithmetic.dox
+-rw-r--r--   0 palomar    (501) staff       (20)    12421 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialMatrixClass.dox
+-rw-r--r--   0 palomar    (501) staff       (20)    12006 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialReductionsVisitorsBroadcasting.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     1910 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialReshapeSlicing.dox
+-rw-r--r--   0 palomar    (501) staff       (20)    20478 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialSparse.dox
+-rw-r--r--   0 palomar    (501) staff       (20)       89 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialSparse_example_details.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     6888 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/UnalignedArrayAssert.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     6633 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/UsingBlasLapackBackends.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     6020 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/UsingIntelMKL.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     1437 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/UsingNVCC.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     2924 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/WrongStackAlignment.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     7960 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/eigen_navtree_hacks.js
+-rw-r--r--   0 palomar    (501) staff       (20)     4409 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/eigendoxy.css
+-rw-r--r--   0 palomar    (501) staff       (20)     1362 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/eigendoxy_footer.html.in
+-rw-r--r--   0 palomar    (501) staff       (20)     2243 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/eigendoxy_header.html.in
+-rw-r--r--   0 palomar    (501) staff       (20)     5337 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/eigendoxy_layout.xml.in
+-rw-r--r--   0 palomar    (501) staff       (20)     1095 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/eigendoxy_tabs.css
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.130272 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/
+-rw-r--r--   0 palomar    (501) staff       (20)       34 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/.krazy
+-rw-r--r--   0 palomar    (501) staff       (20)      685 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)      766 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/CustomizingEigen_Inheritance.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      189 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Cwise_erf.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      190 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Cwise_erfc.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      192 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Cwise_lgamma.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      282 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/DenseBase_middleCols_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      282 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/DenseBase_middleRows_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      283 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/DenseBase_template_int_middleCols.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      283 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/DenseBase_template_int_middleRows.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      206 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/QuickStart_example.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      305 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/QuickStart_example2_dynamic.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      289 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/QuickStart_example2_fixed.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      677 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TemplateKeyword_flexible.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      508 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TemplateKeyword_simple.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1589 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TutorialInplaceLU.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      622 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgComputeTwice.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      371 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgExComputeSolveError.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      381 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgExSolveColPivHouseholderQR.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      356 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgExSolveLDLT.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      348 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgInverseDeterminant.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      600 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgRankRevealing.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      405 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgSVDSolve.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      534 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      377 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgSetThreshold.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      466 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ArrayClass_accessors.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      400 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ArrayClass_addition.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      410 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ArrayClass_cwise_other.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      444 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ArrayClass_interop.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      591 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      237 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ArrayClass_mult.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      523 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_BlockOperations_block_assignment.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      390 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_BlockOperations_colrow.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      448 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_BlockOperations_corner.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      413 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_BlockOperations_print_block.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      348 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_BlockOperations_vector.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      401 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_PartialLU_solve.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      440 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_1nn.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      356 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      361 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple_rowwise.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      247 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_colwise.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      502 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_maxnorm.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      513 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      675 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      447 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_operatornorm.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      244 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_rowwise.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      531 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      680 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_simple_example_dynamic_size.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      282 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_simple_example_fixed_size.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      737 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/class_Block.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      526 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/class_CwiseBinaryOp.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      561 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/class_CwiseUnaryOp.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      371 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/class_CwiseUnaryOp_ptrfun.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      697 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/class_FixedBlock.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      673 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/class_FixedVectorBlock.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      775 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/class_VectorBlock.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      418 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/function_taking_eigenbase.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      594 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/function_taking_ref.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      366 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      145 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.entry
+-rw-r--r--   0 palomar    (501) staff       (20)      948 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.evaluator
+-rw-r--r--   0 palomar    (501) staff       (20)      591 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.expression
+-rw-r--r--   0 palomar    (501) staff       (20)      146 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.main
+-rw-r--r--   0 palomar    (501) staff       (20)       85 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.preamble
+-rw-r--r--   0 palomar    (501) staff       (20)      605 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.traits
+-rw-r--r--   0 palomar    (501) staff       (20)     1320 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/make_circulant2.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4275 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/matrixfree_cg.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2438 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/nullary_indexing.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      471 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/tut_arithmetic_add_sub.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      393 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/tut_arithmetic_dot_cross.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      612 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/tut_arithmetic_matrix_mul.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      529 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/tut_arithmetic_redux_basic.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      353 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/tut_arithmetic_scalar_mul_div.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      343 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/tut_matrix_coefficient_accessors.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      489 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/tut_matrix_resize.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      229 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/tut_matrix_resize_fixed_size.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       86 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/ftv2node.png
+-rw-r--r--   0 palomar    (501) staff       (20)      229 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/ftv2pnode.png
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.612282 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/
+-rw-r--r--   0 palomar    (501) staff       (20)       34 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/.krazy
+-rw-r--r--   0 palomar    (501) staff       (20)      210 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/AngleAxis_mimic_euler.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      393 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/BiCGSTAB_simple.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      406 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/BiCGSTAB_step_by_step.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1114 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)      324 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/ColPivHouseholderQR_solve.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      792 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/ComplexEigenSolver_compute.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      216 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/ComplexEigenSolver_eigenvalues.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      194 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/ComplexEigenSolver_eigenvectors.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      301 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/ComplexSchur_compute.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      263 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/ComplexSchur_matrixT.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      221 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/ComplexSchur_matrixU.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       45 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_abs.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       46 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_abs2.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       55 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_acos.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       85 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_arg.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      232 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_array_power_array.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       55 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_asin.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       65 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_atan.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       64 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_boolean_and.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      105 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_boolean_not.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       64 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_boolean_or.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       63 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_boolean_xor.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       92 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_ceil.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       58 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_cos.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       64 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_cosh.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       44 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_cube.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       52 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_equal_equal.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       43 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_exp.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       93 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_floor.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       51 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_greater.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       52 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_greater_equal.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       47 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_inverse.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      104 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_isFinite.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      101 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_isInf.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      101 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_isNaN.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       51 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_less.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       52 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_less_equal.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       43 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_log.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       47 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_log10.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       54 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_max.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       54 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_min.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       39 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_minus.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       45 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_minus_equal.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       52 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_not_equal.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       39 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_plus.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       45 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_plus_equal.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       53 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_pow.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      141 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_product.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       49 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_quotient.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       93 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_round.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       85 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_scalar_power_array.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       45 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_sign.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       58 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_sin.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       64 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_sinh.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       55 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_slash_equal.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       44 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_sqrt.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       46 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_square.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       58 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_tan.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       64 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_tanh.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       55 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Cwise_times_equal.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      117 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/DenseBase_LinSpaced.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      420 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/DenseBase_LinSpacedInt.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      139 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/DenseBase_LinSpaced_seq.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       60 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/DenseBase_setLinSpaced.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      411 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/DirectionWise_hnormalized.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      186 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/DirectionWise_replicate.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      179 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/DirectionWise_replicate_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      800 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      361 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/EigenSolver_compute.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      176 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/EigenSolver_eigenvalues.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      181 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/EigenSolver_eigenvectors.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      430 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/EigenSolver_pseudoEigenvectors.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      325 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/FullPivHouseholderQR_solve.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      369 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/FullPivLU_image.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      317 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/FullPivLU_kernel.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      413 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/FullPivLU_solve.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      456 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/GeneralizedEigenSolver.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      339 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/HessenbergDecomposition_compute.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      391 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/HessenbergDecomposition_matrixH.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      482 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/HessenbergDecomposition_packedMatrix.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      300 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/HouseholderQR_householderQ.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      357 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/HouseholderQR_solve.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1316 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/HouseholderSequence_HouseholderSequence.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      603 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/IOFormat.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      614 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/JacobiSVD_basic.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      235 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Jacobi_makeGivens.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      292 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Jacobi_makeJacobi.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      519 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/LLT_example.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      456 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/LLT_solve.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      192 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/LeastSquaresNormalEquations.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      177 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/LeastSquaresQR.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      164 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Map_general_stride.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      199 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Map_inner_stride.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      138 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Map_outer_stride.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      182 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Map_placement_new.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       93 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Map_simple.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      169 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_adjoint.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      523 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_all.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      207 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_applyOnTheLeft.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      292 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_applyOnTheRight.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       70 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_array.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      234 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_array_const.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       56 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_asDiagonal.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      244 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_block_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      250 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_block_int_int_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      271 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_bottomLeftCorner_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      274 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_bottomRightCorner_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      242 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_bottomRows_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      119 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cast.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       82 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_col.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      287 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_colwise.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      410 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_computeInverseAndDetWithCheck.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      318 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_computeInverseWithCheck.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       80 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseAbs.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       81 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseAbs2.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      276 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseEqual.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       87 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseInverse.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       60 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseMax.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       60 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseMin.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      286 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseNotEqual.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      153 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseProduct.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       65 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseQuotient.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       80 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseSign.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       50 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_cwiseSqrt.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      188 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_diagonal.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      270 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_diagonal_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      274 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_diagonal_template_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      160 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_eigenvalues.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      226 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_end_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      467 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_eval.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      274 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_fixedBlock_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      376 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_hnormalized.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      486 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_homogeneous.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       50 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_identity.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       42 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_identity_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      145 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_inverse.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      241 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_isDiagonal.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      235 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_isIdentity.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      216 2024-03-01 03:00:56.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_isOnes.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      293 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_isOrthogonal.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      231 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_isUnitary.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      215 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_isZero.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      236 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_leftCols_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      129 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_noalias.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       75 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_ones.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       77 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_ones_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       37 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_ones_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      132 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_operatorNorm.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      171 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_prod.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       42 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_random.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       37 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_random_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       39 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_random_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      170 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_replicate.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      163 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_replicate_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      407 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_reverse.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      239 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_rightCols_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       82 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_row.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      281 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_rowwise.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      244 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_segment_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      115 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_select.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      361 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_selfadjointView.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      290 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_set.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       83 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_setIdentity.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       72 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_setOnes.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       72 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_setRandom.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       72 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_setZero.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      226 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_start_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      248 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_bottomRows.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      230 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_end.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      264 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_block_int_int_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      274 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      301 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      277 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_bottomRightCorner.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      304 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_bottomRightCorner_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      265 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_topLeftCorner.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      292 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_topLeftCorner_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      268 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_topRightCorner.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      295 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_int_topRightCorner_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      242 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_leftCols.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      245 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_rightCols.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      244 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_segment.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      230 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_start.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      239 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_template_int_topRows.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      262 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_topLeftCorner_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      265 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_topRightCorner_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      233 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_topRows_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      414 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_transpose.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      573 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_triangularView.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       71 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_zero.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       73 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_zero_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       37 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_zero_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      157 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Matrix_Map_stride.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      111 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Matrix_resize_NoChange_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      235 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Matrix_resize_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      111 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Matrix_resize_int_NoChange.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      407 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Matrix_resize_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       52 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Matrix_setConstant_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       55 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Matrix_setConstant_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       52 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Matrix_setIdentity_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       45 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Matrix_setOnes_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       48 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Matrix_setOnes_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       47 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Matrix_setRandom_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       50 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Matrix_setRandom_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       45 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Matrix_setZero_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       48 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Matrix_setZero_int_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      372 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/PartialPivLU_solve.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      263 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/PartialRedux_count.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      176 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/PartialRedux_maxCoeff.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      176 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/PartialRedux_minCoeff.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      169 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/PartialRedux_norm.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      169 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/PartialRedux_prod.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      180 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/PartialRedux_squaredNorm.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      164 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/PartialRedux_sum.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      819 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/RealQZ_compute.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      429 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/RealSchur_RealSchur_MatrixType.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      343 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/RealSchur_compute.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      362 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      816 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      826 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      365 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      396 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType2.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      180 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_eigenvalues.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      193 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_eigenvectors.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      426 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_operatorInverseSqrt.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      363 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_operatorSqrt.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      184 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/SelfAdjointView_eigenvalues.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      157 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/SelfAdjointView_operatorNorm.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      411 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/SparseMatrix_coeffs.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      267 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_block.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      270 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_block_correct.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      591 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_cwise.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       76 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_mult1.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      230 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_mult2.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       86 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_mult3.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      101 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_mult4.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      109 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_mult5.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      525 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/TopicStorageOrders_example.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      520 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Triangular_solve.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      445 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tridiagonalization_Tridiagonalization_MatrixType.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      392 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tridiagonalization_compute.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      475 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tridiagonalization_decomposeInPlace.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      552 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tridiagonalization_diagonal.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      303 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tridiagonalization_householderCoefficients.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      394 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tridiagonalization_packedMatrix.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      132 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_AdvancedInitialization_Block.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      168 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_AdvancedInitialization_CommaTemporary.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      266 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_AdvancedInitialization_Join.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      272 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_AdvancedInitialization_LinSpaced.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      878 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      332 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_AdvancedInitialization_Zero.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      299 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_Map_rowmajor.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      896 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_Map_using.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      170 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_ReshapeMat2Mat.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      298 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_ReshapeMat2Vec.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      610 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_SlicingCol.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      179 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_SlicingVec.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       70 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_commainit_01.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      113 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_commainit_01b.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      215 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_commainit_02.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      146 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_solve_matrix_inverse.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      318 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_solve_multiple_rhs.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      368 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_solve_reuse_decomposition.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      256 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_solve_singular.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      273 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_solve_triangular.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      159 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_solve_triangular_inplace.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      504 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/VectorwiseOp_homogeneous.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      536 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Vectorwise_reverse.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      732 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/class_FullPivLU.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      506 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/compile_snippet.cpp.in
+-rw-r--r--   0 palomar    (501) staff       (20)      468 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/tut_arithmetic_redux_minmax.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      187 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/tut_arithmetic_transpose_aliasing.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      277 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/tut_arithmetic_transpose_conjugate.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      173 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/tut_arithmetic_transpose_inplace.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      193 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/tut_matrix_assignment_resizing.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.615897 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/special_examples/
+-rw-r--r--   0 palomar    (501) staff       (20)     1142 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/special_examples/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     1183 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/special_examples/Tutorial_sparse_example.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1576 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/special_examples/Tutorial_sparse_example_details.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      336 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/special_examples/random_cpp11.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2544 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/tutorial.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      254 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/eigen3.pc.in
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.660189 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/
+-rw-r--r--   0 palomar    (501) staff       (20)     2791 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)      245 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/bdcsvd_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      233 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/block_nonconst_ctor_on_const_xpr_0.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      233 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/block_nonconst_ctor_on_const_xpr_1.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      261 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/block_nonconst_ctor_on_const_xpr_2.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      262 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/block_on_const_type_actually_const_0.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      262 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/block_on_const_type_actually_const_1.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      257 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/colpivqr_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      245 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/const_qualified_block_method_retval_0.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      240 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/const_qualified_block_method_retval_1.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      239 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/const_qualified_diagonal_method_retval.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      241 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/const_qualified_transpose_method_retval.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      271 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/cwiseunaryview_nonconst_ctor_on_const_xpr.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      296 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/cwiseunaryview_on_const_type_actually_const.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      228 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/diagonal_nonconst_ctor_on_const_xpr.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      250 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/diagonal_on_const_type_actually_const.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      276 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/eigensolver_cplx.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      259 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/eigensolver_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      156 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/failtest_sanity_check.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      247 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/fullpivlu_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      258 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/fullpivqr_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      248 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/jacobisvd_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      250 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/ldlt_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      248 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/llt_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      224 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/map_nonconst_ctor_on_const_ptr_0.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      246 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/map_nonconst_ctor_on_const_ptr_1.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      270 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/map_nonconst_ctor_on_const_ptr_2.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      314 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/map_nonconst_ctor_on_const_ptr_3.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      321 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/map_nonconst_ctor_on_const_ptr_4.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      249 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/map_on_const_type_actually_const_0.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      241 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/map_on_const_type_actually_const_1.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      250 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/partialpivlu_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      251 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/qr_int.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      263 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/ref_1.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      213 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/ref_2.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      231 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/ref_3.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      227 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/ref_4.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      238 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/ref_5.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      241 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/selfadjointview_nonconst_ctor_on_const_xpr.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      266 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/selfadjointview_on_const_type_actually_const.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      302 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/sparse_ref_1.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      238 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/sparse_ref_2.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      271 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/sparse_ref_3.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      235 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/sparse_ref_4.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      285 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/sparse_ref_5.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      290 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/sparse_storage_mismatch.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      217 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/swap_1.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      210 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/swap_2.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      213 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/ternary_1.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      225 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/ternary_2.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      229 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/transpose_nonconst_ctor_on_const_xpr.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      254 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/transpose_on_const_type_actually_const.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      238 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/triangularview_nonconst_ctor_on_const_xpr.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      265 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/triangularview_on_const_type_actually_const.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.699743 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/
+-rw-r--r--   0 palomar    (501) staff       (20)    10884 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     2205 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/cholesky.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2831 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/clacgv.f
+-rw-r--r--   0 palomar    (501) staff       (20)     2340 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/cladiv.f
+-rw-r--r--   0 palomar    (501) staff       (20)     6295 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/clarf.f
+-rw-r--r--   0 palomar    (501) staff       (20)    23424 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/clarfb.f
+-rw-r--r--   0 palomar    (501) staff       (20)     5344 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/clarfg.f
+-rw-r--r--   0 palomar    (501) staff       (20)    10450 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/clarft.f
+-rw-r--r--   0 palomar    (501) staff       (20)      578 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/complex_double.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      577 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/complex_single.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2969 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dladiv.f
+-rw-r--r--   0 palomar    (501) staff       (20)     5259 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dlamch.f
+-rw-r--r--   0 palomar    (501) staff       (20)     2514 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dlapy2.f
+-rw-r--r--   0 palomar    (501) staff       (20)     2737 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dlapy3.f
+-rw-r--r--   0 palomar    (501) staff       (20)     6167 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dlarf.f
+-rw-r--r--   0 palomar    (501) staff       (20)    22749 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dlarfb.f
+-rw-r--r--   0 palomar    (501) staff       (20)     4946 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dlarfg.f
+-rw-r--r--   0 palomar    (501) staff       (20)    10222 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dlarft.f
+-rw-r--r--   0 palomar    (501) staff       (20)      562 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/double.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1282 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dsecnd_NONE.f
+-rw-r--r--   0 palomar    (501) staff       (20)     1826 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/eigenvalues.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2957 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/ilaclc.f
+-rw-r--r--   0 palomar    (501) staff       (20)     2997 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/ilaclr.f
+-rw-r--r--   0 palomar    (501) staff       (20)     2952 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/iladlc.f
+-rw-r--r--   0 palomar    (501) staff       (20)     3000 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/iladlr.f
+-rw-r--r--   0 palomar    (501) staff       (20)     2941 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/ilaslc.f
+-rw-r--r--   0 palomar    (501) staff       (20)     2988 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/ilaslr.f
+-rw-r--r--   0 palomar    (501) staff       (20)     2962 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/ilazlc.f
+-rw-r--r--   0 palomar    (501) staff       (20)     3010 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/ilazlr.f
+-rw-r--r--   0 palomar    (501) staff       (20)      877 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/lapack_common.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2655 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/lu.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1258 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/second_NONE.f
+-rw-r--r--   0 palomar    (501) staff       (20)      561 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/single.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2897 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/sladiv.f
+-rw-r--r--   0 palomar    (501) staff       (20)     5261 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/slamch.f
+-rw-r--r--   0 palomar    (501) staff       (20)     2490 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/slapy2.f
+-rw-r--r--   0 palomar    (501) staff       (20)     2701 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/slapy3.f
+-rw-r--r--   0 palomar    (501) staff       (20)     6117 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/slarf.f
+-rw-r--r--   0 palomar    (501) staff       (20)    22727 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/slarfb.f
+-rw-r--r--   0 palomar    (501) staff       (20)     4908 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/slarfg.f
+-rw-r--r--   0 palomar    (501) staff       (20)    10183 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/slarft.f
+-rw-r--r--   0 palomar    (501) staff       (20)     4891 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/svd.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2839 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/zlacgv.f
+-rw-r--r--   0 palomar    (501) staff       (20)     2364 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/zladiv.f
+-rw-r--r--   0 palomar    (501) staff       (20)     6278 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/zlarf.f
+-rw-r--r--   0 palomar    (501) staff       (20)    23498 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/zlarfb.f
+-rw-r--r--   0 palomar    (501) staff       (20)     5359 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/zlarfg.f
+-rw-r--r--   0 palomar    (501) staff       (20)    10453 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/zlarft.f
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.705984 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/scripts/
+-rw-r--r--   0 palomar    (501) staff       (20)      328 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/scripts/CMakeLists.txt
+-rwxr-xr-x   0 palomar    (501) staff       (20)      574 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/scripts/buildtests.in
+-rw-r--r--   0 palomar    (501) staff       (20)     1566 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/scripts/cdashtesting.cmake.in
+-rwxr-xr-x   0 palomar    (501) staff       (20)      670 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/scripts/check.in
+-rwxr-xr-x   0 palomar    (501) staff       (20)       44 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/scripts/debug.in
+-rw-r--r--   0 palomar    (501) staff       (20)     6384 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/scripts/eigen_gen_credits.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      738 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/scripts/eigen_gen_docs
+-rwxr-xr-x   0 palomar    (501) staff       (20)       46 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/scripts/release.in
+-rw-r--r--   0 palomar    (501) staff       (20)     2368 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/scripts/relicense.py
+-rw-r--r--   0 palomar    (501) staff       (20)      216 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/signature_of_eigen3_matrix_library
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.866994 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/
+-rw-r--r--   0 palomar    (501) staff       (20)    12197 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     8251 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/adjoint.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    19185 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/array.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    12295 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/array_for_matrix.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      953 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/array_of_string.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2334 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/array_replicate.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4877 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/array_reverse.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2424 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/bandmatrix.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    10604 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/basicstuff.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4234 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/bdcsvd.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1460 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/bicgstab.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    11602 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/block.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5534 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/boostmultiprec.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      174 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/bug1213.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      147 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/bug1213.h
+-rw-r--r--   0 palomar    (501) staff       (20)      279 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/bug1213_main.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    17757 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/cholesky.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2686 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/cholmod_support.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2923 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/commainitializer.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1533 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/conjugate_gradient.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4280 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/conservative_resize.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2226 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/constructor.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6440 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/corners.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1749 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/ctorleak.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5345 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/cuda_basic.cu
+-rw-r--r--   0 palomar    (501) staff       (20)     3368 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/cuda_common.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5054 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/denseLM.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2579 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/dense_storage.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2267 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/determinant.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4107 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/diagonal.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     7157 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/diagonalmatrices.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2221 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/dontalign.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4630 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/dynalloc.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2188 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/eigen2support.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6212 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/eigensolver_complex.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4038 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/eigensolver_generalized_real.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6174 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/eigensolver_generic.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    11023 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/eigensolver_selfadjoint.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)        0 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/evaluator_common.h
+-rw-r--r--   0 palomar    (501) staff       (20)    19757 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/evaluators.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3629 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/exceptions.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4248 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/fastmath.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1866 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/first_aligned.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5557 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/geo_alignedbox.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3554 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/geo_eulerangles.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5462 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/geo_homogeneous.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     7556 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/geo_hyperplane.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4830 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/geo_orthomethods.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3916 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/geo_parametrizedline.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    10877 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/geo_quaternion.cpp
+-rwxr-xr-x   0 palomar    (501) staff       (20)    23509 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/geo_transformations.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    10819 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/half_float.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2396 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/hessenberg.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5940 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/householder.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2572 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/incomplete_cholesky.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3872 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/inplace_decomposition.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5688 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/integer_types.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3849 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/inverse.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1095 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/is_same_dense.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2725 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/jacobi.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5453 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/jacobisvd.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6089 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/linearstructure.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1491 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/lscg.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     9867 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/lu.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    31881 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/main.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7940 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/mapped_matrix.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     7300 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/mapstaticmethods.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    10112 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/mapstride.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4715 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/meta.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      743 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/metis_support.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1781 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/miscmatrices.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    17752 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/mixingtypes.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      604 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/mpl2only.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4369 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/nesting_ops.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     8713 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/nomalloc.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    11724 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/nullary.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1692 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/numext.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    24150 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/packetmath.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      947 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/pardiso_support.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1894 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/pastix_support.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6298 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/permutationmatrices.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3196 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/prec_inverse_4x4.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    10790 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14544 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_extra.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4252 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_large.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4088 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_mmtr.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     8803 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_notemporary.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3502 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_selfadjoint.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    11857 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_small.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5421 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_symm.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     7355 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_syrk.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6380 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_trmm.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4242 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_trmv.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4989 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_trsolve.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4586 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/qr.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    12543 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/qr_colpivoting.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5242 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/qr_fullpivoting.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4613 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/qtvector.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4365 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/rand.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3094 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/real_qz.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     7906 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/redux.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    11295 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/ref.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1097 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/resize.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2241 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/rvalue_types.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3561 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/schur_complex.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3956 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/schur_real.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2411 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/selfadjoint.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2147 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/simplicial_cholesky.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2051 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sizeof.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2631 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sizeoverflow.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2125 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/smallvectors.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6396 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4732 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparseLM.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    25875 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse_basic.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    11867 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse_block.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     9989 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse_permutations.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    25566 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse_product.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6117 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse_ref.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    19059 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse_solver.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4691 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse_solvers.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5079 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse_vector.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1783 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparselu.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3815 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparseqr.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1754 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/special_numbers.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1833 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/spqr_support.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     8474 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/stable_norm.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4145 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/stddeque.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4693 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/stddeque_overload.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4115 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/stdlist.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5806 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/stdlist_overload.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5110 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/stdvector.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5008 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/stdvector_overload.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      948 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/superlu_support.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    17971 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/svd_common.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4050 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/svd_fill.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2974 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/swap.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     9470 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/triangular.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5853 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/umeyama.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      991 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/umfpack_support.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5857 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/unalignedassert.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2134 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/unalignedcount.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1750 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/upperbidiagonalization.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    20171 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/vectorization_logic.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     8627 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/vectorwiseop.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3994 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/visitor.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3384 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/zerosized.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.868456 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/
+-rw-r--r--   0 palomar    (501) staff       (20)      263 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/CMakeLists.txt
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.885869 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/
+-rw-r--r--   0 palomar    (501) staff       (20)     4241 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/AdolcForward
+-rw-r--r--   0 palomar    (501) staff       (20)     6095 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/AlignedVector3
+-rw-r--r--   0 palomar    (501) staff       (20)      905 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/ArpackSupport
+-rw-r--r--   0 palomar    (501) staff       (20)     1054 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/AutoDiff
+-rw-r--r--   0 palomar    (501) staff       (20)     5505 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/BVH
+-rw-r--r--   0 palomar    (501) staff       (20)      603 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CMakeLists.txt
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.888571 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/
+-rw-r--r--   0 palomar    (501) staff       (20)      307 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     4313 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/Tensor
+-rw-r--r--   0 palomar    (501) staff       (20)     1273 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/TensorSymmetry
+-rw-r--r--   0 palomar    (501) staff       (20)     1743 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/ThreadPool
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.255905 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.973706 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/
+-rw-r--r--   0 palomar    (501) staff       (20)    60362 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/README.md
+-rw-r--r--   0 palomar    (501) staff       (20)    20561 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
+-rw-r--r--   0 palomar    (501) staff       (20)    11022 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7676 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
+-rw-r--r--   0 palomar    (501) staff       (20)    49692 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14286 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14755 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14653 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
+-rw-r--r--   0 palomar    (501) staff       (20)    26680 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1594 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
+-rw-r--r--   0 palomar    (501) staff       (20)    62023 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
+-rw-r--r--   0 palomar    (501) staff       (20)    18564 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
+-rw-r--r--   0 palomar    (501) staff       (20)    44052 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
+-rw-r--r--   0 palomar    (501) staff       (20)    11006 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
+-rw-r--r--   0 palomar    (501) staff       (20)    47585 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8443 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
+-rw-r--r--   0 palomar    (501) staff       (20)    11445 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2570 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
+-rw-r--r--   0 palomar    (501) staff       (20)    11080 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2474 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5196 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9931 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7674 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
+-rw-r--r--   0 palomar    (501) staff       (20)    15529 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6560 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
+-rw-r--r--   0 palomar    (501) staff       (20)    25305 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
+-rw-r--r--   0 palomar    (501) staff       (20)    10248 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14694 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
+-rw-r--r--   0 palomar    (501) staff       (20)    23299 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14916 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6595 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5412 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14625 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6341 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1316 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2560 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
+-rw-r--r--   0 palomar    (501) staff       (20)    23098 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
+-rw-r--r--   0 palomar    (501) staff       (20)    25810 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8430 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2716 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8527 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7354 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1310 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
+-rw-r--r--   0 palomar    (501) staff       (20)    13527 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5309 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
+-rw-r--r--   0 palomar    (501) staff       (20)    34277 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
+-rw-r--r--   0 palomar    (501) staff       (20)    15746 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
+-rw-r--r--   0 palomar    (501) staff       (20)    10687 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9298 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
+-rw-r--r--   0 palomar    (501) staff       (20)    33938 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
+-rw-r--r--   0 palomar    (501) staff       (20)    30324 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14052 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
+-rw-r--r--   0 palomar    (501) staff       (20)    13633 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
+-rw-r--r--   0 palomar    (501) staff       (20)    10527 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9941 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9489 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5100 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
+-rw-r--r--   0 palomar    (501) staff       (20)    13196 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2446 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSycl.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5046 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclConvertToDeviceExpression.h
+-rw-r--r--   0 palomar    (501) staff       (20)    11561 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExprConstructor.h
+-rw-r--r--   0 palomar    (501) staff       (20)    12530 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractAccessor.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9699 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractFunctors.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5288 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclLeafCount.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6692 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclPlaceHolderExpr.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3090 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclRun.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9752 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclTuple.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9454 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7522 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
+-rw-r--r--   0 palomar    (501) staff       (20)    28192 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.976571 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/
+-rw-r--r--   0 palomar    (501) staff       (20)    10857 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9086 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
+-rw-r--r--   0 palomar    (501) staff       (20)    13021 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.977060 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/util/
+-rw-r--r--   0 palomar    (501) staff       (20)    21047 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.982653 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/
+-rw-r--r--   0 palomar    (501) staff       (20)     8699 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9419 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8444 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4323 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/SimpleThreadPool.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1120 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
+-rw-r--r--   0 palomar    (501) staff       (20)      801 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1084 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
+-rw-r--r--   0 palomar    (501) staff       (20)      715 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.985664 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/
+-rw-r--r--   0 palomar    (501) staff       (20)    22317 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4137 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
+-rw-r--r--   0 palomar    (501) staff       (20)     8298 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/EmulateArray.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9377 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/EmulateCXX11Meta.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3760 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1102 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/EulerAngles
+-rw-r--r--   0 palomar    (501) staff       (20)    13979 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/FFT
+-rw-r--r--   0 palomar    (501) staff       (20)     1295 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/IterativeSolvers
+-rw-r--r--   0 palomar    (501) staff       (20)      944 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/KroneckerProduct
+-rw-r--r--   0 palomar    (501) staff       (20)     1102 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/LevenbergMarquardt
+-rw-r--r--   0 palomar    (501) staff       (20)     7413 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/MPRealSupport
+-rw-r--r--   0 palomar    (501) staff       (20)    17776 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/MatrixFunctions
+-rw-r--r--   0 palomar    (501) staff       (20)      586 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/MoreVectorization
+-rw-r--r--   0 palomar    (501) staff       (20)     5776 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/NonLinearOptimization
+-rw-r--r--   0 palomar    (501) staff       (20)     1773 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/NumericalDiff
+-rw-r--r--   0 palomar    (501) staff       (20)    19066 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/OpenGLSupport
+-rw-r--r--   0 palomar    (501) staff       (20)     4770 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/Polynomials
+-rw-r--r--   0 palomar    (501) staff       (20)      912 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/Skyline
+-rw-r--r--   0 palomar    (501) staff       (20)     1324 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/SparseExtra
+-rw-r--r--   0 palomar    (501) staff       (20)     1574 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/SpecialFunctions
+-rw-r--r--   0 palomar    (501) staff       (20)      871 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/Splines
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.263301 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.987532 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/AutoDiff/
+-rw-r--r--   0 palomar    (501) staff       (20)     3150 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
+-rwxr-xr-x   0 palomar    (501) staff       (20)    28169 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9029 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.988462 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/BVH/
+-rw-r--r--   0 palomar    (501) staff       (20)    12976 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/BVH/BVAlgorithms.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9166 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/BVH/KdBVH.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.989010 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Eigenvalues/
+-rw-r--r--   0 palomar    (501) staff       (20)    29826 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.991019 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/EulerAngles/
+-rw-r--r--   0 palomar    (501) staff       (20)      174 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/EulerAngles/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)    16755 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/EulerAngles/EulerAngles.h
+-rw-r--r--   0 palomar    (501) staff       (20)    11467 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/EulerAngles/EulerSystem.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.992024 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/FFT/
+-rw-r--r--   0 palomar    (501) staff       (20)     9222 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/FFT/ei_fftw_impl.h
+-rw-r--r--   0 palomar    (501) staff       (20)    12275 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.996222 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/
+-rw-r--r--   0 palomar    (501) staff       (20)     5379 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
+-rw-r--r--   0 palomar    (501) staff       (20)    17769 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
+-rw-r--r--   0 palomar    (501) staff       (20)    10442 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/GMRES.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2520 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5354 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/IterationController.h
+-rw-r--r--   0 palomar    (501) staff       (20)    13264 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/MINRES.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5739 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/Scaling.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:45.996914 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/KroneckerProduct/
+-rw-r--r--   0 palomar    (501) staff       (20)    10230 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.001214 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/
+-rw-r--r--   0 palomar    (501) staff       (20)     2194 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     2443 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6648 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
+-rw-r--r--   0 palomar    (501) staff       (20)     5039 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
+-rw-r--r--   0 palomar    (501) staff       (20)     6804 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
+-rw-r--r--   0 palomar    (501) staff       (20)    13292 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.027994 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/
+-rw-r--r--   0 palomar    (501) staff       (20)    16662 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
+-rw-r--r--   0 palomar    (501) staff       (20)    23257 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
+-rw-r--r--   0 palomar    (501) staff       (20)    17427 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
+-rw-r--r--   0 palomar    (501) staff       (20)    23511 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14310 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2107 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.028435 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/MoreVectorization/
+-rw-r--r--   0 palomar    (501) staff       (20)     3035 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.033825 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/
+-rw-r--r--   0 palomar    (501) staff       (20)    19828 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
+-rw-r--r--   0 palomar    (501) staff       (20)    22135 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1864 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/chkder.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1915 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/covar.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3297 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2225 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
+-rw-r--r--   0 palomar    (501) staff       (20)     9111 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3263 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1081 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3082 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1362 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.034724 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NumericalDiff/
+-rw-r--r--   0 palomar    (501) staff       (20)     4020 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.036658 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Polynomials/
+-rw-r--r--   0 palomar    (501) staff       (20)     7745 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Polynomials/Companion.h
+-rw-r--r--   0 palomar    (501) staff       (20)    14376 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4806 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.040591 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/
+-rw-r--r--   0 palomar    (501) staff       (20)    11358 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
+-rw-r--r--   0 palomar    (501) staff       (20)    31065 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineMatrix.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7745 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
+-rw-r--r--   0 palomar    (501) staff       (20)    10853 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineProduct.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7969 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineStorage.h
+-rw-r--r--   0 palomar    (501) staff       (20)     3153 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineUtil.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.044324 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/
+-rw-r--r--   0 palomar    (501) staff       (20)     4260 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h
+-rw-r--r--   0 palomar    (501) staff       (20)    40316 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
+-rw-r--r--   0 palomar    (501) staff       (20)    13744 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7696 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/MarketIO.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7568 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
+-rw-r--r--   0 palomar    (501) staff       (20)    11788 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/RandomSetter.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.048122 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/
+-rw-r--r--   0 palomar    (501) staff       (20)     5441 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7907 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2261 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
+-rw-r--r--   0 palomar    (501) staff       (20)    42539 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2709 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:44.262918 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/arch/
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.048859 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/arch/CUDA/
+-rw-r--r--   0 palomar    (501) staff       (20)     4528 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/arch/CUDA/CudaSpecialFunctions.h
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.051316 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Splines/
+-rw-r--r--   0 palomar    (501) staff       (20)    18316 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Splines/Spline.h
+-rw-r--r--   0 palomar    (501) staff       (20)    16400 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Splines/SplineFitting.h
+-rw-r--r--   0 palomar    (501) staff       (20)     4300 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Splines/SplineFwd.h
+-rw-r--r--   0 palomar    (501) staff       (20)     1875 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/README.txt
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.051957 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/bench/
+-rw-r--r--   0 palomar    (501) staff       (20)     3905 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/bench/bench_svd.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.053787 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/
+-rw-r--r--   0 palomar    (501) staff       (20)      114 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)      830 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/Overview.dox
+-rw-r--r--   0 palomar    (501) staff       (20)     5283 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/eigendoxy_layout.xml.in
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.064738 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/
+-rw-r--r--   0 palomar    (501) staff       (20)     2108 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/BVH_Example.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      667 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     1944 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/EulerAngles.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2522 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/FFT.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      356 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixExponential.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      469 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixFunction.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      375 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixLogarithm.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      364 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixPower.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      424 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixPower_optimal.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      508 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixSine.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      524 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixSinh.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      434 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixSquareRoot.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2392 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/PolynomialSolver1.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      635 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/PolynomialUtils1.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.065622 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/snippets/
+-rw-r--r--   0 palomar    (501) staff       (20)     1137 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/snippets/CMakeLists.txt
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.180271 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/
+-rw-r--r--   0 palomar    (501) staff       (20)     7182 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/BVH.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     9538 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/CMakeLists.txt
+-rw-r--r--   0 palomar    (501) staff       (20)     6481 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/EulerAngles.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)       47 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/FFT.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     9225 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/FFTW.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    65493 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/NonLinearOptimization.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2850 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/NumericalDiff.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2300 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/alignedvector3.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    10599 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/autodiff.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2934 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/autodiff_scalar.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3992 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_eventcount.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    18732 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_meta.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3085 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_non_blocking_thread_pool.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     7016 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_runqueue.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     9142 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_argmax.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     8904 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_argmax_cuda.cu
+-rw-r--r--   0 palomar    (501) staff       (20)     9699 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_assign.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2538 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_broadcast_sycl.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5296 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_broadcasting.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2470 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_cast_float16_cuda.cu
+-rw-r--r--   0 palomar    (501) staff       (20)     2991 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_casts.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    13040 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_chipping.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1983 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_comparisons.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5270 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_complex_cuda.cu
+-rw-r--r--   0 palomar    (501) staff       (20)     2758 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_complex_cwise_ops_cuda.cu
+-rw-r--r--   0 palomar    (501) staff       (20)     4289 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_concatenation.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1652 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_const.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     7280 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_contract_cuda.cu
+-rw-r--r--   0 palomar    (501) staff       (20)    21118 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_contraction.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5362 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_convolution.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    46749 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_cuda.cu
+-rw-r--r--   0 palomar    (501) staff       (20)     2510 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_custom_index.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3203 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_custom_op.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    13374 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_device.cu
+-rw-r--r--   0 palomar    (501) staff       (20)     1125 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_device_sycl.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2099 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_dimension.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      991 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_empty.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     8407 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_expr.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    12770 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_fft.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     7234 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_fixed_size.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2159 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_forced_eval.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2755 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2250 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_generator.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5934 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_ifft.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    33556 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_image_patch.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    18746 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_index_list.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2101 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_inflation.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4121 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_intdiv.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3269 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_io.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1631 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_layout_swap.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      942 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_lvalue.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6707 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_map.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)      985 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_math.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1493 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_mixed_indices.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    15732 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_morphing.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1829 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_notification.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2885 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_of_complex.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2422 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_of_const_values.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    21449 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_of_float16_cuda.cu
+-rw-r--r--   0 palomar    (501) staff       (20)     3758 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_of_strings.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2644 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_padding.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5491 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_patch.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2146 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_random.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2354 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_random_cuda.cu
+-rw-r--r--   0 palomar    (501) staff       (20)    14383 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_reduction.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5457 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_reduction_cuda.cu
+-rw-r--r--   0 palomar    (501) staff       (20)     4935 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_reduction_sycl.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6714 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_ref.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5277 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_reverse.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1478 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_roundings.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2970 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_scan.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2566 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_scan_cuda.cu
+-rw-r--r--   0 palomar    (501) staff       (20)     6229 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_shuffling.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     9616 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_simple.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3016 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_striding.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1888 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_sugar.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5799 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_sycl.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    59071 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_symmetry.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    12691 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_thread_pool.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5718 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_uint128.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4599 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_volume_patch.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1272 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/dgmres.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3810 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/forward_adolc.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1237 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/gmres.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     9096 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/kronecker_product.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    55496 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/levenberg_marquardt.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     4409 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/matrix_exponential.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6540 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/matrix_function.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     2106 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/matrix_functions.h
+-rw-r--r--   0 palomar    (501) staff       (20)     7150 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/matrix_power.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1042 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/matrix_square_root.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     1650 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/minres.cpp
+drwxr-xr-x   0 palomar    (501) staff       (20)        0 2024-05-26 09:54:46.180885 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/mpreal/
+-rw-r--r--   0 palomar    (501) staff       (20)   118239 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/mpreal/mpreal.h
+-rw-r--r--   0 palomar    (501) staff       (20)     2375 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/mpreal_support.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    10588 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/openglsupport.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     6626 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/polynomialsolver.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     3574 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/polynomialutils.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     5352 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/sparse_extra.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)    16332 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/special_functions.cpp
+-rw-r--r--   0 palomar    (501) staff       (20)     8521 2024-03-01 03:00:57.000000 riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/splines.cpp
```

### Comparing `riskparityportfolio-0.5.1/LICENSE` & `riskparityportfolio-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/PKG-INFO` & `riskparityportfolio-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riskparityportfolio
-Version: 0.5.1
+Version: 0.6.0
 Summary: Blazingly fast design of risk parity portfolios
 Home-page: https://github.com/dppalomar/riskparity.py
 Author: Ze Vinicius & Dani Palomar
 Author-email: jvmirca@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `riskparityportfolio-0.5.1/README.md` & `riskparityportfolio-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/riskparityportfolio.egg-info/PKG-INFO` & `riskparityportfolio-0.6.0/riskparityportfolio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riskparityportfolio
-Version: 0.5.1
+Version: 0.6.0
 Summary: Blazingly fast design of risk parity portfolios
 Home-page: https://github.com/dppalomar/riskparity.py
 Author: Ze Vinicius & Dani Palomar
 Author-email: jvmirca@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `riskparityportfolio-0.5.1/riskparityportfolio.egg-info/SOURCES.txt` & `riskparityportfolio-0.6.0/riskparityportfolio.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,40 @@
+.gitignore
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
+.github/dependabot.yml
+.github/issue_template.md
+.github/workflows/pythonpackage.yml
+docs/Makefile
+docs/source/conf.py
+docs/source/index.rst
+docs/source/tutorials/comparison-with-pyrb.ipynb
+docs/source/tutorials/including-mean-return-and-variance.ipynb
+docs/source/tutorials/index.rst
+docs/source/tutorials/minimal-usage.ipynb
 riskparityportfolio.egg-info/PKG-INFO
 riskparityportfolio.egg-info/SOURCES.txt
 riskparityportfolio.egg-info/dependency_links.txt
 riskparityportfolio.egg-info/not-zip-safe
 riskparityportfolio.egg-info/top_level.txt
 src/riskparityportfolio/__init__.py
+src/riskparityportfolio/my_tests.py
 src/riskparityportfolio/riskfunctions.py
 src/riskparityportfolio/rpp.py
 src/riskparityportfolio/sca.py
 src/riskparityportfolio/vanilla.cpp
 src/riskparityportfolio/vanilla.h
 src/riskparityportfolio/version.py
+src/riskparityportfolio/examples/main.cpp
+src/riskparityportfolio/tests/__init__.py
+src/riskparityportfolio/tests/test_modern_rpp.py
+src/riskparityportfolio/tests/test_vanilla_rpp.py
 third-party/eigen_3.3.7/.hg_archival.txt
 third-party/eigen_3.3.7/.hgeol
 third-party/eigen_3.3.7/.hgignore
 third-party/eigen_3.3.7/.hgtags
 third-party/eigen_3.3.7/CMakeLists.txt
 third-party/eigen_3.3.7/COPYING.BSD
 third-party/eigen_3.3.7/COPYING.GPL
```

### Comparing `riskparityportfolio-0.5.1/setup.py` & `riskparityportfolio-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, Extension
 from setuptools.command.build_ext import build_ext
 import sys
 import setuptools
 import os
 
-__version__ = "0.5.1"
+__version__ = "0.6.0"
 
 # Prepare and send a new release to PyPI
 if "release" in sys.argv[-1]:
     os.system("python setup.py sdist")
     os.system("twine upload dist/*")
     os.system("rm -rf dist/riskparityportfolio*")
     sys.exit()
```

### Comparing `riskparityportfolio-0.5.1/src/riskparityportfolio/riskfunctions.py` & `riskparityportfolio-0.6.0/src/riskparityportfolio/riskfunctions.py`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/src/riskparityportfolio/rpp.py` & `riskparityportfolio-0.6.0/src/riskparityportfolio/rpp.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,32 +14,54 @@
 
 class RiskParityPortfolioValidator:
     def __init__(self):
         pass
 
 
 class RiskParityPortfolio:
-    """Designs risk parity portfolios by solving the following optimization problem
+    """Designs risk parity portfolios by solving the following optimization problem:
 
-    minimize R(w) - alpha * mu.T * w + lambda * w.T Sigma w
-    subject to Cw = c, Dw <= d
+      minimize     R(w) - alpha * mu.T w + lambda * w.T Sigma w
+      subject to   Cw = c, Dw <= d
 
-    where R is a risk concentration function, and alpha and lambda are trade-off
+    where R(w) is a risk concentration function, and alpha and lambda are trade-off
     parameters for the expected return and the variance, respectively.
 
+    The risk concentration R(w) is computed as the squared l2-norm of the risk concentration vector,
+    which by default is obtained from RiskContribOverVarianceMinusBudget():
+
+      R(w) = sum_i (MR_i/sum(MR_i) - budget_i)^2
+
+    where MR_i = w_i * (Sigma @ w)_i are the marginal risks (sum(MR_i) = Var(w)), and
+          budget_i are the risk budgets (by default 1/n).
+
     Parameters
     ----------
     covariance : array, shape=(n, n)
         covariance matrix of the assets
     budget : array, shape=(n,)
         risk budget vector
     weights : array, shape=(n,)
         weights of the portfolio
     risk_concentration : class
         any valid child class of RiskConcentrationFunction
+
+    Examples:
+    # Set up:
+    >>> import numpy as np
+    >>> import riskparityportfolio as rpp
+    >>> n = 10
+    >>> U = np.random.multivariate_normal(mean=np.zeros(n), cov=0.1 * np.eye(n), size=round(.7 * n)).T
+    >>> Sigma = U @ U.T + np.eye(n)
+    # Basic usage with default constraints sum(w) = 1 and w >= 0:
+    >>> my_portfolio = rpp.RiskParityPortfolio(Sigma)
+    >>> my_portfolio.design()
+    >>> my_portfolio.weights
+    # Basic usage with equality and inequality constraints:
+    >>> my_portfolio.design(Cmat=Cmat, cvec=cvec, Dmat=Dmat, dvec=dvec)
     """
 
     def __init__(
         self,
         covariance,
         budget=None,
         weights=None,
@@ -168,17 +190,19 @@
         ----------
         lmd : float
             Hyperparameter associated with the variance
         """
         self.lmd = lmd
         self.has_variance = True
 
-    def design(self, **kwargs):
+    def design(self, verbose=True, **kwargs):
         """Optimize the portfolio.
 
         Parameters
         ----------
+        verbose : boolean
+            Whether to print the optimization process.
         kwargs : dict
-            Dictionary of parameters to be passed to SuccessiveConvexOptimizer.
+            Dictionary of parameters to be passed to SuccessiveConvexOptimizer().
         """
         self.sca = SuccessiveConvexOptimizer(self, **kwargs)
-        self.sca.solve()
+        self.sca.solve(verbose)
```

### Comparing `riskparityportfolio-0.5.1/src/riskparityportfolio/vanilla.cpp` & `riskparityportfolio-0.6.0/src/riskparityportfolio/vanilla.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/src/riskparityportfolio/vanilla.h` & `riskparityportfolio-0.6.0/src/riskparityportfolio/vanilla.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/.hgtags` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/.hgtags`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/COPYING.BSD` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/COPYING.BSD`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/COPYING.GPL` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/COPYING.GPL`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/COPYING.LGPL` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/COPYING.LGPL`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/COPYING.MINPACK` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/COPYING.MINPACK`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/COPYING.MPL2` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/COPYING.MPL2`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/COPYING.README` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/COPYING.README`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/CTestConfig.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/CTestConfig.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/Cholesky` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/CholmodSupport` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/Core` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/Core`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/Eigenvalues` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/Geometry` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/Householder` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/IterativeLinearSolvers` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/Jacobi` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/LU` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/LU`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/MetisSupport` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/OrderingMethods` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/PaStiXSupport` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/PardisoSupport` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/QR` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/QR`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/QtAlignedMalloc` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/SPQRSupport` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/SVD` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/Sparse` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/SparseCholesky` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/SparseCore` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/SparseLU` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/SparseQR` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/StdDeque` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/StdList` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/StdVector` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/SuperLUSupport` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/UmfPackSupport` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Cholesky/LDLT.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Cholesky/LLT.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Cholesky/LLT_LAPACKE.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/CholmodSupport/CholmodSupport.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Array.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/ArrayBase.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/ArrayWrapper.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Assign.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/AssignEvaluator.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Assign_MKL.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/BandMatrix.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Block.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/BooleanRedux.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/CommaInitializer.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/ConditionEstimator.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/CoreEvaluators.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/CoreIterators.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/CwiseBinaryOp.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/CwiseNullaryOp.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/CwiseTernaryOp.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/CwiseUnaryOp.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/CwiseUnaryView.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/DenseBase.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/DenseCoeffsBase.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/DenseStorage.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Diagonal.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/DiagonalMatrix.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/DiagonalProduct.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Dot.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/EigenBase.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/ForceAlignedAccess.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Fuzzy.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/GeneralProduct.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/GenericPacketMath.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/GlobalFunctions.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/IO.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Inverse.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Map.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/MapBase.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/MathFunctions.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/MathFunctionsImpl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Matrix.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/MatrixBase.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/NestByValue.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/NoAlias.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/NumTraits.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/PermutationMatrix.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/PlainObjectBase.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Product.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/ProductEvaluators.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Random.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Redux.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Ref.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Replicate.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/ReturnByValue.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Reverse.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Select.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/SelfAdjointView.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/SelfCwiseBinaryOp.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Solve.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/SolveTriangular.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/SolverBase.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/StableNorm.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Stride.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Swap.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Transpose.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Transpositions.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/TriangularMatrix.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/VectorBlock.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/VectorwiseOp.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/Visitor.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/Complex.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/MathFunctions.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/PacketMath.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/TypeCasting.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX512/PacketMath.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AltiVec/Complex.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/Complex.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/Half.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/Half.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/MathFunctions.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/PacketMath.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/PacketMathHalf.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/PacketMathHalf.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/TypeCasting.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/CUDA/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/Default/ConjHelper.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/Default/Settings.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/NEON/Complex.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/NEON/MathFunctions.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/NEON/PacketMath.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/Complex.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/MathFunctions.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/PacketMath.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/TypeCasting.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/ZVector/Complex.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/arch/ZVector/PacketMath.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/functors/AssignmentFunctors.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/functors/BinaryFunctors.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/functors/NullaryFunctors.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/functors/StlFunctors.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/functors/TernaryFunctors.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/functors/UnaryFunctors.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixVector.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/Parallelizer.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointProduct.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointRank2Update.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularMatrixVector.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularSolverMatrix.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularSolverVector.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/BlasUtil.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/Constants.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/DisableStupidWarnings.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/ForwardDeclarations.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/MKL_support.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/Macros.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/Memory.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/Meta.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/ReenableStupidWarnings.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/StaticAssert.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Core/util/XprHelper.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/ComplexSchur.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/EigenSolver.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/RealQZ.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/RealSchur.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/Tridiagonalization.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/AlignedBox.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/AngleAxis.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/EulerAngles.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/Homogeneous.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/Hyperplane.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/OrthoMethods.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/ParametrizedLine.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/Quaternion.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/Rotation2D.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/RotationBase.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/Scaling.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/Transform.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/Translation.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/Umeyama.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Geometry/arch/Geometry_SSE.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Geometry/arch/Geometry_SSE.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Householder/BlockHouseholder.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Householder/Householder.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Householder/HouseholderSequence.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/Jacobi/Jacobi.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/LU/Determinant.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/LU/FullPivLU.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/LU/InverseImpl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/LU/PartialPivLU.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/LU/arch/Inverse_SSE.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/LU/arch/Inverse_SSE.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/MetisSupport/MetisSupport.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/OrderingMethods/Amd.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/OrderingMethods/Ordering.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/PardisoSupport/PardisoSupport.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/QR/ColPivHouseholderQR.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/QR/FullPivHouseholderQR.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/QR/HouseholderQR.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SVD/BDCSVD.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SVD/JacobiSVD.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SVD/SVDBase.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SVD/UpperBidiagonalization.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/AmbiVector.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/CompressedStorage.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/MappedSparseMatrix.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseAssign.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseBlock.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseColEtree.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseCompressedBase.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseDenseProduct.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseDot.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseFuzzy.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseMap.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseMatrix.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseMatrixBase.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparsePermutation.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseProduct.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseRedux.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseRef.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseSolverBase.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseTranspose.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseTriangularView.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseUtil.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseVector.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseView.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseCore/TriangularSolver.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLUImpl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_Memory.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_Structs.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_Utils.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_pivotL.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_pruneL.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SparseQR/SparseQR.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/StlSupport/StdDeque.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/StlSupport/StdList.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/StlSupport/StdVector.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/StlSupport/details.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/misc/Image.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/misc/Kernel.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/misc/RealSvd2x2.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/misc/blas.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/misc/lapack.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/misc/lapacke.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/plugins/BlockMethods.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/INSTALL` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/INSTALL`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/BenchSparseUtil.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/BenchSparseUtil.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/BenchTimer.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/BenchTimer.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/BenchUtil.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/BenchUtil.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/README.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/README.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/analyze-blocking-sizes.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/analyze-blocking-sizes.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/basicbench.cxxlist` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/basicbench.cxxlist`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/basicbenchmark.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/basicbenchmark.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/basicbenchmark.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/basicbenchmark.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchBlasGemm.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchBlasGemm.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchCholesky.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchCholesky.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchEigenSolver.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchEigenSolver.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchFFT.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchFFT.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchGeometry.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchGeometry.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchVecAdd.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchVecAdd.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/bench_gemm.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/bench_gemm.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/bench_multi_compilers.sh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/bench_multi_compilers.sh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/bench_norm.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/bench_norm.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/bench_reverse.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/bench_reverse.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/bench_unrolling` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/bench_unrolling`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchmark-blocking-sizes.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchmark-blocking-sizes.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchmark.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchmark.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchmarkSlice.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchmarkSlice.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchmarkX.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchmarkX.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchmarkXcwise.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchmarkXcwise.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/benchmark_suite` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/benchmark_suite`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/COPYING` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/COPYING`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/README` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/README`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_aat_product.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_aat_product.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_ata_product.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_ata_product.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_atv_product.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_atv_product.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_axpby.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_axpby.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_axpy.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_axpy.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_cholesky.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_cholesky.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_ger.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_ger.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_hessenberg.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_hessenberg.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_lu_decomp.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_lu_decomp.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_lu_solve.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_lu_solve.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_matrix_matrix_product.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_matrix_matrix_product.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_matrix_matrix_product_bis.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_matrix_matrix_product_bis.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_matrix_vector_product.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_matrix_vector_product.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_partial_lu.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_partial_lu.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_rot.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_rot.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_symv.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_symv.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_syr2.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_syr2.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_trisolve.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_trisolve.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_trisolve_matrix.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_trisolve_matrix.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/actions/action_trmm.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/actions/action_trmm.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindACML.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindACML.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindATLAS.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindATLAS.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindBLAZE.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindBLAZE.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindBlitz.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindBlitz.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindCBLAS.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindCBLAS.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindMKL.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindMKL.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindMTL4.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindMTL4.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindOPENBLAS.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindOPENBLAS.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindPackageHandleStandardArgs.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/FindTvmet.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/FindTvmet.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/action_settings.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/action_settings.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/gnuplot_common_settings.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/gnuplot_common_settings.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/go_mean` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/go_mean`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/mean.cxx` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/mean.cxx`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/mk_gnuplot_script.sh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/mk_gnuplot_script.sh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/mk_mean_script.sh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/mk_mean_script.sh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/mk_new_gnuplot.sh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/mk_new_gnuplot.sh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/perlib_plot_settings.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/perlib_plot_settings.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/regularize.cxx` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/regularize.cxx`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/smooth.cxx` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/smooth.cxx`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/data/smooth_all.sh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/data/smooth_all.sh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/bench.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/bench.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/bench_parameter.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/bench_parameter.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/btl.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/btl.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/init/init_function.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/init/init_function.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/init/init_matrix.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/init/init_matrix.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/init/init_vector.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/init/init_vector.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/static/bench_static.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/static/bench_static.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/static/intel_bench_fixed_size.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/static/intel_bench_fixed_size.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/static/static_size_generator.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/static/static_size_generator.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/STL_perf_analyzer.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/STL_perf_analyzer.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/STL_timer.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/STL_timer.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/portable_perf_analyzer.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/portable_perf_analyzer.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/portable_timer.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/portable_timer.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/x86_perf_analyzer.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/x86_perf_analyzer.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/x86_timer.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/timers/x86_timer.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/size_lin_log.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/size_lin_log.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/size_log.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/size_log.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/utilities.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/utilities.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/xy_file.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/generic_bench/utils/xy_file.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/BLAS/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/BLAS/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/BLAS/blas.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/BLAS/blas.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/BLAS/blas_interface.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/BLAS/blas_interface.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/BLAS/blas_interface_impl.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/BLAS/blas_interface_impl.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/BLAS/c_interface_base.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/BLAS/c_interface_base.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/BLAS/main.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/BLAS/main.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/STL/STL_interface.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/STL/STL_interface.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/STL/main.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/STL/main.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blaze/blaze_interface.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blaze/blaze_interface.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blaze/main.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blaze/main.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blitz/blitz_LU_solve_interface.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blitz/blitz_LU_solve_interface.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blitz/blitz_interface.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blitz/blitz_interface.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blitz/btl_blitz.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blitz/btl_blitz.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blitz/btl_tiny_blitz.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blitz/btl_tiny_blitz.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/blitz/tiny_blitz_interface.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/blitz/tiny_blitz_interface.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen2/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen2/eigen2_interface.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen2/eigen2_interface.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen2/main_adv.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen2/main_adv.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen2/main_linear.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen2/main_linear.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen2/main_matmat.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen2/main_matmat.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen2/main_vecmat.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen2/main_vecmat.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen3/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen3/eigen3_interface.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen3/eigen3_interface.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen3/main_adv.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen3/main_adv.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen3/main_linear.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen3/main_linear.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen3/main_matmat.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen3/main_matmat.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/eigen3/main_vecmat.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/eigen3/main_vecmat.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/gmm/gmm_LU_solve_interface.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/gmm/gmm_LU_solve_interface.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/gmm/gmm_interface.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/gmm/gmm_interface.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/gmm/main.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/gmm/main.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/mtl4/main.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/mtl4/main.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/mtl4/mtl4_interface.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/mtl4/mtl4_interface.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tensors/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tensors/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tensors/main_linear.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tensors/main_linear.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tensors/main_matmat.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tensors/main_matmat.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tensors/main_vecmat.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tensors/main_vecmat.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tensors/tensor_interface.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tensors/tensor_interface.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tvmet/main.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tvmet/main.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/tvmet/tvmet_interface.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/tvmet/tvmet_interface.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/ublas/main.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/ublas/main.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/btl/libs/ublas/ublas_interface.hh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/btl/libs/ublas/ublas_interface.hh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/check_cache_queries.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/check_cache_queries.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/dense_solvers.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/dense_solvers.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/eig33.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/eig33.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/geometry.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/geometry.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/changesets.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/changesets.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/gemm.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/gemm.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/lazy_gemm.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/lazy_gemm.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/make_plot.sh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/make_plot.sh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/run.sh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/perf_monitoring/gemm/run.sh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/product_threshold.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/product_threshold.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/quat_slerp.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/quat_slerp.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/quatmul.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/quatmul.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/sparse_cholesky.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/sparse_cholesky.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/sparse_dense_product.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/sparse_dense_product.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/sparse_lu.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/sparse_lu.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/sparse_product.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/sparse_product.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/sparse_randomsetter.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/sparse_randomsetter.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/sparse_setter.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/sparse_setter.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/sparse_transpose.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/sparse_transpose.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/sparse_trisolver.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/sparse_trisolver.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spbench/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spbench/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spbench/sp_solver.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spbench/sp_solver.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spbench/spbench.dtd` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spbench/spbench.dtd`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spbench/spbenchsolver.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spbench/spbenchsolver.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spbench/spbenchsolver.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spbench/spbenchsolver.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spbench/spbenchstyle.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spbench/spbenchstyle.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spbench/test_sparseLU.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spbench/test_sparseLU.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/spmv.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/spmv.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/README` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/README`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/benchmark.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/benchmark.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/benchmark_main.cc` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/benchmark_main.cc`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/contraction_benchmarks_cpu.cc` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/contraction_benchmarks_cpu.cc`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks_cpu.cc` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks_cpu.cc`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks_fp16_gpu.cu` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks_fp16_gpu.cu`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks_gpu.cu` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks_gpu.cu`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks_sycl.cc` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/tensors/tensor_benchmarks_sycl.cc`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/bench/vdw_new.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/bench/vdw_new.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/BandTriangularSolver.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/BandTriangularSolver.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/GeneralRank1Update.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/GeneralRank1Update.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/PackedSelfadjointProduct.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/PackedSelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/PackedTriangularMatrixVector.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/PackedTriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/PackedTriangularSolverVector.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/PackedTriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/Rank2Update.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/Rank2Update.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/common.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/common.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/complex_double.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/complex_double.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/complex_single.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/complex_single.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/double.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/double.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/chbmv.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/chbmv.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/chpmv.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/chpmv.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/complexdots.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/complexdots.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/ctbmv.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/ctbmv.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/datatypes.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/datatypes.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/drotm.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/drotm.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/drotmg.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/drotmg.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/dsbmv.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/dsbmv.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/dspmv.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/dspmv.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/dtbmv.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/dtbmv.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/lsame.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/lsame.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/srotm.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/srotm.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/srotmg.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/srotmg.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/ssbmv.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/ssbmv.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/sspmv.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/sspmv.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/stbmv.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/stbmv.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/zhbmv.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/zhbmv.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/zhpmv.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/zhpmv.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/f2c/ztbmv.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/f2c/ztbmv.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/fortran/complexdots.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/fortran/complexdots.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/level1_cplx_impl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/level1_cplx_impl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/level1_impl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/level1_impl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/level1_real_impl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/level1_real_impl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/level2_cplx_impl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/level2_cplx_impl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/level2_impl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/level2_impl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/level2_real_impl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/level2_real_impl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/level3_impl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/level3_impl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/single.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/single.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/cblat1.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/cblat1.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/cblat2.dat` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/cblat2.dat`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/cblat2.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/cblat2.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/cblat3.dat` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/cblat3.dat`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/cblat3.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/cblat3.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/dblat1.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/dblat1.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/dblat2.dat` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/dblat2.dat`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/dblat2.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/dblat2.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/dblat3.dat` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/dblat3.dat`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/dblat3.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/dblat3.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/runblastest.sh` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/runblastest.sh`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/sblat1.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/sblat1.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/sblat2.dat` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/sblat2.dat`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/sblat2.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/sblat2.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/sblat3.dat` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/sblat3.dat`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/sblat3.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/sblat3.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/zblat1.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/zblat1.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/zblat2.dat` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/zblat2.dat`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/zblat2.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/zblat2.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/zblat3.dat` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/zblat3.dat`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/blas/testing/zblat3.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/blas/testing/zblat3.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/Eigen3Config.cmake.in` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/Eigen3Config.cmake.in`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/Eigen3ConfigLegacy.cmake.in` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/Eigen3ConfigLegacy.cmake.in`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/EigenConfigureTesting.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/EigenConfigureTesting.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/EigenDetermineOSVersion.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/EigenDetermineOSVersion.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/EigenDetermineVSServicePack.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/EigenDetermineVSServicePack.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/EigenTesting.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/EigenTesting.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/EigenUninstall.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/EigenUninstall.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindBLAS.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindBLAS.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindBLASEXT.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindBLASEXT.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindCholmod.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindCholmod.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindComputeCpp.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindComputeCpp.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindEigen2.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindEigen2.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindEigen3.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindFFTW.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindFFTW.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindGLEW.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindGLEW.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindGMP.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindGMP.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindGSL.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindGSL.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindGoogleHash.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindGoogleHash.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindHWLOC.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindHWLOC.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindLAPACK.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindLAPACK.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindMPFR.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindMPFR.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindMetis.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindMetis.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindPTSCOTCH.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindPTSCOTCH.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindPastix.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindPastix.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindSPQR.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindSPQR.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindScotch.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindScotch.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindStandardMathLibrary.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindStandardMathLibrary.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindSuperLU.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindSuperLU.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/FindUmfpack.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/FindUmfpack.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/RegexUtils.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/RegexUtils.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/cmake/language_support.cmake` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/cmake/language_support.cmake`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/debug/gdb/printers.py` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/debug/gdb/printers.py`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/debug/msvc/eigen.natvis` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/debug/msvc/eigen.natvis`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/debug/msvc/eigen_autoexp_part.dat` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/debug/msvc/eigen_autoexp_part.dat`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/mandelbrot/mandelbrot.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/mandelbrot/mandelbrot.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/mandelbrot/mandelbrot.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/mandelbrot/mandelbrot.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/mix_eigen_and_c/binary_library.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/mix_eigen_and_c/binary_library.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/mix_eigen_and_c/binary_library.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/mix_eigen_and_c/binary_library.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/mix_eigen_and_c/example.c` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/mix_eigen_and_c/example.c`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/camera.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/camera.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/camera.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/camera.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/gpuhelper.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/gpuhelper.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/gpuhelper.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/gpuhelper.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/icosphere.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/icosphere.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/icosphere.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/icosphere.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/quaternion_demo.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/quaternion_demo.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/quaternion_demo.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/quaternion_demo.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/trackball.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/trackball.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/demos/opengl/trackball.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/demos/opengl/trackball.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/A05_PortingFrom2To3.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/A05_PortingFrom2To3.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/AsciiQuickReference.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/AsciiQuickReference.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/B01_Experimental.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/B01_Experimental.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/ClassHierarchy.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/ClassHierarchy.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/CoeffwiseMathFunctionsTable.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/CoeffwiseMathFunctionsTable.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/CustomizingEigen_CustomScalar.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/CustomizingEigen_CustomScalar.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/CustomizingEigen_InheritingMatrix.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/CustomizingEigen_InheritingMatrix.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/CustomizingEigen_NullaryExpr.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/CustomizingEigen_NullaryExpr.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/CustomizingEigen_Plugins.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/CustomizingEigen_Plugins.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/DenseDecompositionBenchmark.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/DenseDecompositionBenchmark.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/Doxyfile.in` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/Eigen_Silly_Professor_64x64.png` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/Eigen_Silly_Professor_64x64.png`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/FixedSizeVectorizable.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/FixedSizeVectorizable.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/FunctionsTakingEigenTypes.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/FunctionsTakingEigenTypes.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/HiPerformance.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/HiPerformance.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/InplaceDecomposition.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/InplaceDecomposition.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/InsideEigenExample.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/InsideEigenExample.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/LeastSquares.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/LeastSquares.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/Manual.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/Manual.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/MatrixfreeSolverExample.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/MatrixfreeSolverExample.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/NewExpressionType.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/NewExpressionType.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/Overview.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/Overview.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/PassingByValue.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/PassingByValue.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/Pitfalls.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/Pitfalls.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/PreprocessorDirectives.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/PreprocessorDirectives.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/QuickReference.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/QuickReference.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/QuickStartGuide.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/QuickStartGuide.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/SparseLinearSystems.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/SparseLinearSystems.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/SparseQuickReference.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/SparseQuickReference.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/StlContainers.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/StlContainers.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/StorageOrders.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/StorageOrders.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/StructHavingEigenMembers.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/StructHavingEigenMembers.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TemplateKeyword.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TemplateKeyword.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TopicAliasing.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TopicAliasing.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TopicAssertions.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TopicAssertions.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TopicCMakeGuide.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TopicCMakeGuide.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TopicLazyEvaluation.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TopicLazyEvaluation.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TopicLinearAlgebraDecompositions.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TopicLinearAlgebraDecompositions.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TopicMultithreading.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TopicMultithreading.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialAdvancedInitialization.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialAdvancedInitialization.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialArrayClass.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialArrayClass.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialBlockOperations.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialBlockOperations.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialGeometry.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialGeometry.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialLinearAlgebra.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialLinearAlgebra.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialMapClass.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialMapClass.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialMatrixArithmetic.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialMatrixArithmetic.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialMatrixClass.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialMatrixClass.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialReductionsVisitorsBroadcasting.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialReductionsVisitorsBroadcasting.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialReshapeSlicing.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialReshapeSlicing.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/TutorialSparse.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/TutorialSparse.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/UnalignedArrayAssert.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/UnalignedArrayAssert.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/UsingBlasLapackBackends.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/UsingBlasLapackBackends.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/UsingIntelMKL.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/UsingIntelMKL.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/UsingNVCC.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/UsingNVCC.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/WrongStackAlignment.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/WrongStackAlignment.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/eigen_navtree_hacks.js` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/eigen_navtree_hacks.js`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/eigendoxy.css` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/eigendoxy.css`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/eigendoxy_footer.html.in` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/eigendoxy_footer.html.in`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/eigendoxy_header.html.in` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/eigendoxy_header.html.in`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/eigendoxy_layout.xml.in` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/eigendoxy_layout.xml.in`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/eigendoxy_tabs.css` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/eigendoxy_tabs.css`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/CustomizingEigen_Inheritance.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/CustomizingEigen_Inheritance.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TemplateKeyword_flexible.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TemplateKeyword_flexible.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TutorialInplaceLU.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TutorialInplaceLU.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgComputeTwice.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgComputeTwice.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgRankRevealing.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgRankRevealing.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_BlockOperations_block_assignment.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_BlockOperations_block_assignment.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/Tutorial_simple_example_dynamic_size.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/Tutorial_simple_example_dynamic_size.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/class_Block.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/class_Block.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/class_CwiseBinaryOp.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/class_CwiseBinaryOp.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/class_CwiseUnaryOp.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/class_CwiseUnaryOp.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/class_FixedBlock.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/class_FixedBlock.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/class_FixedVectorBlock.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/class_FixedVectorBlock.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/class_VectorBlock.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/class_VectorBlock.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/function_taking_ref.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/function_taking_ref.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.evaluator` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.evaluator`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.expression` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.expression`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.traits` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/make_circulant.cpp.traits`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/make_circulant2.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/make_circulant2.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/matrixfree_cg.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/matrixfree_cg.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/nullary_indexing.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/nullary_indexing.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/tut_arithmetic_matrix_mul.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/tut_arithmetic_matrix_mul.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/examples/tut_arithmetic_redux_basic.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/examples/tut_arithmetic_redux_basic.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/ComplexEigenSolver_compute.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/ComplexEigenSolver_compute.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/HouseholderSequence_HouseholderSequence.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/HouseholderSequence_HouseholderSequence.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/IOFormat.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/IOFormat.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/JacobiSVD_basic.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/JacobiSVD_basic.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/LLT_example.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/LLT_example.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_all.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_all.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/MatrixBase_triangularView.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/MatrixBase_triangularView.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/RealQZ_compute.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/RealQZ_compute.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_cwise.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/TopicAliasing_cwise.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/TopicStorageOrders_example.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/TopicStorageOrders_example.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Triangular_solve.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Triangular_solve.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tridiagonalization_diagonal.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tridiagonalization_diagonal.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_Map_using.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_Map_using.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Tutorial_SlicingCol.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Tutorial_SlicingCol.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/Vectorwise_reverse.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/Vectorwise_reverse.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/snippets/class_FullPivLU.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/snippets/class_FullPivLU.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/special_examples/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/special_examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/special_examples/Tutorial_sparse_example.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/special_examples/Tutorial_sparse_example.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/special_examples/Tutorial_sparse_example_details.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/special_examples/Tutorial_sparse_example_details.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/doc/tutorial.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/doc/tutorial.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/failtest/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/failtest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/cholesky.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/cholesky.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/clacgv.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/clacgv.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/cladiv.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/cladiv.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/clarf.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/clarf.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/clarfb.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/clarfb.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/clarfg.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/clarfg.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/clarft.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/clarft.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/complex_double.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/complex_double.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/complex_single.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/complex_single.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dladiv.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dladiv.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dlamch.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dlamch.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dlapy2.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dlapy2.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dlapy3.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dlapy3.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dlarf.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dlarf.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dlarfb.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dlarfb.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dlarfg.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dlarfg.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dlarft.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dlarft.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/double.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/double.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/dsecnd_NONE.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/dsecnd_NONE.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/eigenvalues.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/eigenvalues.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/ilaclc.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/ilaclc.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/ilaclr.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/ilaclr.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/iladlc.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/iladlc.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/iladlr.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/iladlr.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/ilaslc.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/ilaslc.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/ilaslr.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/ilaslr.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/ilazlc.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/ilazlc.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/ilazlr.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/ilazlr.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/lapack_common.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/lapack_common.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/lu.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/lu.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/second_NONE.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/second_NONE.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/single.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/single.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/sladiv.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/sladiv.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/slamch.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/slamch.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/slapy2.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/slapy2.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/slapy3.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/slapy3.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/slarf.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/slarf.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/slarfb.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/slarfb.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/slarfg.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/slarfg.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/slarft.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/slarft.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/svd.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/svd.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/zlacgv.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/zlacgv.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/zladiv.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/zladiv.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/zlarf.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/zlarf.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/zlarfb.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/zlarfb.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/zlarfg.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/zlarfg.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/lapack/zlarft.f` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/lapack/zlarft.f`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/scripts/buildtests.in` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/scripts/buildtests.in`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/scripts/cdashtesting.cmake.in` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/scripts/cdashtesting.cmake.in`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/scripts/check.in` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/scripts/check.in`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/scripts/eigen_gen_credits.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/scripts/eigen_gen_credits.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/scripts/eigen_gen_docs` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/scripts/eigen_gen_docs`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/scripts/relicense.py` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/scripts/relicense.py`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/adjoint.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/adjoint.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/array.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/array.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/array_for_matrix.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/array_for_matrix.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/array_of_string.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/array_of_string.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/array_replicate.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/array_replicate.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/array_reverse.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/array_reverse.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/bandmatrix.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/bandmatrix.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/basicstuff.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/basicstuff.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/bdcsvd.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/bdcsvd.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/bicgstab.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/bicgstab.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/block.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/block.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/boostmultiprec.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/boostmultiprec.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/cholesky.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/cholesky.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/cholmod_support.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/cholmod_support.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/commainitializer.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/commainitializer.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/conjugate_gradient.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/conjugate_gradient.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/conservative_resize.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/conservative_resize.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/constructor.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/constructor.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/corners.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/corners.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/ctorleak.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/ctorleak.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/cuda_basic.cu` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/cuda_basic.cu`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/cuda_common.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/cuda_common.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/denseLM.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/denseLM.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/dense_storage.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/dense_storage.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/determinant.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/determinant.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/diagonal.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/diagonal.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/diagonalmatrices.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/diagonalmatrices.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/dontalign.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/dontalign.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/dynalloc.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/dynalloc.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/eigen2support.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/eigen2support.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/eigensolver_complex.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/eigensolver_complex.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/eigensolver_generalized_real.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/eigensolver_generalized_real.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/eigensolver_generic.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/eigensolver_generic.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/eigensolver_selfadjoint.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/eigensolver_selfadjoint.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/evaluators.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/evaluators.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/exceptions.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/exceptions.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/fastmath.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/fastmath.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/first_aligned.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/first_aligned.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/geo_alignedbox.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/geo_alignedbox.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/geo_eulerangles.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/geo_eulerangles.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/geo_homogeneous.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/geo_homogeneous.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/geo_hyperplane.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/geo_hyperplane.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/geo_orthomethods.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/geo_orthomethods.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/geo_parametrizedline.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/geo_parametrizedline.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/geo_quaternion.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/geo_quaternion.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/geo_transformations.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/geo_transformations.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/half_float.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/half_float.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/hessenberg.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/hessenberg.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/householder.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/householder.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/incomplete_cholesky.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/incomplete_cholesky.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/inplace_decomposition.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/inplace_decomposition.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/integer_types.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/integer_types.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/inverse.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/inverse.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/is_same_dense.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/is_same_dense.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/jacobi.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/jacobi.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/jacobisvd.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/jacobisvd.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/linearstructure.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/linearstructure.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/lscg.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/lscg.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/lu.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/lu.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/main.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/main.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/mapped_matrix.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/mapped_matrix.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/mapstaticmethods.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/mapstaticmethods.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/mapstride.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/mapstride.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/meta.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/meta.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/metis_support.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/metis_support.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/miscmatrices.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/miscmatrices.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/mixingtypes.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/mixingtypes.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/mpl2only.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/mpl2only.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/nesting_ops.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/nesting_ops.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/nomalloc.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/nomalloc.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/nullary.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/nullary.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/numext.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/numext.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/packetmath.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/packetmath.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/pardiso_support.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/pardiso_support.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/pastix_support.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/pastix_support.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/permutationmatrices.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/permutationmatrices.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/prec_inverse_4x4.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/prec_inverse_4x4.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_extra.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_extra.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_large.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_large.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_mmtr.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_mmtr.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_notemporary.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_notemporary.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_selfadjoint.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_selfadjoint.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_small.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_small.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_symm.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_symm.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_syrk.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_syrk.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_trmm.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_trmm.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_trmv.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_trmv.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/product_trsolve.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/product_trsolve.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/qr.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/qr.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/qr_colpivoting.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/qr_colpivoting.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/qr_fullpivoting.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/qr_fullpivoting.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/qtvector.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/qtvector.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/rand.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/rand.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/real_qz.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/real_qz.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/redux.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/redux.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/ref.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/ref.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/resize.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/resize.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/rvalue_types.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/rvalue_types.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/schur_complex.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/schur_complex.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/schur_real.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/schur_real.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/selfadjoint.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/selfadjoint.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/simplicial_cholesky.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/simplicial_cholesky.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sizeof.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sizeof.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sizeoverflow.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sizeoverflow.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/smallvectors.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/smallvectors.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparseLM.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparseLM.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse_basic.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse_basic.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse_block.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse_block.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse_permutations.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse_permutations.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse_product.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse_product.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse_ref.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse_ref.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse_solver.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse_solver.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse_solvers.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse_solvers.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparse_vector.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparse_vector.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparselu.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparselu.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/sparseqr.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/sparseqr.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/special_numbers.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/special_numbers.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/spqr_support.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/spqr_support.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/stable_norm.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/stable_norm.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/stddeque.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/stddeque.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/stddeque_overload.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/stddeque_overload.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/stdlist.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/stdlist.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/stdlist_overload.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/stdlist_overload.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/stdvector.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/stdvector.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/stdvector_overload.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/stdvector_overload.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/superlu_support.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/superlu_support.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/svd_common.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/svd_common.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/svd_fill.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/svd_fill.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/swap.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/swap.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/triangular.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/triangular.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/umeyama.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/umeyama.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/umfpack_support.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/umfpack_support.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/unalignedassert.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/unalignedassert.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/unalignedcount.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/unalignedcount.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/upperbidiagonalization.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/upperbidiagonalization.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/vectorization_logic.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/vectorization_logic.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/vectorwiseop.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/vectorwiseop.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/visitor.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/visitor.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/test/zerosized.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/test/zerosized.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/AdolcForward` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/AdolcForward`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/AlignedVector3` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/AlignedVector3`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/ArpackSupport` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/ArpackSupport`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/AutoDiff` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/AutoDiff`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/BVH` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/BVH`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/Tensor` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/Tensor`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/TensorSymmetry` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/TensorSymmetry`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/ThreadPool` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/ThreadPool`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/README.md` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/README.md`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/Tensor.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/Tensor.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSycl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSycl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclConvertToDeviceExpression.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclConvertToDeviceExpression.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExprConstructor.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExprConstructor.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractAccessor.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractAccessor.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractFunctors.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractFunctors.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclLeafCount.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclLeafCount.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclPlaceHolderExpr.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclPlaceHolderExpr.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclRun.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclRun.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclTuple.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorSyclTuple.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/SimpleThreadPool.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/SimpleThreadPool.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/CXX11Meta.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/CXX11Meta.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/EmulateArray.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/EmulateArray.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/EmulateCXX11Meta.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/EmulateCXX11Meta.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/EulerAngles` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/EulerAngles`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/FFT` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/FFT`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/IterativeSolvers` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/IterativeSolvers`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/KroneckerProduct` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/KroneckerProduct`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/LevenbergMarquardt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/LevenbergMarquardt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/MPRealSupport` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/MPRealSupport`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/MatrixFunctions` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/MatrixFunctions`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/MoreVectorization` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/MoreVectorization`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/NonLinearOptimization` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/NonLinearOptimization`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/NumericalDiff` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/NumericalDiff`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/OpenGLSupport` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/OpenGLSupport`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/Polynomials` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/Polynomials`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/Skyline` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/Skyline`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/SparseExtra` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/SparseExtra`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/SpecialFunctions` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/SpecialFunctions`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/Splines` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/Splines`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/BVH/BVAlgorithms.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/BVH/BVAlgorithms.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/BVH/KdBVH.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/BVH/KdBVH.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/EulerAngles/EulerAngles.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/EulerAngles/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/EulerAngles/EulerSystem.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/EulerAngles/EulerSystem.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/FFT/ei_fftw_impl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/FFT/ei_fftw_impl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/FFT/ei_kissfft_impl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/FFT/ei_kissfft_impl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/DGMRES.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/DGMRES.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/GMRES.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/GMRES.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/IterationController.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/IterationController.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/MINRES.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/MINRES.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/Scaling.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/IterativeSolvers/Scaling.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/StemFunction.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/MatrixFunctions/StemFunction.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/MoreVectorization/MathFunctions.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/MoreVectorization/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/chkder.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/chkder.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/covar.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/covar.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/dogleg.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/dogleg.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/lmpar.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/lmpar.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/r1updt.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/r1updt.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Polynomials/Companion.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Polynomials/Companion.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Polynomials/PolynomialSolver.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Polynomials/PolynomialSolver.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Polynomials/PolynomialUtils.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Polynomials/PolynomialUtils.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineMatrix.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineMatrix.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineProduct.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineProduct.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineStorage.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineStorage.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineUtil.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Skyline/SkylineUtil.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/MarketIO.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/MarketIO.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/RandomSetter.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SparseExtra/RandomSetter.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/arch/CUDA/CudaSpecialFunctions.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/SpecialFunctions/arch/CUDA/CudaSpecialFunctions.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Splines/Spline.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Splines/Spline.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Splines/SplineFitting.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Splines/SplineFitting.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/Eigen/src/Splines/SplineFwd.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/Eigen/src/Splines/SplineFwd.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/README.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/README.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/bench/bench_svd.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/bench/bench_svd.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/Overview.dox` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/Overview.dox`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/eigendoxy_layout.xml.in` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/eigendoxy_layout.xml.in`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/BVH_Example.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/BVH_Example.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/EulerAngles.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/EulerAngles.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/FFT.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/FFT.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixSinh.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/MatrixSinh.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/PolynomialSolver1.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/PolynomialSolver1.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/examples/PolynomialUtils1.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/examples/PolynomialUtils1.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/doc/snippets/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/doc/snippets/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/BVH.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/BVH.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/CMakeLists.txt` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/EulerAngles.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/EulerAngles.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/FFTW.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/FFTW.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/NonLinearOptimization.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/NonLinearOptimization.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/NumericalDiff.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/NumericalDiff.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/alignedvector3.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/alignedvector3.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/autodiff.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/autodiff.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/autodiff_scalar.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/autodiff_scalar.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_eventcount.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_eventcount.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_meta.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_meta.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_non_blocking_thread_pool.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_non_blocking_thread_pool.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_runqueue.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_runqueue.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_argmax.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_argmax.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_argmax_cuda.cu` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_argmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_assign.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_assign.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_broadcast_sycl.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_broadcast_sycl.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_broadcasting.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_broadcasting.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_cast_float16_cuda.cu` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_cast_float16_cuda.cu`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_casts.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_casts.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_chipping.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_chipping.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_comparisons.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_comparisons.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_complex_cuda.cu` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_complex_cuda.cu`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_complex_cwise_ops_cuda.cu` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_complex_cwise_ops_cuda.cu`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_concatenation.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_concatenation.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_const.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_const.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_contract_cuda.cu` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_contract_cuda.cu`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_contraction.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_contraction.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_convolution.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_convolution.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_cuda.cu` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_cuda.cu`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_custom_index.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_custom_index.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_custom_op.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_custom_op.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_device.cu` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_device.cu`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_device_sycl.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_device_sycl.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_dimension.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_dimension.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_empty.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_empty.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_expr.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_expr.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_fft.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_fft.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_fixed_size.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_fixed_size.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_forced_eval.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_forced_eval.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_generator.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_generator.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_ifft.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_ifft.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_image_patch.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_image_patch.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_index_list.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_index_list.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_inflation.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_inflation.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_intdiv.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_intdiv.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_io.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_io.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_layout_swap.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_layout_swap.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_lvalue.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_lvalue.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_map.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_map.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_math.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_math.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_mixed_indices.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_mixed_indices.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_morphing.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_morphing.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_notification.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_notification.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_of_complex.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_of_complex.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_of_const_values.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_of_const_values.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_of_float16_cuda.cu` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_of_float16_cuda.cu`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_of_strings.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_of_strings.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_padding.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_padding.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_patch.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_patch.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_random.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_random.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_random_cuda.cu` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_random_cuda.cu`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_reduction.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_reduction.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_reduction_cuda.cu` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_reduction_cuda.cu`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_reduction_sycl.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_reduction_sycl.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_ref.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_ref.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_reverse.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_reverse.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_roundings.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_roundings.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_scan.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_scan.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_scan_cuda.cu` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_scan_cuda.cu`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_shuffling.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_shuffling.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_simple.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_simple.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_striding.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_striding.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_sugar.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_sugar.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_sycl.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_sycl.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_symmetry.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_symmetry.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_thread_pool.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_thread_pool.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_uint128.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_uint128.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_volume_patch.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/cxx11_tensor_volume_patch.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/dgmres.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/dgmres.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/forward_adolc.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/forward_adolc.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/gmres.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/gmres.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/kronecker_product.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/kronecker_product.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/levenberg_marquardt.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/levenberg_marquardt.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/matrix_exponential.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/matrix_exponential.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/matrix_function.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/matrix_function.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/matrix_functions.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/matrix_functions.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/matrix_power.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/matrix_power.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/matrix_square_root.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/matrix_square_root.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/minres.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/minres.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/mpreal/mpreal.h` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/mpreal/mpreal.h`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/mpreal_support.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/mpreal_support.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/openglsupport.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/openglsupport.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/polynomialsolver.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/polynomialsolver.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/polynomialutils.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/polynomialutils.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/sparse_extra.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/sparse_extra.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/special_functions.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/special_functions.cpp`

 * *Files identical despite different names*

### Comparing `riskparityportfolio-0.5.1/third-party/eigen_3.3.7/unsupported/test/splines.cpp` & `riskparityportfolio-0.6.0/third-party/eigen_3.3.7/unsupported/test/splines.cpp`

 * *Files identical despite different names*

