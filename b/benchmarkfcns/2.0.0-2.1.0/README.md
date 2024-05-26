# Comparing `tmp/benchmarkfcns-2.0.0.tar.gz` & `tmp/benchmarkfcns-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchmarkfcns-2.0.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "benchmarkfcns-2.1.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `benchmarkfcns-2.0.0.tar` & `benchmarkfcns-2.1.0.tar`

### file list

```diff
@@ -1,1938 +1,1941 @@
--rw-r--r--   0        0        0     1656 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/.github/workflows/build.yaml
--rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/.gitignore
--rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/.gitmodules
--rw-r--r--   0        0        0     1098 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1104 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/CMakeLists.txt
--rw-r--r--   0        0        0     1086 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/LICENSE
--rw-r--r--   0        0        0     2038 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/README.md
--rw-r--r--   0        0        0     7407 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/optimiser/matlab/abc/FoodSources.m
--rw-r--r--   0        0        0     6188 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/optimiser/matlab/abc/abc.m
--rw-r--r--   0        0        0     2242 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/optimiser/matlab/abc/abcoptions.m
--rw-r--r--   0        0        0    17154 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/optimiser/python/abc.py
--rw-r--r--   0        0        0     2606 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    28412 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/benchmarkfcns.cpp
--rw-r--r--   0        0        0     6040 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/benchmarkfcns.h
--rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/.git
--rw-r--r--   0        0        0      292 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/.gitignore
--rw-r--r--   0        0        0     2744 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/.gitlab/issue_templates/Bug Report.md
--rw-r--r--   0        0        0      201 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/.gitlab/issue_templates/Feature Request.md
--rw-r--r--   0        0        0     1394 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/.gitlab/merge_request_templates/Merge Request Template.md
--rw-r--r--   0        0        0      571 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/.hgeol
--rw-r--r--   0        0        0    24767 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/CMakeLists.txt
--rw-r--r--   0        0        0    11362 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/COPYING.APACHE
--rw-r--r--   0        0        0     1517 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/COPYING.BSD
--rw-r--r--   0        0        0    35147 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/COPYING.GPL
--rw-r--r--   0        0        0    26530 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/COPYING.LGPL
--rw-r--r--   0        0        0     2193 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/COPYING.MINPACK
--rw-r--r--   0        0        0    16726 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/COPYING.MPL2
--rw-r--r--   0        0        0      779 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/COPYING.README
--rw-r--r--   0        0        0      584 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/CTestConfig.cmake
--rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/CTestCustom.cmake.in
--rw-r--r--   0        0        0     1161 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/Cholesky
--rw-r--r--   0        0        0     1900 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/CholmodSupport
--rw-r--r--   0        0        0    12799 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/Core
--rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/Dense
--rw-r--r--   0        0        0       35 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/Eigen
--rw-r--r--   0        0        0     1777 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/Eigenvalues
--rw-r--r--   0        0        0     1940 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/Geometry
--rw-r--r--   0        0        0      829 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/Householder
--rw-r--r--   0        0        0     2083 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/IterativeLinearSolvers
--rw-r--r--   0        0        0      894 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/Jacobi
--rw-r--r--   0        0        0     1389 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/KLUSupport
--rw-r--r--   0        0        0     1268 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/LU
--rw-r--r--   0        0        0      991 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/MetisSupport
--rw-r--r--   0        0        0     2451 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/OrderingMethods
--rw-r--r--   0        0        0     1751 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/PaStiXSupport
--rw-r--r--   0        0        0     1116 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/PardisoSupport
--rw-r--r--   0        0        0     1272 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/QR
--rw-r--r--   0        0        0      900 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/QtAlignedMalloc
--rw-r--r--   0        0        0     1162 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/SPQRSupport
--rw-r--r--   0        0        0     1584 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/SVD
--rw-r--r--   0        0        0      888 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/Sparse
--rw-r--r--   0        0        0     1235 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/SparseCholesky
--rw-r--r--   0        0        0     2240 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/SparseCore
--rw-r--r--   0        0        0     1814 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/SparseLU
--rw-r--r--   0        0        0     1195 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/SparseQR
--rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/StdDeque
--rw-r--r--   0        0        0      726 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/StdList
--rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/StdVector
--rw-r--r--   0        0        0     2243 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/SuperLUSupport
--rw-r--r--   0        0        0     1382 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/UmfPackSupport
--rw-r--r--   0        0        0    24934 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0        0        0    18760 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0        0        0     3974 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Cholesky/LLT_LAPACKE.h
--rw-r--r--   0        0        0    25441 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/CholmodSupport/CholmodSupport.h
--rw-r--r--   0        0        0    19214 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/ArithmeticSequence.h
--rw-r--r--   0        0        0    16782 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Array.h
--rw-r--r--   0        0        0     8217 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0        0        0     7018 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0        0        0     2738 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Assign.h
--rw-r--r--   0        0        0    41673 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/AssignEvaluator.h
--rwxr-xr-x   0        0        0    12488 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0        0        0    14075 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0        0        0    18648 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Block.h
--rw-r--r--   0        0        0     4429 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0        0        0     5981 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0        0        0     6990 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0        0        0    63841 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0        0        0     4745 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0        0        0     7909 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0        0        0    36282 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0        0        0     8256 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0        0        0     3937 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0        0        0     5551 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0        0        0    31529 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/DenseBase.h
--rw-r--r--   0        0        0    24484 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0        0        0    25360 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0        0        0     9870 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Diagonal.h
--rw-r--r--   0        0        0    14670 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0        0        0      988 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0        0        0    11654 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Dot.h
--rw-r--r--   0        0        0     5841 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/EigenBase.h
--rw-r--r--   0        0        0     4909 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0        0        0     5759 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0        0        0    21679 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0        0        0    38812 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0        0        0    11543 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0        0        0     8238 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/IO.h
--rw-r--r--   0        0        0     9620 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/IndexedView.h
--rw-r--r--   0        0        0     3503 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Inverse.h
--rw-r--r--   0        0        0     7256 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Map.h
--rw-r--r--   0        0        0    11281 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/MapBase.h
--rw-r--r--   0        0        0    60784 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0        0        0     7156 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0        0        0    24343 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Matrix.h
--rw-r--r--   0        0        0    23856 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0        0        0     2520 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/NestByValue.h
--rw-r--r--   0        0        0     3620 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/NoAlias.h
--rw-r--r--   0        0        0    12884 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/NumTraits.h
--rw-r--r--   0        0        0     9207 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/PartialReduxEvaluator.h
--rw-r--r--   0        0        0    20748 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0        0        0    49193 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0        0        0     7336 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Product.h
--rw-r--r--   0        0        0    53832 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0        0        0     7756 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Random.h
--rw-r--r--   0        0        0    19195 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Redux.h
--rw-r--r--   0        0        0    17821 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Ref.h
--rw-r--r--   0        0        0     5656 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Replicate.h
--rw-r--r--   0        0        0    17033 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Reshaped.h
--rw-r--r--   0        0        0     4284 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0        0        0     7522 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Reverse.h
--rw-r--r--   0        0        0     6143 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Select.h
--rw-r--r--   0        0        0    14999 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0        0        0     1697 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0        0        0     6837 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Solve.h
--rw-r--r--   0        0        0     9368 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0        0        0     6170 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/SolverBase.h
--rw-r--r--   0        0        0     8700 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/StableNorm.h
--rw-r--r--   0        0        0    21641 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/StlIterators.h
--rw-r--r--   0        0        0     4212 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Stride.h
--rw-r--r--   0        0        0     2765 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Swap.h
--rw-r--r--   0        0        0    17606 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Transpose.h
--rw-r--r--   0        0        0    13567 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Transpositions.h
--rw-r--r--   0        0        0    38277 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0        0        0     3488 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0        0        0    35168 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0        0        0    11997 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Visitor.h
--rw-r--r--   0        0        0    15223 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0        0        0     8102 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0        0        0    64608 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0        0        0     2564 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX/TypeCasting.h
--rw-r--r--   0        0        0    17160 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX512/Complex.h
--rw-r--r--   0        0        0    13344 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0        0        0    87891 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-r--r--   0        0        0     2134 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX512/TypeCasting.h
--rw-r--r--   0        0        0    16540 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0        0        0     2323 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-r--r--   0        0        0   119355 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-r--r--   0        0        0     9490 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-r--r--   0        0        0    24820 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rwxr-xr-x   0        0        0   102394 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/PacketMath.h
--rw-r--r--   0        0        0    17317 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/CUDA/Complex.h
--rw-r--r--   0        0        0    26903 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/BFloat16.h
--rw-r--r--   0        0        0     5251 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0        0        0    67696 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-r--r--   0        0        0     3770 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-r--r--   0        0        0    35534 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/Half.h
--rw-r--r--   0        0        0     1746 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/Settings.h
--rw-r--r--   0        0        0     3746 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/TypeCasting.h
--rw-r--r--   0        0        0     2695 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-r--r--   0        0        0    57047 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-r--r--   0        0        0     2256 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/GPU/TypeCasting.h
--rw-r--r--   0        0        0      691 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/HIP/hcc/math_constants.h
--rw-r--r--   0        0        0    17541 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/MSA/Complex.h
--rw-r--r--   0        0        0    16159 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-r--r--   0        0        0    33615 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/MSA/PacketMath.h
--rw-r--r--   0        0        0    22503 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0        0        0     6815 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-r--r--   0        0        0     3083 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0        0        0   189525 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-r--r--   0        0        0    51286 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/TypeCasting.h
--rw-r--r--   0        0        0    14251 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0        0        0     6765 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxr-xr-x   0        0        0    64465 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0        0        0     3650 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SSE/TypeCasting.h
--rw-r--r--   0        0        0     1194 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-r--r--   0        0        0    21200 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-r--r--   0        0        0     1351 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SVE/TypeCasting.h
--rw-r--r--   0        0        0     7428 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-r--r--   0        0        0    12539 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-r--r--   0        0        0    27786 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-r--r--   0        0        0    21856 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-r--r--   0        0        0     2626 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/TypeCasting.h
--rw-r--r--   0        0        0    16728 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0        0        0     8024 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxr-xr-x   0        0        0    36894 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/ZVector/PacketMath.h
--rw-r--r--   0        0        0     6686 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0        0        0    20921 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0        0        0     8334 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0        0        0     4998 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0        0        0      607 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0        0        0    40146 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/UnaryFunctors.h
--rw-r--r--   0        0        0   108448 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0        0        0    20104 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0        0        0    15948 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0        0        0     6936 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0        0        0     5106 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0        0        0    21724 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0        0        0     6368 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0        0        0     5582 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0        0        0    21354 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0        0        0    11570 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0        0        0     9958 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0        0        0     5209 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0        0        0     6164 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0        0        0     4126 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0        0        0    20987 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0        0        0    13867 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0        0        0    14722 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0        0        0    10571 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0        0        0    14678 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0        0        0     6707 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0        0        0     5882 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverVector.h
--rwxr-xr-x   0        0        0    23156 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0        0        0    19876 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/ConfigureVectorization.h
--rw-r--r--   0        0        0    21931 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/Constants.h
--rwxr-xr-x   0        0        0     4892 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0        0        0    15555 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/ForwardDeclarations.h
--rw-r--r--   0        0        0     6696 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/IndexedViewHelper.h
--rw-r--r--   0        0        0    10949 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/IntegralConstant.h
--rwxr-xr-x   0        0        0     4268 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0        0        0    52909 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/Macros.h
--rw-r--r--   0        0        0    46661 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/Memory.h
--rwxr-xr-x   0        0        0    29336 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/Meta.h
--rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0        0        0     1024 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0        0        0     1432 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/ReshapedHelper.h
--rw-r--r--   0        0        0    10676 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0        0        0    12003 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/SymbolicIndex.h
--rw-r--r--   0        0        0    35762 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/XprHelper.h
--rw-r--r--   0        0        0    12559 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0        0        0    17274 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0        0        0     4178 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0        0        0    22970 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0        0        0    17176 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0        0        0     9716 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0        0        0    14349 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0        0        0     5575 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0        0        0    23640 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0        0        0    21078 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0        0        0     3650 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0        0        0    35182 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0        0        0     4104 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0        0        0    22764 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/Tridiagonalization.h
--rw-r--r--   0        0        0    18939 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0        0        0     8403 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0        0        0     3624 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0        0        0    20726 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0        0        0    11962 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0        0        0     8955 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0        0        0     9812 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0        0        0    34367 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0        0        0     6862 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0        0        0     8063 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0        0        0     6724 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0        0        0    61930 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Transform.h
--rw-r--r--   0        0        0     7664 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Translation.h
--rw-r--r--   0        0        0     6190 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Umeyama.h
--rw-r--r--   0        0        0     5945 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/arch/Geometry_SIMD.h
--rw-r--r--   0        0        0     4784 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0        0        0     5365 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Householder/Householder.h
--rw-r--r--   0        0        0    23611 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Householder/HouseholderSequence.h
--rw-r--r--   0        0        0     6771 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0        0        0     6850 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0        0        0     8887 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0        0        0    15036 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0        0        0    14940 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0        0        0    13379 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0        0        0     7349 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0        0        0     4212 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
--rw-r--r--   0        0        0    16383 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Jacobi/Jacobi.h
--rw-r--r--   0        0        0    11555 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/KLUSupport/KLUSupport.h
--rw-r--r--   0        0        0     3439 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/LU/Determinant.h
--rw-r--r--   0        0        0    32383 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0        0        0    15727 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0        0        0    22069 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0        0        0     3555 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/LU/PartialPivLU_LAPACKE.h
--rw-r--r--   0        0        0    13693 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/LU/arch/InverseSize4.h
--rw-r--r--   0        0        0     4588 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/MetisSupport/MetisSupport.h
--rw-r--r--   0        0        0    16105 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0        0        0    61681 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0        0        0     5248 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/OrderingMethods/Ordering.h
--rw-r--r--   0        0        0    22249 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/PaStiXSupport/PaStiXSupport.h
--rw-r--r--   0        0        0    20092 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/PardisoSupport/PardisoSupport.h
--rw-r--r--   0        0        0    25498 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0        0        0     4662 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0        0        0    23429 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0        0        0    26768 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0        0        0    14641 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0        0        0     2993 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/QR/HouseholderQR_LAPACKE.h
--rw-r--r--   0        0        0    11826 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
--rw-r--r--   0        0        0    54214 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0        0        0    32988 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0        0        0     5099 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0        0        0    14743 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0        0        0    15957 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SVD/UpperBidiagonalization.h
--rw-r--r--   0        0        0    24216 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0        0        0     5830 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
--rw-r--r--   0        0        0    10670 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0        0        0     8743 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0        0        0    13166 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0        0        0     2191 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0        0        0    11368 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0        0        0    24360 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0        0        0     6485 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0        0        0    13606 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0        0        0    25524 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0        0        0     4757 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0        0        0    13256 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0        0        0     5808 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0        0        0     3080 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0        0        0     1107 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0        0        0    12589 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0        0        0    57475 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0        0        0    17451 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0        0        0     7329 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0        0        0     7593 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0        0        0     1699 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0        0        0    15600 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0        0        0    25889 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0        0        0     4424 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0        0        0     8704 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0        0        0     3175 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0        0        0     6437 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0        0        0     6827 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0        0        0    14832 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0        0        0     8127 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0        0        0     9657 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/TriangularSolver.h
--rw-r--r--   0        0        0    33316 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0        0        0     4303 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0        0        0     7602 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0        0        0     4974 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0        0        0    12837 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0        0        0     2049 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0        0        0     6712 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0        0        0     6584 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0        0        0     3681 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0        0        0    10217 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0        0        0     4181 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0        0        0     5723 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0        0        0     8485 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0        0        0     9028 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0        0        0     4979 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0        0        0     4545 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0        0        0     2889 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_relax_snode.h
--rw-r--r--   0        0        0    29167 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseQR/SparseQR.h
--rw-r--r--   0        0        0     4730 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0        0        0     4155 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0        0        0     5338 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0        0        0     2809 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/StlSupport/details.h
--rw-r--r--   0        0        0    34324 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SuperLUSupport/SuperLUSupport.h
--rw-r--r--   0        0        0    24456 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/UmfPackSupport/UmfPackSupport.h
--rw-r--r--   0        0        0     2913 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/misc/Image.h
--rw-r--r--   0        0        0     2742 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/misc/Kernel.h
--rw-r--r--   0        0        0     1748 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0        0        0    30560 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/misc/blas.h
--rw-r--r--   0        0        0     7834 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/misc/lapack.h
--rwxr-xr-x   0        0        0  1058369 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/misc/lapacke.h
--rw-r--r--   0        0        0      474 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/misc/lapacke_mangling.h
--rw-r--r--   0        0        0    14060 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0        0        0    21431 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0        0        0    59020 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0        0        0     4828 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0        0        0     6089 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0        0        0    12283 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/IndexedViewMethods.h
--rw-r--r--   0        0        0     6387 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0        0        0     3350 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-r--r--   0        0        0     6915 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/ReshapedMethods.h
--rw-r--r--   0        0        0     1145 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/INSTALL
--rw-r--r--   0        0        0      288 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/README.md
--rw-r--r--   0        0        0     3932 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/BenchSparseUtil.h
--rw-r--r--   0        0        0     4486 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/BenchTimer.h
--rw-r--r--   0        0        0     2529 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/BenchUtil.h
--rw-r--r--   0        0        0     2008 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/README.txt
--rw-r--r--   0        0        0    28983 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/analyze-blocking-sizes.cpp
--rw-r--r--   0        0        0     1421 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/basicbench.cxxlist
--rw-r--r--   0        0        0     1107 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/basicbenchmark.cpp
--rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/basicbenchmark.h
--rw-r--r--   0        0        0     6313 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchBlasGemm.cpp
--rw-r--r--   0        0        0     3548 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchCholesky.cpp
--rw-r--r--   0        0        0     5788 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchEigenSolver.cpp
--rw-r--r--   0        0        0     2806 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchFFT.cpp
--rw-r--r--   0        0        0     3598 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchGeometry.cpp
--rw-r--r--   0        0        0     5193 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchVecAdd.cpp
--rw-r--r--   0        0        0    11435 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/bench_gemm.cpp
--rw-r--r--   0        0        0     1352 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/bench_move_semantics.cpp
--rwxr-xr-x   0        0        0      618 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/bench_multi_compilers.sh
--rw-r--r--   0        0        0    11622 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/bench_norm.cpp
--rw-r--r--   0        0        0     2159 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/bench_reverse.cpp
--rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/bench_sum.cpp
--rwxr-xr-x   0        0        0      651 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/bench_unrolling
--rw-r--r--   0        0        0    22259 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchmark-blocking-sizes.cpp
--rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchmark.cpp
--rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchmarkSlice.cpp
--rw-r--r--   0        0        0      640 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchmarkX.cpp
--rw-r--r--   0        0        0      605 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchmarkXcwise.cpp
--rwxr-xr-x   0        0        0     1209 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchmark_suite
--rw-r--r--   0        0        0     2782 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/CMakeLists.txt
--rw-r--r--   0        0        0    18109 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/COPYING
--rw-r--r--   0        0        0     6447 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/README
--rw-r--r--   0        0        0     3374 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_aat_product.hh
--rw-r--r--   0        0        0     3354 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_ata_product.hh
--rw-r--r--   0        0        0     3670 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_atv_product.hh
--rw-r--r--   0        0        0     3371 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_axpby.hh
--rw-r--r--   0        0        0     3340 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_axpy.hh
--rw-r--r--   0        0        0     3202 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_cholesky.hh
--rw-r--r--   0        0        0     3460 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_ger.hh
--rw-r--r--   0        0        0     5598 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_hessenberg.hh
--rw-r--r--   0        0        0     3151 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_lu_decomp.hh
--rw-r--r--   0        0        0     3598 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_lu_solve.hh
--rw-r--r--   0        0        0     3886 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_matrix_matrix_product.hh
--rw-r--r--   0        0        0     3982 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_matrix_matrix_product_bis.hh
--rw-r--r--   0        0        0     3989 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_matrix_vector_product.hh
--rw-r--r--   0        0        0     3188 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_partial_lu.hh
--rw-r--r--   0        0        0     3019 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_rot.hh
--rw-r--r--   0        0        0     3691 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_symv.hh
--rw-r--r--   0        0        0     3664 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_syr2.hh
--rw-r--r--   0        0        0     3425 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_trisolve.hh
--rw-r--r--   0        0        0     4061 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_trisolve_matrix.hh
--rw-r--r--   0        0        0     3907 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_trmm.hh
--rw-r--r--   0        0        0      464 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/basic_actions.hh
--rw-r--r--   0        0        0      918 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindACML.cmake
--rw-r--r--   0        0        0     1290 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindATLAS.cmake
--rw-r--r--   0        0        0      781 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindBLAZE.cmake
--rw-r--r--   0        0        0     1058 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindBlitz.cmake
--rw-r--r--   0        0        0      634 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindCBLAS.cmake
--rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindGMM.cmake
--rw-r--r--   0        0        0     1232 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindMKL.cmake
--rw-r--r--   0        0        0      787 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindMTL4.cmake
--rw-r--r--   0        0        0      604 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindOPENBLAS.cmake
--rw-r--r--   0        0        0     2372 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0        0        0      798 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindTvmet.cmake
--rw-r--r--   0        0        0     1315 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake
--rw-r--r--   0        0        0      869 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/CMakeLists.txt
--rw-r--r--   0        0        0     1368 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/action_settings.txt
--rw-r--r--   0        0        0     2224 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/gnuplot_common_settings.hh
--rwxr-xr-x   0        0        0     2092 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/go_mean
--rw-r--r--   0        0        0     5306 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/mean.cxx
--rw-r--r--   0        0        0     1850 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/mk_gnuplot_script.sh
--rw-r--r--   0        0        0      929 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/mk_mean_script.sh
--rwxr-xr-x   0        0        0     1742 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/mk_new_gnuplot.sh
--rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/perlib_plot_settings.txt
--rw-r--r--   0        0        0     3425 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/regularize.cxx
--rw-r--r--   0        0        0     5112 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/smooth.cxx
--rwxr-xr-x   0        0        0     1687 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/smooth_all.sh
--rw-r--r--   0        0        0     4827 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/bench.hh
--rw-r--r--   0        0        0     1916 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/bench_parameter.hh
--rw-r--r--   0        0        0     6748 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/btl.hh
--rw-r--r--   0        0        0     1478 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/init/init_function.hh
--rw-r--r--   0        0        0     2295 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/init/init_matrix.hh
--rw-r--r--   0        0        0     1416 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/init/init_vector.hh
--rw-r--r--   0        0        0     2278 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/static/bench_static.hh
--rw-r--r--   0        0        0     1948 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/static/intel_bench_fixed_size.hh
--rw-r--r--   0        0        0     2222 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/static/static_size_generator.hh
--rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/STL_perf_analyzer.hh
--rw-r--r--   0        0        0     2522 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/STL_timer.hh
--rw-r--r--   0        0        0     1994 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh
--rw-r--r--   0        0        0     2938 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/portable_perf_analyzer.hh
--rw-r--r--   0        0        0     3534 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh
--rwxr-xr-x   0        0        0     3534 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/portable_timer.hh
--rw-r--r--   0        0        0     2927 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/x86_perf_analyzer.hh
--rw-r--r--   0        0        0     5294 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/x86_timer.hh
--rw-r--r--   0        0        0     1658 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/utils/size_lin_log.hh
--rw-r--r--   0        0        0     1646 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/utils/size_log.hh
--rw-r--r--   0        0        0     2745 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/utils/utilities.h
--rw-r--r--   0        0        0     2214 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/utils/xy_file.hh
--rw-r--r--   0        0        0     1468 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/CMakeLists.txt
--rw-r--r--   0        0        0    35158 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/blas.h
--rw-r--r--   0        0        0     2891 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/blas_interface.hh
--rw-r--r--   0        0        0     4811 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/blas_interface_impl.hh
--rw-r--r--   0        0        0     1634 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/c_interface_base.h
--rw-r--r--   0        0        0     2960 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/main.cpp
--rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/STL/CMakeLists.txt
--rw-r--r--   0        0        0     5802 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/STL/STL_interface.hh
--rw-r--r--   0        0        0     1828 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/STL/main.cpp
--rw-r--r--   0        0        0      475 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/blaze/CMakeLists.txt
--rw-r--r--   0        0        0     4122 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/blaze/blaze_interface.hh
--rw-r--r--   0        0        0     1636 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/blaze/main.cpp
--rw-r--r--   0        0        0      378 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/CMakeLists.txt
--rw-r--r--   0        0        0     5364 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/blitz_LU_solve_interface.hh
--rw-r--r--   0        0        0     4129 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/blitz_interface.hh
--rw-r--r--   0        0        0     1962 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/btl_blitz.cpp
--rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/btl_tiny_blitz.cpp
--rw-r--r--   0        0        0     3100 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/tiny_blitz_interface.hh
--rw-r--r--   0        0        0      768 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/CMakeLists.txt
--rw-r--r--   0        0        0     1664 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp
--rw-r--r--   0        0        0     5151 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/eigen2_interface.hh
--rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/main_adv.cpp
--rw-r--r--   0        0        0     1205 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/main_linear.cpp
--rw-r--r--   0        0        0     1384 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/main_matmat.cpp
--rw-r--r--   0        0        0     1456 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/main_vecmat.cpp
--rw-r--r--   0        0        0     3207 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/CMakeLists.txt
--rw-r--r--   0        0        0     1664 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp
--rw-r--r--   0        0        0     8187 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/eigen3_interface.hh
--rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/main_adv.cpp
--rw-r--r--   0        0        0     1285 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/main_linear.cpp
--rw-r--r--   0        0        0     1378 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/main_matmat.cpp
--rw-r--r--   0        0        0     1447 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/main_vecmat.cpp
--rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/gmm/CMakeLists.txt
--rw-r--r--   0        0        0     5364 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/gmm/gmm_LU_solve_interface.hh
--rw-r--r--   0        0        0     4174 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/gmm/gmm_interface.hh
--rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/gmm/main.cpp
--rw-r--r--   0        0        0      153 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/mtl4/.kdbgrc.main
--rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/mtl4/CMakeLists.txt
--rw-r--r--   0        0        0     1943 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/mtl4/main.cpp
--rw-r--r--   0        0        0     5364 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh
--rw-r--r--   0        0        0     4210 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/mtl4/mtl4_interface.hh
--rw-r--r--   0        0        0     2130 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/CMakeLists.txt
--rw-r--r--   0        0        0      671 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/main_linear.cpp
--rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/main_matmat.cpp
--rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/main_vecmat.cpp
--rw-r--r--   0        0        0     3190 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/tensor_interface.hh
--rw-r--r--   0        0        0      131 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/tvmet/CMakeLists.txt
--rw-r--r--   0        0        0     1460 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/tvmet/main.cpp
--rw-r--r--   0        0        0     3017 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/tvmet/tvmet_interface.hh
--rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/ublas/CMakeLists.txt
--rw-r--r--   0        0        0     1785 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/ublas/main.cpp
--rw-r--r--   0        0        0     4341 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/ublas/ublas_interface.hh
--rw-r--r--   0        0        0     3269 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/check_cache_queries.cpp
--rw-r--r--   0        0        0     6416 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/dense_solvers.cpp
--rw-r--r--   0        0        0     7243 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/eig33.cpp
--rw-r--r--   0        0        0     3307 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/geometry.cpp
--rw-r--r--   0        0        0     6574 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/changesets.txt
--rw-r--r--   0        0        0      193 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemm.cpp
--rw-r--r--   0        0        0     1382 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemm_common.h
--rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemm_settings.txt
--rw-r--r--   0        0        0      114 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemm_square_settings.txt
--rw-r--r--   0        0        0      193 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemv.cpp
--rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemv_common.h
--rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemv_settings.txt
--rw-r--r--   0        0        0       88 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemv_square_settings.txt
--rw-r--r--   0        0        0      205 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemvt.cpp
--rw-r--r--   0        0        0     2466 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/lazy_gemm.cpp
--rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/lazy_gemm_settings.txt
--rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/llt.cpp
--rwxr-xr-x   0        0        0     2693 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/make_plot.sh
--rw-r--r--   0        0        0     3813 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/chart_footer.html
--rw-r--r--   0        0        0    14775 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/chart_header.html
--rw-r--r--   0        0        0       25 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/footer.html
--rw-r--r--   0        0        0      884 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/header.html
--rw-r--r--   0        0        0   151723 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/s1.js
--rw-r--r--   0        0        0   241320 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/s2.js
--rwxr-xr-x   0        0        0     4090 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/run.sh
--rwxr-xr-x   0        0        0     2031 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/runall.sh
--rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/trmv_lo.cpp
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/trmv_lot.cpp
--rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/trmv_up.cpp
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/trmv_upt.cpp
--rw-r--r--   0        0        0     3232 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/product_threshold.cpp
--rw-r--r--   0        0        0     6006 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/quat_slerp.cpp
--rw-r--r--   0        0        0     1097 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/quatmul.cpp
--rw-r--r--   0        0        0     6260 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/sparse_cholesky.cpp
--rw-r--r--   0        0        0     5101 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/sparse_dense_product.cpp
--rw-r--r--   0        0        0     3011 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/sparse_lu.cpp
--rw-r--r--   0        0        0     8999 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/sparse_product.cpp
--rw-r--r--   0        0        0     3393 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/sparse_randomsetter.cpp
--rw-r--r--   0        0        0    13761 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/sparse_setter.cpp
--rw-r--r--   0        0        0     2347 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/sparse_transpose.cpp
--rw-r--r--   0        0        0     6114 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/sparse_trisolver.cpp
--rw-r--r--   0        0        0     3061 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/spbench/CMakeLists.txt
--rw-r--r--   0        0        0     3975 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/spbench/sp_solver.cpp
--rw-r--r--   0        0        0     1856 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/spbench/spbench.dtd
--rw-r--r--   0        0        0     3301 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/spbench/spbenchsolver.cpp
--rw-r--r--   0        0        0    18167 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/spbench/spbenchsolver.h
--rw-r--r--   0        0        0     3825 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/spbench/spbenchstyle.h
--rw-r--r--   0        0        0     2831 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/spbench/test_sparseLU.cpp
--rw-r--r--   0        0        0     6096 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/spmv.cpp
--rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/README
--rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/benchmark.h
--rw-r--r--   0        0        0     6834 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/benchmark_main.cc
--rw-r--r--   0        0        0     1389 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/contraction_benchmarks_cpu.cc
--rwxr-xr-x   0        0        0      729 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/eigen_sycl_bench.sh
--rw-r--r--   0        0        0      647 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/eigen_sycl_bench_contract.sh
--rw-r--r--   0        0        0    20459 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks.h
--rw-r--r--   0        0        0     6264 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks_cpu.cc
--rw-r--r--   0        0        0     3381 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks_fp16_gpu.cu
--rw-r--r--   0        0        0     3373 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks_gpu.cu
--rw-r--r--   0        0        0     6273 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks_sycl.cc
--rw-r--r--   0        0        0    11331 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/tensor_contract_sycl_bench.cc
--rw-r--r--   0        0        0     1203 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/vdw_new.cpp
--rw-r--r--   0        0        0     3614 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/BandTriangularSolver.h
--rw-r--r--   0        0        0     1730 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/CMakeLists.txt
--rw-r--r--   0        0        0     1608 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/GeneralRank1Update.h
--rw-r--r--   0        0        0     2036 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/PackedSelfadjointProduct.h
--rw-r--r--   0        0        0     3165 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/PackedTriangularMatrixVector.h
--rw-r--r--   0        0        0     3191 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/PackedTriangularSolverVector.h
--rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/README.txt
--rw-r--r--   0        0        0     2168 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/Rank2Update.h
--rw-r--r--   0        0        0     4672 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/common.h
--rw-r--r--   0        0        0      647 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/complex_double.cpp
--rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/complex_single.cpp
--rw-r--r--   0        0        0     1507 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/double.cpp
--rw-r--r--   0        0        0    15108 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/chbmv.c
--rw-r--r--   0        0        0    13026 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/chpmv.c
--rw-r--r--   0        0        0     2310 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/complexdots.c
--rw-r--r--   0        0        0    18945 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/ctbmv.c
--rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/d_cnjg.c
--rw-r--r--   0        0        0      657 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/datatypes.h
--rw-r--r--   0        0        0     4968 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/drotm.c
--rw-r--r--   0        0        0     6193 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/drotmg.c
--rw-r--r--   0        0        0    10188 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/dsbmv.c
--rw-r--r--   0        0        0     8075 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/dspmv.c
--rw-r--r--   0        0        0    11657 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/dtbmv.c
--rw-r--r--   0        0        0     2976 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/lsame.c
--rw-r--r--   0        0        0      105 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/r_cnjg.c
--rw-r--r--   0        0        0     4902 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/srotm.c
--rw-r--r--   0        0        0     6056 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/srotmg.c
--rw-r--r--   0        0        0    10210 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/ssbmv.c
--rw-r--r--   0        0        0     8051 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/sspmv.c
--rw-r--r--   0        0        0    11643 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/stbmv.c
--rw-r--r--   0        0        0    15144 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/zhbmv.c
--rw-r--r--   0        0        0    13060 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/zhpmv.c
--rw-r--r--   0        0        0    18973 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/ztbmv.c
--rw-r--r--   0        0        0      979 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/fortran/complexdots.f
--rw-r--r--   0        0        0     5646 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/level1_cplx_impl.h
--rw-r--r--   0        0        0     3892 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/level1_impl.h
--rw-r--r--   0        0        0     4267 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/level1_real_impl.h
--rw-r--r--   0        0        0    12223 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/level2_cplx_impl.h
--rw-r--r--   0        0        0    25172 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/level2_impl.h
--rw-r--r--   0        0        0    10499 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/level2_real_impl.h
--rw-r--r--   0        0        0    38043 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/level3_impl.h
--rw-r--r--   0        0        0      763 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/single.cpp
--rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/CMakeLists.txt
--rw-r--r--   0        0        0    32110 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/cblat1.f
--rw-r--r--   0        0        0     1546 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/cblat2.dat
--rw-r--r--   0        0        0   116657 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/cblat2.f
--rw-r--r--   0        0        0     1046 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/cblat3.dat
--rw-r--r--   0        0        0   131550 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/cblat3.f
--rw-r--r--   0        0        0    44820 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/dblat1.f
--rw-r--r--   0        0        0     1466 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/dblat2.dat
--rw-r--r--   0        0        0   112335 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/dblat2.f
--rw-r--r--   0        0        0      882 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/dblat3.dat
--rw-r--r--   0        0        0   104262 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/dblat3.f
--rwxr-xr-x   0        0        0     1016 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/runblastest.sh
--rw-r--r--   0        0        0    43389 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/sblat1.f
--rw-r--r--   0        0        0     1466 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/sblat2.dat
--rw-r--r--   0        0        0   112251 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/sblat2.f
--rw-r--r--   0        0        0      882 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/sblat3.dat
--rw-r--r--   0        0        0   104172 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/sblat3.f
--rw-r--r--   0        0        0    32115 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/zblat1.f
--rw-r--r--   0        0        0     1546 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/zblat2.dat
--rw-r--r--   0        0        0   117003 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/zblat2.f
--rw-r--r--   0        0        0     1046 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/zblat3.dat
--rw-r--r--   0        0        0   131995 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/zblat3.f
--rw-r--r--   0        0        0      389 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/xerbla.cpp
--rw-r--r--   0        0        0     6736 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/ci/CTest2JUnit.xsl
--rw-r--r--   0        0        0     4910 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/ci/README.md
--rw-r--r--   0        0        0     5024 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/ci/build.gitlab-ci.yml
--rw-r--r--   0        0        0     3490 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/ci/smoketests.gitlab-ci.yml
--rw-r--r--   0        0        0    10349 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/ci/test.gitlab-ci.yml
--rw-r--r--   0        0        0     2171 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/ComputeCppCompilerChecks.cmake
--rw-r--r--   0        0        0      475 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/ComputeCppIRMap.cmake
--rw-r--r--   0        0        0      802 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/Eigen3Config.cmake.in
--rw-r--r--   0        0        0     1397 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/Eigen3ConfigLegacy.cmake.in
--rw-r--r--   0        0        0     2779 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/EigenConfigureTesting.cmake
--rw-r--r--   0        0        0     1562 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/EigenDetermineOSVersion.cmake
--rw-r--r--   0        0        0     1814 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/EigenDetermineVSServicePack.cmake
--rw-r--r--   0        0        0     2321 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/EigenSmokeTestList.cmake
--rw-r--r--   0        0        0    29205 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/EigenTesting.cmake
--rw-r--r--   0        0        0     1196 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/EigenUninstall.cmake
--rw-r--r--   0        0        0      517 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindAdolc.cmake
--rw-r--r--   0        0        0    42828 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindBLAS.cmake
--rw-r--r--   0        0        0    13179 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindBLASEXT.cmake
--rw-r--r--   0        0        0     2413 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindCHOLMOD.cmake
--rw-r--r--   0        0        0    16685 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindComputeCpp.cmake
--rw-r--r--   0        0        0     2636 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindEigen2.cmake
--rw-r--r--   0        0        0     3509 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindEigen3.cmake
--rw-r--r--   0        0        0     2783 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindFFTW.cmake
--rw-r--r--   0        0        0     2943 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindGLEW.cmake
--rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindGMP.cmake
--rw-r--r--   0        0        0     4992 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindGSL.cmake
--rw-r--r--   0        0        0      846 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindGoogleHash.cmake
--rw-r--r--   0        0        0    11729 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindHWLOC.cmake
--rw-r--r--   0        0        0     1281 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindKLU.cmake
--rw-r--r--   0        0        0     9734 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindLAPACK.cmake
--rw-r--r--   0        0        0     2632 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindMPFR.cmake
--rw-r--r--   0        0        0     3524 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindMPREAL.cmake
--rw-r--r--   0        0        0     8969 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindMetis.cmake
--rw-r--r--   0        0        0    23160 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindPASTIX.cmake
--rw-r--r--   0        0        0    14417 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindPTSCOTCH.cmake
--rw-r--r--   0        0        0    12034 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindSCOTCH.cmake
--rw-r--r--   0        0        0     1142 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindSPQR.cmake
--rw-r--r--   0        0        0     2482 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindStandardMathLibrary.cmake
--rw-r--r--   0        0        0     2261 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindSuperLU.cmake
--rw-r--r--   0        0        0     5111 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindTriSYCL.cmake
--rw-r--r--   0        0        0     1662 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindUMFPACK.cmake
--rw-r--r--   0        0        0      910 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/RegexUtils.cmake
--rw-r--r--   0        0        0      177 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/UseEigen3.cmake
--rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/debug/gdb/__init__.py
--rw-r--r--   0        0        0     9617 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/debug/gdb/printers.py
--rw-r--r--   0        0        0    11661 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/debug/msvc/eigen.natvis
--rw-r--r--   0        0        0     7566 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/debug/msvc/eigen_autoexp_part.dat
--rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/CMakeLists.txt
--rw-r--r--   0        0        0      462 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/mandelbrot/CMakeLists.txt
--rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/mandelbrot/README
--rw-r--r--   0        0        0     7509 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/mandelbrot/mandelbrot.cpp
--rw-r--r--   0        0        0     1888 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/mandelbrot/mandelbrot.h
--rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/mix_eigen_and_c/README
--rw-r--r--   0        0        0     4158 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/mix_eigen_and_c/binary_library.cpp
--rw-r--r--   0        0        0     3346 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/mix_eigen_and_c/binary_library.h
--rw-r--r--   0        0        0     1616 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/mix_eigen_and_c/example.c
--rw-r--r--   0        0        0      695 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/CMakeLists.txt
--rw-r--r--   0        0        0      403 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/README
--rw-r--r--   0        0        0     5981 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/camera.cpp
--rw-r--r--   0        0        0     3435 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/camera.h
--rw-r--r--   0        0        0     3974 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/gpuhelper.cpp
--rw-r--r--   0        0        0     7177 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/gpuhelper.h
--rw-r--r--   0        0        0     3927 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/icosphere.cpp
--rw-r--r--   0        0        0      869 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/icosphere.h
--rw-r--r--   0        0        0    19192 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/quaternion_demo.cpp
--rw-r--r--   0        0        0     2635 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/quaternion_demo.h
--rw-r--r--   0        0        0     1756 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/trackball.cpp
--rw-r--r--   0        0        0      943 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/trackball.h
--rw-r--r--   0        0        0    11165 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/AsciiQuickReference.txt
--rw-r--r--   0        0        0     2425 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/B01_Experimental.dox
--rw-r--r--   0        0        0     4935 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/CMakeLists.txt
--rw-r--r--   0        0        0     6332 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/ClassHierarchy.dox
--rw-r--r--   0        0        0    18692 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/CoeffwiseMathFunctionsTable.dox
--rw-r--r--   0        0        0     4423 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/CustomizingEigen_CustomScalar.dox
--rw-r--r--   0        0        0     1337 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/CustomizingEigen_InheritingMatrix.dox
--rw-r--r--   0        0        0     3658 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/CustomizingEigen_NullaryExpr.dox
--rw-r--r--   0        0        0     3658 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/CustomizingEigen_Plugins.dox
--rw-r--r--   0        0        0     5021 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/DenseDecompositionBenchmark.dox
--rw-r--r--   0        0        0    86035 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/Doxyfile.in
--rw-r--r--   0        0        0     8355 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/Eigen_Silly_Professor_64x64.png
--rw-r--r--   0        0        0     1906 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/FixedSizeVectorizable.dox
--rw-r--r--   0        0        0    13458 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/FunctionsTakingEigenTypes.dox
--rw-r--r--   0        0        0     5429 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/HiPerformance.dox
--rw-r--r--   0        0        0     3797 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/InplaceDecomposition.dox
--rw-r--r--   0        0        0    30585 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/InsideEigenExample.dox
--rw-r--r--   0        0        0     3150 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/LeastSquares.dox
--rw-r--r--   0        0        0     6761 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/Manual.dox
--rw-r--r--   0        0        0      758 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/MatrixfreeSolverExample.dox
--rw-r--r--   0        0        0     5610 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/NewExpressionType.dox
--rw-r--r--   0        0        0     1929 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/Overview.dox
--rw-r--r--   0        0        0     1166 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/PassingByValue.dox
--rw-r--r--   0        0        0     7018 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/Pitfalls.dox
--rw-r--r--   0        0        0    14277 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/PreprocessorDirectives.dox
--rw-r--r--   0        0        0    29844 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/QuickReference.dox
--rw-r--r--   0        0        0     6578 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/QuickStartGuide.dox
--rw-r--r--   0        0        0    19902 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/SparseLinearSystems.dox
--rw-r--r--   0        0        0     8312 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/SparseQuickReference.dox
--rw-r--r--   0        0        0     3923 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/StlContainers.dox
--rw-r--r--   0        0        0     4119 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/StorageOrders.dox
--rw-r--r--   0        0        0     7026 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/StructHavingEigenMembers.dox
--rw-r--r--   0        0        0     6157 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TemplateKeyword.dox
--rw-r--r--   0        0        0    10269 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TopicAliasing.dox
--rw-r--r--   0        0        0     5285 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TopicAssertions.dox
--rw-r--r--   0        0        0     1914 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TopicCMakeGuide.dox
--rw-r--r--   0        0        0      173 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TopicEigenExpressionTemplates.dox
--rw-r--r--   0        0        0     6314 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TopicLazyEvaluation.dox
--rw-r--r--   0        0        0     9068 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TopicLinearAlgebraDecompositions.dox
--rw-r--r--   0        0        0     3749 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TopicMultithreading.dox
--rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TopicResizing.dox
--rw-r--r--   0        0        0      145 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TopicScalarTypes.dox
--rw-r--r--   0        0        0       97 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TopicVectorization.dox
--rw-r--r--   0        0        0     6900 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialAdvancedInitialization.dox
--rw-r--r--   0        0        0     8523 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialArrayClass.dox
--rw-r--r--   0        0        0     8288 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialBlockOperations.dox
--rw-r--r--   0        0        0     9731 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialGeometry.dox
--rw-r--r--   0        0        0    11860 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialLinearAlgebra.dox
--rw-r--r--   0        0        0     3988 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialMapClass.dox
--rw-r--r--   0        0        0     9865 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialMatrixArithmetic.dox
--rw-r--r--   0        0        0    13680 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialMatrixClass.dox
--rw-r--r--   0        0        0    12006 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialReductionsVisitorsBroadcasting.dox
--rw-r--r--   0        0        0     2981 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialReshape.dox
--rw-r--r--   0        0        0     2142 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialSTL.dox
--rw-r--r--   0        0        0     8209 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialSlicingIndexing.dox
--rw-r--r--   0        0        0    20483 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialSparse.dox
--rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialSparse_example_details.dox
--rw-r--r--   0        0        0     8737 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/UnalignedArrayAssert.dox
--rw-r--r--   0        0        0     6633 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/UsingBlasLapackBackends.dox
--rw-r--r--   0        0        0     6113 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/UsingIntelMKL.dox
--rw-r--r--   0        0        0     1855 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/UsingNVCC.dox
--rw-r--r--   0        0        0     2924 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/WrongStackAlignment.dox
--rw-r--r--   0        0        0     8006 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/eigen_navtree_hacks.js
--rw-r--r--   0        0        0     4584 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/eigendoxy.css
--rw-r--r--   0        0        0      680 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/eigendoxy_footer.html.in
--rw-r--r--   0        0        0     2521 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/eigendoxy_header.html.in
--rw-r--r--   0        0        0     5337 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/eigendoxy_layout.xml.in
--rw-r--r--   0        0        0     1095 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/eigendoxy_tabs.css
--rw-r--r--   0        0        0       34 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/.krazy
--rw-r--r--   0        0        0      607 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/CMakeLists.txt
--rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/CustomizingEigen_Inheritance.cpp
--rw-r--r--   0        0        0      189 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Cwise_erf.cpp
--rw-r--r--   0        0        0      190 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Cwise_erfc.cpp
--rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Cwise_lgamma.cpp
--rw-r--r--   0        0        0      282 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/DenseBase_middleCols_int.cpp
--rw-r--r--   0        0        0      282 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/DenseBase_middleRows_int.cpp
--rw-r--r--   0        0        0      283 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/DenseBase_template_int_middleCols.cpp
--rw-r--r--   0        0        0      283 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/DenseBase_template_int_middleRows.cpp
--rw-r--r--   0        0        0      206 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/QuickStart_example.cpp
--rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/QuickStart_example2_dynamic.cpp
--rw-r--r--   0        0        0      289 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/QuickStart_example2_fixed.cpp
--rw-r--r--   0        0        0      677 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TemplateKeyword_flexible.cpp
--rw-r--r--   0        0        0      508 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TemplateKeyword_simple.cpp
--rw-r--r--   0        0        0     1589 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TutorialInplaceLU.cpp
--rw-r--r--   0        0        0      622 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgComputeTwice.cpp
--rw-r--r--   0        0        0      371 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgExComputeSolveError.cpp
--rw-r--r--   0        0        0      381 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgExSolveColPivHouseholderQR.cpp
--rw-r--r--   0        0        0      356 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgExSolveLDLT.cpp
--rw-r--r--   0        0        0      348 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgInverseDeterminant.cpp
--rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgRankRevealing.cpp
--rw-r--r--   0        0        0      405 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgSVDSolve.cpp
--rw-r--r--   0        0        0      534 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp
--rw-r--r--   0        0        0      377 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgSetThreshold.cpp
--rw-r--r--   0        0        0      466 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_accessors.cpp
--rw-r--r--   0        0        0      400 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_addition.cpp
--rw-r--r--   0        0        0      410 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_cwise_other.cpp
--rw-r--r--   0        0        0      444 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_interop.cpp
--rw-r--r--   0        0        0      591 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp
--rw-r--r--   0        0        0      237 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_mult.cpp
--rw-r--r--   0        0        0      523 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_block_assignment.cpp
--rw-r--r--   0        0        0      390 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_colrow.cpp
--rw-r--r--   0        0        0      448 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_corner.cpp
--rw-r--r--   0        0        0      413 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_print_block.cpp
--rw-r--r--   0        0        0      348 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_vector.cpp
--rw-r--r--   0        0        0      401 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_PartialLU_solve.cpp
--rw-r--r--   0        0        0      440 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_1nn.cpp
--rw-r--r--   0        0        0      356 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple.cpp
--rw-r--r--   0        0        0      361 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple_rowwise.cpp
--rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_colwise.cpp
--rw-r--r--   0        0        0      502 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_maxnorm.cpp
--rw-r--r--   0        0        0      513 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp
--rw-r--r--   0        0        0      447 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_operatornorm.cpp
--rw-r--r--   0        0        0      244 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_rowwise.cpp
--rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp
--rw-r--r--   0        0        0      680 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_simple_example_dynamic_size.cpp
--rw-r--r--   0        0        0      282 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_simple_example_fixed_size.cpp
--rw-r--r--   0        0        0      737 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/class_Block.cpp
--rw-r--r--   0        0        0      526 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/class_CwiseBinaryOp.cpp
--rw-r--r--   0        0        0      561 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/class_CwiseUnaryOp.cpp
--rw-r--r--   0        0        0      371 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/class_CwiseUnaryOp_ptrfun.cpp
--rw-r--r--   0        0        0      697 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/class_FixedBlock.cpp
--rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/class_FixedReshaped.cpp
--rw-r--r--   0        0        0      673 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/class_FixedVectorBlock.cpp
--rw-r--r--   0        0        0      545 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/class_Reshaped.cpp
--rw-r--r--   0        0        0      775 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/class_VectorBlock.cpp
--rw-r--r--   0        0        0      418 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/function_taking_eigenbase.cpp
--rw-r--r--   0        0        0      594 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/function_taking_ref.cpp
--rw-r--r--   0        0        0      366 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp
--rw-r--r--   0        0        0      145 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.entry
--rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.evaluator
--rw-r--r--   0        0        0      591 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.expression
--rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.main
--rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.preamble
--rw-r--r--   0        0        0      605 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.traits
--rw-r--r--   0        0        0     1320 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/make_circulant2.cpp
--rw-r--r--   0        0        0     4275 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/matrixfree_cg.cpp
--rw-r--r--   0        0        0     2455 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/nullary_indexing.cpp
--rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/tut_arithmetic_add_sub.cpp
--rw-r--r--   0        0        0      393 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/tut_arithmetic_dot_cross.cpp
--rw-r--r--   0        0        0      612 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/tut_arithmetic_matrix_mul.cpp
--rw-r--r--   0        0        0      529 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/tut_arithmetic_redux_basic.cpp
--rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/tut_arithmetic_scalar_mul_div.cpp
--rw-r--r--   0        0        0      343 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/tut_matrix_coefficient_accessors.cpp
--rw-r--r--   0        0        0      489 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/tut_matrix_resize.cpp
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/tut_matrix_resize_fixed_size.cpp
--rw-r--r--   0        0        0       86 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/ftv2node.png
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/ftv2pnode.png
--rw-r--r--   0        0        0       34 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/.krazy
--rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/AngleAxis_mimic_euler.cpp
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Array_initializer_list_23_cxx11.cpp
--rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Array_initializer_list_vector_cxx11.cpp
--rw-r--r--   0        0        0      102 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Array_variadic_ctor_cxx11.cpp
--rw-r--r--   0        0        0      394 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/BiCGSTAB_simple.cpp
--rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/BiCGSTAB_step_by_step.cpp
--rw-r--r--   0        0        0     1624 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/CMakeLists.txt
--rw-r--r--   0        0        0      324 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/ColPivHouseholderQR_solve.cpp
--rw-r--r--   0        0        0      792 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/ComplexEigenSolver_compute.cpp
--rw-r--r--   0        0        0      216 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/ComplexEigenSolver_eigenvalues.cpp
--rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/ComplexEigenSolver_eigenvectors.cpp
--rw-r--r--   0        0        0      301 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/ComplexSchur_compute.cpp
--rw-r--r--   0        0        0      263 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/ComplexSchur_matrixT.cpp
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/ComplexSchur_matrixU.cpp
--rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_abs.cpp
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_abs2.cpp
--rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_acos.cpp
--rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_arg.cpp
--rw-r--r--   0        0        0      232 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_array_power_array.cpp
--rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_asin.cpp
--rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_atan.cpp
--rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_boolean_and.cpp
--rw-r--r--   0        0        0      105 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_boolean_not.cpp
--rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_boolean_or.cpp
--rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_boolean_xor.cpp
--rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_ceil.cpp
--rw-r--r--   0        0        0       58 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_cos.cpp
--rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_cosh.cpp
--rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_cube.cpp
--rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_equal_equal.cpp
--rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_exp.cpp
--rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_floor.cpp
--rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_greater.cpp
--rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_greater_equal.cpp
--rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_inverse.cpp
--rw-r--r--   0        0        0      104 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_isFinite.cpp
--rw-r--r--   0        0        0      101 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_isInf.cpp
--rw-r--r--   0        0        0      101 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_isNaN.cpp
--rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_less.cpp
--rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_less_equal.cpp
--rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_log.cpp
--rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_log10.cpp
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_max.cpp
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_min.cpp
--rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_minus.cpp
--rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_minus_equal.cpp
--rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_not_equal.cpp
--rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_plus.cpp
--rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_plus_equal.cpp
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_pow.cpp
--rw-r--r--   0        0        0      141 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_product.cpp
--rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_quotient.cpp
--rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_rint.cpp
--rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_round.cpp
--rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_scalar_power_array.cpp
--rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_sign.cpp
--rw-r--r--   0        0        0       58 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_sin.cpp
--rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_sinh.cpp
--rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_slash_equal.cpp
--rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_sqrt.cpp
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_square.cpp
--rw-r--r--   0        0        0       58 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_tan.cpp
--rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_tanh.cpp
--rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_times_equal.cpp
--rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/DenseBase_LinSpaced.cpp
--rw-r--r--   0        0        0      420 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/DenseBase_LinSpacedInt.cpp
--rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/DenseBase_LinSpaced_seq_deprecated.cpp
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/DenseBase_setLinSpaced.cpp
--rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/DirectionWise_hnormalized.cpp
--rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/DirectionWise_replicate.cpp
--rw-r--r--   0        0        0      179 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/DirectionWise_replicate_int.cpp
--rw-r--r--   0        0        0      800 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp
--rw-r--r--   0        0        0      361 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/EigenSolver_compute.cpp
--rw-r--r--   0        0        0      176 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/EigenSolver_eigenvalues.cpp
--rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/EigenSolver_eigenvectors.cpp
--rw-r--r--   0        0        0      430 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/EigenSolver_pseudoEigenvectors.cpp
--rw-r--r--   0        0        0      325 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/FullPivHouseholderQR_solve.cpp
--rw-r--r--   0        0        0      369 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/FullPivLU_image.cpp
--rw-r--r--   0        0        0      317 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/FullPivLU_kernel.cpp
--rw-r--r--   0        0        0      413 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/FullPivLU_solve.cpp
--rw-r--r--   0        0        0      456 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/GeneralizedEigenSolver.cpp
--rw-r--r--   0        0        0      339 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/HessenbergDecomposition_compute.cpp
--rw-r--r--   0        0        0      391 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/HessenbergDecomposition_matrixH.cpp
--rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/HessenbergDecomposition_packedMatrix.cpp
--rw-r--r--   0        0        0      300 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/HouseholderQR_householderQ.cpp
--rw-r--r--   0        0        0      357 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/HouseholderQR_solve.cpp
--rw-r--r--   0        0        0     1316 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/HouseholderSequence_HouseholderSequence.cpp
--rw-r--r--   0        0        0      603 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/IOFormat.cpp
--rw-r--r--   0        0        0      614 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/JacobiSVD_basic.cpp
--rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Jacobi_makeGivens.cpp
--rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Jacobi_makeJacobi.cpp
--rw-r--r--   0        0        0      519 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/LLT_example.cpp
--rw-r--r--   0        0        0      456 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/LLT_solve.cpp
--rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/LeastSquaresNormalEquations.cpp
--rw-r--r--   0        0        0      177 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/LeastSquaresQR.cpp
--rw-r--r--   0        0        0      164 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Map_general_stride.cpp
--rw-r--r--   0        0        0      199 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Map_inner_stride.cpp
--rw-r--r--   0        0        0      138 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Map_outer_stride.cpp
--rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Map_placement_new.cpp
--rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Map_simple.cpp
--rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_adjoint.cpp
--rw-r--r--   0        0        0      523 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_all.cpp
--rw-r--r--   0        0        0      207 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_applyOnTheLeft.cpp
--rw-r--r--   0        0        0      292 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_applyOnTheRight.cpp
--rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_array.cpp
--rw-r--r--   0        0        0      234 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_array_const.cpp
--rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_asDiagonal.cpp
--rw-r--r--   0        0        0      244 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_block_int_int.cpp
--rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_block_int_int_int_int.cpp
--rw-r--r--   0        0        0      271 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_bottomLeftCorner_int_int.cpp
--rw-r--r--   0        0        0      274 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_bottomRightCorner_int_int.cpp
--rw-r--r--   0        0        0      242 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_bottomRows_int.cpp
--rw-r--r--   0        0        0      119 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cast.cpp
--rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_col.cpp
--rw-r--r--   0        0        0      287 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_colwise.cpp
--rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_colwise_iterator_cxx11.cpp
--rw-r--r--   0        0        0      410 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_computeInverseAndDetWithCheck.cpp
--rw-r--r--   0        0        0      318 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_computeInverseWithCheck.cpp
--rw-r--r--   0        0        0       80 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseAbs.cpp
--rw-r--r--   0        0        0       81 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseAbs2.cpp
--rw-r--r--   0        0        0       95 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseArg.cpp
--rw-r--r--   0        0        0      276 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseEqual.cpp
--rw-r--r--   0        0        0       87 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseInverse.cpp
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseMax.cpp
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseMin.cpp
--rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseNotEqual.cpp
--rw-r--r--   0        0        0      153 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseProduct.cpp
--rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseQuotient.cpp
--rw-r--r--   0        0        0       80 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseSign.cpp
--rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseSqrt.cpp
--rw-r--r--   0        0        0      188 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_diagonal.cpp
--rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_diagonal_int.cpp
--rw-r--r--   0        0        0      274 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_diagonal_template_int.cpp
--rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_eigenvalues.cpp
--rw-r--r--   0        0        0      226 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_end_int.cpp
--rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_eval.cpp
--rw-r--r--   0        0        0      274 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_fixedBlock_int_int.cpp
--rw-r--r--   0        0        0      377 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_hnormalized.cpp
--rw-r--r--   0        0        0      487 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_homogeneous.cpp
--rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_identity.cpp
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_identity_int_int.cpp
--rw-r--r--   0        0        0      145 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_inverse.cpp
--rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_isDiagonal.cpp
--rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_isIdentity.cpp
--rw-r--r--   0        0        0      216 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_isOnes.cpp
--rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_isOrthogonal.cpp
--rw-r--r--   0        0        0      231 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_isUnitary.cpp
--rw-r--r--   0        0        0      215 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_isZero.cpp
--rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_leftCols_int.cpp
--rw-r--r--   0        0        0      129 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_noalias.cpp
--rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_ones.cpp
--rw-r--r--   0        0        0       77 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_ones_int.cpp
--rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_ones_int_int.cpp
--rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_operatorNorm.cpp
--rw-r--r--   0        0        0      171 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_prod.cpp
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_random.cpp
--rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_random_int.cpp
--rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_random_int_int.cpp
--rw-r--r--   0        0        0      170 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_replicate.cpp
--rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_replicate_int_int.cpp
--rw-r--r--   0        0        0      291 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_reshaped_auto.cpp
--rw-r--r--   0        0        0      178 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_reshaped_fixed.cpp
--rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_reshaped_int_int.cpp
--rw-r--r--   0        0        0      287 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_reshaped_to_vector.cpp
--rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_reverse.cpp
--rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_rightCols_int.cpp
--rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_row.cpp
--rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_rowwise.cpp
--rw-r--r--   0        0        0      244 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_segment_int_int.cpp
--rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_select.cpp
--rw-r--r--   0        0        0      361 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_selfadjointView.cpp
--rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_set.cpp
--rw-r--r--   0        0        0       83 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_setIdentity.cpp
--rw-r--r--   0        0        0       72 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_setOnes.cpp
--rw-r--r--   0        0        0       72 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_setRandom.cpp
--rw-r--r--   0        0        0       72 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_setZero.cpp
--rw-r--r--   0        0        0      226 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_start_int.cpp
--rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_bottomRows.cpp
--rw-r--r--   0        0        0      230 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_end.cpp
--rw-r--r--   0        0        0      264 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_block_int_int_int_int.cpp
--rw-r--r--   0        0        0      274 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner.cpp
--rw-r--r--   0        0        0      301 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner_int_int.cpp
--rw-r--r--   0        0        0      277 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_bottomRightCorner.cpp
--rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_bottomRightCorner_int_int.cpp
--rw-r--r--   0        0        0      265 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_topLeftCorner.cpp
--rw-r--r--   0        0        0      292 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_topLeftCorner_int_int.cpp
--rw-r--r--   0        0        0      268 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_topRightCorner.cpp
--rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_topRightCorner_int_int.cpp
--rw-r--r--   0        0        0      242 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_leftCols.cpp
--rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_rightCols.cpp
--rw-r--r--   0        0        0      244 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_segment.cpp
--rw-r--r--   0        0        0      230 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_start.cpp
--rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_topRows.cpp
--rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_topLeftCorner_int_int.cpp
--rw-r--r--   0        0        0      265 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_topRightCorner_int_int.cpp
--rw-r--r--   0        0        0      233 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_topRows_int.cpp
--rw-r--r--   0        0        0      414 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_transpose.cpp
--rw-r--r--   0        0        0      573 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_triangularView.cpp
--rw-r--r--   0        0        0       71 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_zero.cpp
--rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_zero_int.cpp
--rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_zero_int_int.cpp
--rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_Map_stride.cpp
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_initializer_list_23_cxx11.cpp
--rw-r--r--   0        0        0       40 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_initializer_list_vector_cxx11.cpp
--rw-r--r--   0        0        0      111 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_resize_NoChange_int.cpp
--rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_resize_int.cpp
--rw-r--r--   0        0        0      111 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_resize_int_NoChange.cpp
--rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_resize_int_int.cpp
--rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setConstant_int.cpp
--rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setConstant_int_int.cpp
--rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setIdentity_int_int.cpp
--rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setOnes_int.cpp
--rw-r--r--   0        0        0       48 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setOnes_int_int.cpp
--rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setRandom_int.cpp
--rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setRandom_int_int.cpp
--rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setZero_int.cpp
--rw-r--r--   0        0        0       48 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setZero_int_int.cpp
--rw-r--r--   0        0        0      104 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_variadic_ctor_cxx11.cpp
--rw-r--r--   0        0        0      372 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/PartialPivLU_solve.cpp
--rw-r--r--   0        0        0      263 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/PartialRedux_count.cpp
--rw-r--r--   0        0        0      176 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/PartialRedux_maxCoeff.cpp
--rw-r--r--   0        0        0      176 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/PartialRedux_minCoeff.cpp
--rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/PartialRedux_norm.cpp
--rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/PartialRedux_prod.cpp
--rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/PartialRedux_squaredNorm.cpp
--rw-r--r--   0        0        0      164 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/PartialRedux_sum.cpp
--rw-r--r--   0        0        0      819 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/RealQZ_compute.cpp
--rw-r--r--   0        0        0      429 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/RealSchur_RealSchur_MatrixType.cpp
--rw-r--r--   0        0        0      343 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/RealSchur_compute.cpp
--rw-r--r--   0        0        0      362 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver.cpp
--rw-r--r--   0        0        0      816 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp
--rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp
--rw-r--r--   0        0        0      365 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType.cpp
--rw-r--r--   0        0        0      396 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType2.cpp
--rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_eigenvalues.cpp
--rw-r--r--   0        0        0      193 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_eigenvectors.cpp
--rw-r--r--   0        0        0      426 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_operatorInverseSqrt.cpp
--rw-r--r--   0        0        0      363 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_operatorSqrt.cpp
--rw-r--r--   0        0        0      184 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointView_eigenvalues.cpp
--rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointView_operatorNorm.cpp
--rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Slicing_arrayexpr.cpp
--rw-r--r--   0        0        0      369 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Slicing_custom_padding_cxx11.cpp
--rw-r--r--   0        0        0      190 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Slicing_rawarray_cxx11.cpp
--rw-r--r--   0        0        0      164 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Slicing_stdvector_cxx11.cpp
--rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/SparseMatrix_coeffs.cpp
--rw-r--r--   0        0        0      267 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_block.cpp
--rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_block_correct.cpp
--rw-r--r--   0        0        0      591 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_cwise.cpp
--rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_mult1.cpp
--rw-r--r--   0        0        0      230 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_mult2.cpp
--rw-r--r--   0        0        0       86 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_mult3.cpp
--rw-r--r--   0        0        0      102 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_mult4.cpp
--rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_mult5.cpp
--rw-r--r--   0        0        0      525 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/TopicStorageOrders_example.cpp
--rw-r--r--   0        0        0      520 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Triangular_solve.cpp
--rw-r--r--   0        0        0      445 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tridiagonalization_Tridiagonalization_MatrixType.cpp
--rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tridiagonalization_compute.cpp
--rw-r--r--   0        0        0      550 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tridiagonalization_decomposeInPlace.cpp
--rw-r--r--   0        0        0      552 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tridiagonalization_diagonal.cpp
--rw-r--r--   0        0        0      303 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tridiagonalization_householderCoefficients.cpp
--rw-r--r--   0        0        0      394 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tridiagonalization_packedMatrix.cpp
--rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_Block.cpp
--rw-r--r--   0        0        0      168 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_CommaTemporary.cpp
--rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_Join.cpp
--rw-r--r--   0        0        0      272 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_LinSpaced.cpp
--rw-r--r--   0        0        0      878 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp
--rw-r--r--   0        0        0      332 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_Zero.cpp
--rw-r--r--   0        0        0      299 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_Map_rowmajor.cpp
--rw-r--r--   0        0        0      896 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_Map_using.cpp
--rw-r--r--   0        0        0      171 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_ReshapeMat2Mat.cpp
--rw-r--r--   0        0        0      299 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_ReshapeMat2Vec.cpp
--rw-r--r--   0        0        0      611 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_SlicingCol.cpp
--rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_SlicingVec.cpp
--rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_commainit_01.cpp
--rw-r--r--   0        0        0      113 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_commainit_01b.cpp
--rw-r--r--   0        0        0      215 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_commainit_02.cpp
--rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_range_for_loop_1d_cxx11.cpp
--rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_range_for_loop_2d_cxx11.cpp
--rw-r--r--   0        0        0      249 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_reshaped_vs_resize_1.cpp
--rw-r--r--   0        0        0      372 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_reshaped_vs_resize_2.cpp
--rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_solve_matrix_inverse.cpp
--rw-r--r--   0        0        0      318 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_solve_multiple_rhs.cpp
--rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_solve_reuse_decomposition.cpp
--rw-r--r--   0        0        0      256 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_solve_singular.cpp
--rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_solve_triangular.cpp
--rw-r--r--   0        0        0      159 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_solve_triangular_inplace.cpp
--rw-r--r--   0        0        0      203 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_std_sort.cpp
--rw-r--r--   0        0        0      218 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_std_sort_rows_cxx11.cpp
--rw-r--r--   0        0        0      461 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/VectorwiseOp_homogeneous.cpp
--rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Vectorwise_reverse.cpp
--rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/class_FullPivLU.cpp
--rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/compile_snippet.cpp.in
--rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/tut_arithmetic_redux_minmax.cpp
--rw-r--r--   0        0        0      188 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/tut_arithmetic_transpose_aliasing.cpp
--rw-r--r--   0        0        0      277 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/tut_arithmetic_transpose_conjugate.cpp
--rw-r--r--   0        0        0      174 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/tut_arithmetic_transpose_inplace.cpp
--rw-r--r--   0        0        0      193 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/tut_matrix_assignment_resizing.cpp
--rw-r--r--   0        0        0     1114 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/special_examples/CMakeLists.txt
--rw-r--r--   0        0        0     1184 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/special_examples/Tutorial_sparse_example.cpp
--rw-r--r--   0        0        0     1576 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/special_examples/Tutorial_sparse_example_details.cpp
--rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/special_examples/random_cpp11.cpp
--rw-r--r--   0        0        0     2544 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/tutorial.cpp
--rw-r--r--   0        0        0      254 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/eigen3.pc.in
--rw-r--r--   0        0        0     2423 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/CMakeLists.txt
--rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/bdcsvd_int.cpp
--rw-r--r--   0        0        0      233 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/block_nonconst_ctor_on_const_xpr_0.cpp
--rw-r--r--   0        0        0      233 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/block_nonconst_ctor_on_const_xpr_1.cpp
--rw-r--r--   0        0        0      261 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/block_nonconst_ctor_on_const_xpr_2.cpp
--rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/block_on_const_type_actually_const_0.cpp
--rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/block_on_const_type_actually_const_1.cpp
--rw-r--r--   0        0        0      257 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/colpivqr_int.cpp
--rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/const_qualified_block_method_retval_0.cpp
--rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/const_qualified_block_method_retval_1.cpp
--rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/const_qualified_diagonal_method_retval.cpp
--rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/const_qualified_transpose_method_retval.cpp
--rw-r--r--   0        0        0      271 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/cwiseunaryview_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0        0        0      296 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/cwiseunaryview_on_const_type_actually_const.cpp
--rw-r--r--   0        0        0      228 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/diagonal_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/diagonal_on_const_type_actually_const.cpp
--rw-r--r--   0        0        0      276 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/eigensolver_cplx.cpp
--rw-r--r--   0        0        0      259 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/eigensolver_int.cpp
--rw-r--r--   0        0        0      156 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/failtest_sanity_check.cpp
--rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/fullpivlu_int.cpp
--rw-r--r--   0        0        0      258 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/fullpivqr_int.cpp
--rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/initializer_list_1.cpp
--rw-r--r--   0        0        0      222 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/initializer_list_2.cpp
--rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/jacobisvd_int.cpp
--rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/ldlt_int.cpp
--rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/llt_int.cpp
--rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_0.cpp
--rw-r--r--   0        0        0      246 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_1.cpp
--rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_2.cpp
--rw-r--r--   0        0        0      314 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_3.cpp
--rw-r--r--   0        0        0      321 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_4.cpp
--rw-r--r--   0        0        0      249 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/map_on_const_type_actually_const_0.cpp
--rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/map_on_const_type_actually_const_1.cpp
--rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/partialpivlu_int.cpp
--rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/qr_int.cpp
--rw-r--r--   0        0        0      263 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/ref_1.cpp
--rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/ref_2.cpp
--rw-r--r--   0        0        0      231 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/ref_3.cpp
--rw-r--r--   0        0        0      227 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/ref_4.cpp
--rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/ref_5.cpp
--rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/selfadjointview_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/selfadjointview_on_const_type_actually_const.cpp
--rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/sparse_ref_1.cpp
--rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/sparse_ref_2.cpp
--rw-r--r--   0        0        0      271 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/sparse_ref_3.cpp
--rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/sparse_ref_4.cpp
--rw-r--r--   0        0        0      285 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/sparse_ref_5.cpp
--rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/sparse_storage_mismatch.cpp
--rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/swap_1.cpp
--rw-r--r--   0        0        0      211 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/swap_2.cpp
--rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/ternary_1.cpp
--rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/ternary_2.cpp
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/transpose_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0        0        0      254 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/transpose_on_const_type_actually_const.cpp
--rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/triangularview_nonconst_ctor_on_const_xpr.cpp
--rw-r--r--   0        0        0      265 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/triangularview_on_const_type_actually_const.cpp
--rw-r--r--   0        0        0    10876 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/CMakeLists.txt
--rw-r--r--   0        0        0     2205 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/cholesky.cpp
--rw-r--r--   0        0        0     2831 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/clacgv.f
--rw-r--r--   0        0        0     2340 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/cladiv.f
--rw-r--r--   0        0        0     6295 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/clarf.f
--rw-r--r--   0        0        0    23424 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/clarfb.f
--rw-r--r--   0        0        0     5344 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/clarfg.f
--rw-r--r--   0        0        0    10450 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/clarft.f
--rw-r--r--   0        0        0      578 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/complex_double.cpp
--rw-r--r--   0        0        0      577 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/complex_single.cpp
--rw-r--r--   0        0        0     2969 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dladiv.f
--rw-r--r--   0        0        0     5259 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dlamch.f
--rw-r--r--   0        0        0     2514 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dlapy2.f
--rw-r--r--   0        0        0     2737 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dlapy3.f
--rw-r--r--   0        0        0     6167 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dlarf.f
--rw-r--r--   0        0        0    22749 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dlarfb.f
--rw-r--r--   0        0        0     4946 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dlarfg.f
--rw-r--r--   0        0        0    10222 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dlarft.f
--rw-r--r--   0        0        0      562 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/double.cpp
--rw-r--r--   0        0        0     1282 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dsecnd_NONE.f
--rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/eigenvalues.cpp
--rw-r--r--   0        0        0     2957 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/ilaclc.f
--rw-r--r--   0        0        0     2997 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/ilaclr.f
--rw-r--r--   0        0        0     2952 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/iladlc.f
--rw-r--r--   0        0        0     3000 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/iladlr.f
--rw-r--r--   0        0        0     2941 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/ilaslc.f
--rw-r--r--   0        0        0     2988 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/ilaslr.f
--rw-r--r--   0        0        0     2962 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/ilazlc.f
--rw-r--r--   0        0        0     3010 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/ilazlr.f
--rw-r--r--   0        0        0      877 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/lapack_common.h
--rw-r--r--   0        0        0     2655 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/lu.cpp
--rw-r--r--   0        0        0     1258 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/second_NONE.f
--rw-r--r--   0        0        0      561 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/single.cpp
--rw-r--r--   0        0        0     2897 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/sladiv.f
--rw-r--r--   0        0        0     5261 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/slamch.f
--rw-r--r--   0        0        0     2490 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/slapy2.f
--rw-r--r--   0        0        0     2701 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/slapy3.f
--rw-r--r--   0        0        0     6117 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/slarf.f
--rw-r--r--   0        0        0    22727 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/slarfb.f
--rw-r--r--   0        0        0     4908 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/slarfg.f
--rw-r--r--   0        0        0    10183 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/slarft.f
--rw-r--r--   0        0        0     4891 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/svd.cpp
--rw-r--r--   0        0        0     2839 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/zlacgv.f
--rw-r--r--   0        0        0     2364 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/zladiv.f
--rw-r--r--   0        0        0     6278 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/zlarf.f
--rw-r--r--   0        0        0    23498 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/zlarfb.f
--rw-r--r--   0        0        0     5359 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/zlarfg.f
--rw-r--r--   0        0        0    10453 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/zlarft.f
--rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/CMakeLists.txt
--rwxr-xr-x   0        0        0      577 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/buildtests.in
--rw-r--r--   0        0        0     1569 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/cdashtesting.cmake.in
--rwxr-xr-x   0        0        0      670 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/check.in
--rwxr-xr-x   0        0        0       44 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/debug.in
--rw-r--r--   0        0        0     6384 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/eigen_gen_credits.cpp
--rw-r--r--   0        0        0      738 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/eigen_gen_docs
--rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/eigen_gen_split_test_help.cmake
--rwxr-xr-x   0        0        0     1009 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/eigen_monitor_perf.sh
--rwxr-xr-x   0        0        0       46 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/release.in
--rw-r--r--   0        0        0     2368 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/relicense.py
--rw-r--r--   0        0        0      216 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/signature_of_eigen3_matrix_library
--rw-r--r--   0        0        0     5707 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/AnnoyingScalar.h
--rw-r--r--   0        0        0    14452 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/CMakeLists.txt
--rw-r--r--   0        0        0     1079 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/MovableScalar.h
--rw-r--r--   0        0        0      605 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/SafeScalar.h
--rw-r--r--   0        0        0     8668 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/adjoint.cpp
--rw-r--r--   0        0        0    27758 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/array_cwise.cpp
--rw-r--r--   0        0        0    12883 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/array_for_matrix.cpp
--rw-r--r--   0        0        0      961 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/array_of_string.cpp
--rw-r--r--   0        0        0     2342 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/array_replicate.cpp
--rw-r--r--   0        0        0     6383 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/array_reverse.cpp
--rw-r--r--   0        0        0     2432 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/bandmatrix.cpp
--rw-r--r--   0        0        0    13366 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/basicstuff.cpp
--rw-r--r--   0        0        0     4443 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/bdcsvd.cpp
--rw-r--r--   0        0        0    17931 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/bfloat16_float.cpp
--rw-r--r--   0        0        0     1473 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/bicgstab.cpp
--rw-r--r--   0        0        0     6413 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/blasutil.cpp
--rw-r--r--   0        0        0    14816 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/block.cpp
--rw-r--r--   0        0        0     5731 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/boostmultiprec.cpp
--rw-r--r--   0        0        0      174 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/bug1213.cpp
--rw-r--r--   0        0        0      147 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/bug1213.h
--rw-r--r--   0        0        0      279 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/bug1213_main.cpp
--rw-r--r--   0        0        0    18340 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/cholesky.cpp
--rw-r--r--   0        0        0     3377 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/cholmod_support.cpp
--rw-r--r--   0        0        0     3150 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/commainitializer.cpp
--rw-r--r--   0        0        0     1543 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/conjugate_gradient.cpp
--rw-r--r--   0        0        0     5369 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/conservative_resize.cpp
--rw-r--r--   0        0        0     2562 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/constructor.cpp
--rw-r--r--   0        0        0     6448 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/corners.cpp
--rw-r--r--   0        0        0     2016 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/ctorleak.cpp
--rw-r--r--   0        0        0     5062 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/denseLM.cpp
--rw-r--r--   0        0        0     7256 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/dense_storage.cpp
--rw-r--r--   0        0        0     2275 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/determinant.cpp
--rw-r--r--   0        0        0     4115 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/diagonal.cpp
--rw-r--r--   0        0        0     6686 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/diagonal_matrix_variadic_ctor.cpp
--rw-r--r--   0        0        0     7531 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/diagonalmatrices.cpp
--rw-r--r--   0        0        0     2229 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/dontalign.cpp
--rw-r--r--   0        0        0     4760 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/dynalloc.cpp
--rw-r--r--   0        0        0     2196 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/eigen2support.cpp
--rw-r--r--   0        0        0     6221 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/eigensolver_complex.cpp
--rw-r--r--   0        0        0     4046 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/eigensolver_generalized_real.cpp
--rw-r--r--   0        0        0     9459 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/eigensolver_generic.cpp
--rw-r--r--   0        0        0    11419 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/eigensolver_selfadjoint.cpp
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/evaluator_common.h
--rw-r--r--   0        0        0    21038 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/evaluators.cpp
--rw-r--r--   0        0        0     1916 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/exceptions.cpp
--rw-r--r--   0        0        0     5256 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/fastmath.cpp
--rw-r--r--   0        0        0     1874 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/first_aligned.cpp
--rw-r--r--   0        0        0    18093 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/geo_alignedbox.cpp
--rw-r--r--   0        0        0     3562 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/geo_eulerangles.cpp
--rw-r--r--   0        0        0     5470 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/geo_homogeneous.cpp
--rw-r--r--   0        0        0     7304 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/geo_hyperplane.cpp
--rw-r--r--   0        0        0     4838 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/geo_orthomethods.cpp
--rw-r--r--   0        0        0     4974 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/geo_parametrizedline.cpp
--rw-r--r--   0        0        0    11568 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/geo_quaternion.cpp
--rw-r--r--   0        0        0    26366 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/geo_transformations.cpp
--rw-r--r--   0        0        0    16082 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/gpu_basic.cu
--rw-r--r--   0        0        0     5456 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/gpu_common.h
--rw-r--r--   0        0        0    14524 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/half_float.cpp
--rw-r--r--   0        0        0     2404 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/hessenberg.cpp
--rw-r--r--   0        0        0     6286 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/householder.cpp
--rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/incomplete_cholesky.cpp
--rw-r--r--   0        0        0    19424 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/indexed_view.cpp
--rw-r--r--   0        0        0    12744 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/initializer_list_construction.cpp
--rw-r--r--   0        0        0     3880 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/inplace_decomposition.cpp
--rw-r--r--   0        0        0     5793 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/integer_types.cpp
--rw-r--r--   0        0        0     4701 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/inverse.cpp
--rw-r--r--   0        0        0     1833 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/io.cpp
--rw-r--r--   0        0        0     1368 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/is_same_dense.cpp
--rw-r--r--   0        0        0     2733 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/jacobi.cpp
--rw-r--r--   0        0        0     5877 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/jacobisvd.cpp
--rw-r--r--   0        0        0      955 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/klu_support.cpp
--rw-r--r--   0        0        0     6130 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/linearstructure.cpp
--rw-r--r--   0        0        0     1499 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/lscg.cpp
--rw-r--r--   0        0        0     9075 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/lu.cpp
--rw-r--r--   0        0        0    33109 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/main.h
--rw-r--r--   0        0        0     7943 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/mapped_matrix.cpp
--rw-r--r--   0        0        0     7471 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/mapstaticmethods.cpp
--rw-r--r--   0        0        0    11369 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/mapstride.cpp
--rw-r--r--   0        0        0     7339 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/meta.cpp
--rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/metis_support.cpp
--rw-r--r--   0        0        0     1789 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/miscmatrices.cpp
--rw-r--r--   0        0        0    17824 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/mixingtypes.cpp
--rw-r--r--   0        0        0      635 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/mpl2only.cpp
--rw-r--r--   0        0        0     1208 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/nestbyvalue.cpp
--rw-r--r--   0        0        0     4377 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/nesting_ops.cpp
--rw-r--r--   0        0        0     8700 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/nomalloc.cpp
--rw-r--r--   0        0        0    12806 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/nullary.cpp
--rw-r--r--   0        0        0     3212 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/num_dimensions.cpp
--rw-r--r--   0        0        0     9042 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/numext.cpp
--rw-r--r--   0        0        0    55436 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/packetmath.cpp
--rw-r--r--   0        0        0     9016 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/packetmath_test_shared.h
--rw-r--r--   0        0        0      955 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/pardiso_support.cpp
--rw-r--r--   0        0        0     1902 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/pastix_support.cpp
--rw-r--r--   0        0        0     7031 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/permutationmatrices.cpp
--rw-r--r--   0        0        0     3120 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/prec_inverse_4x4.cpp
--rw-r--r--   0        0        0    11880 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product.h
--rw-r--r--   0        0        0    15711 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_extra.cpp
--rw-r--r--   0        0        0     5395 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_large.cpp
--rw-r--r--   0        0        0     4447 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_mmtr.cpp
--rw-r--r--   0        0        0    10988 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_notemporary.cpp
--rw-r--r--   0        0        0     3510 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_selfadjoint.cpp
--rw-r--r--   0        0        0    12656 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_small.cpp
--rw-r--r--   0        0        0     6133 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_symm.cpp
--rw-r--r--   0        0        0     7856 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_syrk.cpp
--rw-r--r--   0        0        0     6921 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_trmm.cpp
--rw-r--r--   0        0        0     4250 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_trmv.cpp
--rw-r--r--   0        0        0     6102 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_trsolve.cpp
--rw-r--r--   0        0        0     4673 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/qr.cpp
--rw-r--r--   0        0        0    13867 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/qr_colpivoting.cpp
--rw-r--r--   0        0        0     5600 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/qr_fullpivoting.cpp
--rw-r--r--   0        0        0     4621 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/qtvector.cpp
--rw-r--r--   0        0        0     4373 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/rand.cpp
--rw-r--r--   0        0        0     7174 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/random_without_cast_overflow.h
--rw-r--r--   0        0        0     3102 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/real_qz.cpp
--rw-r--r--   0        0        0     8239 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/redux.cpp
--rw-r--r--   0        0        0    14363 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/ref.cpp
--rw-r--r--   0        0        0    10706 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/reshape.cpp
--rw-r--r--   0        0        0     1105 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/resize.cpp
--rw-r--r--   0        0        0     5668 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/rvalue_types.cpp
--rw-r--r--   0        0        0     3569 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/schur_complex.cpp
--rw-r--r--   0        0        0     3964 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/schur_real.cpp
--rw-r--r--   0        0        0     2419 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/selfadjoint.cpp
--rw-r--r--   0        0        0     2564 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/simplicial_cholesky.cpp
--rw-r--r--   0        0        0     2038 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sizeof.cpp
--rw-r--r--   0        0        0     2639 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sizeoverflow.cpp
--rw-r--r--   0        0        0     2133 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/smallvectors.cpp
--rw-r--r--   0        0        0     1716 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/solverbase.h
--rw-r--r--   0        0        0     6216 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse.h
--rw-r--r--   0        0        0     4740 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparseLM.cpp
--rw-r--r--   0        0        0    29343 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse_basic.cpp
--rw-r--r--   0        0        0    12153 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse_block.cpp
--rw-r--r--   0        0        0     9997 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse_permutations.cpp
--rw-r--r--   0        0        0    25557 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse_product.cpp
--rw-r--r--   0        0        0     6125 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse_ref.cpp
--rw-r--r--   0        0        0    24396 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse_solver.h
--rw-r--r--   0        0        0     5142 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse_solvers.cpp
--rw-r--r--   0        0        0     5087 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse_vector.cpp
--rw-r--r--   0        0        0     1791 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparselu.cpp
--rw-r--r--   0        0        0     4587 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparseqr.cpp
--rw-r--r--   0        0        0     1762 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/special_numbers.cpp
--rw-r--r--   0        0        0   159516 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/split_test_helper.h
--rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/spqr_support.cpp
--rw-r--r--   0        0        0    10379 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/stable_norm.cpp
--rw-r--r--   0        0        0     4260 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/stddeque.cpp
--rw-r--r--   0        0        0     4738 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/stddeque_overload.cpp
--rw-r--r--   0        0        0     4232 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/stdlist.cpp
--rw-r--r--   0        0        0     5852 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/stdlist_overload.cpp
--rw-r--r--   0        0        0     5116 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/stdvector.cpp
--rw-r--r--   0        0        0     5014 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/stdvector_overload.cpp
--rw-r--r--   0        0        0    19411 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/stl_iterators.cpp
--rw-r--r--   0        0        0      956 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/superlu_support.cpp
--rw-r--r--   0        0        0    19317 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/svd_common.h
--rw-r--r--   0        0        0     4050 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/svd_fill.h
--rw-r--r--   0        0        0     2940 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/swap.cpp
--rw-r--r--   0        0        0     2742 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/symbolic_index.cpp
--rw-r--r--   0        0        0    11918 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/triangular.cpp
--rw-r--r--   0        0        0     2024 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/type_alias.cpp
--rw-r--r--   0        0        0     5859 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/umeyama.cpp
--rw-r--r--   0        0        0     1171 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/umfpack_support.cpp
--rw-r--r--   0        0        0     2565 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/unalignedcount.cpp
--rw-r--r--   0        0        0     1716 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/upperbidiagonalization.cpp
--rw-r--r--   0        0        0    20351 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/vectorization_logic.cpp
--rw-r--r--   0        0        0    11489 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/vectorwiseop.cpp
--rw-r--r--   0        0        0     6384 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/visitor.cpp
--rw-r--r--   0        0        0     3734 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/zerosized.cpp
--rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/CMakeLists.txt
--rw-r--r--   0        0        0     4422 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/AdolcForward
--rw-r--r--   0        0        0     6349 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/AlignedVector3
--rw-r--r--   0        0        0      884 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/ArpackSupport
--rw-r--r--   0        0        0     1181 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/AutoDiff
--rw-r--r--   0        0        0     5523 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/BVH
--rw-r--r--   0        0        0      603 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CMakeLists.txt
--rw-r--r--   0        0        0      307 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/CMakeLists.txt
--rw-r--r--   0        0        0     4187 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/Tensor
--rw-r--r--   0        0        0     1267 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/TensorSymmetry
--rw-r--r--   0        0        0     2087 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/ThreadPool
--rw-r--r--   0        0        0    62365 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/README.md
--rw-r--r--   0        0        0    21269 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
--rw-r--r--   0        0        0    12448 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
--rw-r--r--   0        0        0    10323 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
--rw-r--r--   0        0        0    57932 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
--rw-r--r--   0        0        0    60851 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h
--rw-r--r--   0        0        0    42150 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
--rw-r--r--   0        0        0    19707 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
--rw-r--r--   0        0        0    15665 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
--rw-r--r--   0        0        0    45320 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
--rw-r--r--   0        0        0     2675 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
--rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
--rw-r--r--   0        0        0    63402 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h
--rw-r--r--   0        0        0    23586 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
--rwxr-xr-x   0        0        0    89042 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h
--rw-r--r--   0        0        0    70687 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
--rw-r--r--   0        0        0    18803 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
--rw-r--r--   0        0        0    48686 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
--rw-r--r--   0        0        0    27527 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h
--rw-r--r--   0        0        0     8642 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
--rw-r--r--   0        0        0    13146 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
--rw-r--r--   0        0        0     4896 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
--rw-r--r--   0        0        0      215 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
--rw-r--r--   0        0        0     3427 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
--rw-r--r--   0        0        0    12837 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h
--rw-r--r--   0        0        0    40367 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
--rw-r--r--   0        0        0    15203 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
--rw-r--r--   0        0        0     7674 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
--rw-r--r--   0        0        0    17751 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
--rw-r--r--   0        0        0     8556 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
--rw-r--r--   0        0        0    40005 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
--rw-r--r--   0        0        0    26655 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
--rw-r--r--   0        0        0    16115 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
--rw-r--r--   0        0        0    24345 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
--rw-r--r--   0        0        0    14486 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
--rw-r--r--   0        0        0     8782 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
--rw-r--r--   0        0        0     8320 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
--rw-r--r--   0        0        0    15269 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
--rw-r--r--   0        0        0    10920 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
--rw-r--r--   0        0        0     1316 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
--rw-r--r--   0        0        0     4068 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h
--rw-r--r--   0        0        0     1267 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h
--rw-r--r--   0        0        0     2560 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
--rw-r--r--   0        0        0    28066 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
--rw-r--r--   0        0        0    25692 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
--rw-r--r--   0        0        0     9094 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
--rw-r--r--   0        0        0     2730 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
--rw-r--r--   0        0        0     9041 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
--rw-r--r--   0        0        0     7769 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
--rw-r--r--   0        0        0     3642 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
--rw-r--r--   0        0        0    14191 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
--rw-r--r--   0        0        0     8104 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
--rw-r--r--   0        0        0    43284 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
--rw-r--r--   0        0        0    28764 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
--rw-r--r--   0        0        0    11474 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
--rw-r--r--   0        0        0    12385 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
--rw-r--r--   0        0        0    44395 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h
--rw-r--r--   0        0        0    40719 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h
--rw-r--r--   0        0        0    30074 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
--rw-r--r--   0        0        0    14793 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
--rw-r--r--   0        0        0    16938 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
--rw-r--r--   0        0        0    20091 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
--rw-r--r--   0        0        0    25279 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h
--rw-r--r--   0        0        0    18256 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
--rw-r--r--   0        0        0     5481 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
--rw-r--r--   0        0        0    13513 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
--rw-r--r--   0        0        0    10152 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h
--rw-r--r--   0        0        0     9432 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
--rw-r--r--   0        0        0     7552 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
--rw-r--r--   0        0        0    30089 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
--rw-r--r--   0        0        0    10857 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
--rw-r--r--   0        0        0     9086 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
--rw-r--r--   0        0        0    13021 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
--rw-r--r--   0        0        0    21046 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
--rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h
--rw-r--r--   0        0        0     9121 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
--rw-r--r--   0        0        0    17075 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
--rw-r--r--   0        0        0     9366 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
--rw-r--r--   0        0        0      774 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h
--rw-r--r--   0        0        0     1209 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
--rw-r--r--   0        0        0    11482 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
--rw-r--r--   0        0        0     1680 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
--rw-r--r--   0        0        0      715 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
--rw-r--r--   0        0        0    22752 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
--rw-r--r--   0        0        0     4115 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
--rw-r--r--   0        0        0     8155 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/EmulateArray.h
--rw-r--r--   0        0        0     4174 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
--rw-r--r--   0        0        0     1126 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/EulerAngles
--rw-r--r--   0        0        0    13948 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/FFT
--rw-r--r--   0        0        0     1561 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/IterativeSolvers
--rw-r--r--   0        0        0      944 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/KroneckerProduct
--rw-r--r--   0        0        0     1238 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/LevenbergMarquardt
--rw-r--r--   0        0        0     7656 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/MPRealSupport
--rw-r--r--   0        0        0    17919 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/MatrixFunctions
--rw-r--r--   0        0        0      592 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/MoreVectorization
--rw-r--r--   0        0        0     5963 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/NonLinearOptimization
--rw-r--r--   0        0        0     1779 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/NumericalDiff
--rw-r--r--   0        0        0    19072 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/OpenGLSupport
--rw-r--r--   0        0        0     4749 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/Polynomials
--rw-r--r--   0        0        0      930 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/Skyline
--rw-r--r--   0        0        0     1360 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/SparseExtra
--rw-r--r--   0        0        0     2951 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/SpecialFunctions
--rw-r--r--   0        0        0      996 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/Splines
--rw-r--r--   0        0        0     3150 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
--rwxr-xr-x   0        0        0    29107 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
--rw-r--r--   0        0        0     9029 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
--rw-r--r--   0        0        0    12976 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/BVH/BVAlgorithms.h
--rw-r--r--   0        0        0     9166 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/BVH/KdBVH.h
--rw-r--r--   0        0        0    29075 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
--rw-r--r--   0        0        0      174 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/CMakeLists.txt
--rw-r--r--   0        0        0    15367 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/EulerAngles.h
--rw-r--r--   0        0        0    11620 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/EulerSystem.h
--rw-r--r--   0        0        0     9223 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/FFT/ei_fftw_impl.h
--rw-r--r--   0        0        0    13231 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
--rw-r--r--   0        0        0     5324 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
--rw-r--r--   0        0        0    17769 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
--rw-r--r--   0        0        0    10209 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/GMRES.h
--rwxr-xr-x   0        0        0    14794 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IDRS.h
--rw-r--r--   0        0        0     2520 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
--rw-r--r--   0        0        0     5360 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IterationController.h
--rw-r--r--   0        0        0    12397 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/MINRES.h
--rw-r--r--   0        0        0     5853 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/Scaling.h
--rw-r--r--   0        0        0    10250 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
--rw-r--r--   0        0        0     2194 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt
--rw-r--r--   0        0        0     2443 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
--rw-r--r--   0        0        0     6648 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
--rw-r--r--   0        0        0     5039 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
--rw-r--r--   0        0        0     6805 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
--rw-r--r--   0        0        0    13297 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
--rw-r--r--   0        0        0    16624 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
--rw-r--r--   0        0        0    22671 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
--rw-r--r--   0        0        0    17557 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
--rw-r--r--   0        0        0    23422 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
--rw-r--r--   0        0        0    14212 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
--rw-r--r--   0        0        0     2107 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
--rw-r--r--   0        0        0     3035 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
--rw-r--r--   0        0        0    19837 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
--rw-r--r--   0        0        0    22135 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
--rw-r--r--   0        0        0     1864 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/chkder.h
--rw-r--r--   0        0        0     1915 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/covar.h
--rw-r--r--   0        0        0     3297 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
--rw-r--r--   0        0        0     2225 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
--rw-r--r--   0        0        0     9111 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
--rw-r--r--   0        0        0     3264 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
--rw-r--r--   0        0        0     1081 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
--rw-r--r--   0        0        0     3083 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
--rw-r--r--   0        0        0     1362 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
--rw-r--r--   0        0        0     4020 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
--rw-r--r--   0        0        0     8076 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Polynomials/Companion.h
--rw-r--r--   0        0        0    15683 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
--rw-r--r--   0        0        0     4806 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
--rw-r--r--   0        0        0    11365 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
--rw-r--r--   0        0        0    31105 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineMatrix.h
--rw-r--r--   0        0        0     7837 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
--rw-r--r--   0        0        0    10853 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineProduct.h
--rw-r--r--   0        0        0     7966 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineStorage.h
--rw-r--r--   0        0        0     3153 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineUtil.h
--rw-r--r--   0        0        0     4260 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h
--rw-r--r--   0        0        0    40316 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
--rw-r--r--   0        0        0    13744 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h
--rw-r--r--   0        0        0     8416 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/MarketIO.h
--rw-r--r--   0        0        0     7568 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
--rw-r--r--   0        0        0    12423 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/RandomSetter.h
--rw-r--r--   0        0        0    10015 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h
--rw-r--r--   0        0        0     2724 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h
--rw-r--r--   0        0        0    12641 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h
--rw-r--r--   0        0        0     2544 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h
--rw-r--r--   0        0        0    69632 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h
--rw-r--r--   0        0        0     4006 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h
--rw-r--r--   0        0        0     2489 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h
--rw-r--r--   0        0        0     7694 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
--rw-r--r--   0        0        0     3087 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h
--rw-r--r--   0        0        0    11700 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
--rw-r--r--   0        0        0     2899 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
--rw-r--r--   0        0        0    58539 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
--rw-r--r--   0        0        0     3713 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
--rw-r--r--   0        0        0     1492 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h
--rw-r--r--   0        0        0      398 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX/SpecialFunctions.h
--rw-r--r--   0        0        0     1549 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h
--rw-r--r--   0        0        0      415 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/SpecialFunctions.h
--rw-r--r--   0        0        0    10864 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h
--rw-r--r--   0        0        0     2258 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h
--rw-r--r--   0        0        0     1283 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h
--rw-r--r--   0        0        0    18307 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Splines/Spline.h
--rw-r--r--   0        0        0    16505 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Splines/SplineFitting.h
--rw-r--r--   0        0        0     4312 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Splines/SplineFwd.h
--rw-r--r--   0        0        0     1876 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/README.txt
--rw-r--r--   0        0        0     3906 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/bench/bench_svd.cpp
--rw-r--r--   0        0        0      114 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/CMakeLists.txt
--rw-r--r--   0        0        0      878 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/Overview.dox
--rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/SYCL.dox
--rw-r--r--   0        0        0     5283 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/eigendoxy_layout.xml.in
--rw-r--r--   0        0        0     2108 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/BVH_Example.cpp
--rw-r--r--   0        0        0      736 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/CMakeLists.txt
--rw-r--r--   0        0        0     1847 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/EulerAngles.cpp
--rw-r--r--   0        0        0     2522 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/FFT.cpp
--rw-r--r--   0        0        0      356 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixExponential.cpp
--rw-r--r--   0        0        0      469 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixFunction.cpp
--rw-r--r--   0        0        0      375 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixLogarithm.cpp
--rw-r--r--   0        0        0      364 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixPower.cpp
--rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixPower_optimal.cpp
--rw-r--r--   0        0        0      508 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixSine.cpp
--rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixSinh.cpp
--rw-r--r--   0        0        0      434 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixSquareRoot.cpp
--rw-r--r--   0        0        0     2392 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/PolynomialSolver1.cpp
--rw-r--r--   0        0        0      635 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/PolynomialUtils1.cpp
--rw-r--r--   0        0        0     1409 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/SYCL/CMakeLists.txt
--rw-r--r--   0        0        0     2551 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/SYCL/CwiseMul.cpp
--rw-r--r--   0        0        0     1137 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/snippets/CMakeLists.txt
--rw-r--r--   0        0        0     7190 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/BVH.cpp
--rw-r--r--   0        0        0    15348 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/CMakeLists.txt
--rw-r--r--   0        0        0     9623 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/EulerAngles.cpp
--rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/FFT.cpp
--rw-r--r--   0        0        0     9233 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/FFTW.cpp
--rw-r--r--   0        0        0    64597 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/NonLinearOptimization.cpp
--rw-r--r--   0        0        0     2862 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/NumericalDiff.cpp
--rw-r--r--   0        0        0     2366 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/alignedvector3.cpp
--rw-r--r--   0        0        0    10992 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/autodiff.cpp
--rw-r--r--   0        0        0     2943 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/autodiff_scalar.cpp
--rw-r--r--   0        0        0    16409 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/bessel_functions.cpp
--rw-r--r--   0        0        0     3990 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_eventcount.cpp
--rw-r--r--   0        0        0     1839 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_maxsizevector.cpp
--rw-r--r--   0        0        0    18740 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_meta.cpp
--rw-r--r--   0        0        0     5039 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_non_blocking_thread_pool.cpp
--rw-r--r--   0        0        0     7024 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_runqueue.cpp
--rw-r--r--   0        0        0     9150 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax.cpp
--rw-r--r--   0        0        0     8886 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax_gpu.cu
--rw-r--r--   0        0        0     9949 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax_sycl.cpp
--rw-r--r--   0        0        0     9707 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_assign.cpp
--rw-r--r--   0        0        0    22378 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_block_access.cpp
--rw-r--r--   0        0        0    31888 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_block_eval.cpp
--rw-r--r--   0        0        0    15858 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_block_io.cpp
--rw-r--r--   0        0        0     5708 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_broadcast_sycl.cpp
--rw-r--r--   0        0        0     9209 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_broadcasting.cpp
--rw-r--r--   0        0        0    15767 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_builtins_sycl.cpp
--rw-r--r--   0        0        0     2420 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_cast_float16_gpu.cu
--rw-r--r--   0        0        0     5526 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_casts.cpp
--rw-r--r--   0        0        0    13050 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_chipping.cpp
--rw-r--r--   0        0        0    26158 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_chipping_sycl.cpp
--rw-r--r--   0        0        0     1991 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_comparisons.cpp
--rw-r--r--   0        0        0     2871 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_complex_cwise_ops_gpu.cu
--rw-r--r--   0        0        0     6636 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_complex_gpu.cu
--rw-r--r--   0        0        0     4624 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_concatenation.cpp
--rw-r--r--   0        0        0     8411 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_concatenation_sycl.cpp
--rw-r--r--   0        0        0     1660 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_const.cpp
--rw-r--r--   0        0        0     7350 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_contract_gpu.cu
--rw-r--r--   0        0        0    47521 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_contract_sycl.cpp
--rw-r--r--   0        0        0    23176 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_contraction.cpp
--rw-r--r--   0        0        0     5381 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_convolution.cpp
--rw-r--r--   0        0        0    20033 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_convolution_sycl.cpp
--rw-r--r--   0        0        0     2518 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_index.cpp
--rw-r--r--   0        0        0     3211 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_op.cpp
--rw-r--r--   0        0        0     6806 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_op_sycl.cpp
--rw-r--r--   0        0        0    13495 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_device.cu
--rw-r--r--   0        0        0     3210 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_device_sycl.cpp
--rw-r--r--   0        0        0     2578 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_dimension.cpp
--rw-r--r--   0        0        0      999 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_empty.cpp
--rw-r--r--   0        0        0    30675 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_executor.cpp
--rw-r--r--   0        0        0    14224 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_expr.cpp
--rw-r--r--   0        0        0    13705 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_fft.cpp
--rw-r--r--   0        0        0     7252 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_fixed_size.cpp
--rw-r--r--   0        0        0     2167 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_forced_eval.cpp
--rw-r--r--   0        0        0     3461 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp
--rw-r--r--   0        0        0     2266 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_generator.cpp
--rw-r--r--   0        0        0     5732 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_generator_sycl.cpp
--rw-r--r--   0        0        0    58446 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_gpu.cu
--rw-r--r--   0        0        0     5942 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_ifft.cpp
--rw-r--r--   0        0        0     3890 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_image_op_sycl.cpp
--rw-r--r--   0        0        0    36037 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_image_patch.cpp
--rw-r--r--   0        0        0    62111 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_image_patch_sycl.cpp
--rw-r--r--   0        0        0    18652 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_index_list.cpp
--rw-r--r--   0        0        0     2109 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_inflation.cpp
--rw-r--r--   0        0        0     5101 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_inflation_sycl.cpp
--rw-r--r--   0        0        0     4129 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_intdiv.cpp
--rw-r--r--   0        0        0     3277 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_io.cpp
--rw-r--r--   0        0        0     1639 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_layout_swap.cpp
--rw-r--r--   0        0        0     4730 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_layout_swap_sycl.cpp
--rw-r--r--   0        0        0      950 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_lvalue.cpp
--rw-r--r--   0        0        0     7962 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_map.cpp
--rw-r--r--   0        0        0      993 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_math.cpp
--rw-r--r--   0        0        0     3877 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_math_sycl.cpp
--rw-r--r--   0        0        0     1501 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_mixed_indices.cpp
--rw-r--r--   0        0        0    18215 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_morphing.cpp
--rw-r--r--   0        0        0    17549 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_morphing_sycl.cpp
--rw-r--r--   0        0        0     1734 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_move.cpp
--rw-r--r--   0        0        0     1789 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_notification.cpp
--rw-r--r--   0        0        0     2893 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_of_complex.cpp
--rw-r--r--   0        0        0     2430 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_of_const_values.cpp
--rw-r--r--   0        0        0    21223 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_of_float16_gpu.cu
--rw-r--r--   0        0        0     3766 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_of_strings.cpp
--rw-r--r--   0        0        0     2652 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_padding.cpp
--rw-r--r--   0        0        0     5677 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_padding_sycl.cpp
--rw-r--r--   0        0        0     5499 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_patch.cpp
--rw-r--r--   0        0        0     9385 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_patch_sycl.cpp
--rw-r--r--   0        0        0     2513 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_random.cpp
--rw-r--r--   0        0        0     2355 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_random_gpu.cu
--rw-r--r--   0        0        0     3568 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_random_sycl.cpp
--rw-r--r--   0        0        0    15346 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction.cpp
--rw-r--r--   0        0        0     5410 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction_gpu.cu
--rw-r--r--   0        0        0    42176 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction_sycl.cpp
--rw-r--r--   0        0        0     6722 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_ref.cpp
--rw-r--r--   0        0        0     5285 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reverse.cpp
--rw-r--r--   0        0        0     9283 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reverse_sycl.cpp
--rw-r--r--   0        0        0     1486 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_roundings.cpp
--rw-r--r--   0        0        0     2978 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_scan.cpp
--rw-r--r--   0        0        0     2576 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_scan_gpu.cu
--rw-r--r--   0        0        0     6376 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_scan_sycl.cpp
--rw-r--r--   0        0        0     7692 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_shuffling.cpp
--rw-r--r--   0        0        0     4265 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_shuffling_sycl.cpp
--rw-r--r--   0        0        0     9624 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_simple.cpp
--rw-r--r--   0        0        0     3024 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_striding.cpp
--rw-r--r--   0        0        0     7074 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_striding_sycl.cpp
--rw-r--r--   0        0        0     1896 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_sugar.cpp
--rw-r--r--   0        0        0    14828 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_sycl.cpp
--rw-r--r--   0        0        0    59079 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_symmetry.cpp
--rw-r--r--   0        0        0     4237 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_thread_local.cpp
--rw-r--r--   0        0        0    25491 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_thread_pool.cpp
--rw-r--r--   0        0        0     5129 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_trace.cpp
--rw-r--r--   0        0        0     5757 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_uint128.cpp
--rw-r--r--   0        0        0     4592 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_volume_patch.cpp
--rw-r--r--   0        0        0    11972 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_volume_patch_sycl.cpp
--rw-r--r--   0        0        0     1279 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/dgmres.cpp
--rw-r--r--   0        0        0     3822 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/forward_adolc.cpp
--rw-r--r--   0        0        0     1245 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/gmres.cpp
--rw-r--r--   0        0        0      942 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/idrs.cpp
--rw-r--r--   0        0        0     9075 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/kronecker_product.cpp
--rw-r--r--   0        0        0    55504 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/levenberg_marquardt.cpp
--rw-r--r--   0        0        0     4417 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/matrix_exponential.cpp
--rw-r--r--   0        0        0     7447 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/matrix_function.cpp
--rw-r--r--   0        0        0     2106 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/matrix_functions.h
--rw-r--r--   0        0        0     7178 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/matrix_power.cpp
--rw-r--r--   0        0        0     1050 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/matrix_square_root.cpp
--rw-r--r--   0        0        0     1658 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/minres.cpp
--rw-r--r--   0        0        0     2439 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/mpreal_support.cpp
--rw-r--r--   0        0        0    18637 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/openglsupport.cpp
--rw-r--r--   0        0        0     7486 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/polynomialsolver.cpp
--rw-r--r--   0        0        0     3582 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/polynomialutils.cpp
--rw-r--r--   0        0        0     8414 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/sparse_extra.cpp
--rw-r--r--   0        0        0    22854 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/special_functions.cpp
--rw-r--r--   0        0        0     6372 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/special_packetmath.cpp
--rw-r--r--   0        0        0     8529 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/splines.cpp
--rw-r--r--   0        0        0     3521 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/fcns.cpp
--rw-r--r--   0        0        0    34254 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/C++/main.cpp
--rw-r--r--   0        0        0      134 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/ackleyfcn.tex
--rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/ackleyn2fcn.tex
--rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/ackleyn3fcn.tex
--rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/adjimanfcn.tex
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/alpinen1fcn.tex
--rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/alpinen2fcn.tex
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/bartelsconnfcn.tex
--rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/bealefcn.tex
--rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/birdfcn.tex
--rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/bohachevskyn1fcn.tex
--rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/bohachevskyn2fcn.tex
--rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/boothfcn.tex
--rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/brentfcn.tex
--rw-r--r--   0        0        0       86 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/brownfcn.tex
--rw-r--r--   0        0        0       40 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/bukinn6fcn.tex
--rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/crossintrayfcn.tex
--rw-r--r--   0        0        0       62 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/deckkersaartsfcn.tex
--rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/dropwavefcn.tex
--rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/easomfcn.tex
--rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/eggcratefcn.tex
--rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/elattarfcn.tex
--rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/exponentialfcn.tex
--rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/goldsteinpricefcn.tex
--rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/gramacylacyfcn.tex
--rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/griewankfcn.tex
--rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/happycatfcn.tex
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/himmelblaufcn.tex
--rw-r--r--   0        0        0       58 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/holdertablefcn.tex
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/keanefcn.tex
--rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/leonfcn.tex
--rw-r--r--   0        0        0       74 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/levin13fcn.tex
--rw-r--r--   0        0        0       30 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/matyasfcn.tex
--rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/mccormickfcn.tex
--rw-r--r--   0        0        0       91 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/periodicfcn.tex
--rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/powellsumfcn.tex
--rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/qingfcn.tex
--rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/quarticfcn.tex
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/rastriginfcn.tex
--rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/ridgefcn.tex
--rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/rosenbrockfcn.tex
--rw-r--r--   0        0        0       98 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/salomonfcn.tex
--rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/schaffern1fcn.tex
--rw-r--r--   0        0        0       62 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/schaffern2fcn.tex
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/schaffern3fcn.tex
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/schaffern4fcn.tex
--rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/schwefel220fcn.tex
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/schwefel221fcn.tex
--rw-r--r--   0        0        0       72 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/schwefel222fcn.tex
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/schwefel223fcn.tex
--rw-r--r--   0        0        0       90 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/schwefelfcn.tex
--rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/shubert3fcn.tex
--rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/shubert4fcn.tex
--rw-r--r--   0        0        0       91 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/shubertfcn.tex
--rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/spherefcn.tex
--rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/styblinskitankfcn.tex
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/sumsquaresfcn.tex
--rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/threehumpcamelfcn.tex
--rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/wolfefcn.tex
--rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/xinsheyangn1fcn.tex
--rw-r--r--   0        0        0       83 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/xinsheyangn2fcn.tex
--rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/xinsheyangn3fcn.tex
--rw-r--r--   0        0        0      131 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/xinsheyangn4fcn.tex
--rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/latex/zakharovfcn.tex
--rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/ackleyfcn.m
--rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/ackleyn2fcn.m
--rw-r--r--   0        0        0      833 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/ackleyn3fcn.m
--rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/ackleyn4fcn.m
--rw-r--r--   0        0        0      775 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/adjimanfcn.m
--rw-r--r--   0        0        0      666 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/alpinen1fcn.m
--rw-r--r--   0        0        0      658 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/alpinen2fcn.m
--rw-r--r--   0        0        0      825 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/bartelsconnfcn.m
--rw-r--r--   0        0        0      841 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/bealefcn.m
--rw-r--r--   0        0        0      804 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/birdfcn.m
--rw-r--r--   0        0        0      847 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/bohachevskyn1fcn.m
--rw-r--r--   0        0        0      850 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/bohachevskyn2fcn.m
--rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/boothfcn.m
--rw-r--r--   0        0        0      762 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/brentfcn.m
--rw-r--r--   0        0        0      741 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/brownfcn.m
--rw-r--r--   0        0        0      814 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/bukinn6fcn.m
--rw-r--r--   0        0        0     1898 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/contourfcn.m
--rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/crossintrayfcn.m
--rw-r--r--   0        0        0      846 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/deckkersaartsfcn.m
--rw-r--r--   0        0        0      882 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/dropwavefcn.m
--rw-r--r--   0        0        0      787 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/easomfcn.m
--rw-r--r--   0        0        0      781 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/eggcratefcn.m
--rw-r--r--   0        0        0      902 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/eggholderfcn.m
--rw-r--r--   0        0        0      811 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/elattarfcn.m
--rw-r--r--   0        0        0      657 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/exponentialfcn.m
--rw-r--r--   0        0        0      686 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/giuntafcn.m
--rw-r--r--   0        0        0      990 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/goldsteinpricefcn.m
--rw-r--r--   0        0        0      776 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/gramacyleefcn.m
--rw-r--r--   0        0        0      828 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/griewankfcn.m
--rw-r--r--   0        0        0      855 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/happycatfcn.m
--rw-r--r--   0        0        0      809 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/himmelblaufcn.m
--rw-r--r--   0        0        0      875 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/holdertablefcn.m
--rw-r--r--   0        0        0      843 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/keanefcn.m
--rw-r--r--   0        0        0      737 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/leonfcn.m
--rw-r--r--   0        0        0      873 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/levin13fcn.m
--rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/matyasfcn.m
--rw-r--r--   0        0        0      800 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/mccormickfcn.m
--rw-r--r--   0        0        0     1846 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/meshfcn.m
--rw-r--r--   0        0        0      693 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/periodicfcn.m
--rw-r--r--   0        0        0     1134 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/pichenyfcn.m
--rw-r--r--   0        0        0      811 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/powellsumfcn.m
--rw-r--r--   0        0        0      663 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/qingfcn.m
--rw-r--r--   0        0        0      733 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/quarticfcn.m
--rw-r--r--   0        0        0      682 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/rastriginfcn.m
--rw-r--r--   0        0        0      951 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/ridgefcn.m
--rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/rosenbrockfcn.m
--rw-r--r--   0        0        0      723 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/salomonfcn.m
--rw-r--r--   0        0        0      908 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/schaffern1fcn.m
--rw-r--r--   0        0        0      883 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/schaffern2fcn.m
--rw-r--r--   0        0        0      911 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/schaffern3fcn.m
--rw-r--r--   0        0        0      911 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/schaffern4fcn.m
--rw-r--r--   0        0        0      637 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/schwefel220fcn.m
--rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/schwefel221fcn.m
--rw-r--r--   0        0        0      671 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/schwefel222fcn.m
--rw-r--r--   0        0        0      637 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/schwefel223fcn.m
--rw-r--r--   0        0        0      678 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/schwefelfcn.m
--rw-r--r--   0        0        0      747 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/shubert3fcn.m
--rw-r--r--   0        0        0      743 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/shubert4fcn.m
--rw-r--r--   0        0        0      843 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/shubertfcn.m
--rw-r--r--   0        0        0      585 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/spherefcn.m
--rw-r--r--   0        0        0      810 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/styblinskitankfcn.m
--rw-r--r--   0        0        0      694 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/sumsquaresfcn.m
--rw-r--r--   0        0        0     1848 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/surffcn.m
--rw-r--r--   0        0        0      856 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/threehumpcamelfcn.m
--rw-r--r--   0        0        0      780 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/wolfefcn.m
--rw-r--r--   0        0        0      747 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/xinsheyangn1fcn.m
--rw-r--r--   0        0        0      678 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/xinsheyangn2fcn.m
--rw-r--r--   0        0        0     1456 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/xinsheyangn3fcn.m
--rw-r--r--   0        0        0      718 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/xinsheyangn4fcn.m
--rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/matlab/zakharovfcn.m
--rw-r--r--   0        0        0     2354 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/python/benchmarkfcns/__init__.py
--rw-r--r--   0        0        0     2097 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/python/benchmarkfcns/plotting.py
--rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/src/tests/test_basic.py
--rw-r--r--   0        0        0     2852 2022-11-09 12:37:21.000000 benchmarkfcns-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1656 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/.github/workflows/build.yaml
+-rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/.gitignore
+-rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/.gitmodules
+-rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1104 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/CMakeLists.txt
+-rw-r--r--   0        0        0     1086 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/LICENSE
+-rw-r--r--   0        0        0     5308 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/README.md
+-rw-r--r--   0        0        0   705328 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/image-1.png
+-rw-r--r--   0        0        0     7407 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/optimiser/matlab/abc/FoodSources.m
+-rw-r--r--   0        0        0     6188 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/optimiser/matlab/abc/abc.m
+-rw-r--r--   0        0        0     2242 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/optimiser/matlab/abc/abcoptions.m
+-rw-r--r--   0        0        0    17154 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/optimiser/python/abc.py
+-rw-r--r--   0        0        0     2520 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    28781 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/benchmarkfcns.cpp
+-rw-r--r--   0        0        0     6126 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/benchmarkfcns.h
+-rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/.git
+-rw-r--r--   0        0        0      292 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/.gitignore
+-rw-r--r--   0        0        0     2744 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/.gitlab/issue_templates/Bug Report.md
+-rw-r--r--   0        0        0      201 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/.gitlab/issue_templates/Feature Request.md
+-rw-r--r--   0        0        0     1394 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/.gitlab/merge_request_templates/Merge Request Template.md
+-rw-r--r--   0        0        0      571 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/.hgeol
+-rw-r--r--   0        0        0    24767 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/CMakeLists.txt
+-rw-r--r--   0        0        0    11362 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/COPYING.APACHE
+-rw-r--r--   0        0        0     1517 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/COPYING.BSD
+-rw-r--r--   0        0        0    35147 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/COPYING.GPL
+-rw-r--r--   0        0        0    26530 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/COPYING.LGPL
+-rw-r--r--   0        0        0     2193 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/COPYING.MINPACK
+-rw-r--r--   0        0        0    16726 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/COPYING.MPL2
+-rw-r--r--   0        0        0      779 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/COPYING.README
+-rw-r--r--   0        0        0      584 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/CTestConfig.cmake
+-rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/CTestCustom.cmake.in
+-rw-r--r--   0        0        0     1161 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/Cholesky
+-rw-r--r--   0        0        0     1900 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/CholmodSupport
+-rw-r--r--   0        0        0    12799 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/Core
+-rw-r--r--   0        0        0      122 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/Dense
+-rw-r--r--   0        0        0       35 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/Eigen
+-rw-r--r--   0        0        0     1777 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/Eigenvalues
+-rw-r--r--   0        0        0     1940 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/Geometry
+-rw-r--r--   0        0        0      829 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/Householder
+-rw-r--r--   0        0        0     2083 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/IterativeLinearSolvers
+-rw-r--r--   0        0        0      894 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/Jacobi
+-rw-r--r--   0        0        0     1389 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/KLUSupport
+-rw-r--r--   0        0        0     1268 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/LU
+-rw-r--r--   0        0        0      991 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/MetisSupport
+-rw-r--r--   0        0        0     2451 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/OrderingMethods
+-rw-r--r--   0        0        0     1751 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/PaStiXSupport
+-rw-r--r--   0        0        0     1116 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/PardisoSupport
+-rw-r--r--   0        0        0     1272 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/QR
+-rw-r--r--   0        0        0      900 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/QtAlignedMalloc
+-rw-r--r--   0        0        0     1162 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/SPQRSupport
+-rw-r--r--   0        0        0     1584 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/SVD
+-rw-r--r--   0        0        0      888 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/Sparse
+-rw-r--r--   0        0        0     1235 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/SparseCholesky
+-rw-r--r--   0        0        0     2240 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/SparseCore
+-rw-r--r--   0        0        0     1814 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/SparseLU
+-rw-r--r--   0        0        0     1195 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/SparseQR
+-rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/StdDeque
+-rw-r--r--   0        0        0      726 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/StdList
+-rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/StdVector
+-rw-r--r--   0        0        0     2243 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/SuperLUSupport
+-rw-r--r--   0        0        0     1382 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/UmfPackSupport
+-rw-r--r--   0        0        0    24934 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0        0        0    18760 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0        0        0     3974 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Cholesky/LLT_LAPACKE.h
+-rw-r--r--   0        0        0    25441 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/CholmodSupport/CholmodSupport.h
+-rw-r--r--   0        0        0    19214 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0        0        0    16782 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Array.h
+-rw-r--r--   0        0        0     8217 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0        0        0     7018 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0        0        0     2738 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Assign.h
+-rw-r--r--   0        0        0    41673 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/AssignEvaluator.h
+-rwxr-xr-x   0        0        0    12488 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0        0        0    14075 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0        0        0    18648 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Block.h
+-rw-r--r--   0        0        0     4429 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0        0        0     5981 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0        0        0     6990 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0        0        0    63841 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0        0        0     4745 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0        0        0     7909 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0        0        0    36282 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0        0        0     8256 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0        0        0     3937 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0        0        0     5551 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0        0        0    31529 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0        0        0    24484 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0        0        0    25360 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0        0        0     9870 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0        0        0    14670 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0        0        0      988 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0        0        0    11654 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Dot.h
+-rw-r--r--   0        0        0     5841 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0        0        0     4909 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0        0        0     5759 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0        0        0    21679 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0        0        0    38812 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0        0        0    11543 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0        0        0     8238 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/IO.h
+-rw-r--r--   0        0        0     9620 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0        0        0     3503 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Inverse.h
+-rw-r--r--   0        0        0     7256 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Map.h
+-rw-r--r--   0        0        0    11281 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/MapBase.h
+-rw-r--r--   0        0        0    60784 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0        0        0     7156 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0        0        0    24343 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Matrix.h
+-rw-r--r--   0        0        0    23856 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0        0        0     2520 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0        0        0     3620 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0        0        0    12884 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0        0        0     9207 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0        0        0    20748 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0        0        0    49193 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0        0        0     7336 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Product.h
+-rw-r--r--   0        0        0    53832 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0        0        0     7756 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Random.h
+-rw-r--r--   0        0        0    19195 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Redux.h
+-rw-r--r--   0        0        0    17821 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Ref.h
+-rw-r--r--   0        0        0     5656 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Replicate.h
+-rw-r--r--   0        0        0    17033 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0        0        0     4284 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0        0        0     7522 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Reverse.h
+-rw-r--r--   0        0        0     6143 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Select.h
+-rw-r--r--   0        0        0    14999 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0        0        0     1697 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0        0        0     6837 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Solve.h
+-rw-r--r--   0        0        0     9368 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0        0        0     6170 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0        0        0     8700 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0        0        0    21641 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0        0        0     4212 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Stride.h
+-rw-r--r--   0        0        0     2765 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Swap.h
+-rw-r--r--   0        0        0    17606 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Transpose.h
+-rw-r--r--   0        0        0    13567 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0        0        0    38277 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0        0        0     3488 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0        0        0    35168 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0        0        0    11997 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Visitor.h
+-rw-r--r--   0        0        0    15223 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0        0        0     8102 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0        0        0    64608 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0        0        0     2564 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX/TypeCasting.h
+-rw-r--r--   0        0        0    17160 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0        0        0    13344 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0        0        0    87891 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-r--r--   0        0        0     2134 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX512/TypeCasting.h
+-rw-r--r--   0        0        0    16540 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0        0        0     2323 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0        0        0   119355 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-r--r--   0        0        0     9490 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-r--r--   0        0        0    24820 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rwxr-xr-x   0        0        0   102394 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/PacketMath.h
+-rw-r--r--   0        0        0    17317 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/CUDA/Complex.h
+-rw-r--r--   0        0        0    26903 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-r--r--   0        0        0     5251 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0        0        0    67696 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0        0        0     3770 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-r--r--   0        0        0    35534 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/Half.h
+-rw-r--r--   0        0        0     1746 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/Settings.h
+-rw-r--r--   0        0        0     3746 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/TypeCasting.h
+-rw-r--r--   0        0        0     2695 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0        0        0    57047 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0        0        0     2256 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/GPU/TypeCasting.h
+-rw-r--r--   0        0        0      691 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+-rw-r--r--   0        0        0    17541 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0        0        0    16159 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0        0        0    33615 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/MSA/PacketMath.h
+-rw-r--r--   0        0        0    22503 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0        0        0     6815 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-r--r--   0        0        0     3083 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0        0        0   189525 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0        0        0    51286 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/TypeCasting.h
+-rw-r--r--   0        0        0    14251 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0        0        0     6765 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxr-xr-x   0        0        0    64465 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0        0        0     3650 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SSE/TypeCasting.h
+-rw-r--r--   0        0        0     1194 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-r--r--   0        0        0    21200 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-r--r--   0        0        0     1351 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SVE/TypeCasting.h
+-rw-r--r--   0        0        0     7428 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0        0        0    12539 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0        0        0    27786 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0        0        0    21856 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-r--r--   0        0        0     2626 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/TypeCasting.h
+-rw-r--r--   0        0        0    16728 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0        0        0     8024 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxr-xr-x   0        0        0    36894 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/ZVector/PacketMath.h
+-rw-r--r--   0        0        0     6686 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0        0        0    20921 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0        0        0     8334 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0        0        0     4998 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0        0        0      607 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0        0        0    40146 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/UnaryFunctors.h
+-rw-r--r--   0        0        0   108448 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0        0        0    20104 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0        0        0    15948 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0        0        0     6936 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0        0        0     5106 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0        0        0    21724 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0        0        0     6368 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0        0        0     5582 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0        0        0    21354 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0        0        0    11570 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0        0        0     9958 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0        0        0     5209 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0        0        0     6164 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0        0        0     4126 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0        0        0    20987 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0        0        0    13867 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0        0        0    14722 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0        0        0    10571 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0        0        0    14678 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0        0        0     6707 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0        0        0     5882 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverVector.h
+-rwxr-xr-x   0        0        0    23156 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0        0        0    19876 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0        0        0    21931 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/Constants.h
+-rwxr-xr-x   0        0        0     4892 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0        0        0    15555 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0        0        0     6696 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0        0        0    10949 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/IntegralConstant.h
+-rwxr-xr-x   0        0        0     4268 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0        0        0    52909 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0        0        0    46661 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/Memory.h
+-rwxr-xr-x   0        0        0    29336 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0        0        0     1024 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0        0        0     1432 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0        0        0    10676 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0        0        0    12003 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0        0        0    35762 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/XprHelper.h
+-rw-r--r--   0        0        0    12559 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0        0        0    17274 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0        0        0     4178 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0        0        0    22970 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0        0        0    17176 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0        0        0     9716 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0        0        0    14349 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0        0        0     5575 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0        0        0    23640 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0        0        0    21078 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0        0        0     3650 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0        0        0    35182 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0        0        0     4104 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0        0        0    22764 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/Tridiagonalization.h
+-rw-r--r--   0        0        0    18939 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0        0        0     8403 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0        0        0     3624 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0        0        0    20726 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0        0        0    11962 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0        0        0     8955 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0        0        0     9812 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0        0        0    34367 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0        0        0     6862 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0        0        0     8063 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0        0        0     6724 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0        0        0    61930 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0        0        0     7664 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0        0        0     6190 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Umeyama.h
+-rw-r--r--   0        0        0     5945 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/arch/Geometry_SIMD.h
+-rw-r--r--   0        0        0     4784 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0        0        0     5365 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Householder/Householder.h
+-rw-r--r--   0        0        0    23611 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Householder/HouseholderSequence.h
+-rw-r--r--   0        0        0     6771 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0        0        0     6850 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0        0        0     8887 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0        0        0    15036 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0        0        0    14940 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0        0        0    13379 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0        0        0     7349 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0        0        0     4212 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+-rw-r--r--   0        0        0    16383 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Jacobi/Jacobi.h
+-rw-r--r--   0        0        0    11555 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/KLUSupport/KLUSupport.h
+-rw-r--r--   0        0        0     3439 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/LU/Determinant.h
+-rw-r--r--   0        0        0    32383 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0        0        0    15727 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0        0        0    22069 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0        0        0     3555 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/LU/PartialPivLU_LAPACKE.h
+-rw-r--r--   0        0        0    13693 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/LU/arch/InverseSize4.h
+-rw-r--r--   0        0        0     4588 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/MetisSupport/MetisSupport.h
+-rw-r--r--   0        0        0    16105 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0        0        0    61681 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0        0        0     5248 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/OrderingMethods/Ordering.h
+-rw-r--r--   0        0        0    22249 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/PaStiXSupport/PaStiXSupport.h
+-rw-r--r--   0        0        0    20092 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/PardisoSupport/PardisoSupport.h
+-rw-r--r--   0        0        0    25498 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0        0        0     4662 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0        0        0    23429 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0        0        0    26768 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0        0        0    14641 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0        0        0     2993 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/QR/HouseholderQR_LAPACKE.h
+-rw-r--r--   0        0        0    11826 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+-rw-r--r--   0        0        0    54214 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0        0        0    32988 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0        0        0     5099 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0        0        0    14743 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0        0        0    15957 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SVD/UpperBidiagonalization.h
+-rw-r--r--   0        0        0    24216 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0        0        0     5830 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+-rw-r--r--   0        0        0    10670 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0        0        0     8743 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0        0        0    13166 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0        0        0     2191 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0        0        0    11368 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0        0        0    24360 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0        0        0     6485 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0        0        0    13606 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0        0        0    25524 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0        0        0     4757 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0        0        0    13256 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0        0        0     5808 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0        0        0     3080 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0        0        0     1107 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0        0        0    12589 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0        0        0    57475 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0        0        0    17451 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0        0        0     7329 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0        0        0     7593 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0        0        0     1699 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0        0        0    15600 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0        0        0    25889 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0        0        0     4424 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0        0        0     8704 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0        0        0     3175 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0        0        0     6437 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0        0        0     6827 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0        0        0    14832 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0        0        0     8127 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0        0        0     9657 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/TriangularSolver.h
+-rw-r--r--   0        0        0    33316 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0        0        0     4303 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0        0        0     7602 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0        0        0     4974 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0        0        0    12837 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0        0        0     2049 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0        0        0     6712 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0        0        0     6584 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0        0        0     3681 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0        0        0    10217 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0        0        0     4181 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0        0        0     5723 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0        0        0     8485 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0        0        0     9028 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0        0        0     4979 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0        0        0     4545 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0        0        0     2889 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_relax_snode.h
+-rw-r--r--   0        0        0    29167 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseQR/SparseQR.h
+-rw-r--r--   0        0        0     4730 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0        0        0     4155 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0        0        0     5338 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0        0        0     2809 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/StlSupport/details.h
+-rw-r--r--   0        0        0    34324 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SuperLUSupport/SuperLUSupport.h
+-rw-r--r--   0        0        0    24456 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/UmfPackSupport/UmfPackSupport.h
+-rw-r--r--   0        0        0     2913 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/misc/Image.h
+-rw-r--r--   0        0        0     2742 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/misc/Kernel.h
+-rw-r--r--   0        0        0     1748 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0        0        0    30560 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/misc/blas.h
+-rw-r--r--   0        0        0     7834 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/misc/lapack.h
+-rwxr-xr-x   0        0        0  1058369 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/misc/lapacke.h
+-rw-r--r--   0        0        0      474 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/misc/lapacke_mangling.h
+-rw-r--r--   0        0        0    14060 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0        0        0    21431 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0        0        0    59020 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0        0        0     4828 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0        0        0     6089 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0        0        0    12283 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/IndexedViewMethods.h
+-rw-r--r--   0        0        0     6387 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0        0        0     3350 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0        0        0     6915 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/ReshapedMethods.h
+-rw-r--r--   0        0        0     1145 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/INSTALL
+-rw-r--r--   0        0        0      288 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/README.md
+-rw-r--r--   0        0        0     3932 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/BenchSparseUtil.h
+-rw-r--r--   0        0        0     4486 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/BenchTimer.h
+-rw-r--r--   0        0        0     2529 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/BenchUtil.h
+-rw-r--r--   0        0        0     2008 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/README.txt
+-rw-r--r--   0        0        0    28983 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/analyze-blocking-sizes.cpp
+-rw-r--r--   0        0        0     1421 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/basicbench.cxxlist
+-rw-r--r--   0        0        0     1107 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/basicbenchmark.cpp
+-rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/basicbenchmark.h
+-rw-r--r--   0        0        0     6313 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchBlasGemm.cpp
+-rw-r--r--   0        0        0     3548 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchCholesky.cpp
+-rw-r--r--   0        0        0     5788 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchEigenSolver.cpp
+-rw-r--r--   0        0        0     2806 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchFFT.cpp
+-rw-r--r--   0        0        0     3598 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchGeometry.cpp
+-rw-r--r--   0        0        0     5193 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchVecAdd.cpp
+-rw-r--r--   0        0        0    11435 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/bench_gemm.cpp
+-rw-r--r--   0        0        0     1352 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/bench_move_semantics.cpp
+-rwxr-xr-x   0        0        0      618 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/bench_multi_compilers.sh
+-rw-r--r--   0        0        0    11622 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/bench_norm.cpp
+-rw-r--r--   0        0        0     2159 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/bench_reverse.cpp
+-rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/bench_sum.cpp
+-rwxr-xr-x   0        0        0      651 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/bench_unrolling
+-rw-r--r--   0        0        0    22259 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchmark-blocking-sizes.cpp
+-rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchmark.cpp
+-rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchmarkSlice.cpp
+-rw-r--r--   0        0        0      640 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchmarkX.cpp
+-rw-r--r--   0        0        0      605 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchmarkXcwise.cpp
+-rwxr-xr-x   0        0        0     1209 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchmark_suite
+-rw-r--r--   0        0        0     2782 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/CMakeLists.txt
+-rw-r--r--   0        0        0    18109 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/COPYING
+-rw-r--r--   0        0        0     6447 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/README
+-rw-r--r--   0        0        0     3374 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_aat_product.hh
+-rw-r--r--   0        0        0     3354 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_ata_product.hh
+-rw-r--r--   0        0        0     3670 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_atv_product.hh
+-rw-r--r--   0        0        0     3371 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_axpby.hh
+-rw-r--r--   0        0        0     3340 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_axpy.hh
+-rw-r--r--   0        0        0     3202 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_cholesky.hh
+-rw-r--r--   0        0        0     3460 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_ger.hh
+-rw-r--r--   0        0        0     5598 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_hessenberg.hh
+-rw-r--r--   0        0        0     3151 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_lu_decomp.hh
+-rw-r--r--   0        0        0     3598 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_lu_solve.hh
+-rw-r--r--   0        0        0     3886 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_matrix_matrix_product.hh
+-rw-r--r--   0        0        0     3982 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_matrix_matrix_product_bis.hh
+-rw-r--r--   0        0        0     3989 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_matrix_vector_product.hh
+-rw-r--r--   0        0        0     3188 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_partial_lu.hh
+-rw-r--r--   0        0        0     3019 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_rot.hh
+-rw-r--r--   0        0        0     3691 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_symv.hh
+-rw-r--r--   0        0        0     3664 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_syr2.hh
+-rw-r--r--   0        0        0     3425 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_trisolve.hh
+-rw-r--r--   0        0        0     4061 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_trisolve_matrix.hh
+-rw-r--r--   0        0        0     3907 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_trmm.hh
+-rw-r--r--   0        0        0      464 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/basic_actions.hh
+-rw-r--r--   0        0        0      918 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindACML.cmake
+-rw-r--r--   0        0        0     1290 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindATLAS.cmake
+-rw-r--r--   0        0        0      781 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindBLAZE.cmake
+-rw-r--r--   0        0        0     1058 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindBlitz.cmake
+-rw-r--r--   0        0        0      634 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindCBLAS.cmake
+-rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindGMM.cmake
+-rw-r--r--   0        0        0     1232 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindMKL.cmake
+-rw-r--r--   0        0        0      787 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindMTL4.cmake
+-rw-r--r--   0        0        0      604 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindOPENBLAS.cmake
+-rw-r--r--   0        0        0     2372 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0        0        0      798 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindTvmet.cmake
+-rw-r--r--   0        0        0     1315 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake
+-rw-r--r--   0        0        0      869 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/CMakeLists.txt
+-rw-r--r--   0        0        0     1368 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/action_settings.txt
+-rw-r--r--   0        0        0     2224 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/gnuplot_common_settings.hh
+-rwxr-xr-x   0        0        0     2092 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/go_mean
+-rw-r--r--   0        0        0     5306 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/mean.cxx
+-rw-r--r--   0        0        0     1850 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/mk_gnuplot_script.sh
+-rw-r--r--   0        0        0      929 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/mk_mean_script.sh
+-rwxr-xr-x   0        0        0     1742 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/mk_new_gnuplot.sh
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/perlib_plot_settings.txt
+-rw-r--r--   0        0        0     3425 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/regularize.cxx
+-rw-r--r--   0        0        0     5112 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/smooth.cxx
+-rwxr-xr-x   0        0        0     1687 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/smooth_all.sh
+-rw-r--r--   0        0        0     4827 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/bench.hh
+-rw-r--r--   0        0        0     1916 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/bench_parameter.hh
+-rw-r--r--   0        0        0     6748 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/btl.hh
+-rw-r--r--   0        0        0     1478 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/init/init_function.hh
+-rw-r--r--   0        0        0     2295 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/init/init_matrix.hh
+-rw-r--r--   0        0        0     1416 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/init/init_vector.hh
+-rw-r--r--   0        0        0     2278 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/static/bench_static.hh
+-rw-r--r--   0        0        0     1948 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/static/intel_bench_fixed_size.hh
+-rw-r--r--   0        0        0     2222 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/static/static_size_generator.hh
+-rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/STL_perf_analyzer.hh
+-rw-r--r--   0        0        0     2522 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/STL_timer.hh
+-rw-r--r--   0        0        0     1994 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh
+-rw-r--r--   0        0        0     2938 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/portable_perf_analyzer.hh
+-rw-r--r--   0        0        0     3534 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh
+-rwxr-xr-x   0        0        0     3534 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/portable_timer.hh
+-rw-r--r--   0        0        0     2927 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/x86_perf_analyzer.hh
+-rw-r--r--   0        0        0     5294 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/x86_timer.hh
+-rw-r--r--   0        0        0     1658 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/utils/size_lin_log.hh
+-rw-r--r--   0        0        0     1646 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/utils/size_log.hh
+-rw-r--r--   0        0        0     2745 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/utils/utilities.h
+-rw-r--r--   0        0        0     2214 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/utils/xy_file.hh
+-rw-r--r--   0        0        0     1468 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/CMakeLists.txt
+-rw-r--r--   0        0        0    35158 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/blas.h
+-rw-r--r--   0        0        0     2891 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/blas_interface.hh
+-rw-r--r--   0        0        0     4811 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/blas_interface_impl.hh
+-rw-r--r--   0        0        0     1634 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/c_interface_base.h
+-rw-r--r--   0        0        0     2960 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/main.cpp
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/STL/CMakeLists.txt
+-rw-r--r--   0        0        0     5802 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/STL/STL_interface.hh
+-rw-r--r--   0        0        0     1828 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/STL/main.cpp
+-rw-r--r--   0        0        0      475 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/blaze/CMakeLists.txt
+-rw-r--r--   0        0        0     4122 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/blaze/blaze_interface.hh
+-rw-r--r--   0        0        0     1636 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/blaze/main.cpp
+-rw-r--r--   0        0        0      378 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/CMakeLists.txt
+-rw-r--r--   0        0        0     5364 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/blitz_LU_solve_interface.hh
+-rw-r--r--   0        0        0     4129 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/blitz_interface.hh
+-rw-r--r--   0        0        0     1962 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/btl_blitz.cpp
+-rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/btl_tiny_blitz.cpp
+-rw-r--r--   0        0        0     3100 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/tiny_blitz_interface.hh
+-rw-r--r--   0        0        0      768 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/CMakeLists.txt
+-rw-r--r--   0        0        0     1664 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp
+-rw-r--r--   0        0        0     5151 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/eigen2_interface.hh
+-rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/main_adv.cpp
+-rw-r--r--   0        0        0     1205 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/main_linear.cpp
+-rw-r--r--   0        0        0     1384 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/main_matmat.cpp
+-rw-r--r--   0        0        0     1456 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/main_vecmat.cpp
+-rw-r--r--   0        0        0     3207 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/CMakeLists.txt
+-rw-r--r--   0        0        0     1664 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp
+-rw-r--r--   0        0        0     8187 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/eigen3_interface.hh
+-rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/main_adv.cpp
+-rw-r--r--   0        0        0     1285 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/main_linear.cpp
+-rw-r--r--   0        0        0     1378 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/main_matmat.cpp
+-rw-r--r--   0        0        0     1447 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/main_vecmat.cpp
+-rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/gmm/CMakeLists.txt
+-rw-r--r--   0        0        0     5364 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/gmm/gmm_LU_solve_interface.hh
+-rw-r--r--   0        0        0     4174 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/gmm/gmm_interface.hh
+-rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/gmm/main.cpp
+-rw-r--r--   0        0        0      153 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/mtl4/.kdbgrc.main
+-rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/mtl4/CMakeLists.txt
+-rw-r--r--   0        0        0     1943 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/mtl4/main.cpp
+-rw-r--r--   0        0        0     5364 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh
+-rw-r--r--   0        0        0     4210 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/mtl4/mtl4_interface.hh
+-rw-r--r--   0        0        0     2130 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/CMakeLists.txt
+-rw-r--r--   0        0        0      671 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/main_linear.cpp
+-rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/main_matmat.cpp
+-rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/main_vecmat.cpp
+-rw-r--r--   0        0        0     3190 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/tensor_interface.hh
+-rw-r--r--   0        0        0      131 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/tvmet/CMakeLists.txt
+-rw-r--r--   0        0        0     1460 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/tvmet/main.cpp
+-rw-r--r--   0        0        0     3017 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/tvmet/tvmet_interface.hh
+-rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/ublas/CMakeLists.txt
+-rw-r--r--   0        0        0     1785 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/ublas/main.cpp
+-rw-r--r--   0        0        0     4341 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/ublas/ublas_interface.hh
+-rw-r--r--   0        0        0     3269 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/check_cache_queries.cpp
+-rw-r--r--   0        0        0     6416 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/dense_solvers.cpp
+-rw-r--r--   0        0        0     7243 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/eig33.cpp
+-rw-r--r--   0        0        0     3307 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/geometry.cpp
+-rw-r--r--   0        0        0     6574 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/changesets.txt
+-rw-r--r--   0        0        0      193 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemm.cpp
+-rw-r--r--   0        0        0     1382 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemm_common.h
+-rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemm_settings.txt
+-rw-r--r--   0        0        0      114 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemm_square_settings.txt
+-rw-r--r--   0        0        0      193 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemv.cpp
+-rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemv_common.h
+-rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemv_settings.txt
+-rw-r--r--   0        0        0       88 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemv_square_settings.txt
+-rw-r--r--   0        0        0      205 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemvt.cpp
+-rw-r--r--   0        0        0     2466 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/lazy_gemm.cpp
+-rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/lazy_gemm_settings.txt
+-rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/llt.cpp
+-rwxr-xr-x   0        0        0     2693 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/make_plot.sh
+-rw-r--r--   0        0        0     3813 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/chart_footer.html
+-rw-r--r--   0        0        0    14775 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/chart_header.html
+-rw-r--r--   0        0        0       25 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/footer.html
+-rw-r--r--   0        0        0      884 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/header.html
+-rw-r--r--   0        0        0   151723 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/s1.js
+-rw-r--r--   0        0        0   241320 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/s2.js
+-rwxr-xr-x   0        0        0     4090 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/run.sh
+-rwxr-xr-x   0        0        0     2031 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/runall.sh
+-rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/trmv_lo.cpp
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/trmv_lot.cpp
+-rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/trmv_up.cpp
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/trmv_upt.cpp
+-rw-r--r--   0        0        0     3232 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/product_threshold.cpp
+-rw-r--r--   0        0        0     6006 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/quat_slerp.cpp
+-rw-r--r--   0        0        0     1097 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/quatmul.cpp
+-rw-r--r--   0        0        0     6260 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/sparse_cholesky.cpp
+-rw-r--r--   0        0        0     5101 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/sparse_dense_product.cpp
+-rw-r--r--   0        0        0     3011 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/sparse_lu.cpp
+-rw-r--r--   0        0        0     8999 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/sparse_product.cpp
+-rw-r--r--   0        0        0     3393 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/sparse_randomsetter.cpp
+-rw-r--r--   0        0        0    13761 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/sparse_setter.cpp
+-rw-r--r--   0        0        0     2347 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/sparse_transpose.cpp
+-rw-r--r--   0        0        0     6114 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/sparse_trisolver.cpp
+-rw-r--r--   0        0        0     3061 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/spbench/CMakeLists.txt
+-rw-r--r--   0        0        0     3975 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/spbench/sp_solver.cpp
+-rw-r--r--   0        0        0     1856 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/spbench/spbench.dtd
+-rw-r--r--   0        0        0     3301 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/spbench/spbenchsolver.cpp
+-rw-r--r--   0        0        0    18167 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/spbench/spbenchsolver.h
+-rw-r--r--   0        0        0     3825 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/spbench/spbenchstyle.h
+-rw-r--r--   0        0        0     2831 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/spbench/test_sparseLU.cpp
+-rw-r--r--   0        0        0     6096 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/spmv.cpp
+-rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/README
+-rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/benchmark.h
+-rw-r--r--   0        0        0     6834 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/benchmark_main.cc
+-rw-r--r--   0        0        0     1389 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/contraction_benchmarks_cpu.cc
+-rwxr-xr-x   0        0        0      729 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/eigen_sycl_bench.sh
+-rw-r--r--   0        0        0      647 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/eigen_sycl_bench_contract.sh
+-rw-r--r--   0        0        0    20459 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks.h
+-rw-r--r--   0        0        0     6264 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks_cpu.cc
+-rw-r--r--   0        0        0     3381 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks_fp16_gpu.cu
+-rw-r--r--   0        0        0     3373 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks_gpu.cu
+-rw-r--r--   0        0        0     6273 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks_sycl.cc
+-rw-r--r--   0        0        0    11331 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/tensor_contract_sycl_bench.cc
+-rw-r--r--   0        0        0     1203 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/vdw_new.cpp
+-rw-r--r--   0        0        0     3614 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/BandTriangularSolver.h
+-rw-r--r--   0        0        0     1730 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/CMakeLists.txt
+-rw-r--r--   0        0        0     1608 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/GeneralRank1Update.h
+-rw-r--r--   0        0        0     2036 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/PackedSelfadjointProduct.h
+-rw-r--r--   0        0        0     3165 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/PackedTriangularMatrixVector.h
+-rw-r--r--   0        0        0     3191 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/PackedTriangularSolverVector.h
+-rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/README.txt
+-rw-r--r--   0        0        0     2168 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/Rank2Update.h
+-rw-r--r--   0        0        0     4672 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/common.h
+-rw-r--r--   0        0        0      647 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/complex_double.cpp
+-rw-r--r--   0        0        0      646 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/complex_single.cpp
+-rw-r--r--   0        0        0     1507 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/double.cpp
+-rw-r--r--   0        0        0    15108 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/chbmv.c
+-rw-r--r--   0        0        0    13026 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/chpmv.c
+-rw-r--r--   0        0        0     2310 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/complexdots.c
+-rw-r--r--   0        0        0    18945 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/ctbmv.c
+-rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/d_cnjg.c
+-rw-r--r--   0        0        0      657 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/datatypes.h
+-rw-r--r--   0        0        0     4968 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/drotm.c
+-rw-r--r--   0        0        0     6193 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/drotmg.c
+-rw-r--r--   0        0        0    10188 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/dsbmv.c
+-rw-r--r--   0        0        0     8075 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/dspmv.c
+-rw-r--r--   0        0        0    11657 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/dtbmv.c
+-rw-r--r--   0        0        0     2976 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/lsame.c
+-rw-r--r--   0        0        0      105 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/r_cnjg.c
+-rw-r--r--   0        0        0     4902 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/srotm.c
+-rw-r--r--   0        0        0     6056 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/srotmg.c
+-rw-r--r--   0        0        0    10210 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/ssbmv.c
+-rw-r--r--   0        0        0     8051 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/sspmv.c
+-rw-r--r--   0        0        0    11643 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/stbmv.c
+-rw-r--r--   0        0        0    15144 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/zhbmv.c
+-rw-r--r--   0        0        0    13060 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/zhpmv.c
+-rw-r--r--   0        0        0    18973 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/ztbmv.c
+-rw-r--r--   0        0        0      979 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/fortran/complexdots.f
+-rw-r--r--   0        0        0     5646 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/level1_cplx_impl.h
+-rw-r--r--   0        0        0     3892 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/level1_impl.h
+-rw-r--r--   0        0        0     4267 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/level1_real_impl.h
+-rw-r--r--   0        0        0    12223 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/level2_cplx_impl.h
+-rw-r--r--   0        0        0    25172 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/level2_impl.h
+-rw-r--r--   0        0        0    10499 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/level2_real_impl.h
+-rw-r--r--   0        0        0    38043 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/level3_impl.h
+-rw-r--r--   0        0        0      763 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/single.cpp
+-rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/CMakeLists.txt
+-rw-r--r--   0        0        0    32110 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/cblat1.f
+-rw-r--r--   0        0        0     1546 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/cblat2.dat
+-rw-r--r--   0        0        0   116657 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/cblat2.f
+-rw-r--r--   0        0        0     1046 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/cblat3.dat
+-rw-r--r--   0        0        0   131550 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/cblat3.f
+-rw-r--r--   0        0        0    44820 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/dblat1.f
+-rw-r--r--   0        0        0     1466 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/dblat2.dat
+-rw-r--r--   0        0        0   112335 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/dblat2.f
+-rw-r--r--   0        0        0      882 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/dblat3.dat
+-rw-r--r--   0        0        0   104262 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/dblat3.f
+-rwxr-xr-x   0        0        0     1016 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/runblastest.sh
+-rw-r--r--   0        0        0    43389 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/sblat1.f
+-rw-r--r--   0        0        0     1466 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/sblat2.dat
+-rw-r--r--   0        0        0   112251 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/sblat2.f
+-rw-r--r--   0        0        0      882 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/sblat3.dat
+-rw-r--r--   0        0        0   104172 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/sblat3.f
+-rw-r--r--   0        0        0    32115 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/zblat1.f
+-rw-r--r--   0        0        0     1546 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/zblat2.dat
+-rw-r--r--   0        0        0   117003 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/zblat2.f
+-rw-r--r--   0        0        0     1046 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/zblat3.dat
+-rw-r--r--   0        0        0   131995 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/zblat3.f
+-rw-r--r--   0        0        0      389 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/xerbla.cpp
+-rw-r--r--   0        0        0     6736 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/ci/CTest2JUnit.xsl
+-rw-r--r--   0        0        0     4910 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/ci/README.md
+-rw-r--r--   0        0        0     5024 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/ci/build.gitlab-ci.yml
+-rw-r--r--   0        0        0     3490 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/ci/smoketests.gitlab-ci.yml
+-rw-r--r--   0        0        0    10349 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/ci/test.gitlab-ci.yml
+-rw-r--r--   0        0        0     2171 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/ComputeCppCompilerChecks.cmake
+-rw-r--r--   0        0        0      475 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/ComputeCppIRMap.cmake
+-rw-r--r--   0        0        0      802 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/Eigen3Config.cmake.in
+-rw-r--r--   0        0        0     1397 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/Eigen3ConfigLegacy.cmake.in
+-rw-r--r--   0        0        0     2779 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/EigenConfigureTesting.cmake
+-rw-r--r--   0        0        0     1562 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/EigenDetermineOSVersion.cmake
+-rw-r--r--   0        0        0     1814 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/EigenDetermineVSServicePack.cmake
+-rw-r--r--   0        0        0     2321 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/EigenSmokeTestList.cmake
+-rw-r--r--   0        0        0    29205 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/EigenTesting.cmake
+-rw-r--r--   0        0        0     1196 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/EigenUninstall.cmake
+-rw-r--r--   0        0        0      517 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindAdolc.cmake
+-rw-r--r--   0        0        0    42828 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindBLAS.cmake
+-rw-r--r--   0        0        0    13179 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindBLASEXT.cmake
+-rw-r--r--   0        0        0     2413 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindCHOLMOD.cmake
+-rw-r--r--   0        0        0    16685 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindComputeCpp.cmake
+-rw-r--r--   0        0        0     2636 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindEigen2.cmake
+-rw-r--r--   0        0        0     3509 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindEigen3.cmake
+-rw-r--r--   0        0        0     2783 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindFFTW.cmake
+-rw-r--r--   0        0        0     2943 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindGLEW.cmake
+-rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindGMP.cmake
+-rw-r--r--   0        0        0     4992 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindGSL.cmake
+-rw-r--r--   0        0        0      846 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindGoogleHash.cmake
+-rw-r--r--   0        0        0    11729 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindHWLOC.cmake
+-rw-r--r--   0        0        0     1281 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindKLU.cmake
+-rw-r--r--   0        0        0     9734 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindLAPACK.cmake
+-rw-r--r--   0        0        0     2632 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindMPFR.cmake
+-rw-r--r--   0        0        0     3524 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindMPREAL.cmake
+-rw-r--r--   0        0        0     8969 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindMetis.cmake
+-rw-r--r--   0        0        0    23160 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindPASTIX.cmake
+-rw-r--r--   0        0        0    14417 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindPTSCOTCH.cmake
+-rw-r--r--   0        0        0    12034 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindSCOTCH.cmake
+-rw-r--r--   0        0        0     1142 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindSPQR.cmake
+-rw-r--r--   0        0        0     2482 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindStandardMathLibrary.cmake
+-rw-r--r--   0        0        0     2261 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindSuperLU.cmake
+-rw-r--r--   0        0        0     5111 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindTriSYCL.cmake
+-rw-r--r--   0        0        0     1662 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindUMFPACK.cmake
+-rw-r--r--   0        0        0      910 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/RegexUtils.cmake
+-rw-r--r--   0        0        0      177 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/UseEigen3.cmake
+-rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/debug/gdb/__init__.py
+-rw-r--r--   0        0        0     9617 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/debug/gdb/printers.py
+-rw-r--r--   0        0        0    11661 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/debug/msvc/eigen.natvis
+-rw-r--r--   0        0        0     7566 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/debug/msvc/eigen_autoexp_part.dat
+-rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/CMakeLists.txt
+-rw-r--r--   0        0        0      462 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/mandelbrot/CMakeLists.txt
+-rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/mandelbrot/README
+-rw-r--r--   0        0        0     7509 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/mandelbrot/mandelbrot.cpp
+-rw-r--r--   0        0        0     1888 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/mandelbrot/mandelbrot.h
+-rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/mix_eigen_and_c/README
+-rw-r--r--   0        0        0     4158 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/mix_eigen_and_c/binary_library.cpp
+-rw-r--r--   0        0        0     3346 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/mix_eigen_and_c/binary_library.h
+-rw-r--r--   0        0        0     1616 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/mix_eigen_and_c/example.c
+-rw-r--r--   0        0        0      695 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/CMakeLists.txt
+-rw-r--r--   0        0        0      403 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/README
+-rw-r--r--   0        0        0     5981 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/camera.cpp
+-rw-r--r--   0        0        0     3435 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/camera.h
+-rw-r--r--   0        0        0     3974 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/gpuhelper.cpp
+-rw-r--r--   0        0        0     7177 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/gpuhelper.h
+-rw-r--r--   0        0        0     3927 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/icosphere.cpp
+-rw-r--r--   0        0        0      869 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/icosphere.h
+-rw-r--r--   0        0        0    19192 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/quaternion_demo.cpp
+-rw-r--r--   0        0        0     2635 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/quaternion_demo.h
+-rw-r--r--   0        0        0     1756 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/trackball.cpp
+-rw-r--r--   0        0        0      943 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/trackball.h
+-rw-r--r--   0        0        0    11165 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/AsciiQuickReference.txt
+-rw-r--r--   0        0        0     2425 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/B01_Experimental.dox
+-rw-r--r--   0        0        0     4935 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/CMakeLists.txt
+-rw-r--r--   0        0        0     6332 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/ClassHierarchy.dox
+-rw-r--r--   0        0        0    18692 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/CoeffwiseMathFunctionsTable.dox
+-rw-r--r--   0        0        0     4423 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/CustomizingEigen_CustomScalar.dox
+-rw-r--r--   0        0        0     1337 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/CustomizingEigen_InheritingMatrix.dox
+-rw-r--r--   0        0        0     3658 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/CustomizingEigen_NullaryExpr.dox
+-rw-r--r--   0        0        0     3658 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/CustomizingEigen_Plugins.dox
+-rw-r--r--   0        0        0     5021 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/DenseDecompositionBenchmark.dox
+-rw-r--r--   0        0        0    86035 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/Doxyfile.in
+-rw-r--r--   0        0        0     8355 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/Eigen_Silly_Professor_64x64.png
+-rw-r--r--   0        0        0     1906 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/FixedSizeVectorizable.dox
+-rw-r--r--   0        0        0    13458 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/FunctionsTakingEigenTypes.dox
+-rw-r--r--   0        0        0     5429 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/HiPerformance.dox
+-rw-r--r--   0        0        0     3797 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/InplaceDecomposition.dox
+-rw-r--r--   0        0        0    30585 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/InsideEigenExample.dox
+-rw-r--r--   0        0        0     3150 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/LeastSquares.dox
+-rw-r--r--   0        0        0     6761 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/Manual.dox
+-rw-r--r--   0        0        0      758 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/MatrixfreeSolverExample.dox
+-rw-r--r--   0        0        0     5610 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/NewExpressionType.dox
+-rw-r--r--   0        0        0     1929 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/Overview.dox
+-rw-r--r--   0        0        0     1166 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/PassingByValue.dox
+-rw-r--r--   0        0        0     7018 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/Pitfalls.dox
+-rw-r--r--   0        0        0    14277 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/PreprocessorDirectives.dox
+-rw-r--r--   0        0        0    29844 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/QuickReference.dox
+-rw-r--r--   0        0        0     6578 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/QuickStartGuide.dox
+-rw-r--r--   0        0        0    19902 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/SparseLinearSystems.dox
+-rw-r--r--   0        0        0     8312 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/SparseQuickReference.dox
+-rw-r--r--   0        0        0     3923 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/StlContainers.dox
+-rw-r--r--   0        0        0     4119 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/StorageOrders.dox
+-rw-r--r--   0        0        0     7026 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/StructHavingEigenMembers.dox
+-rw-r--r--   0        0        0     6157 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TemplateKeyword.dox
+-rw-r--r--   0        0        0    10269 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TopicAliasing.dox
+-rw-r--r--   0        0        0     5285 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TopicAssertions.dox
+-rw-r--r--   0        0        0     1914 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TopicCMakeGuide.dox
+-rw-r--r--   0        0        0      173 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TopicEigenExpressionTemplates.dox
+-rw-r--r--   0        0        0     6314 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TopicLazyEvaluation.dox
+-rw-r--r--   0        0        0     9068 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TopicLinearAlgebraDecompositions.dox
+-rw-r--r--   0        0        0     3749 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TopicMultithreading.dox
+-rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TopicResizing.dox
+-rw-r--r--   0        0        0      145 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TopicScalarTypes.dox
+-rw-r--r--   0        0        0       97 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TopicVectorization.dox
+-rw-r--r--   0        0        0     6900 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialAdvancedInitialization.dox
+-rw-r--r--   0        0        0     8523 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialArrayClass.dox
+-rw-r--r--   0        0        0     8288 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialBlockOperations.dox
+-rw-r--r--   0        0        0     9731 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialGeometry.dox
+-rw-r--r--   0        0        0    11860 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialLinearAlgebra.dox
+-rw-r--r--   0        0        0     3988 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialMapClass.dox
+-rw-r--r--   0        0        0     9865 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialMatrixArithmetic.dox
+-rw-r--r--   0        0        0    13680 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialMatrixClass.dox
+-rw-r--r--   0        0        0    12006 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialReductionsVisitorsBroadcasting.dox
+-rw-r--r--   0        0        0     2981 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialReshape.dox
+-rw-r--r--   0        0        0     2142 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialSTL.dox
+-rw-r--r--   0        0        0     8209 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialSlicingIndexing.dox
+-rw-r--r--   0        0        0    20483 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialSparse.dox
+-rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialSparse_example_details.dox
+-rw-r--r--   0        0        0     8737 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/UnalignedArrayAssert.dox
+-rw-r--r--   0        0        0     6633 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/UsingBlasLapackBackends.dox
+-rw-r--r--   0        0        0     6113 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/UsingIntelMKL.dox
+-rw-r--r--   0        0        0     1855 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/UsingNVCC.dox
+-rw-r--r--   0        0        0     2924 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/WrongStackAlignment.dox
+-rw-r--r--   0        0        0     8006 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/eigen_navtree_hacks.js
+-rw-r--r--   0        0        0     4584 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/eigendoxy.css
+-rw-r--r--   0        0        0      680 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/eigendoxy_footer.html.in
+-rw-r--r--   0        0        0     2521 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/eigendoxy_header.html.in
+-rw-r--r--   0        0        0     5337 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/eigendoxy_layout.xml.in
+-rw-r--r--   0        0        0     1095 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/eigendoxy_tabs.css
+-rw-r--r--   0        0        0       34 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/.krazy
+-rw-r--r--   0        0        0      607 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/CMakeLists.txt
+-rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/CustomizingEigen_Inheritance.cpp
+-rw-r--r--   0        0        0      189 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Cwise_erf.cpp
+-rw-r--r--   0        0        0      190 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Cwise_erfc.cpp
+-rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Cwise_lgamma.cpp
+-rw-r--r--   0        0        0      282 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/DenseBase_middleCols_int.cpp
+-rw-r--r--   0        0        0      282 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/DenseBase_middleRows_int.cpp
+-rw-r--r--   0        0        0      283 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/DenseBase_template_int_middleCols.cpp
+-rw-r--r--   0        0        0      283 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/DenseBase_template_int_middleRows.cpp
+-rw-r--r--   0        0        0      206 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/QuickStart_example.cpp
+-rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/QuickStart_example2_dynamic.cpp
+-rw-r--r--   0        0        0      289 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/QuickStart_example2_fixed.cpp
+-rw-r--r--   0        0        0      677 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TemplateKeyword_flexible.cpp
+-rw-r--r--   0        0        0      508 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TemplateKeyword_simple.cpp
+-rw-r--r--   0        0        0     1589 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TutorialInplaceLU.cpp
+-rw-r--r--   0        0        0      622 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgComputeTwice.cpp
+-rw-r--r--   0        0        0      371 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgExComputeSolveError.cpp
+-rw-r--r--   0        0        0      381 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgExSolveColPivHouseholderQR.cpp
+-rw-r--r--   0        0        0      356 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgExSolveLDLT.cpp
+-rw-r--r--   0        0        0      348 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgInverseDeterminant.cpp
+-rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgRankRevealing.cpp
+-rw-r--r--   0        0        0      405 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgSVDSolve.cpp
+-rw-r--r--   0        0        0      534 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp
+-rw-r--r--   0        0        0      377 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgSetThreshold.cpp
+-rw-r--r--   0        0        0      466 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_accessors.cpp
+-rw-r--r--   0        0        0      400 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_addition.cpp
+-rw-r--r--   0        0        0      410 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_cwise_other.cpp
+-rw-r--r--   0        0        0      444 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_interop.cpp
+-rw-r--r--   0        0        0      591 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp
+-rw-r--r--   0        0        0      237 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_mult.cpp
+-rw-r--r--   0        0        0      523 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_block_assignment.cpp
+-rw-r--r--   0        0        0      390 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_colrow.cpp
+-rw-r--r--   0        0        0      448 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_corner.cpp
+-rw-r--r--   0        0        0      413 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_print_block.cpp
+-rw-r--r--   0        0        0      348 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_vector.cpp
+-rw-r--r--   0        0        0      401 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_PartialLU_solve.cpp
+-rw-r--r--   0        0        0      440 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_1nn.cpp
+-rw-r--r--   0        0        0      356 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple.cpp
+-rw-r--r--   0        0        0      361 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple_rowwise.cpp
+-rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_colwise.cpp
+-rw-r--r--   0        0        0      502 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_maxnorm.cpp
+-rw-r--r--   0        0        0      513 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp
+-rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp
+-rw-r--r--   0        0        0      447 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_operatornorm.cpp
+-rw-r--r--   0        0        0      244 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_rowwise.cpp
+-rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp
+-rw-r--r--   0        0        0      680 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_simple_example_dynamic_size.cpp
+-rw-r--r--   0        0        0      282 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_simple_example_fixed_size.cpp
+-rw-r--r--   0        0        0      737 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/class_Block.cpp
+-rw-r--r--   0        0        0      526 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/class_CwiseBinaryOp.cpp
+-rw-r--r--   0        0        0      561 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/class_CwiseUnaryOp.cpp
+-rw-r--r--   0        0        0      371 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/class_CwiseUnaryOp_ptrfun.cpp
+-rw-r--r--   0        0        0      697 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/class_FixedBlock.cpp
+-rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/class_FixedReshaped.cpp
+-rw-r--r--   0        0        0      673 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/class_FixedVectorBlock.cpp
+-rw-r--r--   0        0        0      545 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/class_Reshaped.cpp
+-rw-r--r--   0        0        0      775 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/class_VectorBlock.cpp
+-rw-r--r--   0        0        0      418 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/function_taking_eigenbase.cpp
+-rw-r--r--   0        0        0      594 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/function_taking_ref.cpp
+-rw-r--r--   0        0        0      366 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp
+-rw-r--r--   0        0        0      145 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.entry
+-rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.evaluator
+-rw-r--r--   0        0        0      591 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.expression
+-rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.main
+-rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.preamble
+-rw-r--r--   0        0        0      605 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.traits
+-rw-r--r--   0        0        0     1320 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/make_circulant2.cpp
+-rw-r--r--   0        0        0     4275 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/matrixfree_cg.cpp
+-rw-r--r--   0        0        0     2455 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/nullary_indexing.cpp
+-rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/tut_arithmetic_add_sub.cpp
+-rw-r--r--   0        0        0      393 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/tut_arithmetic_dot_cross.cpp
+-rw-r--r--   0        0        0      612 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/tut_arithmetic_matrix_mul.cpp
+-rw-r--r--   0        0        0      529 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/tut_arithmetic_redux_basic.cpp
+-rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/tut_arithmetic_scalar_mul_div.cpp
+-rw-r--r--   0        0        0      343 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/tut_matrix_coefficient_accessors.cpp
+-rw-r--r--   0        0        0      489 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/tut_matrix_resize.cpp
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/tut_matrix_resize_fixed_size.cpp
+-rw-r--r--   0        0        0       86 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/ftv2node.png
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/ftv2pnode.png
+-rw-r--r--   0        0        0       34 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/.krazy
+-rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/AngleAxis_mimic_euler.cpp
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Array_initializer_list_23_cxx11.cpp
+-rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Array_initializer_list_vector_cxx11.cpp
+-rw-r--r--   0        0        0      102 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Array_variadic_ctor_cxx11.cpp
+-rw-r--r--   0        0        0      394 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/BiCGSTAB_simple.cpp
+-rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/BiCGSTAB_step_by_step.cpp
+-rw-r--r--   0        0        0     1624 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/CMakeLists.txt
+-rw-r--r--   0        0        0      324 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/ColPivHouseholderQR_solve.cpp
+-rw-r--r--   0        0        0      792 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/ComplexEigenSolver_compute.cpp
+-rw-r--r--   0        0        0      216 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/ComplexEigenSolver_eigenvalues.cpp
+-rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/ComplexEigenSolver_eigenvectors.cpp
+-rw-r--r--   0        0        0      301 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/ComplexSchur_compute.cpp
+-rw-r--r--   0        0        0      263 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/ComplexSchur_matrixT.cpp
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/ComplexSchur_matrixU.cpp
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_abs.cpp
+-rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_abs2.cpp
+-rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_acos.cpp
+-rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_arg.cpp
+-rw-r--r--   0        0        0      232 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_array_power_array.cpp
+-rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_asin.cpp
+-rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_atan.cpp
+-rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_boolean_and.cpp
+-rw-r--r--   0        0        0      105 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_boolean_not.cpp
+-rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_boolean_or.cpp
+-rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_boolean_xor.cpp
+-rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_ceil.cpp
+-rw-r--r--   0        0        0       58 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_cos.cpp
+-rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_cosh.cpp
+-rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_cube.cpp
+-rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_equal_equal.cpp
+-rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_exp.cpp
+-rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_floor.cpp
+-rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_greater.cpp
+-rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_greater_equal.cpp
+-rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_inverse.cpp
+-rw-r--r--   0        0        0      104 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_isFinite.cpp
+-rw-r--r--   0        0        0      101 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_isInf.cpp
+-rw-r--r--   0        0        0      101 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_isNaN.cpp
+-rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_less.cpp
+-rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_less_equal.cpp
+-rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_log.cpp
+-rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_log10.cpp
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_max.cpp
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_min.cpp
+-rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_minus.cpp
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_minus_equal.cpp
+-rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_not_equal.cpp
+-rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_plus.cpp
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_plus_equal.cpp
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_pow.cpp
+-rw-r--r--   0        0        0      141 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_product.cpp
+-rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_quotient.cpp
+-rw-r--r--   0        0        0       92 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_rint.cpp
+-rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_round.cpp
+-rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_scalar_power_array.cpp
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_sign.cpp
+-rw-r--r--   0        0        0       58 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_sin.cpp
+-rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_sinh.cpp
+-rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_slash_equal.cpp
+-rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_sqrt.cpp
+-rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_square.cpp
+-rw-r--r--   0        0        0       58 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_tan.cpp
+-rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_tanh.cpp
+-rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Cwise_times_equal.cpp
+-rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/DenseBase_LinSpaced.cpp
+-rw-r--r--   0        0        0      420 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/DenseBase_LinSpacedInt.cpp
+-rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/DenseBase_LinSpaced_seq_deprecated.cpp
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/DenseBase_setLinSpaced.cpp
+-rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/DirectionWise_hnormalized.cpp
+-rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/DirectionWise_replicate.cpp
+-rw-r--r--   0        0        0      179 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/DirectionWise_replicate_int.cpp
+-rw-r--r--   0        0        0      800 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp
+-rw-r--r--   0        0        0      361 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/EigenSolver_compute.cpp
+-rw-r--r--   0        0        0      176 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/EigenSolver_eigenvalues.cpp
+-rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/EigenSolver_eigenvectors.cpp
+-rw-r--r--   0        0        0      430 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/EigenSolver_pseudoEigenvectors.cpp
+-rw-r--r--   0        0        0      325 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/FullPivHouseholderQR_solve.cpp
+-rw-r--r--   0        0        0      369 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/FullPivLU_image.cpp
+-rw-r--r--   0        0        0      317 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/FullPivLU_kernel.cpp
+-rw-r--r--   0        0        0      413 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/FullPivLU_solve.cpp
+-rw-r--r--   0        0        0      456 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/GeneralizedEigenSolver.cpp
+-rw-r--r--   0        0        0      339 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/HessenbergDecomposition_compute.cpp
+-rw-r--r--   0        0        0      391 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/HessenbergDecomposition_matrixH.cpp
+-rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/HessenbergDecomposition_packedMatrix.cpp
+-rw-r--r--   0        0        0      300 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/HouseholderQR_householderQ.cpp
+-rw-r--r--   0        0        0      357 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/HouseholderQR_solve.cpp
+-rw-r--r--   0        0        0     1316 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/HouseholderSequence_HouseholderSequence.cpp
+-rw-r--r--   0        0        0      603 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/IOFormat.cpp
+-rw-r--r--   0        0        0      614 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/JacobiSVD_basic.cpp
+-rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Jacobi_makeGivens.cpp
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Jacobi_makeJacobi.cpp
+-rw-r--r--   0        0        0      519 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/LLT_example.cpp
+-rw-r--r--   0        0        0      456 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/LLT_solve.cpp
+-rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/LeastSquaresNormalEquations.cpp
+-rw-r--r--   0        0        0      177 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/LeastSquaresQR.cpp
+-rw-r--r--   0        0        0      164 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Map_general_stride.cpp
+-rw-r--r--   0        0        0      199 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Map_inner_stride.cpp
+-rw-r--r--   0        0        0      138 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Map_outer_stride.cpp
+-rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Map_placement_new.cpp
+-rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Map_simple.cpp
+-rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_adjoint.cpp
+-rw-r--r--   0        0        0      523 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_all.cpp
+-rw-r--r--   0        0        0      207 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_applyOnTheLeft.cpp
+-rw-r--r--   0        0        0      292 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_applyOnTheRight.cpp
+-rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_array.cpp
+-rw-r--r--   0        0        0      234 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_array_const.cpp
+-rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_asDiagonal.cpp
+-rw-r--r--   0        0        0      244 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_block_int_int.cpp
+-rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_block_int_int_int_int.cpp
+-rw-r--r--   0        0        0      271 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_bottomLeftCorner_int_int.cpp
+-rw-r--r--   0        0        0      274 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_bottomRightCorner_int_int.cpp
+-rw-r--r--   0        0        0      242 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_bottomRows_int.cpp
+-rw-r--r--   0        0        0      119 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cast.cpp
+-rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_col.cpp
+-rw-r--r--   0        0        0      287 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_colwise.cpp
+-rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_colwise_iterator_cxx11.cpp
+-rw-r--r--   0        0        0      410 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_computeInverseAndDetWithCheck.cpp
+-rw-r--r--   0        0        0      318 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_computeInverseWithCheck.cpp
+-rw-r--r--   0        0        0       80 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseAbs.cpp
+-rw-r--r--   0        0        0       81 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseAbs2.cpp
+-rw-r--r--   0        0        0       95 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseArg.cpp
+-rw-r--r--   0        0        0      276 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseEqual.cpp
+-rw-r--r--   0        0        0       87 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseInverse.cpp
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseMax.cpp
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseMin.cpp
+-rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseNotEqual.cpp
+-rw-r--r--   0        0        0      153 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseProduct.cpp
+-rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseQuotient.cpp
+-rw-r--r--   0        0        0       80 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseSign.cpp
+-rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_cwiseSqrt.cpp
+-rw-r--r--   0        0        0      188 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_diagonal.cpp
+-rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_diagonal_int.cpp
+-rw-r--r--   0        0        0      274 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_diagonal_template_int.cpp
+-rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_eigenvalues.cpp
+-rw-r--r--   0        0        0      226 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_end_int.cpp
+-rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_eval.cpp
+-rw-r--r--   0        0        0      274 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_fixedBlock_int_int.cpp
+-rw-r--r--   0        0        0      377 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_hnormalized.cpp
+-rw-r--r--   0        0        0      487 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_homogeneous.cpp
+-rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_identity.cpp
+-rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_identity_int_int.cpp
+-rw-r--r--   0        0        0      145 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_inverse.cpp
+-rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_isDiagonal.cpp
+-rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_isIdentity.cpp
+-rw-r--r--   0        0        0      216 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_isOnes.cpp
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_isOrthogonal.cpp
+-rw-r--r--   0        0        0      231 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_isUnitary.cpp
+-rw-r--r--   0        0        0      215 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_isZero.cpp
+-rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_leftCols_int.cpp
+-rw-r--r--   0        0        0      129 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_noalias.cpp
+-rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_ones.cpp
+-rw-r--r--   0        0        0       77 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_ones_int.cpp
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_ones_int_int.cpp
+-rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_operatorNorm.cpp
+-rw-r--r--   0        0        0      171 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_prod.cpp
+-rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_random.cpp
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_random_int.cpp
+-rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_random_int_int.cpp
+-rw-r--r--   0        0        0      170 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_replicate.cpp
+-rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_replicate_int_int.cpp
+-rw-r--r--   0        0        0      291 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_reshaped_auto.cpp
+-rw-r--r--   0        0        0      178 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_reshaped_fixed.cpp
+-rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_reshaped_int_int.cpp
+-rw-r--r--   0        0        0      287 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_reshaped_to_vector.cpp
+-rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_reverse.cpp
+-rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_rightCols_int.cpp
+-rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_row.cpp
+-rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_rowwise.cpp
+-rw-r--r--   0        0        0      244 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_segment_int_int.cpp
+-rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_select.cpp
+-rw-r--r--   0        0        0      361 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_selfadjointView.cpp
+-rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_set.cpp
+-rw-r--r--   0        0        0       83 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_setIdentity.cpp
+-rw-r--r--   0        0        0       72 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_setOnes.cpp
+-rw-r--r--   0        0        0       72 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_setRandom.cpp
+-rw-r--r--   0        0        0       72 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_setZero.cpp
+-rw-r--r--   0        0        0      226 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_start_int.cpp
+-rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_bottomRows.cpp
+-rw-r--r--   0        0        0      230 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_end.cpp
+-rw-r--r--   0        0        0      264 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_block_int_int_int_int.cpp
+-rw-r--r--   0        0        0      274 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner.cpp
+-rw-r--r--   0        0        0      301 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner_int_int.cpp
+-rw-r--r--   0        0        0      277 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_bottomRightCorner.cpp
+-rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_bottomRightCorner_int_int.cpp
+-rw-r--r--   0        0        0      265 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_topLeftCorner.cpp
+-rw-r--r--   0        0        0      292 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_topLeftCorner_int_int.cpp
+-rw-r--r--   0        0        0      268 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_topRightCorner.cpp
+-rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_int_topRightCorner_int_int.cpp
+-rw-r--r--   0        0        0      242 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_leftCols.cpp
+-rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_rightCols.cpp
+-rw-r--r--   0        0        0      244 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_segment.cpp
+-rw-r--r--   0        0        0      230 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_start.cpp
+-rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_template_int_topRows.cpp
+-rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_topLeftCorner_int_int.cpp
+-rw-r--r--   0        0        0      265 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_topRightCorner_int_int.cpp
+-rw-r--r--   0        0        0      233 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_topRows_int.cpp
+-rw-r--r--   0        0        0      414 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_transpose.cpp
+-rw-r--r--   0        0        0      573 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_triangularView.cpp
+-rw-r--r--   0        0        0       71 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_zero.cpp
+-rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_zero_int.cpp
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_zero_int_int.cpp
+-rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_Map_stride.cpp
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_initializer_list_23_cxx11.cpp
+-rw-r--r--   0        0        0       40 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_initializer_list_vector_cxx11.cpp
+-rw-r--r--   0        0        0      111 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_resize_NoChange_int.cpp
+-rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_resize_int.cpp
+-rw-r--r--   0        0        0      111 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_resize_int_NoChange.cpp
+-rw-r--r--   0        0        0      407 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_resize_int_int.cpp
+-rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setConstant_int.cpp
+-rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setConstant_int_int.cpp
+-rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setIdentity_int_int.cpp
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setOnes_int.cpp
+-rw-r--r--   0        0        0       48 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setOnes_int_int.cpp
+-rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setRandom_int.cpp
+-rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setRandom_int_int.cpp
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setZero_int.cpp
+-rw-r--r--   0        0        0       48 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_setZero_int_int.cpp
+-rw-r--r--   0        0        0      104 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Matrix_variadic_ctor_cxx11.cpp
+-rw-r--r--   0        0        0      372 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/PartialPivLU_solve.cpp
+-rw-r--r--   0        0        0      263 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/PartialRedux_count.cpp
+-rw-r--r--   0        0        0      176 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/PartialRedux_maxCoeff.cpp
+-rw-r--r--   0        0        0      176 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/PartialRedux_minCoeff.cpp
+-rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/PartialRedux_norm.cpp
+-rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/PartialRedux_prod.cpp
+-rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/PartialRedux_squaredNorm.cpp
+-rw-r--r--   0        0        0      164 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/PartialRedux_sum.cpp
+-rw-r--r--   0        0        0      819 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/RealQZ_compute.cpp
+-rw-r--r--   0        0        0      429 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/RealSchur_RealSchur_MatrixType.cpp
+-rw-r--r--   0        0        0      343 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/RealSchur_compute.cpp
+-rw-r--r--   0        0        0      362 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver.cpp
+-rw-r--r--   0        0        0      816 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp
+-rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp
+-rw-r--r--   0        0        0      365 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType.cpp
+-rw-r--r--   0        0        0      396 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType2.cpp
+-rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_eigenvalues.cpp
+-rw-r--r--   0        0        0      193 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_eigenvectors.cpp
+-rw-r--r--   0        0        0      426 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_operatorInverseSqrt.cpp
+-rw-r--r--   0        0        0      363 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_operatorSqrt.cpp
+-rw-r--r--   0        0        0      184 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointView_eigenvalues.cpp
+-rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointView_operatorNorm.cpp
+-rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Slicing_arrayexpr.cpp
+-rw-r--r--   0        0        0      369 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Slicing_custom_padding_cxx11.cpp
+-rw-r--r--   0        0        0      190 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Slicing_rawarray_cxx11.cpp
+-rw-r--r--   0        0        0      164 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Slicing_stdvector_cxx11.cpp
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/SparseMatrix_coeffs.cpp
+-rw-r--r--   0        0        0      267 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_block.cpp
+-rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_block_correct.cpp
+-rw-r--r--   0        0        0      591 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_cwise.cpp
+-rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_mult1.cpp
+-rw-r--r--   0        0        0      230 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_mult2.cpp
+-rw-r--r--   0        0        0       86 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_mult3.cpp
+-rw-r--r--   0        0        0      102 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_mult4.cpp
+-rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_mult5.cpp
+-rw-r--r--   0        0        0      525 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/TopicStorageOrders_example.cpp
+-rw-r--r--   0        0        0      520 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Triangular_solve.cpp
+-rw-r--r--   0        0        0      445 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tridiagonalization_Tridiagonalization_MatrixType.cpp
+-rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tridiagonalization_compute.cpp
+-rw-r--r--   0        0        0      550 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tridiagonalization_decomposeInPlace.cpp
+-rw-r--r--   0        0        0      552 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tridiagonalization_diagonal.cpp
+-rw-r--r--   0        0        0      303 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tridiagonalization_householderCoefficients.cpp
+-rw-r--r--   0        0        0      394 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tridiagonalization_packedMatrix.cpp
+-rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_Block.cpp
+-rw-r--r--   0        0        0      168 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_CommaTemporary.cpp
+-rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_Join.cpp
+-rw-r--r--   0        0        0      272 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_LinSpaced.cpp
+-rw-r--r--   0        0        0      878 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp
+-rw-r--r--   0        0        0      332 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_Zero.cpp
+-rw-r--r--   0        0        0      299 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_Map_rowmajor.cpp
+-rw-r--r--   0        0        0      896 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_Map_using.cpp
+-rw-r--r--   0        0        0      171 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_ReshapeMat2Mat.cpp
+-rw-r--r--   0        0        0      299 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_ReshapeMat2Vec.cpp
+-rw-r--r--   0        0        0      611 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_SlicingCol.cpp
+-rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_SlicingVec.cpp
+-rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_commainit_01.cpp
+-rw-r--r--   0        0        0      113 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_commainit_01b.cpp
+-rw-r--r--   0        0        0      215 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_commainit_02.cpp
+-rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_range_for_loop_1d_cxx11.cpp
+-rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_range_for_loop_2d_cxx11.cpp
+-rw-r--r--   0        0        0      249 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_reshaped_vs_resize_1.cpp
+-rw-r--r--   0        0        0      372 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_reshaped_vs_resize_2.cpp
+-rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_solve_matrix_inverse.cpp
+-rw-r--r--   0        0        0      318 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_solve_multiple_rhs.cpp
+-rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_solve_reuse_decomposition.cpp
+-rw-r--r--   0        0        0      256 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_solve_singular.cpp
+-rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_solve_triangular.cpp
+-rw-r--r--   0        0        0      159 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_solve_triangular_inplace.cpp
+-rw-r--r--   0        0        0      203 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_std_sort.cpp
+-rw-r--r--   0        0        0      218 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_std_sort_rows_cxx11.cpp
+-rw-r--r--   0        0        0      461 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/VectorwiseOp_homogeneous.cpp
+-rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Vectorwise_reverse.cpp
+-rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/class_FullPivLU.cpp
+-rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/compile_snippet.cpp.in
+-rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/tut_arithmetic_redux_minmax.cpp
+-rw-r--r--   0        0        0      188 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/tut_arithmetic_transpose_aliasing.cpp
+-rw-r--r--   0        0        0      277 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/tut_arithmetic_transpose_conjugate.cpp
+-rw-r--r--   0        0        0      174 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/tut_arithmetic_transpose_inplace.cpp
+-rw-r--r--   0        0        0      193 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/tut_matrix_assignment_resizing.cpp
+-rw-r--r--   0        0        0     1114 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/special_examples/CMakeLists.txt
+-rw-r--r--   0        0        0     1184 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/special_examples/Tutorial_sparse_example.cpp
+-rw-r--r--   0        0        0     1576 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/special_examples/Tutorial_sparse_example_details.cpp
+-rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/special_examples/random_cpp11.cpp
+-rw-r--r--   0        0        0     2544 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/tutorial.cpp
+-rw-r--r--   0        0        0      254 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/eigen3.pc.in
+-rw-r--r--   0        0        0     2423 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/CMakeLists.txt
+-rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/bdcsvd_int.cpp
+-rw-r--r--   0        0        0      233 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/block_nonconst_ctor_on_const_xpr_0.cpp
+-rw-r--r--   0        0        0      233 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/block_nonconst_ctor_on_const_xpr_1.cpp
+-rw-r--r--   0        0        0      261 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/block_nonconst_ctor_on_const_xpr_2.cpp
+-rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/block_on_const_type_actually_const_0.cpp
+-rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/block_on_const_type_actually_const_1.cpp
+-rw-r--r--   0        0        0      257 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/colpivqr_int.cpp
+-rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/const_qualified_block_method_retval_0.cpp
+-rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/const_qualified_block_method_retval_1.cpp
+-rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/const_qualified_diagonal_method_retval.cpp
+-rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/const_qualified_transpose_method_retval.cpp
+-rw-r--r--   0        0        0      271 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/cwiseunaryview_nonconst_ctor_on_const_xpr.cpp
+-rw-r--r--   0        0        0      296 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/cwiseunaryview_on_const_type_actually_const.cpp
+-rw-r--r--   0        0        0      228 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/diagonal_nonconst_ctor_on_const_xpr.cpp
+-rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/diagonal_on_const_type_actually_const.cpp
+-rw-r--r--   0        0        0      276 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/eigensolver_cplx.cpp
+-rw-r--r--   0        0        0      259 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/eigensolver_int.cpp
+-rw-r--r--   0        0        0      156 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/failtest_sanity_check.cpp
+-rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/fullpivlu_int.cpp
+-rw-r--r--   0        0        0      258 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/fullpivqr_int.cpp
+-rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/initializer_list_1.cpp
+-rw-r--r--   0        0        0      222 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/initializer_list_2.cpp
+-rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/jacobisvd_int.cpp
+-rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/ldlt_int.cpp
+-rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/llt_int.cpp
+-rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_0.cpp
+-rw-r--r--   0        0        0      246 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_1.cpp
+-rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_2.cpp
+-rw-r--r--   0        0        0      314 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_3.cpp
+-rw-r--r--   0        0        0      321 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/map_nonconst_ctor_on_const_ptr_4.cpp
+-rw-r--r--   0        0        0      249 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/map_on_const_type_actually_const_0.cpp
+-rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/map_on_const_type_actually_const_1.cpp
+-rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/partialpivlu_int.cpp
+-rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/qr_int.cpp
+-rw-r--r--   0        0        0      263 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/ref_1.cpp
+-rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/ref_2.cpp
+-rw-r--r--   0        0        0      231 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/ref_3.cpp
+-rw-r--r--   0        0        0      227 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/ref_4.cpp
+-rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/ref_5.cpp
+-rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/selfadjointview_nonconst_ctor_on_const_xpr.cpp
+-rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/selfadjointview_on_const_type_actually_const.cpp
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/sparse_ref_1.cpp
+-rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/sparse_ref_2.cpp
+-rw-r--r--   0        0        0      271 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/sparse_ref_3.cpp
+-rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/sparse_ref_4.cpp
+-rw-r--r--   0        0        0      285 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/sparse_ref_5.cpp
+-rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/sparse_storage_mismatch.cpp
+-rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/swap_1.cpp
+-rw-r--r--   0        0        0      211 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/swap_2.cpp
+-rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/ternary_1.cpp
+-rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/ternary_2.cpp
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/transpose_nonconst_ctor_on_const_xpr.cpp
+-rw-r--r--   0        0        0      254 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/transpose_on_const_type_actually_const.cpp
+-rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/triangularview_nonconst_ctor_on_const_xpr.cpp
+-rw-r--r--   0        0        0      265 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/triangularview_on_const_type_actually_const.cpp
+-rw-r--r--   0        0        0    10876 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/CMakeLists.txt
+-rw-r--r--   0        0        0     2205 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/cholesky.cpp
+-rw-r--r--   0        0        0     2831 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/clacgv.f
+-rw-r--r--   0        0        0     2340 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/cladiv.f
+-rw-r--r--   0        0        0     6295 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/clarf.f
+-rw-r--r--   0        0        0    23424 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/clarfb.f
+-rw-r--r--   0        0        0     5344 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/clarfg.f
+-rw-r--r--   0        0        0    10450 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/clarft.f
+-rw-r--r--   0        0        0      578 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/complex_double.cpp
+-rw-r--r--   0        0        0      577 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/complex_single.cpp
+-rw-r--r--   0        0        0     2969 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dladiv.f
+-rw-r--r--   0        0        0     5259 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dlamch.f
+-rw-r--r--   0        0        0     2514 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dlapy2.f
+-rw-r--r--   0        0        0     2737 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dlapy3.f
+-rw-r--r--   0        0        0     6167 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dlarf.f
+-rw-r--r--   0        0        0    22749 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dlarfb.f
+-rw-r--r--   0        0        0     4946 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dlarfg.f
+-rw-r--r--   0        0        0    10222 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dlarft.f
+-rw-r--r--   0        0        0      562 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/double.cpp
+-rw-r--r--   0        0        0     1282 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dsecnd_NONE.f
+-rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/eigenvalues.cpp
+-rw-r--r--   0        0        0     2957 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/ilaclc.f
+-rw-r--r--   0        0        0     2997 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/ilaclr.f
+-rw-r--r--   0        0        0     2952 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/iladlc.f
+-rw-r--r--   0        0        0     3000 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/iladlr.f
+-rw-r--r--   0        0        0     2941 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/ilaslc.f
+-rw-r--r--   0        0        0     2988 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/ilaslr.f
+-rw-r--r--   0        0        0     2962 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/ilazlc.f
+-rw-r--r--   0        0        0     3010 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/ilazlr.f
+-rw-r--r--   0        0        0      877 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/lapack_common.h
+-rw-r--r--   0        0        0     2655 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/lu.cpp
+-rw-r--r--   0        0        0     1258 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/second_NONE.f
+-rw-r--r--   0        0        0      561 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/single.cpp
+-rw-r--r--   0        0        0     2897 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/sladiv.f
+-rw-r--r--   0        0        0     5261 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/slamch.f
+-rw-r--r--   0        0        0     2490 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/slapy2.f
+-rw-r--r--   0        0        0     2701 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/slapy3.f
+-rw-r--r--   0        0        0     6117 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/slarf.f
+-rw-r--r--   0        0        0    22727 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/slarfb.f
+-rw-r--r--   0        0        0     4908 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/slarfg.f
+-rw-r--r--   0        0        0    10183 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/slarft.f
+-rw-r--r--   0        0        0     4891 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/svd.cpp
+-rw-r--r--   0        0        0     2839 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/zlacgv.f
+-rw-r--r--   0        0        0     2364 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/zladiv.f
+-rw-r--r--   0        0        0     6278 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/zlarf.f
+-rw-r--r--   0        0        0    23498 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/zlarfb.f
+-rw-r--r--   0        0        0     5359 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/zlarfg.f
+-rw-r--r--   0        0        0    10453 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/zlarft.f
+-rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/CMakeLists.txt
+-rwxr-xr-x   0        0        0      577 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/buildtests.in
+-rw-r--r--   0        0        0     1569 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/cdashtesting.cmake.in
+-rwxr-xr-x   0        0        0      670 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/check.in
+-rwxr-xr-x   0        0        0       44 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/debug.in
+-rw-r--r--   0        0        0     6384 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/eigen_gen_credits.cpp
+-rw-r--r--   0        0        0      738 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/eigen_gen_docs
+-rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/eigen_gen_split_test_help.cmake
+-rwxr-xr-x   0        0        0     1009 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/eigen_monitor_perf.sh
+-rwxr-xr-x   0        0        0       46 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/release.in
+-rw-r--r--   0        0        0     2368 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/relicense.py
+-rw-r--r--   0        0        0      216 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/signature_of_eigen3_matrix_library
+-rw-r--r--   0        0        0     5707 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/AnnoyingScalar.h
+-rw-r--r--   0        0        0    14452 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/CMakeLists.txt
+-rw-r--r--   0        0        0     1079 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/MovableScalar.h
+-rw-r--r--   0        0        0      605 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/SafeScalar.h
+-rw-r--r--   0        0        0     8668 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/adjoint.cpp
+-rw-r--r--   0        0        0    27758 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/array_cwise.cpp
+-rw-r--r--   0        0        0    12883 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/array_for_matrix.cpp
+-rw-r--r--   0        0        0      961 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/array_of_string.cpp
+-rw-r--r--   0        0        0     2342 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/array_replicate.cpp
+-rw-r--r--   0        0        0     6383 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/array_reverse.cpp
+-rw-r--r--   0        0        0     2432 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/bandmatrix.cpp
+-rw-r--r--   0        0        0    13366 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/basicstuff.cpp
+-rw-r--r--   0        0        0     4443 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/bdcsvd.cpp
+-rw-r--r--   0        0        0    17931 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/bfloat16_float.cpp
+-rw-r--r--   0        0        0     1473 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/bicgstab.cpp
+-rw-r--r--   0        0        0     6413 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/blasutil.cpp
+-rw-r--r--   0        0        0    14816 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/block.cpp
+-rw-r--r--   0        0        0     5731 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/boostmultiprec.cpp
+-rw-r--r--   0        0        0      174 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/bug1213.cpp
+-rw-r--r--   0        0        0      147 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/bug1213.h
+-rw-r--r--   0        0        0      279 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/bug1213_main.cpp
+-rw-r--r--   0        0        0    18340 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/cholesky.cpp
+-rw-r--r--   0        0        0     3377 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/cholmod_support.cpp
+-rw-r--r--   0        0        0     3150 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/commainitializer.cpp
+-rw-r--r--   0        0        0     1543 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/conjugate_gradient.cpp
+-rw-r--r--   0        0        0     5369 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/conservative_resize.cpp
+-rw-r--r--   0        0        0     2562 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/constructor.cpp
+-rw-r--r--   0        0        0     6448 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/corners.cpp
+-rw-r--r--   0        0        0     2016 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/ctorleak.cpp
+-rw-r--r--   0        0        0     5062 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/denseLM.cpp
+-rw-r--r--   0        0        0     7256 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/dense_storage.cpp
+-rw-r--r--   0        0        0     2275 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/determinant.cpp
+-rw-r--r--   0        0        0     4115 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/diagonal.cpp
+-rw-r--r--   0        0        0     6686 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/diagonal_matrix_variadic_ctor.cpp
+-rw-r--r--   0        0        0     7531 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/diagonalmatrices.cpp
+-rw-r--r--   0        0        0     2229 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/dontalign.cpp
+-rw-r--r--   0        0        0     4760 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/dynalloc.cpp
+-rw-r--r--   0        0        0     2196 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/eigen2support.cpp
+-rw-r--r--   0        0        0     6221 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/eigensolver_complex.cpp
+-rw-r--r--   0        0        0     4046 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/eigensolver_generalized_real.cpp
+-rw-r--r--   0        0        0     9459 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/eigensolver_generic.cpp
+-rw-r--r--   0        0        0    11419 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/eigensolver_selfadjoint.cpp
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/evaluator_common.h
+-rw-r--r--   0        0        0    21038 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/evaluators.cpp
+-rw-r--r--   0        0        0     1916 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/exceptions.cpp
+-rw-r--r--   0        0        0     5256 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/fastmath.cpp
+-rw-r--r--   0        0        0     1874 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/first_aligned.cpp
+-rw-r--r--   0        0        0    18093 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/geo_alignedbox.cpp
+-rw-r--r--   0        0        0     3562 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/geo_eulerangles.cpp
+-rw-r--r--   0        0        0     5470 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/geo_homogeneous.cpp
+-rw-r--r--   0        0        0     7304 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/geo_hyperplane.cpp
+-rw-r--r--   0        0        0     4838 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/geo_orthomethods.cpp
+-rw-r--r--   0        0        0     4974 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/geo_parametrizedline.cpp
+-rw-r--r--   0        0        0    11568 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/geo_quaternion.cpp
+-rw-r--r--   0        0        0    26366 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/geo_transformations.cpp
+-rw-r--r--   0        0        0    16082 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/gpu_basic.cu
+-rw-r--r--   0        0        0     5456 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/gpu_common.h
+-rw-r--r--   0        0        0    14524 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/half_float.cpp
+-rw-r--r--   0        0        0     2404 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/hessenberg.cpp
+-rw-r--r--   0        0        0     6286 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/householder.cpp
+-rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/incomplete_cholesky.cpp
+-rw-r--r--   0        0        0    19424 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/indexed_view.cpp
+-rw-r--r--   0        0        0    12744 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/initializer_list_construction.cpp
+-rw-r--r--   0        0        0     3880 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/inplace_decomposition.cpp
+-rw-r--r--   0        0        0     5793 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/integer_types.cpp
+-rw-r--r--   0        0        0     4701 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/inverse.cpp
+-rw-r--r--   0        0        0     1833 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/io.cpp
+-rw-r--r--   0        0        0     1368 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/is_same_dense.cpp
+-rw-r--r--   0        0        0     2733 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/jacobi.cpp
+-rw-r--r--   0        0        0     5877 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/jacobisvd.cpp
+-rw-r--r--   0        0        0      955 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/klu_support.cpp
+-rw-r--r--   0        0        0     6130 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/linearstructure.cpp
+-rw-r--r--   0        0        0     1499 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/lscg.cpp
+-rw-r--r--   0        0        0     9075 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/lu.cpp
+-rw-r--r--   0        0        0    33109 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/main.h
+-rw-r--r--   0        0        0     7943 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/mapped_matrix.cpp
+-rw-r--r--   0        0        0     7471 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/mapstaticmethods.cpp
+-rw-r--r--   0        0        0    11369 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/mapstride.cpp
+-rw-r--r--   0        0        0     7339 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/meta.cpp
+-rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/metis_support.cpp
+-rw-r--r--   0        0        0     1789 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/miscmatrices.cpp
+-rw-r--r--   0        0        0    17824 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/mixingtypes.cpp
+-rw-r--r--   0        0        0      635 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/mpl2only.cpp
+-rw-r--r--   0        0        0     1208 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/nestbyvalue.cpp
+-rw-r--r--   0        0        0     4377 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/nesting_ops.cpp
+-rw-r--r--   0        0        0     8700 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/nomalloc.cpp
+-rw-r--r--   0        0        0    12806 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/nullary.cpp
+-rw-r--r--   0        0        0     3212 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/num_dimensions.cpp
+-rw-r--r--   0        0        0     9042 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/numext.cpp
+-rw-r--r--   0        0        0    55436 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/packetmath.cpp
+-rw-r--r--   0        0        0     9016 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/packetmath_test_shared.h
+-rw-r--r--   0        0        0      955 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/pardiso_support.cpp
+-rw-r--r--   0        0        0     1902 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/pastix_support.cpp
+-rw-r--r--   0        0        0     7031 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/permutationmatrices.cpp
+-rw-r--r--   0        0        0     3120 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/prec_inverse_4x4.cpp
+-rw-r--r--   0        0        0    11880 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product.h
+-rw-r--r--   0        0        0    15711 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_extra.cpp
+-rw-r--r--   0        0        0     5395 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_large.cpp
+-rw-r--r--   0        0        0     4447 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_mmtr.cpp
+-rw-r--r--   0        0        0    10988 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_notemporary.cpp
+-rw-r--r--   0        0        0     3510 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_selfadjoint.cpp
+-rw-r--r--   0        0        0    12656 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_small.cpp
+-rw-r--r--   0        0        0     6133 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_symm.cpp
+-rw-r--r--   0        0        0     7856 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_syrk.cpp
+-rw-r--r--   0        0        0     6921 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_trmm.cpp
+-rw-r--r--   0        0        0     4250 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_trmv.cpp
+-rw-r--r--   0        0        0     6102 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_trsolve.cpp
+-rw-r--r--   0        0        0     4673 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/qr.cpp
+-rw-r--r--   0        0        0    13867 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/qr_colpivoting.cpp
+-rw-r--r--   0        0        0     5600 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/qr_fullpivoting.cpp
+-rw-r--r--   0        0        0     4621 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/qtvector.cpp
+-rw-r--r--   0        0        0     4373 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/rand.cpp
+-rw-r--r--   0        0        0     7174 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/random_without_cast_overflow.h
+-rw-r--r--   0        0        0     3102 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/real_qz.cpp
+-rw-r--r--   0        0        0     8239 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/redux.cpp
+-rw-r--r--   0        0        0    14363 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/ref.cpp
+-rw-r--r--   0        0        0    10706 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/reshape.cpp
+-rw-r--r--   0        0        0     1105 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/resize.cpp
+-rw-r--r--   0        0        0     5668 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/rvalue_types.cpp
+-rw-r--r--   0        0        0     3569 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/schur_complex.cpp
+-rw-r--r--   0        0        0     3964 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/schur_real.cpp
+-rw-r--r--   0        0        0     2419 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/selfadjoint.cpp
+-rw-r--r--   0        0        0     2564 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/simplicial_cholesky.cpp
+-rw-r--r--   0        0        0     2038 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sizeof.cpp
+-rw-r--r--   0        0        0     2639 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sizeoverflow.cpp
+-rw-r--r--   0        0        0     2133 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/smallvectors.cpp
+-rw-r--r--   0        0        0     1716 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/solverbase.h
+-rw-r--r--   0        0        0     6216 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse.h
+-rw-r--r--   0        0        0     4740 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparseLM.cpp
+-rw-r--r--   0        0        0    29343 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse_basic.cpp
+-rw-r--r--   0        0        0    12153 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse_block.cpp
+-rw-r--r--   0        0        0     9997 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse_permutations.cpp
+-rw-r--r--   0        0        0    25557 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse_product.cpp
+-rw-r--r--   0        0        0     6125 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse_ref.cpp
+-rw-r--r--   0        0        0    24396 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse_solver.h
+-rw-r--r--   0        0        0     5142 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse_solvers.cpp
+-rw-r--r--   0        0        0     5087 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse_vector.cpp
+-rw-r--r--   0        0        0     1791 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparselu.cpp
+-rw-r--r--   0        0        0     4587 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparseqr.cpp
+-rw-r--r--   0        0        0     1762 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/special_numbers.cpp
+-rw-r--r--   0        0        0   159516 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/split_test_helper.h
+-rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/spqr_support.cpp
+-rw-r--r--   0        0        0    10379 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/stable_norm.cpp
+-rw-r--r--   0        0        0     4260 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/stddeque.cpp
+-rw-r--r--   0        0        0     4738 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/stddeque_overload.cpp
+-rw-r--r--   0        0        0     4232 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/stdlist.cpp
+-rw-r--r--   0        0        0     5852 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/stdlist_overload.cpp
+-rw-r--r--   0        0        0     5116 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/stdvector.cpp
+-rw-r--r--   0        0        0     5014 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/stdvector_overload.cpp
+-rw-r--r--   0        0        0    19411 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/stl_iterators.cpp
+-rw-r--r--   0        0        0      956 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/superlu_support.cpp
+-rw-r--r--   0        0        0    19317 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/svd_common.h
+-rw-r--r--   0        0        0     4050 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/svd_fill.h
+-rw-r--r--   0        0        0     2940 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/swap.cpp
+-rw-r--r--   0        0        0     2742 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/symbolic_index.cpp
+-rw-r--r--   0        0        0    11918 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/triangular.cpp
+-rw-r--r--   0        0        0     2024 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/type_alias.cpp
+-rw-r--r--   0        0        0     5859 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/umeyama.cpp
+-rw-r--r--   0        0        0     1171 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/umfpack_support.cpp
+-rw-r--r--   0        0        0     2565 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/unalignedcount.cpp
+-rw-r--r--   0        0        0     1716 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/upperbidiagonalization.cpp
+-rw-r--r--   0        0        0    20351 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/vectorization_logic.cpp
+-rw-r--r--   0        0        0    11489 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/vectorwiseop.cpp
+-rw-r--r--   0        0        0     6384 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/visitor.cpp
+-rw-r--r--   0        0        0     3734 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/zerosized.cpp
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/CMakeLists.txt
+-rw-r--r--   0        0        0     4422 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/AdolcForward
+-rw-r--r--   0        0        0     6349 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/AlignedVector3
+-rw-r--r--   0        0        0      884 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/ArpackSupport
+-rw-r--r--   0        0        0     1181 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/AutoDiff
+-rw-r--r--   0        0        0     5523 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/BVH
+-rw-r--r--   0        0        0      603 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CMakeLists.txt
+-rw-r--r--   0        0        0      307 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/CMakeLists.txt
+-rw-r--r--   0        0        0     4187 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/Tensor
+-rw-r--r--   0        0        0     1267 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/TensorSymmetry
+-rw-r--r--   0        0        0     2087 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/ThreadPool
+-rw-r--r--   0        0        0    62365 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/README.md
+-rw-r--r--   0        0        0    21269 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
+-rw-r--r--   0        0        0    12448 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
+-rw-r--r--   0        0        0    10323 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
+-rw-r--r--   0        0        0    57932 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
+-rw-r--r--   0        0        0    60851 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h
+-rw-r--r--   0        0        0    42150 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
+-rw-r--r--   0        0        0    19707 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
+-rw-r--r--   0        0        0    15665 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
+-rw-r--r--   0        0        0    45320 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
+-rw-r--r--   0        0        0     2675 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
+-rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
+-rw-r--r--   0        0        0    63402 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h
+-rw-r--r--   0        0        0    23586 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
+-rwxr-xr-x   0        0        0    89042 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h
+-rw-r--r--   0        0        0    70687 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
+-rw-r--r--   0        0        0    18803 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
+-rw-r--r--   0        0        0    48686 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
+-rw-r--r--   0        0        0    27527 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h
+-rw-r--r--   0        0        0     8642 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
+-rw-r--r--   0        0        0    13146 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
+-rw-r--r--   0        0        0     4896 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
+-rw-r--r--   0        0        0      215 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
+-rw-r--r--   0        0        0     3427 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
+-rw-r--r--   0        0        0    12837 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h
+-rw-r--r--   0        0        0    40367 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
+-rw-r--r--   0        0        0    15203 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
+-rw-r--r--   0        0        0     7674 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
+-rw-r--r--   0        0        0    17751 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
+-rw-r--r--   0        0        0     8556 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
+-rw-r--r--   0        0        0    40005 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
+-rw-r--r--   0        0        0    26655 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
+-rw-r--r--   0        0        0    16115 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
+-rw-r--r--   0        0        0    24345 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
+-rw-r--r--   0        0        0    14486 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
+-rw-r--r--   0        0        0     8782 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
+-rw-r--r--   0        0        0     8320 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
+-rw-r--r--   0        0        0    15269 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
+-rw-r--r--   0        0        0    10920 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
+-rw-r--r--   0        0        0     1316 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
+-rw-r--r--   0        0        0     4068 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h
+-rw-r--r--   0        0        0     1267 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h
+-rw-r--r--   0        0        0     2560 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
+-rw-r--r--   0        0        0    28066 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
+-rw-r--r--   0        0        0    25692 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
+-rw-r--r--   0        0        0     9094 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
+-rw-r--r--   0        0        0     2730 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
+-rw-r--r--   0        0        0     9041 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
+-rw-r--r--   0        0        0     7769 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
+-rw-r--r--   0        0        0     3642 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
+-rw-r--r--   0        0        0    14191 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
+-rw-r--r--   0        0        0     8104 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
+-rw-r--r--   0        0        0    43284 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
+-rw-r--r--   0        0        0    28764 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
+-rw-r--r--   0        0        0    11474 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
+-rw-r--r--   0        0        0    12385 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
+-rw-r--r--   0        0        0    44395 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h
+-rw-r--r--   0        0        0    40719 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h
+-rw-r--r--   0        0        0    30074 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
+-rw-r--r--   0        0        0    14793 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
+-rw-r--r--   0        0        0    16938 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
+-rw-r--r--   0        0        0    20091 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
+-rw-r--r--   0        0        0    25279 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h
+-rw-r--r--   0        0        0    18256 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
+-rw-r--r--   0        0        0     5481 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
+-rw-r--r--   0        0        0    13513 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
+-rw-r--r--   0        0        0    10152 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h
+-rw-r--r--   0        0        0     9432 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
+-rw-r--r--   0        0        0     7552 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
+-rw-r--r--   0        0        0    30089 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
+-rw-r--r--   0        0        0    10857 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
+-rw-r--r--   0        0        0     9086 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
+-rw-r--r--   0        0        0    13021 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
+-rw-r--r--   0        0        0    21046 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
+-rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h
+-rw-r--r--   0        0        0     9121 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
+-rw-r--r--   0        0        0    17075 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
+-rw-r--r--   0        0        0     9366 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
+-rw-r--r--   0        0        0      774 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h
+-rw-r--r--   0        0        0     1209 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
+-rw-r--r--   0        0        0    11482 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
+-rw-r--r--   0        0        0     1680 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
+-rw-r--r--   0        0        0      715 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
+-rw-r--r--   0        0        0    22752 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
+-rw-r--r--   0        0        0     4115 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
+-rw-r--r--   0        0        0     8155 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/EmulateArray.h
+-rw-r--r--   0        0        0     4174 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
+-rw-r--r--   0        0        0     1126 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/EulerAngles
+-rw-r--r--   0        0        0    13948 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/FFT
+-rw-r--r--   0        0        0     1561 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/IterativeSolvers
+-rw-r--r--   0        0        0      944 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/KroneckerProduct
+-rw-r--r--   0        0        0     1238 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/LevenbergMarquardt
+-rw-r--r--   0        0        0     7656 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/MPRealSupport
+-rw-r--r--   0        0        0    17919 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/MatrixFunctions
+-rw-r--r--   0        0        0      592 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/MoreVectorization
+-rw-r--r--   0        0        0     5963 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/NonLinearOptimization
+-rw-r--r--   0        0        0     1779 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/NumericalDiff
+-rw-r--r--   0        0        0    19072 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/OpenGLSupport
+-rw-r--r--   0        0        0     4749 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/Polynomials
+-rw-r--r--   0        0        0      930 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/Skyline
+-rw-r--r--   0        0        0     1360 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/SparseExtra
+-rw-r--r--   0        0        0     2951 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/SpecialFunctions
+-rw-r--r--   0        0        0      996 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/Splines
+-rw-r--r--   0        0        0     3150 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
+-rwxr-xr-x   0        0        0    29107 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
+-rw-r--r--   0        0        0     9029 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
+-rw-r--r--   0        0        0    12976 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/BVH/BVAlgorithms.h
+-rw-r--r--   0        0        0     9166 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/BVH/KdBVH.h
+-rw-r--r--   0        0        0    29075 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
+-rw-r--r--   0        0        0      174 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/CMakeLists.txt
+-rw-r--r--   0        0        0    15367 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/EulerAngles.h
+-rw-r--r--   0        0        0    11620 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/EulerSystem.h
+-rw-r--r--   0        0        0     9223 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/FFT/ei_fftw_impl.h
+-rw-r--r--   0        0        0    13231 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
+-rw-r--r--   0        0        0     5324 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
+-rw-r--r--   0        0        0    17769 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
+-rw-r--r--   0        0        0    10209 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/GMRES.h
+-rwxr-xr-x   0        0        0    14794 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IDRS.h
+-rw-r--r--   0        0        0     2520 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
+-rw-r--r--   0        0        0     5360 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IterationController.h
+-rw-r--r--   0        0        0    12397 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/MINRES.h
+-rw-r--r--   0        0        0     5853 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/Scaling.h
+-rw-r--r--   0        0        0    10250 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
+-rw-r--r--   0        0        0     2194 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt
+-rw-r--r--   0        0        0     2443 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
+-rw-r--r--   0        0        0     6648 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
+-rw-r--r--   0        0        0     5039 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
+-rw-r--r--   0        0        0     6805 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
+-rw-r--r--   0        0        0    13297 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
+-rw-r--r--   0        0        0    16624 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
+-rw-r--r--   0        0        0    22671 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
+-rw-r--r--   0        0        0    17557 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
+-rw-r--r--   0        0        0    23422 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
+-rw-r--r--   0        0        0    14212 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
+-rw-r--r--   0        0        0     2107 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
+-rw-r--r--   0        0        0     3035 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
+-rw-r--r--   0        0        0    19837 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
+-rw-r--r--   0        0        0    22135 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
+-rw-r--r--   0        0        0     1864 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/chkder.h
+-rw-r--r--   0        0        0     1915 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/covar.h
+-rw-r--r--   0        0        0     3297 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
+-rw-r--r--   0        0        0     2225 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
+-rw-r--r--   0        0        0     9111 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
+-rw-r--r--   0        0        0     3264 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
+-rw-r--r--   0        0        0     1081 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
+-rw-r--r--   0        0        0     3083 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
+-rw-r--r--   0        0        0     1362 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
+-rw-r--r--   0        0        0     4020 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
+-rw-r--r--   0        0        0     8076 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Polynomials/Companion.h
+-rw-r--r--   0        0        0    15683 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
+-rw-r--r--   0        0        0     4806 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
+-rw-r--r--   0        0        0    11365 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
+-rw-r--r--   0        0        0    31105 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineMatrix.h
+-rw-r--r--   0        0        0     7837 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
+-rw-r--r--   0        0        0    10853 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineProduct.h
+-rw-r--r--   0        0        0     7966 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineStorage.h
+-rw-r--r--   0        0        0     3153 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineUtil.h
+-rw-r--r--   0        0        0     4260 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h
+-rw-r--r--   0        0        0    40316 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
+-rw-r--r--   0        0        0    13744 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h
+-rw-r--r--   0        0        0     8416 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/MarketIO.h
+-rw-r--r--   0        0        0     7568 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
+-rw-r--r--   0        0        0    12423 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/RandomSetter.h
+-rw-r--r--   0        0        0    10015 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h
+-rw-r--r--   0        0        0     2724 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h
+-rw-r--r--   0        0        0    12641 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h
+-rw-r--r--   0        0        0     2544 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h
+-rw-r--r--   0        0        0    69632 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h
+-rw-r--r--   0        0        0     4006 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h
+-rw-r--r--   0        0        0     2489 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h
+-rw-r--r--   0        0        0     7694 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
+-rw-r--r--   0        0        0     3087 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h
+-rw-r--r--   0        0        0    11700 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
+-rw-r--r--   0        0        0     2899 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
+-rw-r--r--   0        0        0    58539 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
+-rw-r--r--   0        0        0     3713 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
+-rw-r--r--   0        0        0     1492 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h
+-rw-r--r--   0        0        0      398 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX/SpecialFunctions.h
+-rw-r--r--   0        0        0     1549 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h
+-rw-r--r--   0        0        0      415 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/SpecialFunctions.h
+-rw-r--r--   0        0        0    10864 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h
+-rw-r--r--   0        0        0     2258 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h
+-rw-r--r--   0        0        0     1283 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h
+-rw-r--r--   0        0        0    18307 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Splines/Spline.h
+-rw-r--r--   0        0        0    16505 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Splines/SplineFitting.h
+-rw-r--r--   0        0        0     4312 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Splines/SplineFwd.h
+-rw-r--r--   0        0        0     1876 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/README.txt
+-rw-r--r--   0        0        0     3906 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/bench/bench_svd.cpp
+-rw-r--r--   0        0        0      114 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/CMakeLists.txt
+-rw-r--r--   0        0        0      878 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/Overview.dox
+-rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/SYCL.dox
+-rw-r--r--   0        0        0     5283 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/eigendoxy_layout.xml.in
+-rw-r--r--   0        0        0     2108 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/BVH_Example.cpp
+-rw-r--r--   0        0        0      736 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/CMakeLists.txt
+-rw-r--r--   0        0        0     1847 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/EulerAngles.cpp
+-rw-r--r--   0        0        0     2522 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/FFT.cpp
+-rw-r--r--   0        0        0      356 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixExponential.cpp
+-rw-r--r--   0        0        0      469 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixFunction.cpp
+-rw-r--r--   0        0        0      375 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixLogarithm.cpp
+-rw-r--r--   0        0        0      364 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixPower.cpp
+-rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixPower_optimal.cpp
+-rw-r--r--   0        0        0      508 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixSine.cpp
+-rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixSinh.cpp
+-rw-r--r--   0        0        0      434 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixSquareRoot.cpp
+-rw-r--r--   0        0        0     2392 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/PolynomialSolver1.cpp
+-rw-r--r--   0        0        0      635 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/PolynomialUtils1.cpp
+-rw-r--r--   0        0        0     1409 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/SYCL/CMakeLists.txt
+-rw-r--r--   0        0        0     2551 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/SYCL/CwiseMul.cpp
+-rw-r--r--   0        0        0     1137 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/snippets/CMakeLists.txt
+-rw-r--r--   0        0        0     7190 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/BVH.cpp
+-rw-r--r--   0        0        0    15348 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/CMakeLists.txt
+-rw-r--r--   0        0        0     9623 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/EulerAngles.cpp
+-rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/FFT.cpp
+-rw-r--r--   0        0        0     9233 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/FFTW.cpp
+-rw-r--r--   0        0        0    64597 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/NonLinearOptimization.cpp
+-rw-r--r--   0        0        0     2862 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/NumericalDiff.cpp
+-rw-r--r--   0        0        0     2366 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/alignedvector3.cpp
+-rw-r--r--   0        0        0    10992 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/autodiff.cpp
+-rw-r--r--   0        0        0     2943 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/autodiff_scalar.cpp
+-rw-r--r--   0        0        0    16409 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/bessel_functions.cpp
+-rw-r--r--   0        0        0     3990 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_eventcount.cpp
+-rw-r--r--   0        0        0     1839 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_maxsizevector.cpp
+-rw-r--r--   0        0        0    18740 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_meta.cpp
+-rw-r--r--   0        0        0     5039 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_non_blocking_thread_pool.cpp
+-rw-r--r--   0        0        0     7024 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_runqueue.cpp
+-rw-r--r--   0        0        0     9150 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax.cpp
+-rw-r--r--   0        0        0     8886 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax_gpu.cu
+-rw-r--r--   0        0        0     9949 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax_sycl.cpp
+-rw-r--r--   0        0        0     9707 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_assign.cpp
+-rw-r--r--   0        0        0    22378 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_block_access.cpp
+-rw-r--r--   0        0        0    31888 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_block_eval.cpp
+-rw-r--r--   0        0        0    15858 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_block_io.cpp
+-rw-r--r--   0        0        0     5708 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_broadcast_sycl.cpp
+-rw-r--r--   0        0        0     9209 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_broadcasting.cpp
+-rw-r--r--   0        0        0    15767 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_builtins_sycl.cpp
+-rw-r--r--   0        0        0     2420 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_cast_float16_gpu.cu
+-rw-r--r--   0        0        0     5526 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_casts.cpp
+-rw-r--r--   0        0        0    13050 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_chipping.cpp
+-rw-r--r--   0        0        0    26158 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_chipping_sycl.cpp
+-rw-r--r--   0        0        0     1991 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_comparisons.cpp
+-rw-r--r--   0        0        0     2871 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_complex_cwise_ops_gpu.cu
+-rw-r--r--   0        0        0     6636 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_complex_gpu.cu
+-rw-r--r--   0        0        0     4624 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_concatenation.cpp
+-rw-r--r--   0        0        0     8411 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_concatenation_sycl.cpp
+-rw-r--r--   0        0        0     1660 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_const.cpp
+-rw-r--r--   0        0        0     7350 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_contract_gpu.cu
+-rw-r--r--   0        0        0    47521 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_contract_sycl.cpp
+-rw-r--r--   0        0        0    23176 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_contraction.cpp
+-rw-r--r--   0        0        0     5381 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_convolution.cpp
+-rw-r--r--   0        0        0    20033 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_convolution_sycl.cpp
+-rw-r--r--   0        0        0     2518 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_index.cpp
+-rw-r--r--   0        0        0     3211 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_op.cpp
+-rw-r--r--   0        0        0     6806 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_op_sycl.cpp
+-rw-r--r--   0        0        0    13495 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_device.cu
+-rw-r--r--   0        0        0     3210 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_device_sycl.cpp
+-rw-r--r--   0        0        0     2578 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_dimension.cpp
+-rw-r--r--   0        0        0      999 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_empty.cpp
+-rw-r--r--   0        0        0    30675 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_executor.cpp
+-rw-r--r--   0        0        0    14224 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_expr.cpp
+-rw-r--r--   0        0        0    13705 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_fft.cpp
+-rw-r--r--   0        0        0     7252 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_fixed_size.cpp
+-rw-r--r--   0        0        0     2167 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_forced_eval.cpp
+-rw-r--r--   0        0        0     3461 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp
+-rw-r--r--   0        0        0     2266 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_generator.cpp
+-rw-r--r--   0        0        0     5732 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_generator_sycl.cpp
+-rw-r--r--   0        0        0    58446 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_gpu.cu
+-rw-r--r--   0        0        0     5942 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_ifft.cpp
+-rw-r--r--   0        0        0     3890 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_image_op_sycl.cpp
+-rw-r--r--   0        0        0    36037 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_image_patch.cpp
+-rw-r--r--   0        0        0    62111 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_image_patch_sycl.cpp
+-rw-r--r--   0        0        0    18652 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_index_list.cpp
+-rw-r--r--   0        0        0     2109 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_inflation.cpp
+-rw-r--r--   0        0        0     5101 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_inflation_sycl.cpp
+-rw-r--r--   0        0        0     4129 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_intdiv.cpp
+-rw-r--r--   0        0        0     3277 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_io.cpp
+-rw-r--r--   0        0        0     1639 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_layout_swap.cpp
+-rw-r--r--   0        0        0     4730 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_layout_swap_sycl.cpp
+-rw-r--r--   0        0        0      950 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_lvalue.cpp
+-rw-r--r--   0        0        0     7962 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_map.cpp
+-rw-r--r--   0        0        0      993 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_math.cpp
+-rw-r--r--   0        0        0     3877 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_math_sycl.cpp
+-rw-r--r--   0        0        0     1501 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_mixed_indices.cpp
+-rw-r--r--   0        0        0    18215 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_morphing.cpp
+-rw-r--r--   0        0        0    17549 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_morphing_sycl.cpp
+-rw-r--r--   0        0        0     1734 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_move.cpp
+-rw-r--r--   0        0        0     1789 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_notification.cpp
+-rw-r--r--   0        0        0     2893 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_of_complex.cpp
+-rw-r--r--   0        0        0     2430 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_of_const_values.cpp
+-rw-r--r--   0        0        0    21223 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_of_float16_gpu.cu
+-rw-r--r--   0        0        0     3766 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_of_strings.cpp
+-rw-r--r--   0        0        0     2652 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_padding.cpp
+-rw-r--r--   0        0        0     5677 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_padding_sycl.cpp
+-rw-r--r--   0        0        0     5499 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_patch.cpp
+-rw-r--r--   0        0        0     9385 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_patch_sycl.cpp
+-rw-r--r--   0        0        0     2513 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_random.cpp
+-rw-r--r--   0        0        0     2355 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_random_gpu.cu
+-rw-r--r--   0        0        0     3568 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_random_sycl.cpp
+-rw-r--r--   0        0        0    15346 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction.cpp
+-rw-r--r--   0        0        0     5410 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction_gpu.cu
+-rw-r--r--   0        0        0    42176 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction_sycl.cpp
+-rw-r--r--   0        0        0     6722 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_ref.cpp
+-rw-r--r--   0        0        0     5285 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reverse.cpp
+-rw-r--r--   0        0        0     9283 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reverse_sycl.cpp
+-rw-r--r--   0        0        0     1486 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_roundings.cpp
+-rw-r--r--   0        0        0     2978 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_scan.cpp
+-rw-r--r--   0        0        0     2576 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_scan_gpu.cu
+-rw-r--r--   0        0        0     6376 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_scan_sycl.cpp
+-rw-r--r--   0        0        0     7692 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_shuffling.cpp
+-rw-r--r--   0        0        0     4265 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_shuffling_sycl.cpp
+-rw-r--r--   0        0        0     9624 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_simple.cpp
+-rw-r--r--   0        0        0     3024 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_striding.cpp
+-rw-r--r--   0        0        0     7074 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_striding_sycl.cpp
+-rw-r--r--   0        0        0     1896 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_sugar.cpp
+-rw-r--r--   0        0        0    14828 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_sycl.cpp
+-rw-r--r--   0        0        0    59079 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_symmetry.cpp
+-rw-r--r--   0        0        0     4237 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_thread_local.cpp
+-rw-r--r--   0        0        0    25491 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_thread_pool.cpp
+-rw-r--r--   0        0        0     5129 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_trace.cpp
+-rw-r--r--   0        0        0     5757 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_uint128.cpp
+-rw-r--r--   0        0        0     4592 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_volume_patch.cpp
+-rw-r--r--   0        0        0    11972 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_volume_patch_sycl.cpp
+-rw-r--r--   0        0        0     1279 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/dgmres.cpp
+-rw-r--r--   0        0        0     3822 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/forward_adolc.cpp
+-rw-r--r--   0        0        0     1245 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/gmres.cpp
+-rw-r--r--   0        0        0      942 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/idrs.cpp
+-rw-r--r--   0        0        0     9075 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/kronecker_product.cpp
+-rw-r--r--   0        0        0    55504 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/levenberg_marquardt.cpp
+-rw-r--r--   0        0        0     4417 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/matrix_exponential.cpp
+-rw-r--r--   0        0        0     7447 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/matrix_function.cpp
+-rw-r--r--   0        0        0     2106 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/matrix_functions.h
+-rw-r--r--   0        0        0     7178 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/matrix_power.cpp
+-rw-r--r--   0        0        0     1050 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/matrix_square_root.cpp
+-rw-r--r--   0        0        0     1658 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/minres.cpp
+-rw-r--r--   0        0        0     2439 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/mpreal_support.cpp
+-rw-r--r--   0        0        0    18637 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/openglsupport.cpp
+-rw-r--r--   0        0        0     7486 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/polynomialsolver.cpp
+-rw-r--r--   0        0        0     3582 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/polynomialutils.cpp
+-rw-r--r--   0        0        0     8414 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/sparse_extra.cpp
+-rw-r--r--   0        0        0    22854 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/special_functions.cpp
+-rw-r--r--   0        0        0     6372 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/special_packetmath.cpp
+-rw-r--r--   0        0        0     8529 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/splines.cpp
+-rw-r--r--   0        0        0     3521 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/fcns.cpp
+-rw-r--r--   0        0        0    34740 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/C++/main.cpp
+-rw-r--r--   0        0        0      134 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/ackleyfcn.tex
+-rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/ackleyn2fcn.tex
+-rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/ackleyn3fcn.tex
+-rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/adjimanfcn.tex
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/alpinen1fcn.tex
+-rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/alpinen2fcn.tex
+-rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/bartelsconnfcn.tex
+-rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/bealefcn.tex
+-rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/birdfcn.tex
+-rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/bohachevskyn1fcn.tex
+-rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/bohachevskyn2fcn.tex
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/boothfcn.tex
+-rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/brentfcn.tex
+-rw-r--r--   0        0        0       86 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/brownfcn.tex
+-rw-r--r--   0        0        0       40 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/bukinn6fcn.tex
+-rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/crossintrayfcn.tex
+-rw-r--r--   0        0        0       62 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/deckkersaartsfcn.tex
+-rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/dropwavefcn.tex
+-rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/easomfcn.tex
+-rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/eggcratefcn.tex
+-rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/elattarfcn.tex
+-rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/exponentialfcn.tex
+-rw-r--r--   0        0        0       31 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/forresterfcn.tex
+-rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/goldsteinpricefcn.tex
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/gramacylacyfcn.tex
+-rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/griewankfcn.tex
+-rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/happycatfcn.tex
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/himmelblaufcn.tex
+-rw-r--r--   0        0        0       58 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/holdertablefcn.tex
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/keanefcn.tex
+-rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/leonfcn.tex
+-rw-r--r--   0        0        0       74 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/levin13fcn.tex
+-rw-r--r--   0        0        0       30 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/matyasfcn.tex
+-rw-r--r--   0        0        0       51 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/mccormickfcn.tex
+-rw-r--r--   0        0        0       91 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/periodicfcn.tex
+-rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/powellsumfcn.tex
+-rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/qingfcn.tex
+-rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/quarticfcn.tex
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/rastriginfcn.tex
+-rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/ridgefcn.tex
+-rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/rosenbrockfcn.tex
+-rw-r--r--   0        0        0       98 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/salomonfcn.tex
+-rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/schaffern1fcn.tex
+-rw-r--r--   0        0        0       62 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/schaffern2fcn.tex
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/schaffern3fcn.tex
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/schaffern4fcn.tex
+-rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/schwefel220fcn.tex
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/schwefel221fcn.tex
+-rw-r--r--   0        0        0       72 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/schwefel222fcn.tex
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/schwefel223fcn.tex
+-rw-r--r--   0        0        0       90 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/schwefelfcn.tex
+-rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/shubert3fcn.tex
+-rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/shubert4fcn.tex
+-rw-r--r--   0        0        0       91 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/shubertfcn.tex
+-rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/spherefcn.tex
+-rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/styblinskitankfcn.tex
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/sumsquaresfcn.tex
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/threehumpcamelfcn.tex
+-rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/wolfefcn.tex
+-rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/xinsheyangn1fcn.tex
+-rw-r--r--   0        0        0       83 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/xinsheyangn2fcn.tex
+-rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/xinsheyangn3fcn.tex
+-rw-r--r--   0        0        0      131 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/xinsheyangn4fcn.tex
+-rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/latex/zakharovfcn.tex
+-rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/ackleyfcn.m
+-rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/ackleyn2fcn.m
+-rw-r--r--   0        0        0      833 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/ackleyn3fcn.m
+-rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/ackleyn4fcn.m
+-rw-r--r--   0        0        0      775 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/adjimanfcn.m
+-rw-r--r--   0        0        0      666 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/alpinen1fcn.m
+-rw-r--r--   0        0        0      658 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/alpinen2fcn.m
+-rw-r--r--   0        0        0      825 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/bartelsconnfcn.m
+-rw-r--r--   0        0        0      841 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/bealefcn.m
+-rw-r--r--   0        0        0      804 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/birdfcn.m
+-rw-r--r--   0        0        0      847 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/bohachevskyn1fcn.m
+-rw-r--r--   0        0        0      850 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/bohachevskyn2fcn.m
+-rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/boothfcn.m
+-rw-r--r--   0        0        0      762 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/brentfcn.m
+-rw-r--r--   0        0        0      741 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/brownfcn.m
+-rw-r--r--   0        0        0      814 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/bukinn6fcn.m
+-rw-r--r--   0        0        0     1898 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/contourfcn.m
+-rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/crossintrayfcn.m
+-rw-r--r--   0        0        0      846 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/deckkersaartsfcn.m
+-rw-r--r--   0        0        0      882 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/dropwavefcn.m
+-rw-r--r--   0        0        0      787 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/easomfcn.m
+-rw-r--r--   0        0        0      781 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/eggcratefcn.m
+-rw-r--r--   0        0        0      902 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/eggholderfcn.m
+-rw-r--r--   0        0        0      811 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/elattarfcn.m
+-rw-r--r--   0        0        0      657 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/exponentialfcn.m
+-rw-r--r--   0        0        0      743 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/forresterfcn.m
+-rw-r--r--   0        0        0      686 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/giuntafcn.m
+-rw-r--r--   0        0        0      990 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/goldsteinpricefcn.m
+-rw-r--r--   0        0        0      776 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/gramacyleefcn.m
+-rw-r--r--   0        0        0      828 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/griewankfcn.m
+-rw-r--r--   0        0        0      855 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/happycatfcn.m
+-rw-r--r--   0        0        0      809 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/himmelblaufcn.m
+-rw-r--r--   0        0        0      875 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/holdertablefcn.m
+-rw-r--r--   0        0        0      843 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/keanefcn.m
+-rw-r--r--   0        0        0      737 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/leonfcn.m
+-rw-r--r--   0        0        0      873 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/levin13fcn.m
+-rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/matyasfcn.m
+-rw-r--r--   0        0        0      800 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/mccormickfcn.m
+-rw-r--r--   0        0        0     1846 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/meshfcn.m
+-rw-r--r--   0        0        0      693 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/periodicfcn.m
+-rw-r--r--   0        0        0     1134 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/pichenyfcn.m
+-rw-r--r--   0        0        0      811 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/powellsumfcn.m
+-rw-r--r--   0        0        0      663 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/qingfcn.m
+-rw-r--r--   0        0        0      733 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/quarticfcn.m
+-rw-r--r--   0        0        0      682 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/rastriginfcn.m
+-rw-r--r--   0        0        0      951 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/ridgefcn.m
+-rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/rosenbrockfcn.m
+-rw-r--r--   0        0        0      723 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/salomonfcn.m
+-rw-r--r--   0        0        0      908 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/schaffern1fcn.m
+-rw-r--r--   0        0        0      883 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/schaffern2fcn.m
+-rw-r--r--   0        0        0      911 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/schaffern3fcn.m
+-rw-r--r--   0        0        0      911 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/schaffern4fcn.m
+-rw-r--r--   0        0        0      637 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/schwefel220fcn.m
+-rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/schwefel221fcn.m
+-rw-r--r--   0        0        0      671 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/schwefel222fcn.m
+-rw-r--r--   0        0        0      637 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/schwefel223fcn.m
+-rw-r--r--   0        0        0      678 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/schwefelfcn.m
+-rw-r--r--   0        0        0      747 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/shubert3fcn.m
+-rw-r--r--   0        0        0      743 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/shubert4fcn.m
+-rw-r--r--   0        0        0      843 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/shubertfcn.m
+-rw-r--r--   0        0        0      585 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/spherefcn.m
+-rw-r--r--   0        0        0      810 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/styblinskitankfcn.m
+-rw-r--r--   0        0        0      694 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/sumsquaresfcn.m
+-rw-r--r--   0        0        0     1848 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/surffcn.m
+-rw-r--r--   0        0        0      856 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/threehumpcamelfcn.m
+-rw-r--r--   0        0        0      780 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/wolfefcn.m
+-rw-r--r--   0        0        0      747 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/xinsheyangn1fcn.m
+-rw-r--r--   0        0        0      678 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/xinsheyangn2fcn.m
+-rw-r--r--   0        0        0     1456 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/xinsheyangn3fcn.m
+-rw-r--r--   0        0        0      718 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/xinsheyangn4fcn.m
+-rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/matlab/zakharovfcn.m
+-rw-r--r--   0        0        0     2386 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/python/benchmarkfcns/__init__.py
+-rw-r--r--   0        0        0     2097 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/python/benchmarkfcns/plotting.py
+-rw-r--r--   0        0        0      120 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/src/tests/test_basic.py
+-rw-r--r--   0        0        0     6022 2022-11-09 12:37:21.000000 benchmarkfcns-2.1.0/PKG-INFO
```

### Comparing `benchmarkfcns-2.0.0/.github/workflows/build.yaml` & `benchmarkfcns-2.1.0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/.pre-commit-config.yaml` & `benchmarkfcns-2.1.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
 # Standard hooks
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.5.0
   hooks:
-  - id: check-added-large-files
   - id: check-case-conflict
   - id: check-merge-conflict
   - id: check-symlinks
   - id: check-yaml
     exclude: ^conda\.recipe/meta\.yaml$
   - id: debug-statements
   - id: end-of-file-fixer
```

### Comparing `benchmarkfcns-2.0.0/CMakeLists.txt` & `benchmarkfcns-2.1.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/LICENSE` & `benchmarkfcns-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/optimiser/matlab/abc/FoodSources.m` & `benchmarkfcns-2.1.0/optimiser/matlab/abc/FoodSources.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/optimiser/matlab/abc/abc.m` & `benchmarkfcns-2.1.0/optimiser/matlab/abc/abc.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/optimiser/matlab/abc/abcoptions.m` & `benchmarkfcns-2.1.0/optimiser/matlab/abc/abcoptions.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/optimiser/python/abc.py` & `benchmarkfcns-2.1.0/optimiser/python/abc.py`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/pyproject.toml` & `benchmarkfcns-2.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 [tool.poetry]
 name = "Benchmark Functions"
-version = "2.0.0"
+version = "2.1.0"
 description = "A collection of benchmark functions for mathematical optimization algorithms."
 authors = ["Mazhar Ansari Ardeh"]
 
 [build-system]
 requires = ["scikit-build-core>=0.3.3", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "benchmarkfcns"
-version = "2.0.0"
+version = "2.1.0"
 description="A collection of benchmark functions for mathematical optimization algorithms."
 readme = "README.md"
 authors = [
   { name = "Mazhar Ansari Ardeh", email = "mazhar.ansari.ardeh@gmail.com" },
 ]
 requires-python = ">=3.9"
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 
 dependencies = [
```

### Comparing `benchmarkfcns-2.0.0/src/C++/benchmarkfcns.cpp` & `benchmarkfcns-2.1.0/src/C++/benchmarkfcns.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,28 @@
 
     VectorXd exponential(const Ref<const Matrix<double,Dynamic,Dynamic,RowMajor>>& x) {
         VectorXd scores = -exp(-0.5 * x.array().square().rowwise().sum());
 
         return scores;
     }
 
-   VectorXd giunta(const Ref<const Matrix<double,Dynamic,Dynamic,RowMajor>>& x) {
+    VectorXd forrester(const Ref<const Matrix<double,Dynamic,Dynamic,RowMajor>>& x)
+    {
+        int n = x.cols();
+        if (n != 1)
+            throw std::invalid_argument("The Forrester function is only defined on a 1D space.");
+
+        auto X = x.col(0).array();
+
+        VectorXd scores = (6 * X - 2).square() * sin(12 * X - 4);
+
+        return scores;
+    }
+
+    VectorXd giunta(const Ref<const Matrix<double,Dynamic,Dynamic,RowMajor>>& x) {
         VectorXd scores = 0.6 + ((sin(1 - (16.0 / 15.0) * x.array()).square())
                               - (1.0 / 50.0) * sin(4 - (64.0 / 15.0) * x.array())
                               - sin(1 - (16.0 / 15.0) * x.array())).rowwise().sum();
         return scores;
     }
 
     VectorXd goldsteinprice(const Ref<const Matrix<double,Dynamic,Dynamic,RowMajor>>& x) {
```

### Comparing `benchmarkfcns-2.0.0/src/C++/benchmarkfcns.h` & `benchmarkfcns-2.1.0/src/C++/benchmarkfcns.h`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 
     VectorXd eggcrate(const Ref<const Matrix<double,Dynamic,Dynamic,RowMajor>>& x);
 
     VectorXd elattar(const Ref<const Matrix<double,Dynamic,Dynamic,RowMajor>>& x);
 
     VectorXd exponential(const Ref<const Matrix<double,Dynamic,Dynamic,RowMajor>>& x);
 
+    VectorXd forrester(const Ref<const Matrix<double,Dynamic,Dynamic,RowMajor>>& x);
+
     VectorXd giunta(const Ref<const Matrix<double,Dynamic,Dynamic,RowMajor>>& x);
 
     VectorXd goldsteinprice(const Ref<const Matrix<double,Dynamic,Dynamic,RowMajor>>& x);
 
     VectorXd gramacylee(const Ref<const Matrix<double,Dynamic,Dynamic,RowMajor>>& x);
 
     VectorXd griewank(const Ref<const Matrix<double,Dynamic,Dynamic,RowMajor>>& x);
```

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/.gitlab/issue_templates/Bug Report.md` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/.gitlab/issue_templates/Bug Report.md`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/.gitlab/merge_request_templates/Merge Request Template.md` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/.gitlab/merge_request_templates/Merge Request Template.md`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/.gitlab-ci.yml` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/COPYING.APACHE` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/COPYING.APACHE`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/COPYING.BSD` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/COPYING.BSD`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/COPYING.GPL` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/COPYING.GPL`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/COPYING.LGPL` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/COPYING.LGPL`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/COPYING.MINPACK` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/COPYING.MINPACK`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/COPYING.MPL2` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/COPYING.MPL2`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/COPYING.README` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/COPYING.README`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/CTestConfig.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/CTestConfig.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/Cholesky` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/CholmodSupport` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/Core` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/Core`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/Eigenvalues` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/Geometry` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/Householder` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/IterativeLinearSolvers` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/Jacobi` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/KLUSupport` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/KLUSupport`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/LU` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/LU`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/MetisSupport` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/OrderingMethods` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/PaStiXSupport` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/PardisoSupport` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/QR` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/QR`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/QtAlignedMalloc` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/SPQRSupport` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/SVD` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/Sparse` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/SparseCholesky` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/SparseCore` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/SparseLU` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/SparseQR` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/StdDeque` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/StdList` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/StdVector` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/SuperLUSupport` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/UmfPackSupport` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Cholesky/LDLT.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Cholesky/LLT.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Cholesky/LLT_LAPACKE.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/CholmodSupport/CholmodSupport.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/ArithmeticSequence.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Array.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/ArrayBase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/ArrayWrapper.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Assign.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/AssignEvaluator.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Assign_MKL.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/BandMatrix.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Block.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/BooleanRedux.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/CommaInitializer.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/ConditionEstimator.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/CoreEvaluators.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/CoreIterators.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseBinaryOp.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseNullaryOp.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseTernaryOp.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseUnaryOp.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseUnaryView.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/DenseBase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/DenseCoeffsBase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/DenseStorage.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Diagonal.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/DiagonalMatrix.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/DiagonalProduct.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Dot.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/EigenBase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/ForceAlignedAccess.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Fuzzy.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/GeneralProduct.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/GenericPacketMath.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/GlobalFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/IO.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/IndexedView.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Inverse.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Map.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/MapBase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/MathFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/MathFunctionsImpl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Matrix.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/MatrixBase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/NestByValue.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/NoAlias.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/NumTraits.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/PartialReduxEvaluator.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/PermutationMatrix.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/PlainObjectBase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Product.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/ProductEvaluators.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Random.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Redux.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Ref.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Replicate.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Reshaped.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/ReturnByValue.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Reverse.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Select.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/SelfAdjointView.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/SelfCwiseBinaryOp.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Solve.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/SolveTriangular.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/SolverBase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/StableNorm.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/StlIterators.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Stride.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Swap.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Transpose.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Transpositions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/TriangularMatrix.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/VectorBlock.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/VectorwiseOp.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/Visitor.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX/Complex.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX/MathFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX/PacketMath.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX/TypeCasting.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX512/Complex.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX512/PacketMath.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/Complex.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/CUDA/Complex.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/BFloat16.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/ConjHelper.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/Half.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/Settings.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/TypeCasting.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/GPU/MathFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/GPU/PacketMath.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/GPU/TypeCasting.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/MSA/Complex.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/MSA/MathFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/MSA/PacketMath.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/Complex.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/MathFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/PacketMath.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/TypeCasting.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SSE/Complex.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SSE/MathFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SSE/PacketMath.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SSE/TypeCasting.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SVE/MathFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SVE/PacketMath.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SVE/TypeCasting.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/PacketMath.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/ZVector/Complex.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/ZVector/PacketMath.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/AssignmentFunctors.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/BinaryFunctors.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/NullaryFunctors.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/StlFunctors.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/TernaryFunctors.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/UnaryFunctors.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixVector.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/Parallelizer.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointProduct.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointRank2Update.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixVector.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverMatrix.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverVector.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/BlasUtil.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/ConfigureVectorization.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/Constants.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/DisableStupidWarnings.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/ForwardDeclarations.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/IndexedViewHelper.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/IntegralConstant.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/MKL_support.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/Macros.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/Memory.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/Meta.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/ReenableStupidWarnings.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/ReshapedHelper.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/StaticAssert.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/SymbolicIndex.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/XprHelper.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexSchur.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/EigenSolver.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/RealQZ.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/RealSchur.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/Tridiagonalization.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/AlignedBox.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/AngleAxis.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/EulerAngles.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Homogeneous.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Hyperplane.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/OrthoMethods.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/ParametrizedLine.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Quaternion.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Rotation2D.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/RotationBase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Scaling.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Transform.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Translation.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Umeyama.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/arch/Geometry_SIMD.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Geometry/arch/Geometry_SIMD.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Householder/BlockHouseholder.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Householder/Householder.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Householder/HouseholderSequence.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/Jacobi/Jacobi.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/KLUSupport/KLUSupport.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/KLUSupport/KLUSupport.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/LU/Determinant.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/LU/FullPivLU.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/LU/InverseImpl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/LU/PartialPivLU.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/LU/arch/InverseSize4.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/LU/arch/InverseSize4.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/MetisSupport/MetisSupport.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/OrderingMethods/Amd.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/OrderingMethods/Ordering.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/PardisoSupport/PardisoSupport.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/QR/ColPivHouseholderQR.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/QR/FullPivHouseholderQR.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/QR/HouseholderQR.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SVD/BDCSVD.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SVD/JacobiSVD.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SVD/SVDBase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SVD/UpperBidiagonalization.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/AmbiVector.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/CompressedStorage.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/MappedSparseMatrix.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseAssign.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseBlock.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseColEtree.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseCompressedBase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseDenseProduct.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseDot.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseFuzzy.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseMap.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseMatrix.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseMatrixBase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparsePermutation.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseProduct.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseRedux.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseRef.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseSolverBase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseTranspose.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseTriangularView.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseUtil.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseVector.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseView.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/TriangularSolver.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLUImpl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Memory.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Structs.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Utils.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_pivotL.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_pruneL.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SparseQR/SparseQR.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/StlSupport/StdDeque.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/StlSupport/StdList.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/StlSupport/StdVector.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/StlSupport/details.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/misc/Image.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/misc/Kernel.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/misc/RealSvd2x2.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/misc/blas.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/misc/lapack.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/misc/lapacke.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/BlockMethods.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/IndexedViewMethods.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/Eigen/src/plugins/ReshapedMethods.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/INSTALL` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/INSTALL`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/BenchSparseUtil.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/BenchSparseUtil.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/BenchTimer.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/BenchTimer.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/BenchUtil.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/BenchUtil.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/README.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/README.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/analyze-blocking-sizes.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/analyze-blocking-sizes.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/basicbench.cxxlist` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/basicbench.cxxlist`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/basicbenchmark.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/basicbenchmark.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/basicbenchmark.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/basicbenchmark.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchBlasGemm.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchBlasGemm.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchCholesky.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchCholesky.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchEigenSolver.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchEigenSolver.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchFFT.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchFFT.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchGeometry.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchGeometry.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchVecAdd.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchVecAdd.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/bench_gemm.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/bench_gemm.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/bench_move_semantics.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/bench_move_semantics.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/bench_multi_compilers.sh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/bench_multi_compilers.sh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/bench_norm.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/bench_norm.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/bench_reverse.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/bench_reverse.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/bench_unrolling` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/bench_unrolling`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchmark-blocking-sizes.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchmark-blocking-sizes.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchmark.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchmark.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchmarkSlice.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchmarkSlice.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchmarkX.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchmarkX.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchmarkXcwise.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchmarkXcwise.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/benchmark_suite` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/benchmark_suite`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/COPYING` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/COPYING`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/README` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/README`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_aat_product.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_aat_product.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_ata_product.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_ata_product.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_atv_product.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_atv_product.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_axpby.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_axpby.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_axpy.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_axpy.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_cholesky.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_cholesky.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_ger.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_ger.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_hessenberg.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_hessenberg.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_lu_decomp.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_lu_decomp.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_lu_solve.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_lu_solve.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_matrix_matrix_product.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_matrix_matrix_product.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_matrix_matrix_product_bis.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_matrix_matrix_product_bis.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_matrix_vector_product.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_matrix_vector_product.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_partial_lu.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_partial_lu.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_rot.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_rot.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_symv.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_symv.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_syr2.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_syr2.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_trisolve.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_trisolve.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_trisolve_matrix.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_trisolve_matrix.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/actions/action_trmm.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/actions/action_trmm.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindACML.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindACML.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindATLAS.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindATLAS.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindBLAZE.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindBLAZE.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindBlitz.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindBlitz.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindCBLAS.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindCBLAS.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindMKL.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindMKL.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindMTL4.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindMTL4.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindOPENBLAS.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindOPENBLAS.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindPackageHandleStandardArgs.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindTvmet.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/FindTvmet.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/action_settings.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/action_settings.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/gnuplot_common_settings.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/gnuplot_common_settings.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/go_mean` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/go_mean`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/mean.cxx` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/mean.cxx`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/mk_gnuplot_script.sh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/mk_gnuplot_script.sh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/mk_mean_script.sh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/mk_mean_script.sh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/mk_new_gnuplot.sh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/mk_new_gnuplot.sh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/perlib_plot_settings.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/perlib_plot_settings.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/regularize.cxx` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/regularize.cxx`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/smooth.cxx` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/smooth.cxx`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/data/smooth_all.sh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/data/smooth_all.sh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/bench.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/bench.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/bench_parameter.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/bench_parameter.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/btl.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/btl.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/init/init_function.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/init/init_function.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/init/init_matrix.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/init/init_matrix.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/init/init_vector.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/init/init_vector.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/static/bench_static.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/static/bench_static.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/static/intel_bench_fixed_size.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/static/intel_bench_fixed_size.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/static/static_size_generator.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/static/static_size_generator.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/STL_perf_analyzer.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/STL_perf_analyzer.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/STL_timer.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/STL_timer.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/portable_perf_analyzer.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/portable_perf_analyzer.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/portable_timer.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/portable_timer.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/x86_perf_analyzer.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/x86_perf_analyzer.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/x86_timer.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/timers/x86_timer.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/utils/size_lin_log.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/utils/size_lin_log.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/utils/size_log.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/utils/size_log.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/utils/utilities.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/utils/utilities.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/utils/xy_file.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/generic_bench/utils/xy_file.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/blas.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/blas.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/blas_interface.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/blas_interface.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/blas_interface_impl.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/blas_interface_impl.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/c_interface_base.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/c_interface_base.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/main.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/BLAS/main.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/STL/STL_interface.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/STL/STL_interface.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/STL/main.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/STL/main.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/blaze/blaze_interface.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/blaze/blaze_interface.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/blaze/main.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/blaze/main.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/blitz_LU_solve_interface.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/blitz_LU_solve_interface.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/blitz_interface.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/blitz_interface.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/btl_blitz.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/btl_blitz.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/btl_tiny_blitz.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/btl_tiny_blitz.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/tiny_blitz_interface.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/blitz/tiny_blitz_interface.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/eigen2_interface.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/eigen2_interface.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/main_adv.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/main_adv.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/main_linear.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/main_linear.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/main_matmat.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/main_matmat.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/main_vecmat.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen2/main_vecmat.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/eigen3_interface.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/eigen3_interface.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/main_adv.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/main_adv.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/main_linear.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/main_linear.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/main_matmat.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/main_matmat.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/main_vecmat.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/eigen3/main_vecmat.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/gmm/gmm_LU_solve_interface.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/gmm/gmm_LU_solve_interface.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/gmm/gmm_interface.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/gmm/gmm_interface.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/gmm/main.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/gmm/main.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/mtl4/main.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/mtl4/main.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/mtl4/mtl4_interface.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/mtl4/mtl4_interface.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/main_linear.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/main_linear.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/main_matmat.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/main_matmat.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/main_vecmat.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/main_vecmat.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/tensor_interface.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/tensors/tensor_interface.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/tvmet/main.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/tvmet/main.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/tvmet/tvmet_interface.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/tvmet/tvmet_interface.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/ublas/main.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/ublas/main.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/btl/libs/ublas/ublas_interface.hh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/btl/libs/ublas/ublas_interface.hh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/check_cache_queries.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/check_cache_queries.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/dense_solvers.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/dense_solvers.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/eig33.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/eig33.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/geometry.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/geometry.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/changesets.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/changesets.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemm_common.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemm_common.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemv_common.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/gemv_common.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/lazy_gemm.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/lazy_gemm.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/make_plot.sh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/make_plot.sh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/chart_footer.html` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/chart_footer.html`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/chart_header.html` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/chart_header.html`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/header.html` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/header.html`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/s1.js` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/s1.js`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/s2.js` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/resources/s2.js`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/run.sh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/run.sh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/perf_monitoring/runall.sh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/perf_monitoring/runall.sh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/product_threshold.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/product_threshold.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/quat_slerp.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/quat_slerp.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/quatmul.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/quatmul.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/sparse_cholesky.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/sparse_cholesky.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/sparse_dense_product.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/sparse_dense_product.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/sparse_lu.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/sparse_lu.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/sparse_product.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/sparse_product.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/sparse_randomsetter.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/sparse_randomsetter.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/sparse_setter.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/sparse_setter.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/sparse_transpose.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/sparse_transpose.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/sparse_trisolver.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/sparse_trisolver.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/spbench/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/spbench/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/spbench/sp_solver.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/spbench/sp_solver.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/spbench/spbench.dtd` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/spbench/spbench.dtd`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/spbench/spbenchsolver.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/spbench/spbenchsolver.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/spbench/spbenchsolver.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/spbench/spbenchsolver.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/spbench/spbenchstyle.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/spbench/spbenchstyle.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/spbench/test_sparseLU.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/spbench/test_sparseLU.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/spmv.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/spmv.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/README` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/README`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/benchmark.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/benchmark.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/benchmark_main.cc` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/benchmark_main.cc`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/contraction_benchmarks_cpu.cc` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/contraction_benchmarks_cpu.cc`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/eigen_sycl_bench.sh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/eigen_sycl_bench.sh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/eigen_sycl_bench_contract.sh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/eigen_sycl_bench_contract.sh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks_cpu.cc` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks_cpu.cc`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks_fp16_gpu.cu` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks_fp16_gpu.cu`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks_gpu.cu` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks_gpu.cu`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks_sycl.cc` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/tensor_benchmarks_sycl.cc`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/tensors/tensor_contract_sycl_bench.cc` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/tensors/tensor_contract_sycl_bench.cc`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/bench/vdw_new.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/bench/vdw_new.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/BandTriangularSolver.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/BandTriangularSolver.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/GeneralRank1Update.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/GeneralRank1Update.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/PackedSelfadjointProduct.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/PackedSelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/PackedTriangularMatrixVector.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/PackedTriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/PackedTriangularSolverVector.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/PackedTriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/Rank2Update.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/Rank2Update.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/common.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/common.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/complex_double.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/complex_double.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/complex_single.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/complex_single.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/double.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/double.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/chbmv.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/chbmv.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/chpmv.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/chpmv.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/complexdots.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/complexdots.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/ctbmv.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/ctbmv.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/datatypes.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/datatypes.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/drotm.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/drotm.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/drotmg.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/drotmg.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/dsbmv.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/dsbmv.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/dspmv.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/dspmv.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/dtbmv.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/dtbmv.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/lsame.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/lsame.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/srotm.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/srotm.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/srotmg.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/srotmg.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/ssbmv.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/ssbmv.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/sspmv.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/sspmv.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/stbmv.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/stbmv.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/zhbmv.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/zhbmv.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/zhpmv.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/zhpmv.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/f2c/ztbmv.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/f2c/ztbmv.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/fortran/complexdots.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/fortran/complexdots.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/level1_cplx_impl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/level1_cplx_impl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/level1_impl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/level1_impl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/level1_real_impl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/level1_real_impl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/level2_cplx_impl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/level2_cplx_impl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/level2_impl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/level2_impl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/level2_real_impl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/level2_real_impl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/level3_impl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/level3_impl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/single.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/single.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/cblat1.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/cblat1.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/cblat2.dat` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/cblat2.dat`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/cblat2.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/cblat2.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/cblat3.dat` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/cblat3.dat`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/cblat3.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/cblat3.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/dblat1.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/dblat1.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/dblat2.dat` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/dblat2.dat`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/dblat2.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/dblat2.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/dblat3.dat` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/dblat3.dat`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/dblat3.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/dblat3.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/runblastest.sh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/runblastest.sh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/sblat1.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/sblat1.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/sblat2.dat` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/sblat2.dat`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/sblat2.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/sblat2.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/sblat3.dat` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/sblat3.dat`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/sblat3.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/sblat3.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/zblat1.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/zblat1.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/zblat2.dat` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/zblat2.dat`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/zblat2.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/zblat2.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/zblat3.dat` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/zblat3.dat`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/blas/testing/zblat3.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/blas/testing/zblat3.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/ci/CTest2JUnit.xsl` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/ci/CTest2JUnit.xsl`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/ci/README.md` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/ci/README.md`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/ci/build.gitlab-ci.yml` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/ci/build.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/ci/smoketests.gitlab-ci.yml` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/ci/smoketests.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/ci/test.gitlab-ci.yml` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/ci/test.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/ComputeCppCompilerChecks.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/ComputeCppCompilerChecks.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/Eigen3Config.cmake.in` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/Eigen3Config.cmake.in`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/Eigen3ConfigLegacy.cmake.in` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/Eigen3ConfigLegacy.cmake.in`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/EigenConfigureTesting.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/EigenConfigureTesting.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/EigenDetermineOSVersion.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/EigenDetermineOSVersion.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/EigenDetermineVSServicePack.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/EigenDetermineVSServicePack.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/EigenSmokeTestList.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/EigenSmokeTestList.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/EigenTesting.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/EigenTesting.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/EigenUninstall.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/EigenUninstall.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindAdolc.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindAdolc.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindBLAS.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindBLAS.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindBLASEXT.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindBLASEXT.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindCHOLMOD.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindCHOLMOD.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindComputeCpp.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindComputeCpp.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindEigen2.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindEigen2.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindEigen3.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindFFTW.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindFFTW.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindGLEW.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindGLEW.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindGMP.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindGMP.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindGSL.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindGSL.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindGoogleHash.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindGoogleHash.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindHWLOC.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindHWLOC.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindKLU.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindKLU.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindLAPACK.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindLAPACK.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindMPFR.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindMPFR.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindMPREAL.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindMPREAL.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindMetis.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindMetis.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindPASTIX.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindPASTIX.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindPTSCOTCH.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindPTSCOTCH.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindSCOTCH.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindSCOTCH.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindSPQR.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindSPQR.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindStandardMathLibrary.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindStandardMathLibrary.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindSuperLU.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindSuperLU.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindTriSYCL.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindTriSYCL.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/FindUMFPACK.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/FindUMFPACK.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/cmake/RegexUtils.cmake` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/cmake/RegexUtils.cmake`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/debug/gdb/printers.py` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/debug/gdb/printers.py`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/debug/msvc/eigen.natvis` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/debug/msvc/eigen.natvis`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/debug/msvc/eigen_autoexp_part.dat` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/debug/msvc/eigen_autoexp_part.dat`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/mandelbrot/mandelbrot.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/mandelbrot/mandelbrot.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/mandelbrot/mandelbrot.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/mandelbrot/mandelbrot.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/mix_eigen_and_c/binary_library.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/mix_eigen_and_c/binary_library.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/mix_eigen_and_c/binary_library.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/mix_eigen_and_c/binary_library.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/mix_eigen_and_c/example.c` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/mix_eigen_and_c/example.c`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/camera.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/camera.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/camera.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/camera.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/gpuhelper.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/gpuhelper.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/gpuhelper.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/gpuhelper.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/icosphere.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/icosphere.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/icosphere.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/icosphere.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/quaternion_demo.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/quaternion_demo.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/quaternion_demo.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/quaternion_demo.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/trackball.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/trackball.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/demos/opengl/trackball.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/demos/opengl/trackball.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/AsciiQuickReference.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/AsciiQuickReference.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/B01_Experimental.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/B01_Experimental.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/ClassHierarchy.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/ClassHierarchy.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/CoeffwiseMathFunctionsTable.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/CoeffwiseMathFunctionsTable.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/CustomizingEigen_CustomScalar.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/CustomizingEigen_CustomScalar.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/CustomizingEigen_InheritingMatrix.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/CustomizingEigen_InheritingMatrix.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/CustomizingEigen_NullaryExpr.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/CustomizingEigen_NullaryExpr.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/CustomizingEigen_Plugins.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/CustomizingEigen_Plugins.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/DenseDecompositionBenchmark.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/DenseDecompositionBenchmark.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/Doxyfile.in` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/Eigen_Silly_Professor_64x64.png` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/Eigen_Silly_Professor_64x64.png`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/FixedSizeVectorizable.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/FixedSizeVectorizable.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/FunctionsTakingEigenTypes.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/FunctionsTakingEigenTypes.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/HiPerformance.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/HiPerformance.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/InplaceDecomposition.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/InplaceDecomposition.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/InsideEigenExample.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/InsideEigenExample.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/LeastSquares.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/LeastSquares.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/Manual.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/Manual.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/MatrixfreeSolverExample.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/MatrixfreeSolverExample.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/NewExpressionType.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/NewExpressionType.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/Overview.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/Overview.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/PassingByValue.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/PassingByValue.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/Pitfalls.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/Pitfalls.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/PreprocessorDirectives.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/PreprocessorDirectives.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/QuickReference.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/QuickReference.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/QuickStartGuide.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/QuickStartGuide.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/SparseLinearSystems.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/SparseLinearSystems.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/SparseQuickReference.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/SparseQuickReference.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/StlContainers.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/StlContainers.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/StorageOrders.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/StorageOrders.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/StructHavingEigenMembers.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/StructHavingEigenMembers.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TemplateKeyword.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TemplateKeyword.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TopicAliasing.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TopicAliasing.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TopicAssertions.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TopicAssertions.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TopicCMakeGuide.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TopicCMakeGuide.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TopicLazyEvaluation.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TopicLazyEvaluation.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TopicLinearAlgebraDecompositions.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TopicLinearAlgebraDecompositions.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TopicMultithreading.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TopicMultithreading.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialAdvancedInitialization.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialAdvancedInitialization.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialArrayClass.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialArrayClass.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialBlockOperations.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialBlockOperations.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialGeometry.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialGeometry.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialLinearAlgebra.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialLinearAlgebra.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialMapClass.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialMapClass.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialMatrixArithmetic.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialMatrixArithmetic.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialMatrixClass.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialMatrixClass.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialReductionsVisitorsBroadcasting.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialReductionsVisitorsBroadcasting.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialReshape.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialReshape.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialSTL.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialSTL.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialSlicingIndexing.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialSlicingIndexing.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/TutorialSparse.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/TutorialSparse.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/UnalignedArrayAssert.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/UnalignedArrayAssert.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/UsingBlasLapackBackends.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/UsingBlasLapackBackends.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/UsingIntelMKL.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/UsingIntelMKL.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/UsingNVCC.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/UsingNVCC.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/WrongStackAlignment.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/WrongStackAlignment.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/eigen_navtree_hacks.js` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/eigen_navtree_hacks.js`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/eigendoxy.css` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/eigendoxy.css`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/eigendoxy_footer.html.in` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/eigendoxy_footer.html.in`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/eigendoxy_header.html.in` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/eigendoxy_header.html.in`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/eigendoxy_layout.xml.in` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/eigendoxy_layout.xml.in`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/eigendoxy_tabs.css` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/eigendoxy_tabs.css`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/CustomizingEigen_Inheritance.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/CustomizingEigen_Inheritance.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TemplateKeyword_flexible.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TemplateKeyword_flexible.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TutorialInplaceLU.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TutorialInplaceLU.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgComputeTwice.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgComputeTwice.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgRankRevealing.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgRankRevealing.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_block_assignment.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_BlockOperations_block_assignment.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_simple_example_dynamic_size.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/Tutorial_simple_example_dynamic_size.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/class_Block.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/class_Block.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/class_CwiseBinaryOp.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/class_CwiseBinaryOp.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/class_CwiseUnaryOp.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/class_CwiseUnaryOp.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/class_FixedBlock.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/class_FixedBlock.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/class_FixedVectorBlock.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/class_FixedVectorBlock.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/class_Reshaped.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/class_Reshaped.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/class_VectorBlock.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/class_VectorBlock.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/function_taking_ref.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/function_taking_ref.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.evaluator` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.evaluator`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.expression` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.expression`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.traits` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/make_circulant.cpp.traits`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/make_circulant2.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/make_circulant2.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/matrixfree_cg.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/matrixfree_cg.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/nullary_indexing.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/nullary_indexing.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/tut_arithmetic_matrix_mul.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/tut_arithmetic_matrix_mul.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/examples/tut_arithmetic_redux_basic.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/examples/tut_arithmetic_redux_basic.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/ComplexEigenSolver_compute.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/ComplexEigenSolver_compute.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/HouseholderSequence_HouseholderSequence.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/HouseholderSequence_HouseholderSequence.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/IOFormat.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/IOFormat.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/JacobiSVD_basic.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/JacobiSVD_basic.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/LLT_example.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/LLT_example.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_all.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_all.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_triangularView.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/MatrixBase_triangularView.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/RealQZ_compute.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/RealQZ_compute.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_cwise.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/TopicAliasing_cwise.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/TopicStorageOrders_example.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/TopicStorageOrders_example.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Triangular_solve.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Triangular_solve.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tridiagonalization_decomposeInPlace.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tridiagonalization_decomposeInPlace.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tridiagonalization_diagonal.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tridiagonalization_diagonal.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_Map_using.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_Map_using.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_SlicingCol.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Tutorial_SlicingCol.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/Vectorwise_reverse.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/Vectorwise_reverse.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/class_FullPivLU.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/class_FullPivLU.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/snippets/compile_snippet.cpp.in` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/snippets/compile_snippet.cpp.in`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/special_examples/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/special_examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/special_examples/Tutorial_sparse_example.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/special_examples/Tutorial_sparse_example.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/special_examples/Tutorial_sparse_example_details.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/special_examples/Tutorial_sparse_example_details.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/doc/tutorial.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/doc/tutorial.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/failtest/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/failtest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/cholesky.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/cholesky.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/clacgv.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/clacgv.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/cladiv.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/cladiv.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/clarf.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/clarf.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/clarfb.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/clarfb.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/clarfg.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/clarfg.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/clarft.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/clarft.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/complex_double.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/complex_double.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/complex_single.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/complex_single.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dladiv.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dladiv.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dlamch.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dlamch.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dlapy2.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dlapy2.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dlapy3.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dlapy3.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dlarf.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dlarf.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dlarfb.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dlarfb.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dlarfg.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dlarfg.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dlarft.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dlarft.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/double.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/double.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/dsecnd_NONE.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/dsecnd_NONE.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/eigenvalues.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/eigenvalues.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/ilaclc.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/ilaclc.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/ilaclr.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/ilaclr.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/iladlc.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/iladlc.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/iladlr.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/iladlr.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/ilaslc.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/ilaslc.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/ilaslr.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/ilaslr.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/ilazlc.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/ilazlc.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/ilazlr.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/ilazlr.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/lapack_common.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/lapack_common.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/lu.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/lu.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/second_NONE.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/second_NONE.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/single.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/single.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/sladiv.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/sladiv.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/slamch.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/slamch.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/slapy2.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/slapy2.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/slapy3.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/slapy3.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/slarf.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/slarf.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/slarfb.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/slarfb.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/slarfg.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/slarfg.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/slarft.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/slarft.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/svd.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/svd.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/zlacgv.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/zlacgv.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/zladiv.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/zladiv.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/zlarf.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/zlarf.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/zlarfb.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/zlarfb.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/zlarfg.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/zlarfg.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/lapack/zlarft.f` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/lapack/zlarft.f`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/buildtests.in` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/buildtests.in`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/cdashtesting.cmake.in` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/cdashtesting.cmake.in`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/check.in` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/check.in`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/eigen_gen_credits.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/eigen_gen_credits.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/eigen_gen_docs` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/eigen_gen_docs`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/eigen_monitor_perf.sh` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/eigen_monitor_perf.sh`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/scripts/relicense.py` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/scripts/relicense.py`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/AnnoyingScalar.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/AnnoyingScalar.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/MovableScalar.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/MovableScalar.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/SafeScalar.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/SafeScalar.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/adjoint.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/adjoint.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/array_cwise.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/array_cwise.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/array_for_matrix.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/array_for_matrix.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/array_of_string.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/array_of_string.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/array_replicate.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/array_replicate.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/array_reverse.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/array_reverse.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/bandmatrix.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/bandmatrix.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/basicstuff.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/basicstuff.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/bdcsvd.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/bdcsvd.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/bfloat16_float.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/bfloat16_float.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/bicgstab.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/bicgstab.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/blasutil.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/blasutil.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/block.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/block.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/boostmultiprec.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/boostmultiprec.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/cholesky.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/cholesky.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/cholmod_support.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/cholmod_support.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/commainitializer.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/commainitializer.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/conjugate_gradient.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/conjugate_gradient.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/conservative_resize.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/conservative_resize.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/constructor.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/constructor.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/corners.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/corners.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/ctorleak.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/ctorleak.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/denseLM.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/denseLM.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/dense_storage.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/dense_storage.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/determinant.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/determinant.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/diagonal.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/diagonal.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/diagonal_matrix_variadic_ctor.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/diagonal_matrix_variadic_ctor.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/diagonalmatrices.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/diagonalmatrices.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/dontalign.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/dontalign.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/dynalloc.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/dynalloc.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/eigen2support.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/eigen2support.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/eigensolver_complex.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/eigensolver_complex.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/eigensolver_generalized_real.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/eigensolver_generalized_real.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/eigensolver_generic.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/eigensolver_generic.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/eigensolver_selfadjoint.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/eigensolver_selfadjoint.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/evaluators.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/evaluators.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/exceptions.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/exceptions.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/fastmath.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/fastmath.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/first_aligned.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/first_aligned.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/geo_alignedbox.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/geo_alignedbox.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/geo_eulerangles.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/geo_eulerangles.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/geo_homogeneous.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/geo_homogeneous.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/geo_hyperplane.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/geo_hyperplane.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/geo_orthomethods.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/geo_orthomethods.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/geo_parametrizedline.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/geo_parametrizedline.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/geo_quaternion.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/geo_quaternion.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/geo_transformations.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/geo_transformations.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/gpu_basic.cu` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/gpu_basic.cu`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/gpu_common.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/gpu_common.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/half_float.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/half_float.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/hessenberg.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/hessenberg.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/householder.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/householder.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/incomplete_cholesky.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/incomplete_cholesky.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/indexed_view.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/indexed_view.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/initializer_list_construction.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/initializer_list_construction.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/inplace_decomposition.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/inplace_decomposition.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/integer_types.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/integer_types.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/inverse.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/inverse.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/io.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/io.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/is_same_dense.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/is_same_dense.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/jacobi.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/jacobi.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/jacobisvd.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/jacobisvd.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/klu_support.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/klu_support.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/linearstructure.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/linearstructure.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/lscg.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/lscg.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/lu.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/lu.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/main.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/main.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/mapped_matrix.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/mapped_matrix.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/mapstaticmethods.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/mapstaticmethods.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/mapstride.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/mapstride.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/meta.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/meta.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/metis_support.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/metis_support.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/miscmatrices.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/miscmatrices.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/mixingtypes.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/mixingtypes.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/mpl2only.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/mpl2only.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/nestbyvalue.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/nestbyvalue.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/nesting_ops.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/nesting_ops.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/nomalloc.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/nomalloc.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/nullary.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/nullary.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/num_dimensions.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/num_dimensions.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/numext.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/numext.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/packetmath.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/packetmath.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/packetmath_test_shared.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/packetmath_test_shared.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/pardiso_support.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/pardiso_support.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/pastix_support.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/pastix_support.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/permutationmatrices.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/permutationmatrices.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/prec_inverse_4x4.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/prec_inverse_4x4.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_extra.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_extra.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_large.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_large.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_mmtr.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_mmtr.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_notemporary.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_notemporary.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_selfadjoint.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_selfadjoint.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_small.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_small.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_symm.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_symm.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_syrk.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_syrk.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_trmm.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_trmm.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_trmv.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_trmv.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/product_trsolve.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/product_trsolve.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/qr.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/qr.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/qr_colpivoting.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/qr_colpivoting.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/qr_fullpivoting.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/qr_fullpivoting.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/qtvector.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/qtvector.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/rand.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/rand.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/random_without_cast_overflow.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/random_without_cast_overflow.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/real_qz.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/real_qz.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/redux.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/redux.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/ref.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/ref.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/reshape.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/reshape.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/resize.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/resize.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/rvalue_types.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/rvalue_types.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/schur_complex.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/schur_complex.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/schur_real.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/schur_real.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/selfadjoint.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/selfadjoint.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/simplicial_cholesky.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/simplicial_cholesky.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sizeof.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sizeof.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sizeoverflow.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sizeoverflow.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/smallvectors.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/smallvectors.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/solverbase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/solverbase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparseLM.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparseLM.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse_basic.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse_basic.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse_block.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse_block.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse_permutations.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse_permutations.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse_product.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse_product.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse_ref.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse_ref.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse_solver.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse_solver.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse_solvers.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse_solvers.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparse_vector.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparse_vector.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparselu.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparselu.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/sparseqr.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/sparseqr.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/special_numbers.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/special_numbers.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/split_test_helper.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/split_test_helper.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/spqr_support.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/spqr_support.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/stable_norm.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/stable_norm.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/stddeque.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/stddeque.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/stddeque_overload.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/stddeque_overload.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/stdlist.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/stdlist.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/stdlist_overload.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/stdlist_overload.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/stdvector.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/stdvector.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/stdvector_overload.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/stdvector_overload.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/stl_iterators.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/stl_iterators.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/superlu_support.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/superlu_support.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/svd_common.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/svd_common.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/svd_fill.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/svd_fill.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/swap.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/swap.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/symbolic_index.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/symbolic_index.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/triangular.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/triangular.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/type_alias.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/type_alias.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/umeyama.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/umeyama.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/umfpack_support.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/umfpack_support.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/unalignedcount.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/unalignedcount.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/upperbidiagonalization.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/upperbidiagonalization.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/vectorization_logic.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/vectorization_logic.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/vectorwiseop.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/vectorwiseop.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/visitor.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/visitor.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/test/zerosized.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/test/zerosized.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/AdolcForward` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/AdolcForward`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/AlignedVector3` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/AlignedVector3`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/ArpackSupport` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/ArpackSupport`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/AutoDiff` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/AutoDiff`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/BVH` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/BVH`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/Tensor` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/Tensor`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/TensorSymmetry` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/TensorSymmetry`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/ThreadPool` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/ThreadPool`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/README.md` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/README.md`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/Tensor.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/Tensor.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/CXX11Meta.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/CXX11Meta.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/EmulateArray.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/EmulateArray.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/EulerAngles` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/EulerAngles`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/FFT` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/FFT`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/IterativeSolvers` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/IterativeSolvers`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/KroneckerProduct` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/KroneckerProduct`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/LevenbergMarquardt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/LevenbergMarquardt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/MPRealSupport` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/MPRealSupport`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/MatrixFunctions` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/MatrixFunctions`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/MoreVectorization` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/MoreVectorization`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/NonLinearOptimization` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/NonLinearOptimization`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/NumericalDiff` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/NumericalDiff`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/OpenGLSupport` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/OpenGLSupport`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/Polynomials` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/Polynomials`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/Skyline` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/Skyline`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/SparseExtra` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/SparseExtra`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/SpecialFunctions` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/SpecialFunctions`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/Splines` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/Splines`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/BVH/BVAlgorithms.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/BVH/BVAlgorithms.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/BVH/KdBVH.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/BVH/KdBVH.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/EulerAngles.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/EulerSystem.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/EulerAngles/EulerSystem.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/FFT/ei_fftw_impl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/FFT/ei_fftw_impl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/FFT/ei_kissfft_impl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/FFT/ei_kissfft_impl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/DGMRES.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/DGMRES.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/GMRES.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/GMRES.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IDRS.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IDRS.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IterationController.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/IterationController.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/MINRES.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/MINRES.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/Scaling.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/IterativeSolvers/Scaling.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/StemFunction.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MatrixFunctions/StemFunction.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MoreVectorization/MathFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/MoreVectorization/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/chkder.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/chkder.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/covar.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/covar.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/dogleg.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/dogleg.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/lmpar.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/lmpar.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/r1updt.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/r1updt.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Polynomials/Companion.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Polynomials/Companion.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Polynomials/PolynomialSolver.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Polynomials/PolynomialSolver.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Polynomials/PolynomialUtils.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Polynomials/PolynomialUtils.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineMatrix.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineMatrix.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineProduct.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineProduct.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineStorage.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineStorage.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineUtil.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Skyline/SkylineUtil.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/MarketIO.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/MarketIO.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/RandomSetter.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SparseExtra/RandomSetter.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Splines/Spline.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Splines/Spline.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Splines/SplineFitting.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Splines/SplineFitting.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Splines/SplineFwd.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/Eigen/src/Splines/SplineFwd.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/README.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/README.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/bench/bench_svd.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/bench/bench_svd.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/Overview.dox` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/Overview.dox`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/eigendoxy_layout.xml.in` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/eigendoxy_layout.xml.in`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/BVH_Example.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/BVH_Example.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/EulerAngles.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/EulerAngles.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/FFT.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/FFT.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixSinh.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/MatrixSinh.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/PolynomialSolver1.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/PolynomialSolver1.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/PolynomialUtils1.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/PolynomialUtils1.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/SYCL/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/SYCL/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/examples/SYCL/CwiseMul.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/examples/SYCL/CwiseMul.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/doc/snippets/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/doc/snippets/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/BVH.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/BVH.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/CMakeLists.txt` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/EulerAngles.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/EulerAngles.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/FFTW.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/FFTW.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/NonLinearOptimization.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/NonLinearOptimization.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/NumericalDiff.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/NumericalDiff.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/alignedvector3.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/alignedvector3.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/autodiff.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/autodiff.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/autodiff_scalar.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/autodiff_scalar.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/bessel_functions.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/bessel_functions.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_eventcount.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_eventcount.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_maxsizevector.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_maxsizevector.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_meta.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_meta.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_non_blocking_thread_pool.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_non_blocking_thread_pool.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_runqueue.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_runqueue.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax_gpu.cu` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax_gpu.cu`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_argmax_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_assign.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_assign.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_block_access.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_block_access.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_block_eval.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_block_eval.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_block_io.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_block_io.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_broadcast_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_broadcast_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_broadcasting.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_broadcasting.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_builtins_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_builtins_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_cast_float16_gpu.cu` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_cast_float16_gpu.cu`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_casts.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_casts.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_chipping.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_chipping.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_chipping_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_chipping_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_comparisons.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_comparisons.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_complex_cwise_ops_gpu.cu` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_complex_cwise_ops_gpu.cu`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_complex_gpu.cu` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_complex_gpu.cu`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_concatenation.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_concatenation.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_concatenation_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_concatenation_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_const.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_const.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_contract_gpu.cu` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_contract_gpu.cu`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_contract_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_contract_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_contraction.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_contraction.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_convolution.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_convolution.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_convolution_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_convolution_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_index.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_index.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_op.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_op.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_op_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_custom_op_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_device.cu` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_device.cu`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_device_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_device_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_dimension.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_dimension.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_empty.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_empty.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_executor.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_executor.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_expr.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_expr.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_fft.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_fft.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_fixed_size.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_fixed_size.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_forced_eval.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_forced_eval.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_generator.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_generator.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_generator_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_generator_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_gpu.cu` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_gpu.cu`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_ifft.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_ifft.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_image_op_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_image_op_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_image_patch.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_image_patch.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_image_patch_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_image_patch_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_index_list.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_index_list.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_inflation.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_inflation.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_inflation_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_inflation_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_intdiv.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_intdiv.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_io.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_io.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_layout_swap.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_layout_swap.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_layout_swap_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_layout_swap_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_lvalue.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_lvalue.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_map.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_map.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_math.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_math.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_math_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_math_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_mixed_indices.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_mixed_indices.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_morphing.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_morphing.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_morphing_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_morphing_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_move.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_move.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_notification.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_notification.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_of_complex.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_of_complex.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_of_const_values.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_of_const_values.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_of_float16_gpu.cu` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_of_float16_gpu.cu`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_of_strings.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_of_strings.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_padding.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_padding.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_padding_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_padding_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_patch.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_patch.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_patch_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_patch_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_random.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_random.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_random_gpu.cu` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_random_gpu.cu`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_random_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_random_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction_gpu.cu` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction_gpu.cu`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reduction_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_ref.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_ref.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reverse.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reverse.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reverse_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_reverse_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_roundings.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_roundings.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_scan.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_scan.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_scan_gpu.cu` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_scan_gpu.cu`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_scan_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_scan_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_shuffling.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_shuffling.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_shuffling_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_shuffling_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_simple.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_simple.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_striding.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_striding.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_striding_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_striding_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_sugar.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_sugar.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_symmetry.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_symmetry.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_thread_local.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_thread_local.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_thread_pool.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_thread_pool.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_trace.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_trace.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_uint128.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_uint128.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_volume_patch.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_volume_patch.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_volume_patch_sycl.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/cxx11_tensor_volume_patch_sycl.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/dgmres.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/dgmres.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/forward_adolc.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/forward_adolc.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/gmres.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/gmres.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/idrs.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/idrs.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/kronecker_product.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/kronecker_product.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/levenberg_marquardt.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/levenberg_marquardt.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/matrix_exponential.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/matrix_exponential.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/matrix_function.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/matrix_function.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/matrix_functions.h` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/matrix_functions.h`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/matrix_power.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/matrix_power.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/matrix_square_root.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/matrix_square_root.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/minres.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/minres.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/mpreal_support.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/mpreal_support.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/openglsupport.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/openglsupport.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/polynomialsolver.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/polynomialsolver.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/polynomialutils.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/polynomialutils.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/sparse_extra.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/sparse_extra.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/special_functions.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/special_functions.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/special_packetmath.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/special_packetmath.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/eigen-3.4.0/unsupported/test/splines.cpp` & `benchmarkfcns-2.1.0/src/C++/eigen-3.4.0/unsupported/test/splines.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/fcns.cpp` & `benchmarkfcns-2.1.0/src/C++/fcns.cpp`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/C++/main.cpp` & `benchmarkfcns-2.1.0/src/C++/main.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -265,14 +265,24 @@
         function at point X. `exponential` accepts a matrix of size M-by-N and
         returns a vetor SCORES of size M-by-1 in which each row contains the
         function value for the corresponding row of X.
         For more information, please visit:
         benchmarkfcns.info/doc/exponentialfcn
     )pbdoc");
 
+    m.def("forrester", &forrester, R"pbdoc(
+        Computes the value of the Forrester benchmark function.
+        SCORES = forrester(X) computes the value of the Forrester function at
+        point X. `forrester` accepts a matrix of size M-by-N and returns a vetor
+        SCORES of size M-by-1 in which each row contains the
+        function value for the corresponding row of X.
+        For more information, please visit:
+        benchmarkfcns.info/doc/forresterfcn
+    )pbdoc");
+
     m.def("giunta", &giunta, R"pbdoc(
         Computes the value of the Giunta function.
         SCORES = giunta(X) computes the value of the Alpine N. 1
         function at point X. `giunta` accepts a matrix of size M-by-N and
         returns a vetor SCORES of size M-by-1 in which each row contains the
         function value for the corresponding row of X.
         For more information, please visit:
```

### Comparing `benchmarkfcns-2.0.0/src/matlab/ackleyfcn.m` & `benchmarkfcns-2.1.0/src/matlab/ackleyfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/ackleyn2fcn.m` & `benchmarkfcns-2.1.0/src/matlab/ackleyn2fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/ackleyn3fcn.m` & `benchmarkfcns-2.1.0/src/matlab/ackleyn3fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/ackleyn4fcn.m` & `benchmarkfcns-2.1.0/src/matlab/ackleyn4fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/adjimanfcn.m` & `benchmarkfcns-2.1.0/src/matlab/adjimanfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/alpinen1fcn.m` & `benchmarkfcns-2.1.0/src/matlab/alpinen1fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/alpinen2fcn.m` & `benchmarkfcns-2.1.0/src/matlab/alpinen2fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/bartelsconnfcn.m` & `benchmarkfcns-2.1.0/src/matlab/bartelsconnfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/bealefcn.m` & `benchmarkfcns-2.1.0/src/matlab/bealefcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/birdfcn.m` & `benchmarkfcns-2.1.0/src/matlab/birdfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/bohachevskyn1fcn.m` & `benchmarkfcns-2.1.0/src/matlab/bohachevskyn1fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/bohachevskyn2fcn.m` & `benchmarkfcns-2.1.0/src/matlab/bohachevskyn2fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/boothfcn.m` & `benchmarkfcns-2.1.0/src/matlab/boothfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/brentfcn.m` & `benchmarkfcns-2.1.0/src/matlab/brentfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/brownfcn.m` & `benchmarkfcns-2.1.0/src/matlab/brownfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/bukinn6fcn.m` & `benchmarkfcns-2.1.0/src/matlab/bukinn6fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/contourfcn.m` & `benchmarkfcns-2.1.0/src/matlab/contourfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/crossintrayfcn.m` & `benchmarkfcns-2.1.0/src/matlab/crossintrayfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/deckkersaartsfcn.m` & `benchmarkfcns-2.1.0/src/matlab/deckkersaartsfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/dropwavefcn.m` & `benchmarkfcns-2.1.0/src/matlab/dropwavefcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/easomfcn.m` & `benchmarkfcns-2.1.0/src/matlab/easomfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/eggcratefcn.m` & `benchmarkfcns-2.1.0/src/matlab/eggcratefcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/eggholderfcn.m` & `benchmarkfcns-2.1.0/src/matlab/eggholderfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/elattarfcn.m` & `benchmarkfcns-2.1.0/src/matlab/elattarfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/exponentialfcn.m` & `benchmarkfcns-2.1.0/src/matlab/exponentialfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/giuntafcn.m` & `benchmarkfcns-2.1.0/src/matlab/giuntafcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/goldsteinpricefcn.m` & `benchmarkfcns-2.1.0/src/matlab/goldsteinpricefcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/gramacyleefcn.m` & `benchmarkfcns-2.1.0/src/matlab/gramacyleefcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/griewankfcn.m` & `benchmarkfcns-2.1.0/src/matlab/griewankfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/happycatfcn.m` & `benchmarkfcns-2.1.0/src/matlab/happycatfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/himmelblaufcn.m` & `benchmarkfcns-2.1.0/src/matlab/himmelblaufcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/holdertablefcn.m` & `benchmarkfcns-2.1.0/src/matlab/holdertablefcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/keanefcn.m` & `benchmarkfcns-2.1.0/src/matlab/keanefcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/leonfcn.m` & `benchmarkfcns-2.1.0/src/matlab/leonfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/levin13fcn.m` & `benchmarkfcns-2.1.0/src/matlab/levin13fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/matyasfcn.m` & `benchmarkfcns-2.1.0/src/matlab/matyasfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/mccormickfcn.m` & `benchmarkfcns-2.1.0/src/matlab/mccormickfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/meshfcn.m` & `benchmarkfcns-2.1.0/src/matlab/meshfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/periodicfcn.m` & `benchmarkfcns-2.1.0/src/matlab/periodicfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/pichenyfcn.m` & `benchmarkfcns-2.1.0/src/matlab/pichenyfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/powellsumfcn.m` & `benchmarkfcns-2.1.0/src/matlab/powellsumfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/qingfcn.m` & `benchmarkfcns-2.1.0/src/matlab/qingfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/quarticfcn.m` & `benchmarkfcns-2.1.0/src/matlab/quarticfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/rastriginfcn.m` & `benchmarkfcns-2.1.0/src/matlab/rastriginfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/ridgefcn.m` & `benchmarkfcns-2.1.0/src/matlab/ridgefcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/rosenbrockfcn.m` & `benchmarkfcns-2.1.0/src/matlab/rosenbrockfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/salomonfcn.m` & `benchmarkfcns-2.1.0/src/matlab/salomonfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/schaffern1fcn.m` & `benchmarkfcns-2.1.0/src/matlab/schaffern1fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/schaffern2fcn.m` & `benchmarkfcns-2.1.0/src/matlab/schaffern2fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/schaffern3fcn.m` & `benchmarkfcns-2.1.0/src/matlab/schaffern3fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/schaffern4fcn.m` & `benchmarkfcns-2.1.0/src/matlab/schaffern4fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/schwefel220fcn.m` & `benchmarkfcns-2.1.0/src/matlab/schwefel220fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/schwefel221fcn.m` & `benchmarkfcns-2.1.0/src/matlab/schwefel221fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/schwefel222fcn.m` & `benchmarkfcns-2.1.0/src/matlab/schwefel222fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/schwefel223fcn.m` & `benchmarkfcns-2.1.0/src/matlab/schwefel223fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/schwefelfcn.m` & `benchmarkfcns-2.1.0/src/matlab/schwefelfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/shubert3fcn.m` & `benchmarkfcns-2.1.0/src/matlab/shubert3fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/shubert4fcn.m` & `benchmarkfcns-2.1.0/src/matlab/shubert4fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/shubertfcn.m` & `benchmarkfcns-2.1.0/src/matlab/shubertfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/spherefcn.m` & `benchmarkfcns-2.1.0/src/matlab/spherefcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/styblinskitankfcn.m` & `benchmarkfcns-2.1.0/src/matlab/styblinskitankfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/sumsquaresfcn.m` & `benchmarkfcns-2.1.0/src/matlab/sumsquaresfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/surffcn.m` & `benchmarkfcns-2.1.0/src/matlab/surffcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/threehumpcamelfcn.m` & `benchmarkfcns-2.1.0/src/matlab/threehumpcamelfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/wolfefcn.m` & `benchmarkfcns-2.1.0/src/matlab/wolfefcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/xinsheyangn1fcn.m` & `benchmarkfcns-2.1.0/src/matlab/xinsheyangn1fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/xinsheyangn2fcn.m` & `benchmarkfcns-2.1.0/src/matlab/xinsheyangn2fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/xinsheyangn3fcn.m` & `benchmarkfcns-2.1.0/src/matlab/xinsheyangn3fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/xinsheyangn4fcn.m` & `benchmarkfcns-2.1.0/src/matlab/xinsheyangn4fcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/matlab/zakharovfcn.m` & `benchmarkfcns-2.1.0/src/matlab/zakharovfcn.m`

 * *Files identical despite different names*

### Comparing `benchmarkfcns-2.0.0/src/python/benchmarkfcns/__init__.py` & `benchmarkfcns-2.1.0/src/python/benchmarkfcns/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     deckkersaarts,
     dropwave,
     easom,
     eggcrate,
     eggholder,
     elattar,
     exponential,
+    forrester,
     giunta,
     goldsteinprice,
     gramacylee,
     griewank,
     happycat,
     himmelblau,
     holdertable,
@@ -100,14 +101,15 @@
     "deckkersaarts",
     "dropwave",
     "easom",
     "eggholder",
     "eggcrate",
     "elattar",
     "exponential",
+    "forrester",
     "giunta",
     "goldsteinprice",
     "gramacylee",
     "griewank",
     "happycat",
     "holdertable",
     "himmelblau",
```

### Comparing `benchmarkfcns-2.0.0/src/python/benchmarkfcns/plotting.py` & `benchmarkfcns-2.1.0/src/python/benchmarkfcns/plotting.py`

 * *Files identical despite different names*

