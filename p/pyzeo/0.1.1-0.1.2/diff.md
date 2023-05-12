# Comparing `tmp/pyzeo-0.1.1.tar.gz` & `tmp/pyzeo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzeo-0.1.1.tar", last modified: Tue Mar 14 10:57:56 2023, max compression
+gzip compressed data, was "pyzeo-0.1.2.tar", last modified: Fri May 12 12:02:50 2023, max compression
```

## Comparing `pyzeo-0.1.1.tar` & `pyzeo-0.1.2.tar`

### file list

```diff
@@ -1,483 +1,484 @@
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.595559 pyzeo-0.1.1/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11357 2023-02-24 10:55:17.000000 pyzeo-0.1.1/LICENSE
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      168 2023-03-13 09:16:12.000000 pyzeo-0.1.1/MANIFEST.in
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      784 2023-03-14 10:57:56.595559 pyzeo-0.1.1/PKG-INFO
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1374 2023-03-13 10:03:26.000000 pyzeo-0.1.1/README.md
--rw-rw-r--   0 lauri     (1000) lauri     (1000)       38 2023-03-14 10:57:56.595559 pyzeo-0.1.1/setup.cfg
--rwxrwxr-x   0 lauri     (1000) lauri     (1000)     7501 2023-03-14 10:57:53.000000 pyzeo-0.1.1/setup.py
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.531563 pyzeo-0.1.1/src/
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.535563 pyzeo-0.1.1/src/Eigen/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      304 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/Array
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      607 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      775 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/Cholesky
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1696 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/CholmodSupport
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    12826 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/Core
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      122 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/Dense
--rw-rw-r--   0 lauri     (1000) lauri     (1000)       37 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/Eigen
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3295 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/Eigen2Support
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1394 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/Eigenvalues
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1605 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/Geometry
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      580 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/Householder
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1594 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/IterativeLinearSolvers
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      645 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/Jacobi
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      983 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/LU
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      712 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/LeastSquares
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      697 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/MetisSupport
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2189 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/OrderingMethods
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1467 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/PaStiXSupport
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      864 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/PardisoSupport
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      926 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/QR
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      637 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/QtAlignedMalloc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      956 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/SPQRSupport
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      858 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/SVD
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      594 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/Sparse
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1433 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/SparseCholesky
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1835 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/SparseCore
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1776 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/SparseLU
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      991 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/SparseQR
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      749 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/StdDeque
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      682 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/StdList
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      755 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/StdVector
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1904 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/SuperLUSupport
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1177 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/UmfPackSupport
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.535563 pyzeo-0.1.1/src/Eigen/src/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      308 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/CMakeLists.txt
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.535563 pyzeo-0.1.1/src/Eigen/src/Cholesky/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      153 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/Cholesky/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    21661 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/Cholesky/LDLT.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    16203 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/Cholesky/LLT.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4020 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/Cholesky/LLT_MKL.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.539563 pyzeo-0.1.1/src/Eigen/src/CholmodSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      172 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/CholmodSupport/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    20355 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.547562 pyzeo-0.1.1/src/Eigen/src/Core/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11996 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Array.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8337 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/ArrayBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8385 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/ArrayWrapper.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    23731 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Assign.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11283 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Assign_MKL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13049 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/BandMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    16288 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Block.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3924 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/BooleanRedux.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      215 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5574 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/CommaInitializer.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1941 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/CoreIterators.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9859 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/CwiseBinaryOp.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    29399 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/CwiseNullaryOp.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4736 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/CwiseUnaryOp.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5483 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/CwiseUnaryView.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    22751 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/DenseBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    27635 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/DenseCoeffsBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    16986 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/DenseStorage.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9011 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Diagonal.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11581 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/DiagonalMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5988 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/DiagonalProduct.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9429 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Dot.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4804 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/EigenBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4199 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Flagged.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4460 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/ForceAlignedAccess.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    38870 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Functors.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5588 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Fuzzy.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    28225 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/GeneralProduct.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    12329 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/GenericPacketMath.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3649 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/GlobalFunctions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7497 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/IO.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8154 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Map.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8577 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/MapBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    21952 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/MathFunctions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    17357 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Matrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    24221 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/MatrixBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3211 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/NestByValue.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5355 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/NoAlias.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6360 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/NumTraits.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    25137 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/PermutationMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    35852 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/PlainObjectBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11320 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/ProductBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5417 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Random.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14180 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Redux.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11796 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Ref.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6999 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Replicate.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3511 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/ReturnByValue.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7795 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Reverse.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6097 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Select.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11572 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/SelfAdjointView.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6889 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    10229 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/SolveTriangular.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6761 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/StableNorm.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3620 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Stride.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4398 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Swap.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14944 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Transpose.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15357 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Transpositions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    30357 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/TriangularMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3417 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/VectorBlock.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    26987 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/VectorwiseOp.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7097 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/Visitor.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.547562 pyzeo-0.1.1/src/Eigen/src/Core/arch/
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.547562 pyzeo-0.1.1/src/Eigen/src/Core/arch/AltiVec/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      178 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/arch/AltiVec/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8376 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    18796 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/arch/AltiVec/PacketMath.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)       97 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/arch/CMakeLists.txt
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.547562 pyzeo-0.1.1/src/Eigen/src/Core/arch/Default/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      178 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/arch/Default/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1746 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/arch/Default/Settings.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.547562 pyzeo-0.1.1/src/Eigen/src/Core/arch/NEON/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      169 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/arch/NEON/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8369 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/arch/NEON/Complex.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15539 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/arch/NEON/PacketMath.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.551562 pyzeo-0.1.1/src/Eigen/src/Core/arch/SSE/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      166 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/arch/SSE/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    18154 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/arch/SSE/Complex.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15673 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/arch/SSE/MathFunctions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    26279 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/arch/SSE/PacketMath.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.555562 pyzeo-0.1.1/src/Eigen/src/Core/products/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      166 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    19318 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/CoeffBasedProduct.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    46257 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    16097 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13873 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6537 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_MKL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4652 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/GeneralMatrixMatrix_MKL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    23060 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5647 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/GeneralMatrixVector_MKL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4300 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/Parallelizer.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15772 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    10349 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/SelfadjointMatrixMatrix_MKL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    10749 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5026 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/SelfadjointMatrixVector_MKL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5833 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/SelfadjointProduct.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4014 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    18425 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13015 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/TriangularMatrixMatrix_MKL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15000 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9791 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/TriangularMatrixVector_MKL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13943 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5841 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/TriangularSolverMatrix_MKL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5380 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/products/TriangularSolverVector.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.555562 pyzeo-0.1.1/src/Eigen/src/Core/util/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    10365 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/util/BlasUtil.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      157 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/util/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    17252 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/util/Constants.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2089 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13801 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/util/ForwardDeclarations.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5143 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/util/MKL_support.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    18527 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/util/Macros.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    38278 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/util/Memory.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9817 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/util/Meta.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)       85 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/util/NonMPL2.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      325 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9340 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/util/StaticAssert.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    17273 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Core/util/XprHelper.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.559562 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4287 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Block.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      195 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7473 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Cwise.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    10098 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/CwiseOperators.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.559562 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6191 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/AlignedBox.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2636 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/All.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6991 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/AngleAxis.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      179 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    10565 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/Hyperplane.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5675 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/ParametrizedLine.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    16947 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/Quaternion.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4932 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/Rotation2D.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4565 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/RotationBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5659 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/Scaling.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    28229 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/Transform.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6067 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/Translation.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4466 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/LU.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2134 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Lazy.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6935 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/LeastSquares.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      613 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Macros.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2800 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/MathFunctions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1666 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Memory.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2964 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Meta.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3624 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Minor.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1781 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/QR.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    18471 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/SVD.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1525 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/TriangularSolver.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2664 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigen2Support/VectorBlock.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.563561 pyzeo-0.1.1/src/Eigen/src/Eigenvalues/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      162 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigenvalues/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    12298 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    16829 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4015 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigenvalues/ComplexSchur_MKL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    21840 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigenvalues/EigenSolver.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13975 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9746 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14254 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5679 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    22522 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigenvalues/RealQZ.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    19679 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigenvalues/RealSchur.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3651 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigenvalues/RealSchur_MKL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    30235 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4196 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_MKL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    22417 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.567561 pyzeo-0.1.1/src/Eigen/src/Geometry/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14016 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/AlignedBox.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7621 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/AngleAxis.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      177 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3497 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/EulerAngles.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11663 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/Homogeneous.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11421 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/Hyperplane.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8318 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/OrthoMethods.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7768 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/ParametrizedLine.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    29313 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/Quaternion.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5233 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/Rotation2D.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7699 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/RotationBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6290 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/Scaling.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    56228 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/Transform.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7201 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/Translation.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6738 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/Umeyama.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.567561 pyzeo-0.1.1/src/Eigen/src/Geometry/arch/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      168 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/arch/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3880 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/Geometry/arch/Geometry_SSE.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.567561 pyzeo-0.1.1/src/Eigen/src/Householder/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2747 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/Householder/BlockHouseholder.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      162 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/Householder/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5246 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/Householder/Householder.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    19172 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/Householder/HouseholderSequence.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.567561 pyzeo-0.1.1/src/Eigen/src/IterativeLinearSolvers/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4456 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8151 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      195 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/IterativeLinearSolvers/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8830 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15315 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9122 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.567561 pyzeo-0.1.1/src/Eigen/src/Jacobi/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      147 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/Jacobi/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14312 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/Jacobi/Jacobi.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.567561 pyzeo-0.1.1/src/Eigen/src/LU/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      160 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/LU/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3052 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/LU/Determinant.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    28311 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/LU/FullPivLU.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14450 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/LU/Inverse.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    18201 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/LU/PartialPivLU.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3479 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/LU/PartialPivLU_MKL.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.567561 pyzeo-0.1.1/src/Eigen/src/LU/arch/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      150 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/LU/arch/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13092 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/LU/arch/Inverse_SSE.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.571561 pyzeo-0.1.1/src/Eigen/src/MetisSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      166 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/MetisSupport/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4416 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/MetisSupport/MetisSupport.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.571561 pyzeo-0.1.1/src/Eigen/src/OrderingMethods/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    16004 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/OrderingMethods/Amd.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      174 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/OrderingMethods/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    61585 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4928 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/OrderingMethods/Ordering.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.571561 pyzeo-0.1.1/src/Eigen/src/PaStiXSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      169 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/PaStiXSupport/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    23340 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.571561 pyzeo-0.1.1/src/Eigen/src/PardisoSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      172 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/PardisoSupport/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    20488 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.571561 pyzeo-0.1.1/src/Eigen/src/QR/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      135 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/QR/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    22186 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/QR/ColPivHouseholderQR.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4478 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/QR/ColPivHouseholderQR_MKL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    23492 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/QR/FullPivHouseholderQR.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13460 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/QR/HouseholderQR.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2993 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/QR/HouseholderQR_MKL.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.571561 pyzeo-0.1.1/src/Eigen/src/SPQRSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      163 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/SPQRSupport/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    12083 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.571561 pyzeo-0.1.1/src/Eigen/src/SVD/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      138 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SVD/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    39487 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SVD/JacobiSVD.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4654 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SVD/JacobiSVD_MKL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5782 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SVD/UpperBidiagonalization.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.575561 pyzeo-0.1.1/src/Eigen/src/SparseCholesky/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      171 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseCholesky/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    23410 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6758 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.579560 pyzeo-0.1.1/src/Eigen/src/SparseCore/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    10035 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/AmbiVector.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      160 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6707 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/CompressedStorage.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8739 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6250 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    22878 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseBlock.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6173 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseColEtree.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    12106 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5961 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    10974 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7703 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3164 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseDot.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      984 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseFuzzy.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    45120 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    19117 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6327 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparsePermutation.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6885 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseProduct.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1560 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseRedux.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    18462 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6363 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2493 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseTranspose.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5937 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseTriangularView.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6627 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseUtil.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13642 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseVector.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2799 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseView.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    10091 2017-06-20 10:12:59.000000 pyzeo-0.1.1/src/Eigen/src/SparseCore/TriangularSolver.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.583560 pyzeo-0.1.1/src/Eigen/src/SparseLU/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      153 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    28944 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4268 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLUImpl.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7600 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4993 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9621 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2014 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6631 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6321 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3606 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    10032 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4105 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5710 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8464 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8846 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4919 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4470 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2852 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.583560 pyzeo-0.1.1/src/Eigen/src/SparseQR/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      154 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseQR/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    26449 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SparseQR/SparseQR.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.583560 pyzeo-0.1.1/src/Eigen/src/StlSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      159 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/StlSupport/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5474 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/StlSupport/StdDeque.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4504 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/StlSupport/StdList.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5189 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/StlSupport/StdVector.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2763 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/StlSupport/details.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.583560 pyzeo-0.1.1/src/Eigen/src/SuperLUSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      172 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SuperLUSupport/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    32551 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.583560 pyzeo-0.1.1/src/Eigen/src/UmfPackSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      172 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/UmfPackSupport/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    16269 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.583560 pyzeo-0.1.1/src/Eigen/src/misc/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      141 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/misc/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2997 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/misc/Image.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2817 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/misc/Kernel.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2485 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/misc/Solve.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4697 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/misc/SparseSolve.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    33603 2017-06-20 10:12:58.000000 pyzeo-0.1.1/src/Eigen/src/misc/blas.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.587560 pyzeo-0.1.1/src/Eigen/src/plugins/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9660 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4350 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    34391 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/plugins/BlockMethods.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      150 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/plugins/CMakeLists.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1938 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6603 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6143 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1867 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    17172 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/OMS.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      876 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/OMS.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   122785 2023-01-20 09:36:26.000000 pyzeo-0.1.1/src/area_and_volume.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6648 2023-01-20 13:12:50.000000 pyzeo-0.1.1/src/area_and_volume.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      531 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/arguments.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    65873 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/channel.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9803 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/channel.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    22977 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/cluster.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3713 2017-06-20 10:12:55.000000 pyzeo-0.1.1/src/cluster.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13919 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/cycle.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2768 2017-06-20 10:13:09.000000 pyzeo-0.1.1/src/cycle.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3967 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/feature.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      570 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/general.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    16963 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/geometry.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5417 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/geometry.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4863 2017-06-20 10:13:10.000000 pyzeo-0.1.1/src/gpu_energy.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5698 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/graphstorage.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3814 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/graphstorage.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    21491 2017-06-20 10:13:00.000000 pyzeo-0.1.1/src/grid.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3636 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/grid.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1558 2017-06-20 10:13:00.000000 pyzeo-0.1.1/src/heap.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6778 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/holo_similarity.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1605 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/holograms.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      175 2017-06-20 10:13:00.000000 pyzeo-0.1.1/src/instructions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7196 2023-01-20 13:12:50.000000 pyzeo-0.1.1/src/material.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5696 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/material.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7110 2023-01-20 13:12:50.000000 pyzeo-0.1.1/src/mindist.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3364 2017-06-20 10:13:10.000000 pyzeo-0.1.1/src/mindist.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    32690 2017-06-20 10:13:00.000000 pyzeo-0.1.1/src/net.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5506 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/net.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    43796 2017-06-20 10:13:00.000000 pyzeo-0.1.1/src/network.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4345 2023-01-20 13:12:50.000000 pyzeo-0.1.1/src/network.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    32340 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/networkaccessibility.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11190 2023-01-20 13:12:50.000000 pyzeo-0.1.1/src/networkaccessibility.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    29369 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/networkanalysis.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6393 2017-06-20 10:13:09.000000 pyzeo-0.1.1/src/networkanalysis.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    41783 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/networkinfo.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2236 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/networkinfo.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    67323 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/networkio.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5719 2017-06-20 10:12:55.000000 pyzeo-0.1.1/src/networkio.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   159545 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/networkstorage.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    20848 2017-06-20 10:12:55.000000 pyzeo-0.1.1/src/networkstorage.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1532 2017-06-20 10:13:00.000000 pyzeo-0.1.1/src/poreinfo.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    36101 2023-01-20 13:12:50.000000 pyzeo-0.1.1/src/psd.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1953 2017-06-20 10:13:00.000000 pyzeo-0.1.1/src/psd.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.591560 pyzeo-0.1.1/src/pyzeo/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)        0 2017-06-20 10:12:55.000000 pyzeo-0.1.1/src/pyzeo/__init__.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   210347 2023-03-13 12:49:42.000000 pyzeo-0.1.1/src/pyzeo/area_volume.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   154852 2023-03-13 12:49:43.000000 pyzeo-0.1.1/src/pyzeo/channel.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   271455 2023-03-13 12:49:42.000000 pyzeo-0.1.1/src/pyzeo/cluster.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   160427 2023-03-13 12:49:42.000000 pyzeo-0.1.1/src/pyzeo/cycle.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   221495 2023-03-13 07:28:18.000000 pyzeo-0.1.1/src/pyzeo/geometry.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   173539 2023-03-13 07:28:19.000000 pyzeo-0.1.1/src/pyzeo/graphstorage.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   157241 2023-03-13 12:49:43.000000 pyzeo-0.1.1/src/pyzeo/high_accuracy.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   163148 2023-03-13 12:49:43.000000 pyzeo-0.1.1/src/pyzeo/netinfo.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   260879 2023-03-13 07:28:19.000000 pyzeo-0.1.1/src/pyzeo/netio.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   561739 2023-03-13 12:49:42.000000 pyzeo-0.1.1/src/pyzeo/netstorage.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   165522 2023-03-13 12:49:43.000000 pyzeo-0.1.1/src/pyzeo/psd.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   174709 2023-03-13 12:49:43.000000 pyzeo-0.1.1/src/pyzeo/voronoicell.cpp
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.591560 pyzeo-0.1.1/src/pyzeo.egg-info/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      784 2023-03-14 10:57:56.000000 pyzeo-0.1.1/src/pyzeo.egg-info/PKG-INFO
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14727 2023-03-14 10:57:56.000000 pyzeo-0.1.1/src/pyzeo.egg-info/SOURCES.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)        1 2023-03-14 10:57:56.000000 pyzeo-0.1.1/src/pyzeo.egg-info/dependency_links.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)        1 2023-03-13 09:16:18.000000 pyzeo-0.1.1/src/pyzeo.egg-info/not-zip-safe
--rw-rw-r--   0 lauri     (1000) lauri     (1000)        6 2023-03-14 10:57:56.000000 pyzeo-0.1.1/src/pyzeo.egg-info/top_level.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    47113 2023-01-20 13:12:50.000000 pyzeo-0.1.1/src/ray.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4351 2017-06-20 10:13:09.000000 pyzeo-0.1.1/src/ray.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13873 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/rmsd.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2495 2017-06-20 10:13:10.000000 pyzeo-0.1.1/src/rmsd.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2190 2017-06-20 10:13:10.000000 pyzeo-0.1.1/src/segment.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    23157 2017-06-20 10:13:00.000000 pyzeo-0.1.1/src/sphere_approx.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2338 2017-06-20 10:12:55.000000 pyzeo-0.1.1/src/sphere_approx.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2057 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/string_additions.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      992 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/string_additions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2048 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/symbcalc.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      282 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/symbcalc.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   203257 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/symmetry.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      300 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/symmetry.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    19026 2023-01-20 13:12:50.000000 pyzeo-0.1.1/src/v_network.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3695 2023-01-20 13:12:50.000000 pyzeo-0.1.1/src/v_network.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.519564 pyzeo-0.1.1/src/voro++/
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-03-14 10:57:56.595559 pyzeo-0.1.1/src/voro++/src/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5460 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/c_loops.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15742 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/c_loops.hh
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    79534 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/cell.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    24114 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/cell.hh
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    18651 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/cmd_line.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3849 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/common.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      837 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/common.hh
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4775 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/config.hh
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    22970 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/container.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    28957 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/container.hh
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    29004 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/container_prd.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    26386 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/container_prd.hh
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8213 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/pre_container.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6402 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/pre_container.hh
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6835 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/rad_option.hh
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9161 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/unitcell.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2448 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/unitcell.hh
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4494 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/v_base.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3446 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/v_base.hh
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    40227 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/v_base_wl.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    41664 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/v_compute.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5599 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/v_compute.hh
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      483 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/voro++.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    19831 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/voro++.hh
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5220 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/wall.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4562 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/wall.hh
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      995 2017-06-20 10:14:36.000000 pyzeo-0.1.1/src/voro++/src/worklist.hh
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    17643 2017-06-20 10:12:57.000000 pyzeo-0.1.1/src/voronoicell.cc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6553 2017-06-20 10:13:09.000000 pyzeo-0.1.1/src/voronoicell.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1094 2017-06-20 10:12:56.000000 pyzeo-0.1.1/src/zeo_consts.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    34026 2017-06-20 10:13:00.000000 pyzeo-0.1.1/src/zeojobs.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.283541 pyzeo-0.1.2/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11357 2023-02-24 10:55:17.000000 pyzeo-0.1.2/LICENSE
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      168 2023-03-13 09:16:12.000000 pyzeo-0.1.2/MANIFEST.in
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      784 2023-05-12 12:02:50.283541 pyzeo-0.1.2/PKG-INFO
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1374 2023-03-13 10:03:26.000000 pyzeo-0.1.2/README.md
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       38 2023-05-12 12:02:50.283541 pyzeo-0.1.2/setup.cfg
+-rwxrwxr-x   0 lauri     (1000) lauri     (1000)     3863 2023-05-12 11:56:53.000000 pyzeo-0.1.2/setup.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.219518 pyzeo-0.1.2/src/
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.227520 pyzeo-0.1.2/src/Eigen/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      304 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/Array
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      607 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      775 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/Cholesky
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1696 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/CholmodSupport
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    12826 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/Core
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      122 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/Dense
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       37 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/Eigen
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3295 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/Eigen2Support
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1394 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/Eigenvalues
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1605 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/Geometry
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      580 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/Householder
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1594 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/IterativeLinearSolvers
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      645 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/Jacobi
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      983 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/LU
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      712 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/LeastSquares
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      697 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/MetisSupport
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2189 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/OrderingMethods
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1467 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/PaStiXSupport
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      864 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/PardisoSupport
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      926 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/QR
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      637 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/QtAlignedMalloc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      956 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/SPQRSupport
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      858 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/SVD
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      594 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/Sparse
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1433 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/SparseCholesky
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1835 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/SparseCore
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1776 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/SparseLU
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      991 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/SparseQR
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      749 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/StdDeque
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      682 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/StdList
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      755 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/StdVector
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1904 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/SuperLUSupport
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1177 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/UmfPackSupport
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.227520 pyzeo-0.1.2/src/Eigen/src/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      308 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/CMakeLists.txt
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.227520 pyzeo-0.1.2/src/Eigen/src/Cholesky/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      153 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/Cholesky/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    21661 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/Cholesky/LDLT.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    16203 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/Cholesky/LLT.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4020 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/Cholesky/LLT_MKL.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.227520 pyzeo-0.1.2/src/Eigen/src/CholmodSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      172 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/CholmodSupport/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    20355 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.239525 pyzeo-0.1.2/src/Eigen/src/Core/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11996 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Array.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8337 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/ArrayBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8385 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/ArrayWrapper.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    23731 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Assign.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11283 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Assign_MKL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13049 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/BandMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    16288 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Block.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3924 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/BooleanRedux.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      215 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5574 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/CommaInitializer.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1941 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/CoreIterators.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9859 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/CwiseBinaryOp.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    29399 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/CwiseNullaryOp.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4736 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/CwiseUnaryOp.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5483 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/CwiseUnaryView.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    22751 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/DenseBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    27635 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/DenseCoeffsBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    16986 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/DenseStorage.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9011 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Diagonal.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11581 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/DiagonalMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5988 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/DiagonalProduct.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9429 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Dot.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4804 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/EigenBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4199 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Flagged.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4460 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/ForceAlignedAccess.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    38870 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Functors.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5588 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Fuzzy.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    28225 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/GeneralProduct.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    12329 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/GenericPacketMath.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3649 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/GlobalFunctions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7497 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/IO.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8154 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Map.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8577 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/MapBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    21952 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/MathFunctions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    17357 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Matrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    24221 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/MatrixBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3211 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/NestByValue.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5355 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/NoAlias.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6360 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/NumTraits.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    25137 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/PermutationMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    35852 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/PlainObjectBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11320 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/ProductBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5417 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Random.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14180 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Redux.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11796 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Ref.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6999 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Replicate.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3511 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/ReturnByValue.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7795 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Reverse.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6097 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Select.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11572 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/SelfAdjointView.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6889 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    10229 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/SolveTriangular.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6761 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/StableNorm.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3620 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Stride.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4398 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Swap.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14944 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Transpose.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15357 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Transpositions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    30357 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/TriangularMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3417 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/VectorBlock.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    26987 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/VectorwiseOp.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7097 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/Visitor.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.239525 pyzeo-0.1.2/src/Eigen/src/Core/arch/
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.239525 pyzeo-0.1.2/src/Eigen/src/Core/arch/AltiVec/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      178 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/arch/AltiVec/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8376 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    18796 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/arch/AltiVec/PacketMath.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       97 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/arch/CMakeLists.txt
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.239525 pyzeo-0.1.2/src/Eigen/src/Core/arch/Default/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      178 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/arch/Default/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1746 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/arch/Default/Settings.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.239525 pyzeo-0.1.2/src/Eigen/src/Core/arch/NEON/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      169 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/arch/NEON/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8369 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/arch/NEON/Complex.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15539 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/arch/NEON/PacketMath.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.239525 pyzeo-0.1.2/src/Eigen/src/Core/arch/SSE/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      166 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/arch/SSE/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    18154 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/arch/SSE/Complex.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15673 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    26279 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/arch/SSE/PacketMath.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.243526 pyzeo-0.1.2/src/Eigen/src/Core/products/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      166 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    19318 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/CoeffBasedProduct.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    46257 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    16097 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13873 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6537 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_MKL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4652 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/GeneralMatrixMatrix_MKL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    23060 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5647 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/GeneralMatrixVector_MKL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4300 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/Parallelizer.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15772 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    10349 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/SelfadjointMatrixMatrix_MKL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    10749 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5026 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/SelfadjointMatrixVector_MKL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5833 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4014 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    18425 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13015 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/TriangularMatrixMatrix_MKL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15000 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9791 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/TriangularMatrixVector_MKL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13943 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5841 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/TriangularSolverMatrix_MKL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5380 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/products/TriangularSolverVector.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.247528 pyzeo-0.1.2/src/Eigen/src/Core/util/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    10365 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/util/BlasUtil.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      157 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/util/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    17252 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/util/Constants.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2089 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13801 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5143 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/util/MKL_support.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    18527 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/util/Macros.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    38278 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/util/Memory.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9817 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/util/Meta.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       85 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/util/NonMPL2.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      325 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9340 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/util/StaticAssert.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    17273 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Core/util/XprHelper.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.247528 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4287 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Block.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      195 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7473 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Cwise.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    10098 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/CwiseOperators.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.251529 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6191 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/AlignedBox.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2636 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/All.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6991 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/AngleAxis.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      179 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    10565 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/Hyperplane.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5675 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/ParametrizedLine.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    16947 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/Quaternion.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4932 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/Rotation2D.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4565 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/RotationBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5659 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/Scaling.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    28229 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/Transform.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6067 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/Translation.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4466 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/LU.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2134 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Lazy.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6935 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/LeastSquares.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      613 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Macros.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2800 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/MathFunctions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1666 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Memory.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2964 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Meta.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3624 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Minor.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1781 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/QR.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    18471 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/SVD.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1525 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/TriangularSolver.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2664 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigen2Support/VectorBlock.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.255530 pyzeo-0.1.2/src/Eigen/src/Eigenvalues/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      162 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigenvalues/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    12298 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    16829 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4015 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigenvalues/ComplexSchur_MKL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    21840 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13975 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9746 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14254 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5679 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    22522 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigenvalues/RealQZ.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    19679 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigenvalues/RealSchur.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3651 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigenvalues/RealSchur_MKL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    30235 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4196 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_MKL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    22417 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.255530 pyzeo-0.1.2/src/Eigen/src/Geometry/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14016 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/AlignedBox.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7621 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/AngleAxis.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      177 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3497 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/EulerAngles.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11663 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/Homogeneous.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11421 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/Hyperplane.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8318 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/OrthoMethods.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7768 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/ParametrizedLine.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    29313 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/Quaternion.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5233 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/Rotation2D.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7699 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/RotationBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6290 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/Scaling.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    56228 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/Transform.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7201 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/Translation.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6738 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/Umeyama.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.255530 pyzeo-0.1.2/src/Eigen/src/Geometry/arch/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      168 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/arch/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3880 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/Geometry/arch/Geometry_SSE.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.255530 pyzeo-0.1.2/src/Eigen/src/Householder/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2747 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/Householder/BlockHouseholder.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      162 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/Householder/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5246 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/Householder/Householder.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    19172 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/Householder/HouseholderSequence.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.259532 pyzeo-0.1.2/src/Eigen/src/IterativeLinearSolvers/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4456 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8151 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      195 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/IterativeLinearSolvers/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8830 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15315 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9122 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.259532 pyzeo-0.1.2/src/Eigen/src/Jacobi/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      147 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/Jacobi/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14312 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/Jacobi/Jacobi.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.259532 pyzeo-0.1.2/src/Eigen/src/LU/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      160 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/LU/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3052 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/LU/Determinant.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    28311 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/LU/FullPivLU.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14450 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/LU/Inverse.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    18201 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/LU/PartialPivLU.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3479 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/LU/PartialPivLU_MKL.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.259532 pyzeo-0.1.2/src/Eigen/src/LU/arch/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      150 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/LU/arch/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13092 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/LU/arch/Inverse_SSE.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.259532 pyzeo-0.1.2/src/Eigen/src/MetisSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      166 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/MetisSupport/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4416 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/MetisSupport/MetisSupport.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.259532 pyzeo-0.1.2/src/Eigen/src/OrderingMethods/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    16004 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/OrderingMethods/Amd.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      174 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/OrderingMethods/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    61585 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4928 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/OrderingMethods/Ordering.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.259532 pyzeo-0.1.2/src/Eigen/src/PaStiXSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      169 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/PaStiXSupport/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    23340 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.263533 pyzeo-0.1.2/src/Eigen/src/PardisoSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      172 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/PardisoSupport/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    20488 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.263533 pyzeo-0.1.2/src/Eigen/src/QR/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      135 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/QR/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    22186 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4478 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/QR/ColPivHouseholderQR_MKL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    23492 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13460 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/QR/HouseholderQR.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2993 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/QR/HouseholderQR_MKL.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.263533 pyzeo-0.1.2/src/Eigen/src/SPQRSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      163 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/SPQRSupport/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    12083 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.263533 pyzeo-0.1.2/src/Eigen/src/SVD/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      138 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SVD/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    39487 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SVD/JacobiSVD.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4654 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SVD/JacobiSVD_MKL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5782 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SVD/UpperBidiagonalization.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.263533 pyzeo-0.1.2/src/Eigen/src/SparseCholesky/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      171 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseCholesky/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    23410 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6758 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.267535 pyzeo-0.1.2/src/Eigen/src/SparseCore/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    10035 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/AmbiVector.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      160 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6707 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/CompressedStorage.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8739 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6250 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    22878 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseBlock.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6173 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseColEtree.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    12106 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5961 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    10974 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7703 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3164 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseDot.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      984 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    45120 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    19117 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6327 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparsePermutation.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6885 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseProduct.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1560 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseRedux.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    18462 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6363 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2493 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseTranspose.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5937 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6627 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseUtil.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13642 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseVector.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2799 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseView.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    10091 2017-06-20 10:12:59.000000 pyzeo-0.1.2/src/Eigen/src/SparseCore/TriangularSolver.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.271536 pyzeo-0.1.2/src/Eigen/src/SparseLU/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      153 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    28944 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4268 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7600 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4993 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9621 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2014 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6631 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6321 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3606 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    10032 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4105 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5710 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8464 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8846 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4919 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4470 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2852 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.271536 pyzeo-0.1.2/src/Eigen/src/SparseQR/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      154 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseQR/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    26449 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SparseQR/SparseQR.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.271536 pyzeo-0.1.2/src/Eigen/src/StlSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      159 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/StlSupport/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5474 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/StlSupport/StdDeque.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4504 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/StlSupport/StdList.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5189 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/StlSupport/StdVector.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2763 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/StlSupport/details.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.271536 pyzeo-0.1.2/src/Eigen/src/SuperLUSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      172 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SuperLUSupport/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    32551 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.271536 pyzeo-0.1.2/src/Eigen/src/UmfPackSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      172 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/UmfPackSupport/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    16269 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.275538 pyzeo-0.1.2/src/Eigen/src/misc/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      141 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/misc/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2997 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/misc/Image.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2817 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/misc/Kernel.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2485 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/misc/Solve.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4697 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/misc/SparseSolve.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    33603 2017-06-20 10:12:58.000000 pyzeo-0.1.2/src/Eigen/src/misc/blas.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.275538 pyzeo-0.1.2/src/Eigen/src/plugins/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9660 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4350 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    34391 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/plugins/BlockMethods.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      150 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/plugins/CMakeLists.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1938 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6603 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6143 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1867 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    17172 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/OMS.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      876 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/OMS.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)   122785 2023-01-20 09:36:26.000000 pyzeo-0.1.2/src/area_and_volume.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6648 2023-01-20 13:12:50.000000 pyzeo-0.1.2/src/area_and_volume.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      531 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/arguments.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    65873 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/channel.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9803 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/channel.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    22977 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/cluster.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3713 2017-06-20 10:12:55.000000 pyzeo-0.1.2/src/cluster.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13919 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/cycle.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2768 2017-06-20 10:13:09.000000 pyzeo-0.1.2/src/cycle.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3967 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/feature.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      570 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/general.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    16963 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/geometry.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5417 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/geometry.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4863 2017-06-20 10:13:10.000000 pyzeo-0.1.2/src/gpu_energy.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5698 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/graphstorage.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3814 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/graphstorage.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    21491 2017-06-20 10:13:00.000000 pyzeo-0.1.2/src/grid.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3636 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/grid.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1558 2017-06-20 10:13:00.000000 pyzeo-0.1.2/src/heap.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6778 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/holo_similarity.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1605 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/holograms.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      175 2017-06-20 10:13:00.000000 pyzeo-0.1.2/src/instructions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7196 2023-01-20 13:12:50.000000 pyzeo-0.1.2/src/material.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5696 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/material.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7110 2023-01-20 13:12:50.000000 pyzeo-0.1.2/src/mindist.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3364 2017-06-20 10:13:10.000000 pyzeo-0.1.2/src/mindist.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    32690 2017-06-20 10:13:00.000000 pyzeo-0.1.2/src/net.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5506 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/net.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    43796 2017-06-20 10:13:00.000000 pyzeo-0.1.2/src/network.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4345 2023-01-20 13:12:50.000000 pyzeo-0.1.2/src/network.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    32340 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/networkaccessibility.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11190 2023-01-20 13:12:50.000000 pyzeo-0.1.2/src/networkaccessibility.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    29369 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/networkanalysis.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6393 2017-06-20 10:13:09.000000 pyzeo-0.1.2/src/networkanalysis.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    41783 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/networkinfo.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2236 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/networkinfo.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    67323 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/networkio.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5719 2017-06-20 10:12:55.000000 pyzeo-0.1.2/src/networkio.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)   159545 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/networkstorage.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    20848 2017-06-20 10:12:55.000000 pyzeo-0.1.2/src/networkstorage.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1532 2017-06-20 10:13:00.000000 pyzeo-0.1.2/src/poreinfo.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    36101 2023-01-20 13:12:50.000000 pyzeo-0.1.2/src/psd.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1953 2017-06-20 10:13:00.000000 pyzeo-0.1.2/src/psd.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.275538 pyzeo-0.1.2/src/pyzeo/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      287 2023-05-12 11:47:06.000000 pyzeo-0.1.2/src/pyzeo/__init__.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.279539 pyzeo-0.1.2/src/pyzeo/area_volume/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       49 2023-05-12 11:53:28.000000 pyzeo-0.1.2/src/pyzeo/area_volume/__init__.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.279539 pyzeo-0.1.2/src/pyzeo/cluster/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      128 2023-05-12 11:51:02.000000 pyzeo-0.1.2/src/pyzeo/cluster/__init__.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.279539 pyzeo-0.1.2/src/pyzeo/cycle/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       87 2023-05-12 11:51:44.000000 pyzeo-0.1.2/src/pyzeo/cycle/__init__.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)  1127784 2023-05-12 11:43:39.000000 pyzeo-0.1.2/src/pyzeo/extension.cpp
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.279539 pyzeo-0.1.2/src/pyzeo/high_accuracy/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       50 2023-05-12 11:54:28.000000 pyzeo-0.1.2/src/pyzeo/high_accuracy/__init__.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.279539 pyzeo-0.1.2/src/pyzeo/netstorage/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       40 2023-05-12 11:50:11.000000 pyzeo-0.1.2/src/pyzeo/netstorage/__init__.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.279539 pyzeo-0.1.2/src/pyzeo/psd/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       56 2023-05-12 11:52:49.000000 pyzeo-0.1.2/src/pyzeo/psd/__init__.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.279539 pyzeo-0.1.2/src/pyzeo.egg-info/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      784 2023-05-12 12:02:50.000000 pyzeo-0.1.2/src/pyzeo.egg-info/PKG-INFO
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14659 2023-05-12 12:02:50.000000 pyzeo-0.1.2/src/pyzeo.egg-info/SOURCES.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)        1 2023-05-12 12:02:50.000000 pyzeo-0.1.2/src/pyzeo.egg-info/dependency_links.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)        1 2023-05-12 11:58:08.000000 pyzeo-0.1.2/src/pyzeo.egg-info/not-zip-safe
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)        6 2023-05-12 12:02:50.000000 pyzeo-0.1.2/src/pyzeo.egg-info/top_level.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    47113 2023-01-20 13:12:50.000000 pyzeo-0.1.2/src/ray.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4351 2017-06-20 10:13:09.000000 pyzeo-0.1.2/src/ray.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13873 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/rmsd.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2495 2017-06-20 10:13:10.000000 pyzeo-0.1.2/src/rmsd.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2190 2017-06-20 10:13:10.000000 pyzeo-0.1.2/src/segment.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    23157 2017-06-20 10:13:00.000000 pyzeo-0.1.2/src/sphere_approx.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2338 2017-06-20 10:12:55.000000 pyzeo-0.1.2/src/sphere_approx.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2057 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/string_additions.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      992 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/string_additions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2048 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/symbcalc.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      282 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/symbcalc.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)   203257 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/symmetry.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      300 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/symmetry.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    19026 2023-01-20 13:12:50.000000 pyzeo-0.1.2/src/v_network.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3695 2023-01-20 13:12:50.000000 pyzeo-0.1.2/src/v_network.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.207513 pyzeo-0.1.2/src/voro++/
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-12 12:02:50.283541 pyzeo-0.1.2/src/voro++/src/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5460 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/c_loops.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15742 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/c_loops.hh
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    79534 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/cell.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    24114 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/cell.hh
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    18651 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/cmd_line.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3849 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/common.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      837 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/common.hh
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4775 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/config.hh
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    22970 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/container.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    28957 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/container.hh
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    29004 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/container_prd.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    26386 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/container_prd.hh
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8213 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/pre_container.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6402 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/pre_container.hh
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6835 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/rad_option.hh
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9161 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/unitcell.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2448 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/unitcell.hh
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4494 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/v_base.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3446 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/v_base.hh
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    40227 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/v_base_wl.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    41664 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/v_compute.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5599 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/v_compute.hh
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      483 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/voro++.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    19831 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/voro++.hh
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5220 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/wall.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4562 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/wall.hh
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      995 2017-06-20 10:14:36.000000 pyzeo-0.1.2/src/voro++/src/worklist.hh
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    17643 2017-06-20 10:12:57.000000 pyzeo-0.1.2/src/voronoicell.cc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6553 2017-06-20 10:13:09.000000 pyzeo-0.1.2/src/voronoicell.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1094 2017-06-20 10:12:56.000000 pyzeo-0.1.2/src/zeo_consts.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    34026 2017-06-20 10:13:00.000000 pyzeo-0.1.2/src/zeojobs.h
```

### Comparing `pyzeo-0.1.1/LICENSE` & `pyzeo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/PKG-INFO` & `pyzeo-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzeo
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python interface to Zeo++
 Home-page: https://github.com/nomad-coe/pyzeo
 Author: Lauri Himanen
 Keywords: zeo++ porous materials science
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Cython
```

### Comparing `pyzeo-0.1.1/README.md` & `pyzeo-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/CMakeLists.txt` & `pyzeo-0.1.2/src/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/Cholesky` & `pyzeo-0.1.2/src/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/CholmodSupport` & `pyzeo-0.1.2/src/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/Core` & `pyzeo-0.1.2/src/Eigen/Core`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/Eigen2Support` & `pyzeo-0.1.2/src/Eigen/Eigen2Support`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/Eigenvalues` & `pyzeo-0.1.2/src/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/Geometry` & `pyzeo-0.1.2/src/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/Householder` & `pyzeo-0.1.2/src/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/IterativeLinearSolvers` & `pyzeo-0.1.2/src/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/Jacobi` & `pyzeo-0.1.2/src/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/LU` & `pyzeo-0.1.2/src/Eigen/LU`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/LeastSquares` & `pyzeo-0.1.2/src/Eigen/LeastSquares`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/MetisSupport` & `pyzeo-0.1.2/src/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/OrderingMethods` & `pyzeo-0.1.2/src/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/PaStiXSupport` & `pyzeo-0.1.2/src/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/PardisoSupport` & `pyzeo-0.1.2/src/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/QR` & `pyzeo-0.1.2/src/Eigen/QR`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/QtAlignedMalloc` & `pyzeo-0.1.2/src/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/SPQRSupport` & `pyzeo-0.1.2/src/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/SVD` & `pyzeo-0.1.2/src/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/Sparse` & `pyzeo-0.1.2/src/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/SparseCholesky` & `pyzeo-0.1.2/src/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/SparseCore` & `pyzeo-0.1.2/src/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/SparseLU` & `pyzeo-0.1.2/src/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/SparseQR` & `pyzeo-0.1.2/src/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/StdDeque` & `pyzeo-0.1.2/src/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/StdList` & `pyzeo-0.1.2/src/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/StdVector` & `pyzeo-0.1.2/src/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/SuperLUSupport` & `pyzeo-0.1.2/src/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/UmfPackSupport` & `pyzeo-0.1.2/src/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Cholesky/LDLT.h` & `pyzeo-0.1.2/src/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Cholesky/LLT.h` & `pyzeo-0.1.2/src/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Cholesky/LLT_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/Cholesky/LLT_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/CholmodSupport/CholmodSupport.h` & `pyzeo-0.1.2/src/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Array.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/ArrayBase.h` & `pyzeo-0.1.2/src/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/ArrayWrapper.h` & `pyzeo-0.1.2/src/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Assign.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Assign_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/BandMatrix.h` & `pyzeo-0.1.2/src/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Block.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/BooleanRedux.h` & `pyzeo-0.1.2/src/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/CommaInitializer.h` & `pyzeo-0.1.2/src/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/CoreIterators.h` & `pyzeo-0.1.2/src/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/CwiseBinaryOp.h` & `pyzeo-0.1.2/src/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/CwiseNullaryOp.h` & `pyzeo-0.1.2/src/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/CwiseUnaryOp.h` & `pyzeo-0.1.2/src/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/CwiseUnaryView.h` & `pyzeo-0.1.2/src/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/DenseBase.h` & `pyzeo-0.1.2/src/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/DenseCoeffsBase.h` & `pyzeo-0.1.2/src/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/DenseStorage.h` & `pyzeo-0.1.2/src/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Diagonal.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/DiagonalMatrix.h` & `pyzeo-0.1.2/src/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/DiagonalProduct.h` & `pyzeo-0.1.2/src/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Dot.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/EigenBase.h` & `pyzeo-0.1.2/src/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Flagged.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Flagged.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/ForceAlignedAccess.h` & `pyzeo-0.1.2/src/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Functors.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Functors.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Fuzzy.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/GeneralProduct.h` & `pyzeo-0.1.2/src/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/GenericPacketMath.h` & `pyzeo-0.1.2/src/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/GlobalFunctions.h` & `pyzeo-0.1.2/src/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/IO.h` & `pyzeo-0.1.2/src/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Map.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/MapBase.h` & `pyzeo-0.1.2/src/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/MathFunctions.h` & `pyzeo-0.1.2/src/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Matrix.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/MatrixBase.h` & `pyzeo-0.1.2/src/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/NestByValue.h` & `pyzeo-0.1.2/src/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/NoAlias.h` & `pyzeo-0.1.2/src/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/NumTraits.h` & `pyzeo-0.1.2/src/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/PermutationMatrix.h` & `pyzeo-0.1.2/src/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/PlainObjectBase.h` & `pyzeo-0.1.2/src/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/ProductBase.h` & `pyzeo-0.1.2/src/Eigen/src/Core/ProductBase.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Random.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Redux.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Ref.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Replicate.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/ReturnByValue.h` & `pyzeo-0.1.2/src/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Reverse.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Select.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/SelfAdjointView.h` & `pyzeo-0.1.2/src/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/SelfCwiseBinaryOp.h` & `pyzeo-0.1.2/src/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/SolveTriangular.h` & `pyzeo-0.1.2/src/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/StableNorm.h` & `pyzeo-0.1.2/src/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Stride.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Swap.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Transpose.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Transpositions.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/TriangularMatrix.h` & `pyzeo-0.1.2/src/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/VectorBlock.h` & `pyzeo-0.1.2/src/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/VectorwiseOp.h` & `pyzeo-0.1.2/src/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/Visitor.h` & `pyzeo-0.1.2/src/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/arch/AltiVec/Complex.h` & `pyzeo-0.1.2/src/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `pyzeo-0.1.2/src/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/arch/Default/Settings.h` & `pyzeo-0.1.2/src/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/arch/NEON/Complex.h` & `pyzeo-0.1.2/src/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/arch/NEON/PacketMath.h` & `pyzeo-0.1.2/src/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/arch/SSE/Complex.h` & `pyzeo-0.1.2/src/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/arch/SSE/MathFunctions.h` & `pyzeo-0.1.2/src/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/arch/SSE/PacketMath.h` & `pyzeo-0.1.2/src/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/CoeffBasedProduct.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/CoeffBasedProduct.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/GeneralMatrixMatrix_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/GeneralMatrixMatrix_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/GeneralMatrixVector.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/GeneralMatrixVector_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/GeneralMatrixVector_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/Parallelizer.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/SelfadjointMatrixMatrix_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/SelfadjointMatrixMatrix_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/SelfadjointMatrixVector_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/SelfadjointMatrixVector_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/SelfadjointProduct.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/SelfadjointRank2Update.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/TriangularMatrixMatrix_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/TriangularMatrixMatrix_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/TriangularMatrixVector.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/TriangularMatrixVector_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/TriangularMatrixVector_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/TriangularSolverMatrix.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/TriangularSolverMatrix_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/TriangularSolverMatrix_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/products/TriangularSolverVector.h` & `pyzeo-0.1.2/src/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/util/BlasUtil.h` & `pyzeo-0.1.2/src/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/util/Constants.h` & `pyzeo-0.1.2/src/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/util/DisableStupidWarnings.h` & `pyzeo-0.1.2/src/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/util/ForwardDeclarations.h` & `pyzeo-0.1.2/src/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/util/MKL_support.h` & `pyzeo-0.1.2/src/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/util/Macros.h` & `pyzeo-0.1.2/src/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/util/Memory.h` & `pyzeo-0.1.2/src/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/util/Meta.h` & `pyzeo-0.1.2/src/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/util/StaticAssert.h` & `pyzeo-0.1.2/src/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Core/util/XprHelper.h` & `pyzeo-0.1.2/src/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Block.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Block.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Cwise.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Cwise.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/CwiseOperators.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/CwiseOperators.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/AlignedBox.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/All.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/All.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/AngleAxis.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/Hyperplane.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/ParametrizedLine.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/Quaternion.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/Rotation2D.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/RotationBase.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/Scaling.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/Transform.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Geometry/Translation.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/LU.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/LU.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Lazy.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Lazy.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/LeastSquares.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/LeastSquares.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Macros.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Macros.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/MathFunctions.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Memory.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Memory.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Meta.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Meta.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/Minor.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/Minor.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/QR.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/QR.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/SVD.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/SVD.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/TriangularSolver.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigen2Support/VectorBlock.h` & `pyzeo-0.1.2/src/Eigen/src/Eigen2Support/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `pyzeo-0.1.2/src/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigenvalues/ComplexSchur.h` & `pyzeo-0.1.2/src/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigenvalues/ComplexSchur_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/Eigenvalues/ComplexSchur_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigenvalues/EigenSolver.h` & `pyzeo-0.1.2/src/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `pyzeo-0.1.2/src/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `pyzeo-0.1.2/src/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `pyzeo-0.1.2/src/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `pyzeo-0.1.2/src/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigenvalues/RealQZ.h` & `pyzeo-0.1.2/src/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigenvalues/RealSchur.h` & `pyzeo-0.1.2/src/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigenvalues/RealSchur_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/Eigenvalues/RealSchur_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `pyzeo-0.1.2/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Eigenvalues/Tridiagonalization.h` & `pyzeo-0.1.2/src/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Geometry/AlignedBox.h` & `pyzeo-0.1.2/src/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Geometry/AngleAxis.h` & `pyzeo-0.1.2/src/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Geometry/EulerAngles.h` & `pyzeo-0.1.2/src/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Geometry/Homogeneous.h` & `pyzeo-0.1.2/src/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Geometry/Hyperplane.h` & `pyzeo-0.1.2/src/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Geometry/OrthoMethods.h` & `pyzeo-0.1.2/src/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Geometry/ParametrizedLine.h` & `pyzeo-0.1.2/src/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Geometry/Quaternion.h` & `pyzeo-0.1.2/src/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Geometry/Rotation2D.h` & `pyzeo-0.1.2/src/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Geometry/RotationBase.h` & `pyzeo-0.1.2/src/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Geometry/Scaling.h` & `pyzeo-0.1.2/src/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Geometry/Transform.h` & `pyzeo-0.1.2/src/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Geometry/Translation.h` & `pyzeo-0.1.2/src/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Geometry/Umeyama.h` & `pyzeo-0.1.2/src/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Geometry/arch/Geometry_SSE.h` & `pyzeo-0.1.2/src/Eigen/src/Geometry/arch/Geometry_SSE.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Householder/BlockHouseholder.h` & `pyzeo-0.1.2/src/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Householder/Householder.h` & `pyzeo-0.1.2/src/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Householder/HouseholderSequence.h` & `pyzeo-0.1.2/src/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `pyzeo-0.1.2/src/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `pyzeo-0.1.2/src/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `pyzeo-0.1.2/src/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `pyzeo-0.1.2/src/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `pyzeo-0.1.2/src/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/Jacobi/Jacobi.h` & `pyzeo-0.1.2/src/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/LU/Determinant.h` & `pyzeo-0.1.2/src/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/LU/FullPivLU.h` & `pyzeo-0.1.2/src/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/LU/Inverse.h` & `pyzeo-0.1.2/src/Eigen/src/LU/Inverse.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/LU/PartialPivLU.h` & `pyzeo-0.1.2/src/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/LU/PartialPivLU_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/LU/PartialPivLU_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/LU/arch/Inverse_SSE.h` & `pyzeo-0.1.2/src/Eigen/src/LU/arch/Inverse_SSE.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/MetisSupport/MetisSupport.h` & `pyzeo-0.1.2/src/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/OrderingMethods/Amd.h` & `pyzeo-0.1.2/src/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `pyzeo-0.1.2/src/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/OrderingMethods/Ordering.h` & `pyzeo-0.1.2/src/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `pyzeo-0.1.2/src/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/PardisoSupport/PardisoSupport.h` & `pyzeo-0.1.2/src/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/QR/ColPivHouseholderQR.h` & `pyzeo-0.1.2/src/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/QR/ColPivHouseholderQR_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/QR/ColPivHouseholderQR_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/QR/FullPivHouseholderQR.h` & `pyzeo-0.1.2/src/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/QR/HouseholderQR.h` & `pyzeo-0.1.2/src/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/QR/HouseholderQR_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/QR/HouseholderQR_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `pyzeo-0.1.2/src/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SVD/JacobiSVD.h` & `pyzeo-0.1.2/src/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SVD/JacobiSVD_MKL.h` & `pyzeo-0.1.2/src/Eigen/src/SVD/JacobiSVD_MKL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SVD/UpperBidiagonalization.h` & `pyzeo-0.1.2/src/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/AmbiVector.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/CompressedStorage.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/MappedSparseMatrix.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseBlock.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseColEtree.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseDenseProduct.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseDot.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseFuzzy.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseMatrix.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseMatrixBase.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparsePermutation.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseProduct.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseRedux.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseTranspose.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseTriangularView.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseUtil.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseVector.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/SparseView.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseCore/TriangularSolver.h` & `pyzeo-0.1.2/src/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLUImpl.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_Memory.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_Structs.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_Utils.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_pivotL.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_pruneL.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `pyzeo-0.1.2/src/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SparseQR/SparseQR.h` & `pyzeo-0.1.2/src/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/StlSupport/StdDeque.h` & `pyzeo-0.1.2/src/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/StlSupport/StdList.h` & `pyzeo-0.1.2/src/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/StlSupport/StdVector.h` & `pyzeo-0.1.2/src/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/StlSupport/details.h` & `pyzeo-0.1.2/src/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `pyzeo-0.1.2/src/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `pyzeo-0.1.2/src/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/misc/Image.h` & `pyzeo-0.1.2/src/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/misc/Kernel.h` & `pyzeo-0.1.2/src/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/misc/Solve.h` & `pyzeo-0.1.2/src/Eigen/src/misc/Solve.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/misc/SparseSolve.h` & `pyzeo-0.1.2/src/Eigen/src/misc/SparseSolve.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/misc/blas.h` & `pyzeo-0.1.2/src/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `pyzeo-0.1.2/src/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `pyzeo-0.1.2/src/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/plugins/BlockMethods.h` & `pyzeo-0.1.2/src/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `pyzeo-0.1.2/src/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `pyzeo-0.1.2/src/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `pyzeo-0.1.2/src/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `pyzeo-0.1.2/src/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/OMS.cc` & `pyzeo-0.1.2/src/OMS.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/OMS.h` & `pyzeo-0.1.2/src/OMS.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/area_and_volume.cc` & `pyzeo-0.1.2/src/area_and_volume.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/area_and_volume.h` & `pyzeo-0.1.2/src/area_and_volume.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/arguments.h` & `pyzeo-0.1.2/src/arguments.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/channel.cc` & `pyzeo-0.1.2/src/channel.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/channel.h` & `pyzeo-0.1.2/src/channel.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/cluster.cc` & `pyzeo-0.1.2/src/cluster.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/cluster.h` & `pyzeo-0.1.2/src/cluster.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/cycle.cc` & `pyzeo-0.1.2/src/cycle.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/cycle.h` & `pyzeo-0.1.2/src/cycle.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/feature.h` & `pyzeo-0.1.2/src/feature.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/general.h` & `pyzeo-0.1.2/src/general.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/geometry.cc` & `pyzeo-0.1.2/src/geometry.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/geometry.h` & `pyzeo-0.1.2/src/geometry.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/gpu_energy.h` & `pyzeo-0.1.2/src/gpu_energy.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/graphstorage.cc` & `pyzeo-0.1.2/src/graphstorage.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/graphstorage.h` & `pyzeo-0.1.2/src/graphstorage.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/grid.cc` & `pyzeo-0.1.2/src/grid.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/grid.h` & `pyzeo-0.1.2/src/grid.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/heap.h` & `pyzeo-0.1.2/src/heap.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/holo_similarity.h` & `pyzeo-0.1.2/src/holo_similarity.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/holograms.h` & `pyzeo-0.1.2/src/holograms.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/material.cc` & `pyzeo-0.1.2/src/material.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/material.h` & `pyzeo-0.1.2/src/material.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/mindist.cc` & `pyzeo-0.1.2/src/mindist.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/mindist.h` & `pyzeo-0.1.2/src/mindist.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/net.cc` & `pyzeo-0.1.2/src/net.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/net.h` & `pyzeo-0.1.2/src/net.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/network.cc` & `pyzeo-0.1.2/src/network.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/network.h` & `pyzeo-0.1.2/src/network.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/networkaccessibility.cc` & `pyzeo-0.1.2/src/networkaccessibility.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/networkaccessibility.h` & `pyzeo-0.1.2/src/networkaccessibility.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/networkanalysis.cc` & `pyzeo-0.1.2/src/networkanalysis.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/networkanalysis.h` & `pyzeo-0.1.2/src/networkanalysis.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/networkinfo.cc` & `pyzeo-0.1.2/src/networkinfo.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/networkinfo.h` & `pyzeo-0.1.2/src/networkinfo.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/networkio.cc` & `pyzeo-0.1.2/src/networkio.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/networkio.h` & `pyzeo-0.1.2/src/networkio.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/networkstorage.cc` & `pyzeo-0.1.2/src/networkstorage.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/networkstorage.h` & `pyzeo-0.1.2/src/networkstorage.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/poreinfo.h` & `pyzeo-0.1.2/src/poreinfo.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/psd.cc` & `pyzeo-0.1.2/src/psd.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/psd.h` & `pyzeo-0.1.2/src/psd.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/pyzeo.egg-info/PKG-INFO` & `pyzeo-0.1.2/src/pyzeo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzeo
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python interface to Zeo++
 Home-page: https://github.com/nomad-coe/pyzeo
 Author: Lauri Himanen
 Keywords: zeo++ porous materials science
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Cython
```

### Comparing `pyzeo-0.1.1/src/pyzeo.egg-info/SOURCES.txt` & `pyzeo-0.1.2/src/pyzeo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -387,31 +387,26 @@
 src/Eigen/src/plugins/BlockMethods.h
 src/Eigen/src/plugins/CMakeLists.txt
 src/Eigen/src/plugins/CommonCwiseBinaryOps.h
 src/Eigen/src/plugins/CommonCwiseUnaryOps.h
 src/Eigen/src/plugins/MatrixCwiseBinaryOps.h
 src/Eigen/src/plugins/MatrixCwiseUnaryOps.h
 src/pyzeo/__init__.py
-src/pyzeo/area_volume.cpp
-src/pyzeo/channel.cpp
-src/pyzeo/cluster.cpp
-src/pyzeo/cycle.cpp
-src/pyzeo/geometry.cpp
-src/pyzeo/graphstorage.cpp
-src/pyzeo/high_accuracy.cpp
-src/pyzeo/netinfo.cpp
-src/pyzeo/netio.cpp
-src/pyzeo/netstorage.cpp
-src/pyzeo/psd.cpp
-src/pyzeo/voronoicell.cpp
+src/pyzeo/extension.cpp
 src/pyzeo.egg-info/PKG-INFO
 src/pyzeo.egg-info/SOURCES.txt
 src/pyzeo.egg-info/dependency_links.txt
 src/pyzeo.egg-info/not-zip-safe
 src/pyzeo.egg-info/top_level.txt
+src/pyzeo/area_volume/__init__.py
+src/pyzeo/cluster/__init__.py
+src/pyzeo/cycle/__init__.py
+src/pyzeo/high_accuracy/__init__.py
+src/pyzeo/netstorage/__init__.py
+src/pyzeo/psd/__init__.py
 src/voro++/src/c_loops.cc
 src/voro++/src/c_loops.hh
 src/voro++/src/cell.cc
 src/voro++/src/cell.hh
 src/voro++/src/cmd_line.cc
 src/voro++/src/common.cc
 src/voro++/src/common.hh
```

### Comparing `pyzeo-0.1.1/src/ray.cc` & `pyzeo-0.1.2/src/ray.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/ray.h` & `pyzeo-0.1.2/src/ray.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/rmsd.cc` & `pyzeo-0.1.2/src/rmsd.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/rmsd.h` & `pyzeo-0.1.2/src/rmsd.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/segment.h` & `pyzeo-0.1.2/src/segment.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/sphere_approx.cc` & `pyzeo-0.1.2/src/sphere_approx.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/sphere_approx.h` & `pyzeo-0.1.2/src/sphere_approx.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/string_additions.cc` & `pyzeo-0.1.2/src/string_additions.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/string_additions.h` & `pyzeo-0.1.2/src/string_additions.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/symbcalc.cc` & `pyzeo-0.1.2/src/symbcalc.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/symmetry.cc` & `pyzeo-0.1.2/src/symmetry.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/v_network.cc` & `pyzeo-0.1.2/src/v_network.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/v_network.h` & `pyzeo-0.1.2/src/v_network.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/c_loops.cc` & `pyzeo-0.1.2/src/voro++/src/c_loops.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/c_loops.hh` & `pyzeo-0.1.2/src/voro++/src/c_loops.hh`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/cell.cc` & `pyzeo-0.1.2/src/voro++/src/cell.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/cell.hh` & `pyzeo-0.1.2/src/voro++/src/cell.hh`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/cmd_line.cc` & `pyzeo-0.1.2/src/voro++/src/cmd_line.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/common.cc` & `pyzeo-0.1.2/src/voro++/src/common.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/common.hh` & `pyzeo-0.1.2/src/voro++/src/common.hh`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/config.hh` & `pyzeo-0.1.2/src/voro++/src/config.hh`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/container.cc` & `pyzeo-0.1.2/src/voro++/src/container.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/container.hh` & `pyzeo-0.1.2/src/voro++/src/container.hh`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/container_prd.cc` & `pyzeo-0.1.2/src/voro++/src/container_prd.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/container_prd.hh` & `pyzeo-0.1.2/src/voro++/src/container_prd.hh`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/pre_container.cc` & `pyzeo-0.1.2/src/voro++/src/pre_container.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/pre_container.hh` & `pyzeo-0.1.2/src/voro++/src/pre_container.hh`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/rad_option.hh` & `pyzeo-0.1.2/src/voro++/src/rad_option.hh`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/unitcell.cc` & `pyzeo-0.1.2/src/voro++/src/unitcell.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/unitcell.hh` & `pyzeo-0.1.2/src/voro++/src/unitcell.hh`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/v_base.cc` & `pyzeo-0.1.2/src/voro++/src/v_base.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/v_base.hh` & `pyzeo-0.1.2/src/voro++/src/v_base.hh`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/v_base_wl.cc` & `pyzeo-0.1.2/src/voro++/src/v_base_wl.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/v_compute.cc` & `pyzeo-0.1.2/src/voro++/src/v_compute.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/v_compute.hh` & `pyzeo-0.1.2/src/voro++/src/v_compute.hh`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/voro++.hh` & `pyzeo-0.1.2/src/voro++/src/voro++.hh`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/wall.cc` & `pyzeo-0.1.2/src/voro++/src/wall.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/wall.hh` & `pyzeo-0.1.2/src/voro++/src/wall.hh`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voro++/src/worklist.hh` & `pyzeo-0.1.2/src/voro++/src/worklist.hh`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voronoicell.cc` & `pyzeo-0.1.2/src/voronoicell.cc`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/voronoicell.h` & `pyzeo-0.1.2/src/voronoicell.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/zeo_consts.h` & `pyzeo-0.1.2/src/zeo_consts.h`

 * *Files identical despite different names*

### Comparing `pyzeo-0.1.1/src/zeojobs.h` & `pyzeo-0.1.2/src/zeojobs.h`

 * *Files identical despite different names*

