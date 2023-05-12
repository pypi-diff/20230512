# Comparing `tmp/torchopt-0.7.0.tar.gz` & `tmp/torchopt-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchopt-0.7.0.tar", last modified: Wed Feb 15 16:05:47 2023, max compression
+gzip compressed data, was "torchopt-0.7.1.tar", last modified: Fri May 12 09:38:43 2023, max compression
```

## Comparing `torchopt-0.7.0.tar` & `torchopt-0.7.1.tar`

### file list

```diff
@@ -1,139 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.791325 torchopt-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-02-15 16:04:19.000000 torchopt-0.7.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-02-15 16:04:19.000000 torchopt-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-15 16:04:19.000000 torchopt-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    27378 2023-02-15 16:05:47.791325 torchopt-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25674 2023-02-15 16:04:19.000000 torchopt-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.759326 torchopt-0.7.0/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.759326 torchopt-0.7.0/include/adam_op/
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-02-15 16:04:19.000000 torchopt-0.7.0/include/adam_op/adam_op.h
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-02-15 16:04:19.000000 torchopt-0.7.0/include/adam_op/adam_op_impl_cpu.h
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-02-15 16:04:19.000000 torchopt-0.7.0/include/adam_op/adam_op_impl_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-02-15 16:04:19.000000 torchopt-0.7.0/include/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-02-15 16:04:19.000000 torchopt-0.7.0/include/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-02-15 16:04:19.000000 torchopt-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 16:05:47.791325 torchopt-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-02-15 16:04:19.000000 torchopt-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.759326 torchopt-0.7.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-02-15 16:04:19.000000 torchopt-0.7.0/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.759326 torchopt-0.7.0/src/adam_op/
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-02-15 16:04:19.000000 torchopt-0.7.0/src/adam_op/adam_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-02-15 16:04:19.000000 torchopt-0.7.0/src/adam_op/adam_op_impl_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    24833 2023-02-15 16:04:19.000000 torchopt-0.7.0/src/adam_op/adam_op_impl_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-02-15 16:04:19.000000 torchopt-0.7.0/src/extension.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.767325 torchopt-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-02-15 16:04:19.000000 torchopt-0.7.0/tests/test_accelerated_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-02-15 16:04:19.000000 torchopt-0.7.0/tests/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-02-15 16:04:19.000000 torchopt-0.7.0/tests/test_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-02-15 16:04:19.000000 torchopt-0.7.0/tests/test_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-15 16:04:19.000000 torchopt-0.7.0/tests/test_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    25384 2023-02-15 16:04:19.000000 torchopt-0.7.0/tests/test_implicit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-02-15 16:04:19.000000 torchopt-0.7.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-02-15 16:04:19.000000 torchopt-0.7.0/tests/test_linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-02-15 16:04:19.000000 torchopt-0.7.0/tests/test_meta_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-02-15 16:04:19.000000 torchopt-0.7.0/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-02-15 16:04:19.000000 torchopt-0.7.0/tests/test_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-02-15 16:04:19.000000 torchopt-0.7.0/tests/test_pytree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-02-15 16:04:19.000000 torchopt-0.7.0/tests/test_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-02-15 16:04:19.000000 torchopt-0.7.0/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-02-15 16:04:19.000000 torchopt-0.7.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-02-15 16:04:19.000000 torchopt-0.7.0/tests/test_zero_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.767325 torchopt-0.7.0/torchopt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.771325 torchopt-0.7.0/torchopt/_C/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/_C/adam_op.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.771325 torchopt-0.7.0/torchopt/accelerated_op/
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/accelerated_op/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.771325 torchopt-0.7.0/torchopt/accelerated_op/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/accelerated_op/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/accelerated_op/_src/adam_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/accelerated_op/adam_op.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.771325 torchopt-0.7.0/torchopt/alias/
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/alias/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/alias/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/alias/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/alias/rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/alias/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/alias/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.771325 torchopt-0.7.0/torchopt/diff/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/diff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.775326 torchopt-0.7.0/torchopt/diff/implicit/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/diff/implicit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/diff/implicit/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.775326 torchopt-0.7.0/torchopt/diff/implicit/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/diff/implicit/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/diff/implicit/nn/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.775326 torchopt-0.7.0/torchopt/diff/zero_order/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/diff/zero_order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17191 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/diff/zero_order/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.775326 torchopt-0.7.0/torchopt/diff/zero_order/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/diff/zero_order/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/diff/zero_order/nn/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.775326 torchopt-0.7.0/torchopt/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/distributed/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/distributed/autograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/distributed/world.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.779326 torchopt-0.7.0/torchopt/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/linalg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/linalg/cg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/linalg/ns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/linalg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.779326 torchopt-0.7.0/torchopt/linear_solve/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/linear_solve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/linear_solve/cg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/linear_solve/inv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/linear_solve/normal_cg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/linear_solve/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.779326 torchopt-0.7.0/torchopt/nn/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/nn/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/nn/stateless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.783326 torchopt-0.7.0/torchopt/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/optim/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/optim/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/optim/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.783326 torchopt-0.7.0/torchopt/optim/func/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/optim/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/optim/func/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.783326 torchopt-0.7.0/torchopt/optim/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/optim/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/optim/meta/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/optim/meta/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/optim/meta/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/optim/meta/rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/optim/meta/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/optim/rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/optim/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/pytree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.787325 torchopt-0.7.0/torchopt/schedule/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/schedule/polynomial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.791325 torchopt-0.7.0/torchopt/transform/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/transform/add_decayed_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/transform/nan_to_num.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/transform/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/transform/scale_by_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/transform/scale_by_rms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/transform/scale_by_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/transform/scale_by_stddev.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/transform/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/transform/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    18245 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-02-15 16:04:20.000000 torchopt-0.7.0/torchopt/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-02-15 16:04:19.000000 torchopt-0.7.0/torchopt/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:05:47.771325 torchopt-0.7.0/torchopt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27378 2023-02-15 16:05:47.000000 torchopt-0.7.0/torchopt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-02-15 16:05:47.000000 torchopt-0.7.0/torchopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 16:05:47.000000 torchopt-0.7.0/torchopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-02-15 16:05:47.000000 torchopt-0.7.0/torchopt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-15 16:05:47.000000 torchopt-0.7.0/torchopt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.299795 torchopt-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-05-12 09:36:32.000000 torchopt-0.7.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-12 09:36:32.000000 torchopt-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-12 09:36:32.000000 torchopt-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-05-12 09:38:43.299795 torchopt-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25802 2023-05-12 09:36:32.000000 torchopt-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:42.859762 torchopt-0.7.1/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:42.863762 torchopt-0.7.1/include/adam_op/
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-12 09:36:32.000000 torchopt-0.7.1/include/adam_op/adam_op.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-12 09:36:32.000000 torchopt-0.7.1/include/adam_op/adam_op_impl_cpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-12 09:36:32.000000 torchopt-0.7.1/include/adam_op/adam_op_impl_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-12 09:36:32.000000 torchopt-0.7.1/include/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-12 09:36:32.000000 torchopt-0.7.1/include/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-05-12 09:36:32.000000 torchopt-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:38:43.299795 torchopt-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-12 09:36:32.000000 torchopt-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:42.867762 torchopt-0.7.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-12 09:36:32.000000 torchopt-0.7.1/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:42.907765 torchopt-0.7.1/src/adam_op/
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-12 09:36:32.000000 torchopt-0.7.1/src/adam_op/adam_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-05-12 09:36:32.000000 torchopt-0.7.1/src/adam_op/adam_op_impl_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24833 2023-05-12 09:36:32.000000 torchopt-0.7.1/src/adam_op/adam_op_impl_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-12 09:36:32.000000 torchopt-0.7.1/src/extension.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.055776 torchopt-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-05-12 09:36:32.000000 torchopt-0.7.1/tests/test_accelerated_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16952 2023-05-12 09:36:32.000000 torchopt-0.7.1/tests/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-12 09:36:32.000000 torchopt-0.7.1/tests/test_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-12 09:36:32.000000 torchopt-0.7.1/tests/test_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-12 09:36:32.000000 torchopt-0.7.1/tests/test_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30624 2023-05-12 09:36:32.000000 torchopt-0.7.1/tests/test_implicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-05-12 09:36:32.000000 torchopt-0.7.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-12 09:36:32.000000 torchopt-0.7.1/tests/test_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-12 09:36:32.000000 torchopt-0.7.1/tests/test_meta_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-05-12 09:36:32.000000 torchopt-0.7.1/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-05-12 09:36:32.000000 torchopt-0.7.1/tests/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-05-12 09:36:32.000000 torchopt-0.7.1/tests/test_pytree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-12 09:36:32.000000 torchopt-0.7.1/tests/test_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-12 09:36:32.000000 torchopt-0.7.1/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-12 09:36:32.000000 torchopt-0.7.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-12 09:36:32.000000 torchopt-0.7.1/tests/test_zero_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.255791 torchopt-0.7.1/torchopt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.255791 torchopt-0.7.1/torchopt/_C/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/_C/adam_op.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.259792 torchopt-0.7.1/torchopt/accelerated_op/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/accelerated_op/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.259792 torchopt-0.7.1/torchopt/accelerated_op/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/accelerated_op/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/accelerated_op/_src/adam_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/accelerated_op/adam_op.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.263792 torchopt-0.7.1/torchopt/alias/
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/alias/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/alias/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/alias/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/alias/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/alias/rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/alias/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/alias/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.263792 torchopt-0.7.1/torchopt/diff/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/diff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.263792 torchopt-0.7.1/torchopt/diff/implicit/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/diff/implicit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18834 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/diff/implicit/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.267792 torchopt-0.7.1/torchopt/diff/implicit/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/diff/implicit/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/diff/implicit/nn/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.267792 torchopt-0.7.1/torchopt/diff/zero_order/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/diff/zero_order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17682 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/diff/zero_order/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.267792 torchopt-0.7.1/torchopt/diff/zero_order/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/diff/zero_order/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/diff/zero_order/nn/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.271793 torchopt-0.7.1/torchopt/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18682 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/distributed/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/distributed/autograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/distributed/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.271793 torchopt-0.7.1/torchopt/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/linalg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/linalg/cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/linalg/ns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/linalg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.275793 torchopt-0.7.1/torchopt/linear_solve/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/linear_solve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/linear_solve/cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/linear_solve/inv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/linear_solve/normal_cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/linear_solve/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.279793 torchopt-0.7.1/torchopt/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20341 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/nn/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/nn/stateless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.283793 torchopt-0.7.1/torchopt/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/optim/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/optim/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/optim/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/optim/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.283793 torchopt-0.7.1/torchopt/optim/func/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/optim/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/optim/func/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.291794 torchopt-0.7.1/torchopt/optim/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/optim/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/optim/meta/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/optim/meta/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/optim/meta/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/optim/meta/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/optim/meta/rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/optim/meta/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/optim/rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/optim/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/pytree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.291794 torchopt-0.7.1/torchopt/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/schedule/exponential_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/schedule/polynomial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.295794 torchopt-0.7.1/torchopt/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/transform/add_decayed_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/transform/nan_to_num.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/transform/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14681 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/transform/scale_by_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/transform/scale_by_rms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/transform/scale_by_rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/transform/scale_by_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/transform/scale_by_stddev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/transform/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/transform/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-05-12 09:36:32.000000 torchopt-0.7.1/torchopt/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:38:43.255791 torchopt-0.7.1/torchopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-05-12 09:38:42.000000 torchopt-0.7.1/torchopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-12 09:38:42.000000 torchopt-0.7.1/torchopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:38:42.000000 torchopt-0.7.1/torchopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-12 09:38:42.000000 torchopt-0.7.1/torchopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 09:38:42.000000 torchopt-0.7.1/torchopt.egg-info/top_level.txt
```

### Comparing `torchopt-0.7.0/CMakeLists.txt` & `torchopt-0.7.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/LICENSE` & `torchopt-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/PKG-INFO` & `torchopt-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: torchopt
-Version: 0.7.0
+Version: 0.7.1
 Summary: An efficient library for differentiable optimization for PyTorch.
 Author: TorchOpt Contributors
 Author-email: Jie Ren <jieren9806@gmail.com>, Xidong Feng <xidong.feng.20@ucl.ac.uk>, Bo Liu <benjaminliu.eecs@gmail.com>, Xuehai Pan <XuehaiPan@pku.edu.cn>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/metaopt/torchopt
 Project-URL: Repository, https://github.com/metaopt/torchopt
 Project-URL: Documentation, https://torchopt.readthedocs.io
 Project-URL: Bug Report, https://github.com/metaopt/torchopt/issues
 Keywords: PyTorch,functorch,JAX,Meta-Learning,Optimizer,Differentiable Optimizer,Functional Programming
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Environment :: GPU
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: lint
 Provides-Extra: test
 License-File: LICENSE
 
 <!-- markdownlint-disable first-line-h1 -->
 <!-- markdownlint-disable html -->
@@ -40,18 +39,18 @@
 
 <div align="center">
   <img src="https://github.com/metaopt/torchopt/raw/HEAD/image/logo-large.png" width="75%" />
 </div>
 
 <div align="center">
 
-  <a>![Python 3.7+](https://img.shields.io/badge/Python-3.7%2B-brightgreen.svg)</a>
+  <a>![Python 3.8+](https://img.shields.io/badge/Python-3.8%2B-brightgreen.svg)</a>
   <a href="https://pypi.org/project/torchopt">![PyPI](https://img.shields.io/pypi/v/torchopt?logo=pypi)</a>
   <a href="https://github.com/metaopt/torchopt/tree/HEAD/tests">![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/metaopt/torchopt/tests.yml?label=tests&logo=github)</a>
-  <a href="https://codecov.io/gh/metaopt/torchopt">![CodeCov](https://img.shields.io/codecov/c/gh/metaopt/torchopt)</a>
+  <a href="https://codecov.io/gh/metaopt/torchopt">![CodeCov](https://img.shields.io/codecov/c/github/metaopt/torchopt/main?logo=codecov)</a>
   <a href="https://torchopt.readthedocs.io">![Documentation Status](https://img.shields.io/readthedocs/torchopt?logo=readthedocs)</a>
   <a href="https://pepy.tech/project/torchopt">![Downloads](https://static.pepy.tech/personalized-badge/torchopt?period=total&left_color=grey&right_color=blue&left_text=downloads)</a>
   <a href="https://github.com/metaopt/torchopt/blob/HEAD/LICENSE">![License](https://img.shields.io/github/license/metaopt/torchopt?label=license&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0IiBmaWxsPSIjZmZmZmZmIj48cGF0aCBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik0xMi43NSAyLjc1YS43NS43NSAwIDAwLTEuNSAwVjQuNUg5LjI3NmExLjc1IDEuNzUgMCAwMC0uOTg1LjMwM0w2LjU5NiA1Ljk1N0EuMjUuMjUgMCAwMTYuNDU1IDZIMi4zNTNhLjc1Ljc1IDAgMTAwIDEuNUgzLjkzTC41NjMgMTUuMThhLjc2Mi43NjIgMCAwMC4yMS44OGMuMDguMDY0LjE2MS4xMjUuMzA5LjIyMS4xODYuMTIxLjQ1Mi4yNzguNzkyLjQzMy42OC4zMTEgMS42NjIuNjIgMi44NzYuNjJhNi45MTkgNi45MTkgMCAwMDIuODc2LS42MmMuMzQtLjE1NS42MDYtLjMxMi43OTItLjQzMy4xNS0uMDk3LjIzLS4xNTguMzEtLjIyM2EuNzUuNzUgMCAwMC4yMDktLjg3OEw1LjU2OSA3LjVoLjg4NmMuMzUxIDAgLjY5NC0uMTA2Ljk4NC0uMzAzbDEuNjk2LTEuMTU0QS4yNS4yNSAwIDAxOS4yNzUgNmgxLjk3NXYxNC41SDYuNzYzYS43NS43NSAwIDAwMCAxLjVoMTAuNDc0YS43NS43NSAwIDAwMC0xLjVIMTIuNzVWNmgxLjk3NGMuMDUgMCAuMS4wMTUuMTQuMDQzbDEuNjk3IDEuMTU0Yy4yOS4xOTcuNjMzLjMwMy45ODQuMzAzaC44ODZsLTMuMzY4IDcuNjhhLjc1Ljc1IDAgMDAuMjMuODk2Yy4wMTIuMDA5IDAgMCAuMDAyIDBhMy4xNTQgMy4xNTQgMCAwMC4zMS4yMDZjLjE4NS4xMTIuNDUuMjU2Ljc5LjRhNy4zNDMgNy4zNDMgMCAwMDIuODU1LjU2OCA3LjM0MyA3LjM0MyAwIDAwMi44NTYtLjU2OWMuMzM4LS4xNDMuNjA0LS4yODcuNzktLjM5OWEzLjUgMy41IDAgMDAuMzEtLjIwNi43NS43NSAwIDAwLjIzLS44OTZMMjAuMDcgNy41aDEuNTc4YS43NS43NSAwIDAwMC0xLjVoLTQuMTAyYS4yNS4yNSAwIDAxLS4xNC0uMDQzbC0xLjY5Ny0xLjE1NGExLjc1IDEuNzUgMCAwMC0uOTg0LS4zMDNIMTIuNzVWMi43NXpNMi4xOTMgMTUuMTk4YTUuNDE4IDUuNDE4IDAgMDAyLjU1Ny42MzUgNS40MTggNS40MTggMCAwMDIuNTU3LS42MzVMNC43NSA5LjM2OGwtMi41NTcgNS44M3ptMTQuNTEtLjAyNGMuMDgyLjA0LjE3NC4wODMuMjc1LjEyNi41My4yMjMgMS4zMDUuNDUgMi4yNzIuNDVhNS44NDYgNS44NDYgMCAwMDIuNTQ3LS41NzZMMTkuMjUgOS4zNjdsLTIuNTQ3IDUuODA3eiI+PC9wYXRoPjwvc3ZnPgo=)</a>
 </div>
 
 <p align="center">
   <a href="https://github.com/metaopt/torchopt#installation">Installation</a> |
@@ -66,15 +65,15 @@
 TorchOpt is:
 
 - **Comprehensive**: TorchOpt provides three differentiation modes - explicit differentiation, implicit differentiation, and zero-order differentiation for handling different differentiable optimization situations.
 - **Flexible**: TorchOpt provides both functional and objective-oriented API for users' different preferences. Users can implement differentiable optimization in JAX-like or PyTorch-like style.
 - **Efficient**: TorchOpt provides (1) CPU/GPU acceleration differentiable optimizer (2) RPC-based distributed training framework (3) Fast Tree Operations, to largely increase the training efficiency for bi-level optimization problems.
 
 Beyond differentiable optimization, TorchOpt can also be regarded as a functional optimizer that enables [JAX-like](https://github.com/google/jax) composable functional optimizer for PyTorch.
-With TorchOpt, users can easily conduct neural network optimization in PyTorch with functional style optimizer, similar to [Optax](https://github.com/deepmind/optax) in JAX.
+With TorchOpt, users can easily conduct neural network optimization in PyTorch with a functional style optimizer, similar to [Optax](https://github.com/deepmind/optax) in JAX.
 
 --------------------------------------------------------------------------------
 
 The README is organized as follows:
 
 - [TorchOpt as Functional Optimizer](#torchopt-as-functional-optimizer)
   - [Optax-Like API](#optax-like-api)
@@ -164,19 +163,19 @@
 optimizer.zero_grad()             # zero gradients
 loss.backward()                   # backward
 optimizer.step()                  # step updates
 ```
 
 ### Differentiable
 
-On top of the same optimization function as `torch.optim`, an important benefit of functional optimizer is that one can implement differentiable optimization easily.
-This is particularly helpful when the algorithm requires to differentiate through optimization updates (such as meta-learning practices).
+On top of the same optimization function as `torch.optim`, an important benefit of the functional optimizer is that one can implement differentiable optimization easily.
+This is particularly helpful when the algorithm requires differentiation through optimization updates (such as meta-learning practices).
 We take as the inputs the gradients and optimizer states, and use non-in-place operators to compute and output the updates.
 The processes can be automatically implemented, with the only need from users being to pass the argument `inplace=False` to the functions.
-Check out section [Explicit Gradient (EG)](#explicit-gradient-eg) functional API for example.
+Check out the section [Explicit Gradient](#explicit-gradient-eg) (EG)](#explicit-gradient-eg) functional API for example.
 
 --------------------------------------------------------------------------------
 
 ## TorchOpt for Differentiable Optimization
 
 We design a bilevel-optimization updating scheme, which can be easily extended to realize various differentiable optimization processes.
 
@@ -187,23 +186,23 @@
 As shown above, the scheme contains an outer level that has parameters $\phi$ that can be learned end-to-end through the inner level parameters solution $\theta^{\prime}(\phi)$ by using the best-response derivatives $\partial \theta^{\prime}(\phi) / \partial \phi$.
 TorchOpt supports three differentiation modes.
 It can be seen that the key component of this algorithm is to calculate the best-response (BR) Jacobian.
 From the BR-based perspective, existing gradient methods can be categorized into three groups: explicit gradient over unrolled optimization, implicit differentiation, and zero-order gradient differentiation.
 
 ### Explicit Gradient (EG)
 
-The idea of explicit gradient is to treat the gradient step as a differentiable function and try to backpropagate through the unrolled optimization path.
+The idea of the explicit gradient is to treat the gradient step as a differentiable function and try to backpropagate through the unrolled optimization path.
 This differentiation mode is suitable for algorithms when the inner-level optimization solution is obtained by a few gradient steps, such as [MAML](https://arxiv.org/abs/1703.03400) and [MGRL](https://arxiv.org/abs/1805.09801).
 TorchOpt offers both functional and object-oriented API for EG to fit different user applications.
 
 #### Functional API  <!-- omit in toc -->
 
 The functional API is to conduct optimization in a functional programming style.
 Note that we pass the argument `inplace=False` to the functions to make the optimization differentiable.
-Refer to the tutorial notebook [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb) for more guidances.
+Refer to the tutorial notebook [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb) for more guidance.
 
 ```python
 # Define functional optimizer
 optimizer = torchopt.adam()
 # Define meta and inner parameters
 meta_params = ...
 fmodel, params = make_functional(model)
@@ -219,16 +218,16 @@
 
 loss = outer_loss(fmodel, params, meta_params)
 meta_grads = torch.autograd.grad(loss, meta_params)
 ```
 
 #### OOP API  <!-- omit in toc -->
 
-TorchOpt also provides OOP API compatible with PyTorch programming style.
-Refer to the example and the tutorial notebook [Meta-Optimizer](tutorials/3_Meta_Optimizer.ipynb), [Stop Gradient](tutorials/4_Stop_Gradient.ipynb) for more guidances.
+TorchOpt also provides OOP API compatible with the PyTorch programming style.
+Refer to the example and the tutorial notebook [Meta-Optimizer](tutorials/3_Meta_Optimizer.ipynb), [Stop Gradient](tutorials/4_Stop_Gradient.ipynb) for more guidance.
 
 ```python
 # Define meta and inner parameters
 meta_params = ...
 model = ...
 # Define differentiable optimizer
 optimizer = torchopt.MetaAdam(model)  # a model instance as the argument instead of model.parameters()
@@ -247,15 +246,15 @@
 By treating the solution $\theta^{\prime}$ as an implicit function of $\phi$, the idea of IG is to directly get analytical best-response derivatives $\partial \theta^{\prime} (\phi) / \partial \phi$ by [implicit function theorem](https://en.wikipedia.org/wiki/Implicit_function_theorem).
 This is suitable for algorithms when the inner-level optimal solution is achieved ${\left. \frac{\partial F (\theta, \phi)}{\partial \theta} \right\rvert}_{\theta=\theta^{\prime}} = 0$ or reaches some stationary conditions $F (\theta^{\prime}, \phi) = 0$, such as [iMAML](https://arxiv.org/abs/1909.04630) and [DEQ](https://arxiv.org/abs/1909.01377).
 TorchOpt offers both functional and OOP APIs for supporting both [conjugate gradient-based](https://arxiv.org/abs/1909.04630) and [Neumann series-based](https://arxiv.org/abs/1911.02590) IG methods.
 Refer to the example [iMAML](https://github.com/waterhorse1/torchopt/tree/readme/examples/iMAML) and the notebook [Implicit Gradient](tutorials/5_Implicit_Differentiation.ipynb) for more guidance.
 
 #### Functional API  <!-- omit in toc -->
 
-For implicit gradient, users need to define the stationary condition and TorchOpt provides the decorator to wrap the solve function for enabling implicit gradient computation.
+For the implicit gradient, users need to define the stationary condition and TorchOpt provides the decorator to wrap the solve function for enabling implicit gradient computation.
 
 ```python
 # The stationary condition for the inner-loop
 def stationary(params, meta_params, data):
     # Stationary condition construction
     return stationary condition
 
@@ -272,15 +271,15 @@
 loss = outer_loss(optimal_params)
 
 meta_grads = torch.autograd.grad(loss, meta_params)
 ```
 
 #### OOP API  <!-- omit in toc -->
 
-TorchOpt also offer an OOP API, users need to inherit from the class `torchopt.nn.ImplicitMetaGradientModule` to construct the inner-loop network.
+TorchOpt also offers an OOP API, which users need to inherit from the class `torchopt.nn.ImplicitMetaGradientModule` to construct the inner-loop network.
 Users need to define the stationary condition/objective function and the inner-loop solve function to enable implicit gradient computation.
 
 ```python
 # Inherited from the class ImplicitMetaGradientModule
 # Optionally specify the linear solver (conjugate gradient or Neumann series)
 class InnerNet(ImplicitMetaGradientModule, linear_solve=linear_solver):
     def __init__(self, meta_param):
@@ -320,15 +319,15 @@
 
 ### Zero-order Differentiation (ZD)
 
 When the inner-loop process is non-differentiable or one wants to eliminate the heavy computation burdens in the previous two modes (brought by Hessian), one can choose Zero-order Differentiation (ZD).
 ZD typically gets gradients based on zero-order estimation, such as finite-difference, or [Evolutionary Strategy](https://arxiv.org/abs/1703.03864).
 Instead of optimizing the objective $F$, ES optimizes a smoothed objective.
 TorchOpt provides both functional and OOP APIs for the ES method.
-Refer to the tutorial notebook [Zero-order Differentiation](tutorials/6_Zero_Order_Differentiation.ipynb) for more guidances.
+Refer to the tutorial notebook [Zero-order Differentiation](tutorials/6_Zero_Order_Differentiation.ipynb) for more guidance.
 
 #### Functional API  <!-- omit in toc -->
 
 For zero-order differentiation, users need to define the forward pass calculation and the noise sampling procedure. TorchOpt provides the decorator to wrap the forward function for enabling zero-order differentiation.
 
 ```python
 # Customize the noise sampling function in ES
@@ -347,15 +346,15 @@
     # Forward process
     ...
     return objective  # the returned tensor should be a scalar tensor
 ```
 
 #### OOP API  <!-- omit in toc -->
 
-TorchOpt also offer an OOP API, users need to inherit from the class `torchopt.nn.ZeroOrderGradientModule` to construct the network as an `nn.Module` following a classical PyTorch style.
+TorchOpt also offers an OOP API, which users need to inherit from the class `torchopt.nn.ZeroOrderGradientModule` to construct the network as an `nn.Module` following a classical PyTorch style.
 Users need to define the forward process zero-order gradient procedures `forward()` and a noise sampling function `sample()`.
 
 ```python
 # Inherited from the class ZeroOrderGradientModule
 # Optionally specify the `method` and/or `num_samples` and/or `sigma` used for sampling
 class Net(ZeroOrderGradientModule, method=method, num_samples=num_samples, sigma=sigma):
     def __init__(self, ...):
@@ -388,65 +387,65 @@
 
 ### CPU/GPU accelerated differentiable optimizer
 
 We take the optimizer as a whole instead of separating it into several basic operators (e.g., `sqrt` and `div`).
 Therefore, by manually writing the forward and backward functions, we can perform the symbolic reduction.
 In addition, we can store some intermediate data that can be reused during the backpropagation.
 We write the accelerated functions in C++ OpenMP and CUDA, bind them by [`pybind11`](https://github.com/pybind/pybind11) to allow they can be called by Python, and then define the forward and backward behavior using `torch.autograd.Function`.
-Users can use by simply setting the `use_accelerated_op` flag as `True`.
-Refer to the corresponding sections in tutorials [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb) and [Meta-Optimizer](tutorials/3_Meta_Optimizer.ipynb)
+Users can use it by simply setting the `use_accelerated_op` flag as `True`.
+Refer to the corresponding sections in the tutorials [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb)](tutorials/1_Functional_Optimizer.ipynb) and [Meta-Optimizer](tutorials/3_Meta_Optimizer.ipynb)
 
 ```python
 optimizer = torchopt.MetaAdam(model, lr, use_accelerated_op=True)
 ```
 
 ### Distributed Training
 
 `TorchOpt` provides distributed training features based on the PyTorch RPC module for better training speed and multi-node multi-GPU support.
-Different from the MPI-like parallelization paradigm, which uses multiple homogenous workers and requires carefully designed communication hooks, the RPC APIs allow users to build their optimization pipeline more flexibly.
+Different from the MPI-like parallelization paradigm, which uses multiple homogeneous workers and requires carefully designed communication hooks, the RPC APIs allow users to build their optimization pipeline more flexibly.
 Experimental results show that we achieve an approximately linear relationship between the speed-up ratio and the number of workers.
 Check out the [Distributed Training Documentation](https://torchopt.readthedocs.io/en/latest/distributed/distributed.html) and [distributed MAML example](https://github.com/metaopt/torchopt/tree/main/examples/distributed/few-shot) for more specific guidance.
 
 ### OpTree
 
 We implement the *PyTree* to enable fast nested structure flattening using C++.
 The tree operations (e.g., flatten and unflatten) are very important in enabling functional and Just-In-Time (JIT) features of deep learning frameworks.
 By implementing it in C++, we can use some cache/memory-friendly structures (e.g., `absl::InlinedVector`) to improve the performance.
 For more guidance and comparison results, please refer to our open-source project [`OpTree`](https://github.com/metaopt/optree).
 
 --------------------------------------------------------------------------------
 
 ## Visualization
 
-Complex gradient flow in meta-learning brings in a great challenge for managing the gradient flow and verifying the correctness of it.
+Complex gradient flow in meta-learning brings in a great challenge for managing the gradient flow and verifying its correctness of it.
 TorchOpt provides a visualization tool that draws variable (e.g., network parameters or meta-parameters) names on the gradient graph for better analysis.
 The visualization tool is modified from [`torchviz`](https://github.com/szagoruyko/pytorchviz).
 Refer to the example [visualization code](examples/visualize.py) and the tutorial notebook [Visualization](tutorials/2_Visualization.ipynb) for more details.
 
-The figure below show the visualization result.
+The figure below shows the visualization result.
 Compared with [`torchviz`](https://github.com/szagoruyko/pytorchviz), TorchOpt fuses the operations within the `Adam` together (orange) to reduce the complexity and provide simpler visualization.
 
 <div align="center">
   <img src="https://github.com/metaopt/torchopt/raw/HEAD/image/torchviz-vs-torchopt.jpg" width="80%" />
 </div>
 
 --------------------------------------------------------------------------------
 
 ## Examples
 
-In the [`examples`](examples) directory, we offer several examples of functional optimizers and light-weight meta-learning examples with TorchOpt.
+In the [`examples`](examples) directory, we offer several examples of functional optimizers and lightweight meta-learning examples with TorchOpt.
 
 - [Model-Agnostic Meta-Learning (MAML) - Supervised Learning](https://arxiv.org/abs/1703.03400) (ICML 2017)
 - [Learning to Reweight Examples for Robust Deep Learning](https://arxiv.org/abs/1803.09050) (ICML 2018)
 - [Model-Agnostic Meta-Learning (MAML) - Reinforcement Learning](https://arxiv.org/abs/1703.03400) (ICML 2017)
 - [Meta-Gradient Reinforcement Learning (MGRL)](https://arxiv.org/abs/1805.09801) (NeurIPS 2018)
 - [Learning through opponent learning process (LOLA)](https://arxiv.org/abs/1709.04326) (AAMAS 2018)
 - [Meta-Learning with Implicit Gradients](https://arxiv.org/abs/1909.04630) (NeurIPS 2019)
 
-Also check [`examples`](examples) for more distributed/visualization/functorch-compatible examples.
+Also, check [`examples`](examples) for more distributed/visualization/functorch-compatible examples.
 
 --------------------------------------------------------------------------------
 
 ## Installation
 
 Requirements
```

#### html2text {}

```diff
@@ -1,40 +1,39 @@
-Metadata-Version: 2.1 Name: torchopt Version: 0.7.0 Summary: An efficient
+Metadata-Version: 2.1 Name: torchopt Version: 0.7.1 Summary: An efficient
 library for differentiable optimization for PyTorch. Author: TorchOpt
 Contributors Author-email: Jie Ren
 gmail.com>, Xidong Feng
 feng.20@ucl.ac.uk>, Bo Liu
 eecs@gmail.com>, Xuehai Pan
 pku.edu.cn> License: Apache License, Version 2.0 Project-URL: Homepage, https:/
 /github.com/metaopt/torchopt Project-URL: Repository, https://github.com/
 metaopt/torchopt Project-URL: Documentation, https://torchopt.readthedocs.io
 Project-URL: Bug Report, https://github.com/metaopt/torchopt/issues Keywords:
 PyTorch,functorch,JAX,Meta-Learning,Optimizer,Differentiable
 Optimizer,Functional Programming Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
-:: Linux Classifier: Operating System :: MacOS Classifier: Environment :: GPU
-Classifier: Environment :: GPU :: NVIDIA CUDA Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Education Classifier: Intended
-Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-lint Provides-Extra: test License-File: LICENSE
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: POSIX :: Linux Classifier: Operating System :: MacOS
+Classifier: Environment :: GPU Classifier: Environment :: GPU :: NVIDIA CUDA
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Education Classifier: Intended Audience :: Science/Research Classifier: Topic
+:: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Requires-Python: >=3.8 Description-Content-Type: text/
+markdown Provides-Extra: lint Provides-Extra: test License-File: LICENSE
       [https://github.com/metaopt/torchopt/raw/HEAD/image/logo-large.png]
- ![Python 3.7+](https://img.shields.io/badge/Python-3.7%2B-brightgreen.svg) !
+ ![Python 3.8+](https://img.shields.io/badge/Python-3.8%2B-brightgreen.svg) !
   [PyPI](https://img.shields.io/pypi/v/torchopt?logo=pypi) ![GitHub_Workflow
 Status](https://img.shields.io/github/actions/workflow/status/metaopt/torchopt/
 tests.yml?label=tests&logo=github) ![CodeCov](https://img.shields.io/codecov/c/
-     gh/metaopt/torchopt) ![Documentation_Status](https://img.shields.io/
- readthedocs/torchopt?logo=readthedocs) ![Downloads](https://static.pepy.tech/
-                              personalized-badge/
+  github/metaopt/torchopt/main?logo=codecov) ![Documentation_Status](https://
+  img.shields.io/readthedocs/torchopt?logo=readthedocs) ![Downloads](https://
+                     static.pepy.tech/personalized-badge/
  torchopt?period=total&left_color=grey&right_color=blue&left_text=downloads) !
            [License](https://img.shields.io/github/license/metaopt/
                     torchopt?label=license&logo=data:image/
 svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0IiBmaWxsPSIjZmZmZmZmIj48cGF0aCBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik0xMi43NSAyLjc1YS43NS43NSAwIDAwLTEuNSAwVjQuNUg5LjI3NmExLjc1IDEuNzUgMCAwMC0uOTg1LjMwM0w2LjU5NiA1Ljk1N0EuMjUuMjUgMCAwMTYuNDU1IDZIMi4zNTNhLjc1Ljc1IDAgMTAwIDEuNUgzLjkzTC41NjMgMTUuMThhLjc2Mi43NjIgMCAwMC4yMS44OGMuMDguMDY0LjE2MS4xMjUuMzA5LjIyMS4xODYuMTIxLjQ1Mi4yNzguNzkyLjQzMy42OC4zMTEgMS42NjIuNjIgMi44NzYuNjJhNi45MTkgNi45MTkgMCAwMDIuODc2LS42MmMuMzQtLjE1NS42MDYtLjMxMi43OTItLjQzMy4xNS0uMDk3LjIzLS4xNTguMzEtLjIyM2EuNzUuNzUgMCAwMC4yMDktLjg3OEw1LjU2OSA3LjVoLjg4NmMuMzUxIDAgLjY5NC0uMTA2Ljk4NC0uMzAzbDEuNjk2LTEuMTU0QS4yNS4yNSAwIDAxOS4yNzUgNmgxLjk3NXYxNC41SDYuNzYzYS43NS43NSAwIDAwMCAxLjVoMTAuNDc0YS43NS43NSAwIDAwMC0xLjVIMTIuNzVWNmgxLjk3NGMuMDUgMCAuMS4wMTUuMTQuMDQzbDEuNjk3IDEuMTU0Yy4yOS4xOTcuNjMzLjMwMy45ODQuMzAzaC44ODZsLTMuMzY4IDcuNjhhLjc1Ljc1IDAgMDAuMjMuODk2Yy4wMTIuMDA5IDAgMCAuMDAyIDBhMy4xNTQgMy4xNTQgMCAwMC4zMS4yMDZjLjE4NS4xMTIuNDUuMjU2Ljc5LjRhNy4zNDMgNy4zNDMgMCAwMDIuODU1LjU2OCA3LjM0MyA3LjM0MyAwIDAwMi44NTYtLjU2OWMuMzM4LS4xNDMuNjA0LS4yODcuNzktLjM5OWEzLjUgMy41IDAgMDAuMzEtLjIwNi43NS43NSAwIDAwLjIzLS44OTZMMjAuMDcgNy41aDEuNTc4YS43NS43NSAwIDAwMC0xLjVoLTQuMTAyYS4yNS4yNSAwIDAxLS4xNC0uMDQzbC0xLjY5Ny0xLjE1NGExLjc1IDEuNzUgMCAwMC0uOTg0LS4zMDNIMTIuNzVWMi43NXpNMi4xOTMgMTUuMTk4YTUuNDE4IDUuNDE4IDAgMDAyLjU1Ny42MzUgNS40MTggNS40MTggMCAwMDIuNTU3LS42MzVMNC43NSA5LjM2OGwtMi41NTcgNS44M3ptMTQuNTEtLjAyNGMuMDgyLjA0LjE3NC4wODMuMjc1LjEyNi41My4yMjMgMS4zMDUuNDUgMi4yNzIuNDVhNS44NDYgNS44NDYgMCAwMDIuNTQ3LS41NzZMMTkuMjUgOS4zNjdsLTIuNTQ3IDUuODA3eiI+PC9wYXRoPjwvc3ZnPgo=)
     Installation | Documentation | Tutorials | Examples | Paper | Citation
 **TorchOpt** is an efficient library for differentiable optimization built upon
 [PyTorch](https://pytorch.org). TorchOpt is: - **Comprehensive**: TorchOpt
@@ -45,141 +44,141 @@
 can implement differentiable optimization in JAX-like or PyTorch-like style. -
 **Efficient**: TorchOpt provides (1) CPU/GPU acceleration differentiable
 optimizer (2) RPC-based distributed training framework (3) Fast Tree
 Operations, to largely increase the training efficiency for bi-level
 optimization problems. Beyond differentiable optimization, TorchOpt can also be
 regarded as a functional optimizer that enables [JAX-like](https://github.com/
 google/jax) composable functional optimizer for PyTorch. With TorchOpt, users
-can easily conduct neural network optimization in PyTorch with functional style
-optimizer, similar to [Optax](https://github.com/deepmind/optax) in JAX. ------
--------------------------------------------------------------------------- The
-README is organized as follows: - [TorchOpt as Functional Optimizer](#torchopt-
-as-functional-optimizer) - [Optax-Like API](#optax-like-api) - [PyTorch-Like
-API](#pytorch-like-api) - [Differentiable](#differentiable) - [TorchOpt for
-Differentiable Optimization](#torchopt-for-differentiable-optimization) -
-[Explicit Gradient (EG)](#explicit-gradient-eg) - [Implicit Gradient (IG)]
-(#implicit-gradient-ig) - [Zero-order Differentiation (ZD)](#zero-order-
-differentiation-zd) - [High-Performance and Distributed Training](#high-
-performance-and-distributed-training) - [CPU/GPU accelerated differentiable
-optimizer](#cpugpu-accelerated-differentiable-optimizer) - [Distributed
-Training](#distributed-training) - [OpTree](#optree) - [Visualization]
-(#visualization) - [Examples](#examples) - [Installation](#installation) -
-[Changelog](#changelog) - [Citing TorchOpt](#citing-torchopt) - [The Team]
-(#the-team) - [License](#license) ---------------------------------------------
------------------------------------ ## TorchOpt as Functional Optimizer The
-design of TorchOpt follows the philosophy of functional programming. Aligned
-with [`functorch`](https://github.com/pytorch/functorch), users can conduct
-functional style programming with models, optimizers and training in PyTorch.
-We use the Adam optimizer as an example in the following illustration. You can
-also check out the tutorial notebook [Functional Optimizer](tutorials/
-1_Functional_Optimizer.ipynb) for more details. ### Optax-Like API For those
-users who prefer fully functional programming, we offer Optax-Like API by
-passing gradients and optimizer states to the optimizer function. Here is an
-example coupled with `functorch`: ```python class Net(nn.Module): ... class
-Loader(DataLoader): ... net = Net() # init loader = Loader() optimizer =
-torchopt.adam() model, params = functorch.make_functional(net) # use functorch
-extract network parameters opt_state = optimizer.init(params) # init optimizer
-xs, ys = next(loader) # get data pred = model(params, xs) # forward loss =
-F.cross_entropy(pred, ys) # compute loss grads = torch.autograd.grad(loss,
-params) # compute gradients updates, opt_state = optimizer.update(grads,
-opt_state) # get updates params = torchopt.apply_updates(params, updates) #
-update network parameters ``` We also provide a wrapper
-`torchopt.FuncOptimizer` to make maintaining the optimizer state easier:
-```python net = Net() # init loader = Loader() optimizer =
+can easily conduct neural network optimization in PyTorch with a functional
+style optimizer, similar to [Optax](https://github.com/deepmind/optax) in JAX.
+-------------------------------------------------------------------------------
+- The README is organized as follows: - [TorchOpt as Functional Optimizer]
+(#torchopt-as-functional-optimizer) - [Optax-Like API](#optax-like-api) -
+[PyTorch-Like API](#pytorch-like-api) - [Differentiable](#differentiable) -
+[TorchOpt for Differentiable Optimization](#torchopt-for-differentiable-
+optimization) - [Explicit Gradient (EG)](#explicit-gradient-eg) - [Implicit
+Gradient (IG)](#implicit-gradient-ig) - [Zero-order Differentiation (ZD)]
+(#zero-order-differentiation-zd) - [High-Performance and Distributed Training]
+(#high-performance-and-distributed-training) - [CPU/GPU accelerated
+differentiable optimizer](#cpugpu-accelerated-differentiable-optimizer) -
+[Distributed Training](#distributed-training) - [OpTree](#optree) -
+[Visualization](#visualization) - [Examples](#examples) - [Installation]
+(#installation) - [Changelog](#changelog) - [Citing TorchOpt](#citing-torchopt)
+- [The Team](#the-team) - [License](#license) ---------------------------------
+----------------------------------------------- ## TorchOpt as Functional
+Optimizer The design of TorchOpt follows the philosophy of functional
+programming. Aligned with [`functorch`](https://github.com/pytorch/functorch),
+users can conduct functional style programming with models, optimizers and
+training in PyTorch. We use the Adam optimizer as an example in the following
+illustration. You can also check out the tutorial notebook [Functional
+Optimizer](tutorials/1_Functional_Optimizer.ipynb) for more details. ### Optax-
+Like API For those users who prefer fully functional programming, we offer
+Optax-Like API by passing gradients and optimizer states to the optimizer
+function. Here is an example coupled with `functorch`: ```python class Net
+(nn.Module): ... class Loader(DataLoader): ... net = Net() # init loader =
+Loader() optimizer = torchopt.adam() model, params = functorch.make_functional
+(net) # use functorch extract network parameters opt_state = optimizer.init
+(params) # init optimizer xs, ys = next(loader) # get data pred = model(params,
+xs) # forward loss = F.cross_entropy(pred, ys) # compute loss grads =
+torch.autograd.grad(loss, params) # compute gradients updates, opt_state =
+optimizer.update(grads, opt_state) # get updates params =
+torchopt.apply_updates(params, updates) # update network parameters ``` We also
+provide a wrapper `torchopt.FuncOptimizer` to make maintaining the optimizer
+state easier: ```python net = Net() # init loader = Loader() optimizer =
 torchopt.FuncOptimizer(torchopt.adam()) # wrap with `torchopt.FuncOptimizer`
 model, params = functorch.make_functional(net) # use functorch extract network
 parameters for xs, ys in loader: # get data pred = model(params, xs) # forward
 loss = F.cross_entropy(pred, ys) # compute loss params = optimizer.step(loss,
 params) # update network parameters ``` ### PyTorch-Like API We also design a
 base class `torchopt.Optimizer` that has the same interface as
 `torch.optim.Optimizer`. We offer origin PyTorch APIs (e.g. `zero_grad()` or
 `step()`) by wrapping our Optax-Like API for traditional PyTorch users.
 ```python net = Net() # init loader = Loader() optimizer = torchopt.Adam
 (net.parameters()) xs, ys = next(loader) # get data pred = net(xs) # forward
 loss = F.cross_entropy(pred, ys) # compute loss optimizer.zero_grad() # zero
 gradients loss.backward() # backward optimizer.step() # step updates ``` ###
 Differentiable On top of the same optimization function as `torch.optim`, an
-important benefit of functional optimizer is that one can implement
+important benefit of the functional optimizer is that one can implement
 differentiable optimization easily. This is particularly helpful when the
-algorithm requires to differentiate through optimization updates (such as meta-
+algorithm requires differentiation through optimization updates (such as meta-
 learning practices). We take as the inputs the gradients and optimizer states,
 and use non-in-place operators to compute and output the updates. The processes
 can be automatically implemented, with the only need from users being to pass
-the argument `inplace=False` to the functions. Check out section [Explicit
-Gradient (EG)](#explicit-gradient-eg) functional API for example. -------------
-------------------------------------------------------------------- ## TorchOpt
-for Differentiable Optimization We design a bilevel-optimization updating
-scheme, which can be easily extended to realize various differentiable
-optimization processes.
+the argument `inplace=False` to the functions. Check out the section [Explicit
+Gradient](#explicit-gradient-eg) (EG)](#explicit-gradient-eg) functional API
+for example. ------------------------------------------------------------------
+-------------- ## TorchOpt for Differentiable Optimization We design a bilevel-
+optimization updating scheme, which can be easily extended to realize various
+differentiable optimization processes.
        [https://github.com/metaopt/torchopt/raw/HEAD/image/diffmode.png]
 As shown above, the scheme contains an outer level that has parameters $\phi$
 that can be learned end-to-end through the inner level parameters solution
 $\theta^{\prime}(\phi)$ by using the best-response derivatives $\partial
 \theta^{\prime}(\phi) / \partial \phi$. TorchOpt supports three differentiation
 modes. It can be seen that the key component of this algorithm is to calculate
 the best-response (BR) Jacobian. From the BR-based perspective, existing
 gradient methods can be categorized into three groups: explicit gradient over
 unrolled optimization, implicit differentiation, and zero-order gradient
-differentiation. ### Explicit Gradient (EG) The idea of explicit gradient is to
-treat the gradient step as a differentiable function and try to backpropagate
-through the unrolled optimization path. This differentiation mode is suitable
-for algorithms when the inner-level optimization solution is obtained by a few
-gradient steps, such as [MAML](https://arxiv.org/abs/1703.03400) and [MGRL]
-(https://arxiv.org/abs/1805.09801). TorchOpt offers both functional and object-
-oriented API for EG to fit different user applications. #### Functional API
-The functional API is to conduct optimization in a functional programming
-style. Note that we pass the argument `inplace=False` to the functions to make
-the optimization differentiable. Refer to the tutorial notebook [Functional
-Optimizer](tutorials/1_Functional_Optimizer.ipynb) for more guidances.
-```python # Define functional optimizer optimizer = torchopt.adam() # Define
-meta and inner parameters meta_params = ... fmodel, params = make_functional
-(model) # Initial state state = optimizer.init(params) for iter in range
-(iter_times): loss = inner_loss(fmodel, params, meta_params) grads =
-torch.autograd.grad(loss, params) # Apply non-inplace parameter update updates,
-state = optimizer.update(grads, state, inplace=False) params =
+differentiation. ### Explicit Gradient (EG) The idea of the explicit gradient
+is to treat the gradient step as a differentiable function and try to
+backpropagate through the unrolled optimization path. This differentiation mode
+is suitable for algorithms when the inner-level optimization solution is
+obtained by a few gradient steps, such as [MAML](https://arxiv.org/abs/
+1703.03400) and [MGRL](https://arxiv.org/abs/1805.09801). TorchOpt offers both
+functional and object-oriented API for EG to fit different user applications.
+#### Functional API  The functional API is to conduct optimization in a
+functional programming style. Note that we pass the argument `inplace=False` to
+the functions to make the optimization differentiable. Refer to the tutorial
+notebook [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb) for
+more guidance. ```python # Define functional optimizer optimizer =
+torchopt.adam() # Define meta and inner parameters meta_params = ... fmodel,
+params = make_functional(model) # Initial state state = optimizer.init(params)
+for iter in range(iter_times): loss = inner_loss(fmodel, params, meta_params)
+grads = torch.autograd.grad(loss, params) # Apply non-inplace parameter update
+updates, state = optimizer.update(grads, state, inplace=False) params =
 torchopt.apply_updates(params, updates) loss = outer_loss(fmodel, params,
 meta_params) meta_grads = torch.autograd.grad(loss, meta_params) ``` #### OOP
-API  TorchOpt also provides OOP API compatible with PyTorch programming style.
-Refer to the example and the tutorial notebook [Meta-Optimizer](tutorials/
-3_Meta_Optimizer.ipynb), [Stop Gradient](tutorials/4_Stop_Gradient.ipynb) for
-more guidances. ```python # Define meta and inner parameters meta_params = ...
-model = ... # Define differentiable optimizer optimizer = torchopt.MetaAdam
-(model) # a model instance as the argument instead of model.parameters() for
-iter in range(iter_times): # Perform inner update loss = inner_loss(model,
-meta_params) optimizer.step(loss) loss = outer_loss(model, meta_params)
-loss.backward() ``` ### Implicit Gradient (IG) By treating the solution
-$\theta^{\prime}$ as an implicit function of $\phi$, the idea of IG is to
-directly get analytical best-response derivatives $\partial \theta^{\prime}
-(\phi) / \partial \phi$ by [implicit function theorem](https://
+API  TorchOpt also provides OOP API compatible with the PyTorch programming
+style. Refer to the example and the tutorial notebook [Meta-Optimizer]
+(tutorials/3_Meta_Optimizer.ipynb), [Stop Gradient](tutorials/
+4_Stop_Gradient.ipynb) for more guidance. ```python # Define meta and inner
+parameters meta_params = ... model = ... # Define differentiable optimizer
+optimizer = torchopt.MetaAdam(model) # a model instance as the argument instead
+of model.parameters() for iter in range(iter_times): # Perform inner update
+loss = inner_loss(model, meta_params) optimizer.step(loss) loss = outer_loss
+(model, meta_params) loss.backward() ``` ### Implicit Gradient (IG) By treating
+the solution $\theta^{\prime}$ as an implicit function of $\phi$, the idea of
+IG is to directly get analytical best-response derivatives $\partial \theta^
+{\prime} (\phi) / \partial \phi$ by [implicit function theorem](https://
 en.wikipedia.org/wiki/Implicit_function_theorem). This is suitable for
 algorithms when the inner-level optimal solution is achieved ${\left. \frac
 {\partial F (\theta, \phi)}{\partial \theta} \right\rvert}_{\theta=\theta^
 {\prime}} = 0$ or reaches some stationary conditions $F (\theta^{\prime}, \phi)
 = 0$, such as [iMAML](https://arxiv.org/abs/1909.04630) and [DEQ](https://
 arxiv.org/abs/1909.01377). TorchOpt offers both functional and OOP APIs for
 supporting both [conjugate gradient-based](https://arxiv.org/abs/1909.04630)
 and [Neumann series-based](https://arxiv.org/abs/1911.02590) IG methods. Refer
 to the example [iMAML](https://github.com/waterhorse1/torchopt/tree/readme/
 examples/iMAML) and the notebook [Implicit Gradient](tutorials/
 5_Implicit_Differentiation.ipynb) for more guidance. #### Functional API  For
-implicit gradient, users need to define the stationary condition and TorchOpt
-provides the decorator to wrap the solve function for enabling implicit
-gradient computation. ```python # The stationary condition for the inner-loop
-def stationary(params, meta_params, data): # Stationary condition construction
-return stationary condition # Decorator for wrapping the function # Optionally
-specify the linear solver (conjugate gradient or Neumann series)
+the implicit gradient, users need to define the stationary condition and
+TorchOpt provides the decorator to wrap the solve function for enabling
+implicit gradient computation. ```python # The stationary condition for the
+inner-loop def stationary(params, meta_params, data): # Stationary condition
+construction return stationary condition # Decorator for wrapping the function
+# Optionally specify the linear solver (conjugate gradient or Neumann series)
 @torchopt.diff.implicit.custom_root(stationary, solve=linear_solver) def solve
 (params, meta_params, data): # Forward optimization process for params return
 output # Define params, meta_params and get data params, meta_prams, data =
 ..., ..., ... optimal_params = solve(params, meta_params, data) loss =
 outer_loss(optimal_params) meta_grads = torch.autograd.grad(loss, meta_params)
-``` #### OOP API  TorchOpt also offer an OOP API, users need to inherit from
-the class `torchopt.nn.ImplicitMetaGradientModule` to construct the inner-loop
-network. Users need to define the stationary condition/objective function and
-the inner-loop solve function to enable implicit gradient computation.
+``` #### OOP API  TorchOpt also offers an OOP API, which users need to inherit
+from the class `torchopt.nn.ImplicitMetaGradientModule` to construct the inner-
+loop network. Users need to define the stationary condition/objective function
+and the inner-loop solve function to enable implicit gradient computation.
 ```python # Inherited from the class ImplicitMetaGradientModule # Optionally
 specify the linear solver (conjugate gradient or Neumann series) class InnerNet
 (ImplicitMetaGradientModule, linear_solve=linear_solver): def __init__(self,
 meta_param): super().__init__() self.meta_param = meta_param ... def forward
 (self, batch): # Forward process ... def optimality(self, batch, labels): #
 Stationary condition construction for calculating implicit gradient # NOTE: If
 this method is not implemented, it will be automatically # derived from the
@@ -194,28 +193,28 @@
 process is non-differentiable or one wants to eliminate the heavy computation
 burdens in the previous two modes (brought by Hessian), one can choose Zero-
 order Differentiation (ZD). ZD typically gets gradients based on zero-order
 estimation, such as finite-difference, or [Evolutionary Strategy](https://
 arxiv.org/abs/1703.03864). Instead of optimizing the objective $F$, ES
 optimizes a smoothed objective. TorchOpt provides both functional and OOP APIs
 for the ES method. Refer to the tutorial notebook [Zero-order Differentiation]
-(tutorials/6_Zero_Order_Differentiation.ipynb) for more guidances. ####
+(tutorials/6_Zero_Order_Differentiation.ipynb) for more guidance. ####
 Functional API  For zero-order differentiation, users need to define the
 forward pass calculation and the noise sampling procedure. TorchOpt provides
 the decorator to wrap the forward function for enabling zero-order
 differentiation. ```python # Customize the noise sampling function in ES def
 distribution(sample_shape): # Generate a batch of noise samples # NOTE: The
 distribution should be spherical symmetric and with a constant variance of 1.
 ... return noise_batch # Distribution can also be an instance of
 `torch.distributions.Distribution`, e.g., `torch.distributions.Normal(...)`
 distribution = torch.distributions.Normal(loc=0, scale=1) # Specify method and
 hyper-parameter of ES @torchopt.diff.zero_order(distribution, method) def
 forward(params, batch, labels): # Forward process ... return objective # the
-returned tensor should be a scalar tensor ``` #### OOP API  TorchOpt also offer
-an OOP API, users need to inherit from the class
+returned tensor should be a scalar tensor ``` #### OOP API  TorchOpt also
+offers an OOP API, which users need to inherit from the class
 `torchopt.nn.ZeroOrderGradientModule` to construct the network as an
 `nn.Module` following a classical PyTorch style. Users need to define the
 forward process zero-order gradient procedures `forward()` and a noise sampling
 function `sample()`. ```python # Inherited from the class
 ZeroOrderGradientModule # Optionally specify the `method` and/or `num_samples`
 and/or `sigma` used for sampling class Net(ZeroOrderGradientModule,
 method=method, num_samples=num_samples, sigma=sigma): def __init__(self, ...):
@@ -231,60 +230,61 @@
 the optimizer as a whole instead of separating it into several basic operators
 (e.g., `sqrt` and `div`). Therefore, by manually writing the forward and
 backward functions, we can perform the symbolic reduction. In addition, we can
 store some intermediate data that can be reused during the backpropagation. We
 write the accelerated functions in C++ OpenMP and CUDA, bind them by
 [`pybind11`](https://github.com/pybind/pybind11) to allow they can be called by
 Python, and then define the forward and backward behavior using
-`torch.autograd.Function`. Users can use by simply setting the
-`use_accelerated_op` flag as `True`. Refer to the corresponding sections in
-tutorials [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb) and
-[Meta-Optimizer](tutorials/3_Meta_Optimizer.ipynb) ```python optimizer =
-torchopt.MetaAdam(model, lr, use_accelerated_op=True) ``` ### Distributed
-Training `TorchOpt` provides distributed training features based on the PyTorch
-RPC module for better training speed and multi-node multi-GPU support.
-Different from the MPI-like parallelization paradigm, which uses multiple
-homogenous workers and requires carefully designed communication hooks, the RPC
-APIs allow users to build their optimization pipeline more flexibly.
-Experimental results show that we achieve an approximately linear relationship
-between the speed-up ratio and the number of workers. Check out the
-[Distributed Training Documentation](https://torchopt.readthedocs.io/en/latest/
-distributed/distributed.html) and [distributed MAML example](https://
-github.com/metaopt/torchopt/tree/main/examples/distributed/few-shot) for more
-specific guidance. ### OpTree We implement the *PyTree* to enable fast nested
-structure flattening using C++. The tree operations (e.g., flatten and
-unflatten) are very important in enabling functional and Just-In-Time (JIT)
-features of deep learning frameworks. By implementing it in C++, we can use
-some cache/memory-friendly structures (e.g., `absl::InlinedVector`) to improve
-the performance. For more guidance and comparison results, please refer to our
-open-source project [`OpTree`](https://github.com/metaopt/optree). ------------
--------------------------------------------------------------------- ##
-Visualization Complex gradient flow in meta-learning brings in a great
-challenge for managing the gradient flow and verifying the correctness of it.
-TorchOpt provides a visualization tool that draws variable (e.g., network
-parameters or meta-parameters) names on the gradient graph for better analysis.
-The visualization tool is modified from [`torchviz`](https://github.com/
-szagoruyko/pytorchviz). Refer to the example [visualization code](examples/
-visualize.py) and the tutorial notebook [Visualization](tutorials/
-2_Visualization.ipynb) for more details. The figure below show the
-visualization result. Compared with [`torchviz`](https://github.com/szagoruyko/
-pytorchviz), TorchOpt fuses the operations within the `Adam` together (orange)
-to reduce the complexity and provide simpler visualization.
+`torch.autograd.Function`. Users can use it by simply setting the
+`use_accelerated_op` flag as `True`. Refer to the corresponding sections in the
+tutorials [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb)]
+(tutorials/1_Functional_Optimizer.ipynb) and [Meta-Optimizer](tutorials/
+3_Meta_Optimizer.ipynb) ```python optimizer = torchopt.MetaAdam(model, lr,
+use_accelerated_op=True) ``` ### Distributed Training `TorchOpt` provides
+distributed training features based on the PyTorch RPC module for better
+training speed and multi-node multi-GPU support. Different from the MPI-like
+parallelization paradigm, which uses multiple homogeneous workers and requires
+carefully designed communication hooks, the RPC APIs allow users to build their
+optimization pipeline more flexibly. Experimental results show that we achieve
+an approximately linear relationship between the speed-up ratio and the number
+of workers. Check out the [Distributed Training Documentation](https://
+torchopt.readthedocs.io/en/latest/distributed/distributed.html) and
+[distributed MAML example](https://github.com/metaopt/torchopt/tree/main/
+examples/distributed/few-shot) for more specific guidance. ### OpTree We
+implement the *PyTree* to enable fast nested structure flattening using C++.
+The tree operations (e.g., flatten and unflatten) are very important in
+enabling functional and Just-In-Time (JIT) features of deep learning
+frameworks. By implementing it in C++, we can use some cache/memory-friendly
+structures (e.g., `absl::InlinedVector`) to improve the performance. For more
+guidance and comparison results, please refer to our open-source project
+[`OpTree`](https://github.com/metaopt/optree). --------------------------------
+------------------------------------------------ ## Visualization Complex
+gradient flow in meta-learning brings in a great challenge for managing the
+gradient flow and verifying its correctness of it. TorchOpt provides a
+visualization tool that draws variable (e.g., network parameters or meta-
+parameters) names on the gradient graph for better analysis. The visualization
+tool is modified from [`torchviz`](https://github.com/szagoruyko/pytorchviz).
+Refer to the example [visualization code](examples/visualize.py) and the
+tutorial notebook [Visualization](tutorials/2_Visualization.ipynb) for more
+details. The figure below shows the visualization result. Compared with
+[`torchviz`](https://github.com/szagoruyko/pytorchviz), TorchOpt fuses the
+operations within the `Adam` together (orange) to reduce the complexity and
+provide simpler visualization.
  [https://github.com/metaopt/torchopt/raw/HEAD/image/torchviz-vs-torchopt.jpg]
 -------------------------------------------------------------------------------
 - ## Examples In the [`examples`](examples) directory, we offer several
-examples of functional optimizers and light-weight meta-learning examples with
+examples of functional optimizers and lightweight meta-learning examples with
 TorchOpt. - [Model-Agnostic Meta-Learning (MAML) - Supervised Learning](https:/
 /arxiv.org/abs/1703.03400) (ICML 2017) - [Learning to Reweight Examples for
 Robust Deep Learning](https://arxiv.org/abs/1803.09050) (ICML 2018) - [Model-
 Agnostic Meta-Learning (MAML) - Reinforcement Learning](https://arxiv.org/abs/
 1703.03400) (ICML 2017) - [Meta-Gradient Reinforcement Learning (MGRL)](https:/
 /arxiv.org/abs/1805.09801) (NeurIPS 2018) - [Learning through opponent learning
 process (LOLA)](https://arxiv.org/abs/1709.04326) (AAMAS 2018) - [Meta-Learning
-with Implicit Gradients](https://arxiv.org/abs/1909.04630) (NeurIPS 2019) Also
+with Implicit Gradients](https://arxiv.org/abs/1909.04630) (NeurIPS 2019) Also,
 check [`examples`](examples) for more distributed/visualization/functorch-
 compatible examples. ----------------------------------------------------------
 ---------------------- ## Installation Requirements - PyTorch - (Optional) For
 visualizing computation graphs - [Graphviz](https://graphviz.org/download) (for
 Linux users use `apt/yum install graphviz` or `conda install -c anaconda
 python-graphviz`) **Please follow the instructions at
 pytorch.org> to install PyTorch in your Python environment first.** Then run
```

### Comparing `torchopt-0.7.0/README.md` & `torchopt-0.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 <div align="center">
   <img src="https://github.com/metaopt/torchopt/raw/HEAD/image/logo-large.png" width="75%" />
 </div>
 
 <div align="center">
 
-  <a>![Python 3.7+](https://img.shields.io/badge/Python-3.7%2B-brightgreen.svg)</a>
+  <a>![Python 3.8+](https://img.shields.io/badge/Python-3.8%2B-brightgreen.svg)</a>
   <a href="https://pypi.org/project/torchopt">![PyPI](https://img.shields.io/pypi/v/torchopt?logo=pypi)</a>
   <a href="https://github.com/metaopt/torchopt/tree/HEAD/tests">![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/metaopt/torchopt/tests.yml?label=tests&logo=github)</a>
-  <a href="https://codecov.io/gh/metaopt/torchopt">![CodeCov](https://img.shields.io/codecov/c/gh/metaopt/torchopt)</a>
+  <a href="https://codecov.io/gh/metaopt/torchopt">![CodeCov](https://img.shields.io/codecov/c/github/metaopt/torchopt/main?logo=codecov)</a>
   <a href="https://torchopt.readthedocs.io">![Documentation Status](https://img.shields.io/readthedocs/torchopt?logo=readthedocs)</a>
   <a href="https://pepy.tech/project/torchopt">![Downloads](https://static.pepy.tech/personalized-badge/torchopt?period=total&left_color=grey&right_color=blue&left_text=downloads)</a>
   <a href="https://github.com/metaopt/torchopt/blob/HEAD/LICENSE">![License](https://img.shields.io/github/license/metaopt/torchopt?label=license&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0IiBmaWxsPSIjZmZmZmZmIj48cGF0aCBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik0xMi43NSAyLjc1YS43NS43NSAwIDAwLTEuNSAwVjQuNUg5LjI3NmExLjc1IDEuNzUgMCAwMC0uOTg1LjMwM0w2LjU5NiA1Ljk1N0EuMjUuMjUgMCAwMTYuNDU1IDZIMi4zNTNhLjc1Ljc1IDAgMTAwIDEuNUgzLjkzTC41NjMgMTUuMThhLjc2Mi43NjIgMCAwMC4yMS44OGMuMDguMDY0LjE2MS4xMjUuMzA5LjIyMS4xODYuMTIxLjQ1Mi4yNzguNzkyLjQzMy42OC4zMTEgMS42NjIuNjIgMi44NzYuNjJhNi45MTkgNi45MTkgMCAwMDIuODc2LS42MmMuMzQtLjE1NS42MDYtLjMxMi43OTItLjQzMy4xNS0uMDk3LjIzLS4xNTguMzEtLjIyM2EuNzUuNzUgMCAwMC4yMDktLjg3OEw1LjU2OSA3LjVoLjg4NmMuMzUxIDAgLjY5NC0uMTA2Ljk4NC0uMzAzbDEuNjk2LTEuMTU0QS4yNS4yNSAwIDAxOS4yNzUgNmgxLjk3NXYxNC41SDYuNzYzYS43NS43NSAwIDAwMCAxLjVoMTAuNDc0YS43NS43NSAwIDAwMC0xLjVIMTIuNzVWNmgxLjk3NGMuMDUgMCAuMS4wMTUuMTQuMDQzbDEuNjk3IDEuMTU0Yy4yOS4xOTcuNjMzLjMwMy45ODQuMzAzaC44ODZsLTMuMzY4IDcuNjhhLjc1Ljc1IDAgMDAuMjMuODk2Yy4wMTIuMDA5IDAgMCAuMDAyIDBhMy4xNTQgMy4xNTQgMCAwMC4zMS4yMDZjLjE4NS4xMTIuNDUuMjU2Ljc5LjRhNy4zNDMgNy4zNDMgMCAwMDIuODU1LjU2OCA3LjM0MyA3LjM0MyAwIDAwMi44NTYtLjU2OWMuMzM4LS4xNDMuNjA0LS4yODcuNzktLjM5OWEzLjUgMy41IDAgMDAuMzEtLjIwNi43NS43NSAwIDAwLjIzLS44OTZMMjAuMDcgNy41aDEuNTc4YS43NS43NSAwIDAwMC0xLjVoLTQuMTAyYS4yNS4yNSAwIDAxLS4xNC0uMDQzbC0xLjY5Ny0xLjE1NGExLjc1IDEuNzUgMCAwMC0uOTg0LS4zMDNIMTIuNzVWMi43NXpNMi4xOTMgMTUuMTk4YTUuNDE4IDUuNDE4IDAgMDAyLjU1Ny42MzUgNS40MTggNS40MTggMCAwMDIuNTU3LS42MzVMNC43NSA5LjM2OGwtMi41NTcgNS44M3ptMTQuNTEtLjAyNGMuMDgyLjA0LjE3NC4wODMuMjc1LjEyNi41My4yMjMgMS4zMDUuNDUgMi4yNzIuNDVhNS44NDYgNS44NDYgMCAwMDIuNTQ3LS41NzZMMTkuMjUgOS4zNjdsLTIuNTQ3IDUuODA3eiI+PC9wYXRoPjwvc3ZnPgo=)</a>
 </div>
 
 <p align="center">
   <a href="https://github.com/metaopt/torchopt#installation">Installation</a> |
@@ -30,15 +30,15 @@
 TorchOpt is:
 
 - **Comprehensive**: TorchOpt provides three differentiation modes - explicit differentiation, implicit differentiation, and zero-order differentiation for handling different differentiable optimization situations.
 - **Flexible**: TorchOpt provides both functional and objective-oriented API for users' different preferences. Users can implement differentiable optimization in JAX-like or PyTorch-like style.
 - **Efficient**: TorchOpt provides (1) CPU/GPU acceleration differentiable optimizer (2) RPC-based distributed training framework (3) Fast Tree Operations, to largely increase the training efficiency for bi-level optimization problems.
 
 Beyond differentiable optimization, TorchOpt can also be regarded as a functional optimizer that enables [JAX-like](https://github.com/google/jax) composable functional optimizer for PyTorch.
-With TorchOpt, users can easily conduct neural network optimization in PyTorch with functional style optimizer, similar to [Optax](https://github.com/deepmind/optax) in JAX.
+With TorchOpt, users can easily conduct neural network optimization in PyTorch with a functional style optimizer, similar to [Optax](https://github.com/deepmind/optax) in JAX.
 
 --------------------------------------------------------------------------------
 
 The README is organized as follows:
 
 - [TorchOpt as Functional Optimizer](#torchopt-as-functional-optimizer)
   - [Optax-Like API](#optax-like-api)
@@ -128,19 +128,19 @@
 optimizer.zero_grad()             # zero gradients
 loss.backward()                   # backward
 optimizer.step()                  # step updates
 ```
 
 ### Differentiable
 
-On top of the same optimization function as `torch.optim`, an important benefit of functional optimizer is that one can implement differentiable optimization easily.
-This is particularly helpful when the algorithm requires to differentiate through optimization updates (such as meta-learning practices).
+On top of the same optimization function as `torch.optim`, an important benefit of the functional optimizer is that one can implement differentiable optimization easily.
+This is particularly helpful when the algorithm requires differentiation through optimization updates (such as meta-learning practices).
 We take as the inputs the gradients and optimizer states, and use non-in-place operators to compute and output the updates.
 The processes can be automatically implemented, with the only need from users being to pass the argument `inplace=False` to the functions.
-Check out section [Explicit Gradient (EG)](#explicit-gradient-eg) functional API for example.
+Check out the section [Explicit Gradient](#explicit-gradient-eg) (EG)](#explicit-gradient-eg) functional API for example.
 
 --------------------------------------------------------------------------------
 
 ## TorchOpt for Differentiable Optimization
 
 We design a bilevel-optimization updating scheme, which can be easily extended to realize various differentiable optimization processes.
 
@@ -151,23 +151,23 @@
 As shown above, the scheme contains an outer level that has parameters $\phi$ that can be learned end-to-end through the inner level parameters solution $\theta^{\prime}(\phi)$ by using the best-response derivatives $\partial \theta^{\prime}(\phi) / \partial \phi$.
 TorchOpt supports three differentiation modes.
 It can be seen that the key component of this algorithm is to calculate the best-response (BR) Jacobian.
 From the BR-based perspective, existing gradient methods can be categorized into three groups: explicit gradient over unrolled optimization, implicit differentiation, and zero-order gradient differentiation.
 
 ### Explicit Gradient (EG)
 
-The idea of explicit gradient is to treat the gradient step as a differentiable function and try to backpropagate through the unrolled optimization path.
+The idea of the explicit gradient is to treat the gradient step as a differentiable function and try to backpropagate through the unrolled optimization path.
 This differentiation mode is suitable for algorithms when the inner-level optimization solution is obtained by a few gradient steps, such as [MAML](https://arxiv.org/abs/1703.03400) and [MGRL](https://arxiv.org/abs/1805.09801).
 TorchOpt offers both functional and object-oriented API for EG to fit different user applications.
 
 #### Functional API  <!-- omit in toc -->
 
 The functional API is to conduct optimization in a functional programming style.
 Note that we pass the argument `inplace=False` to the functions to make the optimization differentiable.
-Refer to the tutorial notebook [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb) for more guidances.
+Refer to the tutorial notebook [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb) for more guidance.
 
 ```python
 # Define functional optimizer
 optimizer = torchopt.adam()
 # Define meta and inner parameters
 meta_params = ...
 fmodel, params = make_functional(model)
@@ -183,16 +183,16 @@
 
 loss = outer_loss(fmodel, params, meta_params)
 meta_grads = torch.autograd.grad(loss, meta_params)
 ```
 
 #### OOP API  <!-- omit in toc -->
 
-TorchOpt also provides OOP API compatible with PyTorch programming style.
-Refer to the example and the tutorial notebook [Meta-Optimizer](tutorials/3_Meta_Optimizer.ipynb), [Stop Gradient](tutorials/4_Stop_Gradient.ipynb) for more guidances.
+TorchOpt also provides OOP API compatible with the PyTorch programming style.
+Refer to the example and the tutorial notebook [Meta-Optimizer](tutorials/3_Meta_Optimizer.ipynb), [Stop Gradient](tutorials/4_Stop_Gradient.ipynb) for more guidance.
 
 ```python
 # Define meta and inner parameters
 meta_params = ...
 model = ...
 # Define differentiable optimizer
 optimizer = torchopt.MetaAdam(model)  # a model instance as the argument instead of model.parameters()
@@ -211,15 +211,15 @@
 By treating the solution $\theta^{\prime}$ as an implicit function of $\phi$, the idea of IG is to directly get analytical best-response derivatives $\partial \theta^{\prime} (\phi) / \partial \phi$ by [implicit function theorem](https://en.wikipedia.org/wiki/Implicit_function_theorem).
 This is suitable for algorithms when the inner-level optimal solution is achieved ${\left. \frac{\partial F (\theta, \phi)}{\partial \theta} \right\rvert}_{\theta=\theta^{\prime}} = 0$ or reaches some stationary conditions $F (\theta^{\prime}, \phi) = 0$, such as [iMAML](https://arxiv.org/abs/1909.04630) and [DEQ](https://arxiv.org/abs/1909.01377).
 TorchOpt offers both functional and OOP APIs for supporting both [conjugate gradient-based](https://arxiv.org/abs/1909.04630) and [Neumann series-based](https://arxiv.org/abs/1911.02590) IG methods.
 Refer to the example [iMAML](https://github.com/waterhorse1/torchopt/tree/readme/examples/iMAML) and the notebook [Implicit Gradient](tutorials/5_Implicit_Differentiation.ipynb) for more guidance.
 
 #### Functional API  <!-- omit in toc -->
 
-For implicit gradient, users need to define the stationary condition and TorchOpt provides the decorator to wrap the solve function for enabling implicit gradient computation.
+For the implicit gradient, users need to define the stationary condition and TorchOpt provides the decorator to wrap the solve function for enabling implicit gradient computation.
 
 ```python
 # The stationary condition for the inner-loop
 def stationary(params, meta_params, data):
     # Stationary condition construction
     return stationary condition
 
@@ -236,15 +236,15 @@
 loss = outer_loss(optimal_params)
 
 meta_grads = torch.autograd.grad(loss, meta_params)
 ```
 
 #### OOP API  <!-- omit in toc -->
 
-TorchOpt also offer an OOP API, users need to inherit from the class `torchopt.nn.ImplicitMetaGradientModule` to construct the inner-loop network.
+TorchOpt also offers an OOP API, which users need to inherit from the class `torchopt.nn.ImplicitMetaGradientModule` to construct the inner-loop network.
 Users need to define the stationary condition/objective function and the inner-loop solve function to enable implicit gradient computation.
 
 ```python
 # Inherited from the class ImplicitMetaGradientModule
 # Optionally specify the linear solver (conjugate gradient or Neumann series)
 class InnerNet(ImplicitMetaGradientModule, linear_solve=linear_solver):
     def __init__(self, meta_param):
@@ -284,15 +284,15 @@
 
 ### Zero-order Differentiation (ZD)
 
 When the inner-loop process is non-differentiable or one wants to eliminate the heavy computation burdens in the previous two modes (brought by Hessian), one can choose Zero-order Differentiation (ZD).
 ZD typically gets gradients based on zero-order estimation, such as finite-difference, or [Evolutionary Strategy](https://arxiv.org/abs/1703.03864).
 Instead of optimizing the objective $F$, ES optimizes a smoothed objective.
 TorchOpt provides both functional and OOP APIs for the ES method.
-Refer to the tutorial notebook [Zero-order Differentiation](tutorials/6_Zero_Order_Differentiation.ipynb) for more guidances.
+Refer to the tutorial notebook [Zero-order Differentiation](tutorials/6_Zero_Order_Differentiation.ipynb) for more guidance.
 
 #### Functional API  <!-- omit in toc -->
 
 For zero-order differentiation, users need to define the forward pass calculation and the noise sampling procedure. TorchOpt provides the decorator to wrap the forward function for enabling zero-order differentiation.
 
 ```python
 # Customize the noise sampling function in ES
@@ -311,15 +311,15 @@
     # Forward process
     ...
     return objective  # the returned tensor should be a scalar tensor
 ```
 
 #### OOP API  <!-- omit in toc -->
 
-TorchOpt also offer an OOP API, users need to inherit from the class `torchopt.nn.ZeroOrderGradientModule` to construct the network as an `nn.Module` following a classical PyTorch style.
+TorchOpt also offers an OOP API, which users need to inherit from the class `torchopt.nn.ZeroOrderGradientModule` to construct the network as an `nn.Module` following a classical PyTorch style.
 Users need to define the forward process zero-order gradient procedures `forward()` and a noise sampling function `sample()`.
 
 ```python
 # Inherited from the class ZeroOrderGradientModule
 # Optionally specify the `method` and/or `num_samples` and/or `sigma` used for sampling
 class Net(ZeroOrderGradientModule, method=method, num_samples=num_samples, sigma=sigma):
     def __init__(self, ...):
@@ -352,65 +352,65 @@
 
 ### CPU/GPU accelerated differentiable optimizer
 
 We take the optimizer as a whole instead of separating it into several basic operators (e.g., `sqrt` and `div`).
 Therefore, by manually writing the forward and backward functions, we can perform the symbolic reduction.
 In addition, we can store some intermediate data that can be reused during the backpropagation.
 We write the accelerated functions in C++ OpenMP and CUDA, bind them by [`pybind11`](https://github.com/pybind/pybind11) to allow they can be called by Python, and then define the forward and backward behavior using `torch.autograd.Function`.
-Users can use by simply setting the `use_accelerated_op` flag as `True`.
-Refer to the corresponding sections in tutorials [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb) and [Meta-Optimizer](tutorials/3_Meta_Optimizer.ipynb)
+Users can use it by simply setting the `use_accelerated_op` flag as `True`.
+Refer to the corresponding sections in the tutorials [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb)](tutorials/1_Functional_Optimizer.ipynb) and [Meta-Optimizer](tutorials/3_Meta_Optimizer.ipynb)
 
 ```python
 optimizer = torchopt.MetaAdam(model, lr, use_accelerated_op=True)
 ```
 
 ### Distributed Training
 
 `TorchOpt` provides distributed training features based on the PyTorch RPC module for better training speed and multi-node multi-GPU support.
-Different from the MPI-like parallelization paradigm, which uses multiple homogenous workers and requires carefully designed communication hooks, the RPC APIs allow users to build their optimization pipeline more flexibly.
+Different from the MPI-like parallelization paradigm, which uses multiple homogeneous workers and requires carefully designed communication hooks, the RPC APIs allow users to build their optimization pipeline more flexibly.
 Experimental results show that we achieve an approximately linear relationship between the speed-up ratio and the number of workers.
 Check out the [Distributed Training Documentation](https://torchopt.readthedocs.io/en/latest/distributed/distributed.html) and [distributed MAML example](https://github.com/metaopt/torchopt/tree/main/examples/distributed/few-shot) for more specific guidance.
 
 ### OpTree
 
 We implement the *PyTree* to enable fast nested structure flattening using C++.
 The tree operations (e.g., flatten and unflatten) are very important in enabling functional and Just-In-Time (JIT) features of deep learning frameworks.
 By implementing it in C++, we can use some cache/memory-friendly structures (e.g., `absl::InlinedVector`) to improve the performance.
 For more guidance and comparison results, please refer to our open-source project [`OpTree`](https://github.com/metaopt/optree).
 
 --------------------------------------------------------------------------------
 
 ## Visualization
 
-Complex gradient flow in meta-learning brings in a great challenge for managing the gradient flow and verifying the correctness of it.
+Complex gradient flow in meta-learning brings in a great challenge for managing the gradient flow and verifying its correctness of it.
 TorchOpt provides a visualization tool that draws variable (e.g., network parameters or meta-parameters) names on the gradient graph for better analysis.
 The visualization tool is modified from [`torchviz`](https://github.com/szagoruyko/pytorchviz).
 Refer to the example [visualization code](examples/visualize.py) and the tutorial notebook [Visualization](tutorials/2_Visualization.ipynb) for more details.
 
-The figure below show the visualization result.
+The figure below shows the visualization result.
 Compared with [`torchviz`](https://github.com/szagoruyko/pytorchviz), TorchOpt fuses the operations within the `Adam` together (orange) to reduce the complexity and provide simpler visualization.
 
 <div align="center">
   <img src="https://github.com/metaopt/torchopt/raw/HEAD/image/torchviz-vs-torchopt.jpg" width="80%" />
 </div>
 
 --------------------------------------------------------------------------------
 
 ## Examples
 
-In the [`examples`](examples) directory, we offer several examples of functional optimizers and light-weight meta-learning examples with TorchOpt.
+In the [`examples`](examples) directory, we offer several examples of functional optimizers and lightweight meta-learning examples with TorchOpt.
 
 - [Model-Agnostic Meta-Learning (MAML) - Supervised Learning](https://arxiv.org/abs/1703.03400) (ICML 2017)
 - [Learning to Reweight Examples for Robust Deep Learning](https://arxiv.org/abs/1803.09050) (ICML 2018)
 - [Model-Agnostic Meta-Learning (MAML) - Reinforcement Learning](https://arxiv.org/abs/1703.03400) (ICML 2017)
 - [Meta-Gradient Reinforcement Learning (MGRL)](https://arxiv.org/abs/1805.09801) (NeurIPS 2018)
 - [Learning through opponent learning process (LOLA)](https://arxiv.org/abs/1709.04326) (AAMAS 2018)
 - [Meta-Learning with Implicit Gradients](https://arxiv.org/abs/1909.04630) (NeurIPS 2019)
 
-Also check [`examples`](examples) for more distributed/visualization/functorch-compatible examples.
+Also, check [`examples`](examples) for more distributed/visualization/functorch-compatible examples.
 
 --------------------------------------------------------------------------------
 
 ## Installation
 
 Requirements
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 
       [https://github.com/metaopt/torchopt/raw/HEAD/image/logo-large.png]
- ![Python 3.7+](https://img.shields.io/badge/Python-3.7%2B-brightgreen.svg) !
+ ![Python 3.8+](https://img.shields.io/badge/Python-3.8%2B-brightgreen.svg) !
   [PyPI](https://img.shields.io/pypi/v/torchopt?logo=pypi) ![GitHub_Workflow
 Status](https://img.shields.io/github/actions/workflow/status/metaopt/torchopt/
 tests.yml?label=tests&logo=github) ![CodeCov](https://img.shields.io/codecov/c/
-     gh/metaopt/torchopt) ![Documentation_Status](https://img.shields.io/
- readthedocs/torchopt?logo=readthedocs) ![Downloads](https://static.pepy.tech/
-                              personalized-badge/
+  github/metaopt/torchopt/main?logo=codecov) ![Documentation_Status](https://
+  img.shields.io/readthedocs/torchopt?logo=readthedocs) ![Downloads](https://
+                     static.pepy.tech/personalized-badge/
  torchopt?period=total&left_color=grey&right_color=blue&left_text=downloads) !
            [License](https://img.shields.io/github/license/metaopt/
                     torchopt?label=license&logo=data:image/
 svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0IiBmaWxsPSIjZmZmZmZmIj48cGF0aCBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik0xMi43NSAyLjc1YS43NS43NSAwIDAwLTEuNSAwVjQuNUg5LjI3NmExLjc1IDEuNzUgMCAwMC0uOTg1LjMwM0w2LjU5NiA1Ljk1N0EuMjUuMjUgMCAwMTYuNDU1IDZIMi4zNTNhLjc1Ljc1IDAgMTAwIDEuNUgzLjkzTC41NjMgMTUuMThhLjc2Mi43NjIgMCAwMC4yMS44OGMuMDguMDY0LjE2MS4xMjUuMzA5LjIyMS4xODYuMTIxLjQ1Mi4yNzguNzkyLjQzMy42OC4zMTEgMS42NjIuNjIgMi44NzYuNjJhNi45MTkgNi45MTkgMCAwMDIuODc2LS42MmMuMzQtLjE1NS42MDYtLjMxMi43OTItLjQzMy4xNS0uMDk3LjIzLS4xNTguMzEtLjIyM2EuNzUuNzUgMCAwMC4yMDktLjg3OEw1LjU2OSA3LjVoLjg4NmMuMzUxIDAgLjY5NC0uMTA2Ljk4NC0uMzAzbDEuNjk2LTEuMTU0QS4yNS4yNSAwIDAxOS4yNzUgNmgxLjk3NXYxNC41SDYuNzYzYS43NS43NSAwIDAwMCAxLjVoMTAuNDc0YS43NS43NSAwIDAwMC0xLjVIMTIuNzVWNmgxLjk3NGMuMDUgMCAuMS4wMTUuMTQuMDQzbDEuNjk3IDEuMTU0Yy4yOS4xOTcuNjMzLjMwMy45ODQuMzAzaC44ODZsLTMuMzY4IDcuNjhhLjc1Ljc1IDAgMDAuMjMuODk2Yy4wMTIuMDA5IDAgMCAuMDAyIDBhMy4xNTQgMy4xNTQgMCAwMC4zMS4yMDZjLjE4NS4xMTIuNDUuMjU2Ljc5LjRhNy4zNDMgNy4zNDMgMCAwMDIuODU1LjU2OCA3LjM0MyA3LjM0MyAwIDAwMi44NTYtLjU2OWMuMzM4LS4xNDMuNjA0LS4yODcuNzktLjM5OWEzLjUgMy41IDAgMDAuMzEtLjIwNi43NS43NSAwIDAwLjIzLS44OTZMMjAuMDcgNy41aDEuNTc4YS43NS43NSAwIDAwMC0xLjVoLTQuMTAyYS4yNS4yNSAwIDAxLS4xNC0uMDQzbC0xLjY5Ny0xLjE1NGExLjc1IDEuNzUgMCAwMC0uOTg0LS4zMDNIMTIuNzVWMi43NXpNMi4xOTMgMTUuMTk4YTUuNDE4IDUuNDE4IDAgMDAyLjU1Ny42MzUgNS40MTggNS40MTggMCAwMDIuNTU3LS42MzVMNC43NSA5LjM2OGwtMi41NTcgNS44M3ptMTQuNTEtLjAyNGMuMDgyLjA0LjE3NC4wODMuMjc1LjEyNi41My4yMjMgMS4zMDUuNDUgMi4yNzIuNDVhNS44NDYgNS44NDYgMCAwMDIuNTQ3LS41NzZMMTkuMjUgOS4zNjdsLTIuNTQ3IDUuODA3eiI+PC9wYXRoPjwvc3ZnPgo=)
     Installation | Documentation | Tutorials | Examples | Paper | Citation
 **TorchOpt** is an efficient library for differentiable optimization built upon
 [PyTorch](https://pytorch.org). TorchOpt is: - **Comprehensive**: TorchOpt
@@ -21,141 +21,141 @@
 can implement differentiable optimization in JAX-like or PyTorch-like style. -
 **Efficient**: TorchOpt provides (1) CPU/GPU acceleration differentiable
 optimizer (2) RPC-based distributed training framework (3) Fast Tree
 Operations, to largely increase the training efficiency for bi-level
 optimization problems. Beyond differentiable optimization, TorchOpt can also be
 regarded as a functional optimizer that enables [JAX-like](https://github.com/
 google/jax) composable functional optimizer for PyTorch. With TorchOpt, users
-can easily conduct neural network optimization in PyTorch with functional style
-optimizer, similar to [Optax](https://github.com/deepmind/optax) in JAX. ------
--------------------------------------------------------------------------- The
-README is organized as follows: - [TorchOpt as Functional Optimizer](#torchopt-
-as-functional-optimizer) - [Optax-Like API](#optax-like-api) - [PyTorch-Like
-API](#pytorch-like-api) - [Differentiable](#differentiable) - [TorchOpt for
-Differentiable Optimization](#torchopt-for-differentiable-optimization) -
-[Explicit Gradient (EG)](#explicit-gradient-eg) - [Implicit Gradient (IG)]
-(#implicit-gradient-ig) - [Zero-order Differentiation (ZD)](#zero-order-
-differentiation-zd) - [High-Performance and Distributed Training](#high-
-performance-and-distributed-training) - [CPU/GPU accelerated differentiable
-optimizer](#cpugpu-accelerated-differentiable-optimizer) - [Distributed
-Training](#distributed-training) - [OpTree](#optree) - [Visualization]
-(#visualization) - [Examples](#examples) - [Installation](#installation) -
-[Changelog](#changelog) - [Citing TorchOpt](#citing-torchopt) - [The Team]
-(#the-team) - [License](#license) ---------------------------------------------
------------------------------------ ## TorchOpt as Functional Optimizer The
-design of TorchOpt follows the philosophy of functional programming. Aligned
-with [`functorch`](https://github.com/pytorch/functorch), users can conduct
-functional style programming with models, optimizers and training in PyTorch.
-We use the Adam optimizer as an example in the following illustration. You can
-also check out the tutorial notebook [Functional Optimizer](tutorials/
-1_Functional_Optimizer.ipynb) for more details. ### Optax-Like API For those
-users who prefer fully functional programming, we offer Optax-Like API by
-passing gradients and optimizer states to the optimizer function. Here is an
-example coupled with `functorch`: ```python class Net(nn.Module): ... class
-Loader(DataLoader): ... net = Net() # init loader = Loader() optimizer =
-torchopt.adam() model, params = functorch.make_functional(net) # use functorch
-extract network parameters opt_state = optimizer.init(params) # init optimizer
-xs, ys = next(loader) # get data pred = model(params, xs) # forward loss =
-F.cross_entropy(pred, ys) # compute loss grads = torch.autograd.grad(loss,
-params) # compute gradients updates, opt_state = optimizer.update(grads,
-opt_state) # get updates params = torchopt.apply_updates(params, updates) #
-update network parameters ``` We also provide a wrapper
-`torchopt.FuncOptimizer` to make maintaining the optimizer state easier:
-```python net = Net() # init loader = Loader() optimizer =
+can easily conduct neural network optimization in PyTorch with a functional
+style optimizer, similar to [Optax](https://github.com/deepmind/optax) in JAX.
+-------------------------------------------------------------------------------
+- The README is organized as follows: - [TorchOpt as Functional Optimizer]
+(#torchopt-as-functional-optimizer) - [Optax-Like API](#optax-like-api) -
+[PyTorch-Like API](#pytorch-like-api) - [Differentiable](#differentiable) -
+[TorchOpt for Differentiable Optimization](#torchopt-for-differentiable-
+optimization) - [Explicit Gradient (EG)](#explicit-gradient-eg) - [Implicit
+Gradient (IG)](#implicit-gradient-ig) - [Zero-order Differentiation (ZD)]
+(#zero-order-differentiation-zd) - [High-Performance and Distributed Training]
+(#high-performance-and-distributed-training) - [CPU/GPU accelerated
+differentiable optimizer](#cpugpu-accelerated-differentiable-optimizer) -
+[Distributed Training](#distributed-training) - [OpTree](#optree) -
+[Visualization](#visualization) - [Examples](#examples) - [Installation]
+(#installation) - [Changelog](#changelog) - [Citing TorchOpt](#citing-torchopt)
+- [The Team](#the-team) - [License](#license) ---------------------------------
+----------------------------------------------- ## TorchOpt as Functional
+Optimizer The design of TorchOpt follows the philosophy of functional
+programming. Aligned with [`functorch`](https://github.com/pytorch/functorch),
+users can conduct functional style programming with models, optimizers and
+training in PyTorch. We use the Adam optimizer as an example in the following
+illustration. You can also check out the tutorial notebook [Functional
+Optimizer](tutorials/1_Functional_Optimizer.ipynb) for more details. ### Optax-
+Like API For those users who prefer fully functional programming, we offer
+Optax-Like API by passing gradients and optimizer states to the optimizer
+function. Here is an example coupled with `functorch`: ```python class Net
+(nn.Module): ... class Loader(DataLoader): ... net = Net() # init loader =
+Loader() optimizer = torchopt.adam() model, params = functorch.make_functional
+(net) # use functorch extract network parameters opt_state = optimizer.init
+(params) # init optimizer xs, ys = next(loader) # get data pred = model(params,
+xs) # forward loss = F.cross_entropy(pred, ys) # compute loss grads =
+torch.autograd.grad(loss, params) # compute gradients updates, opt_state =
+optimizer.update(grads, opt_state) # get updates params =
+torchopt.apply_updates(params, updates) # update network parameters ``` We also
+provide a wrapper `torchopt.FuncOptimizer` to make maintaining the optimizer
+state easier: ```python net = Net() # init loader = Loader() optimizer =
 torchopt.FuncOptimizer(torchopt.adam()) # wrap with `torchopt.FuncOptimizer`
 model, params = functorch.make_functional(net) # use functorch extract network
 parameters for xs, ys in loader: # get data pred = model(params, xs) # forward
 loss = F.cross_entropy(pred, ys) # compute loss params = optimizer.step(loss,
 params) # update network parameters ``` ### PyTorch-Like API We also design a
 base class `torchopt.Optimizer` that has the same interface as
 `torch.optim.Optimizer`. We offer origin PyTorch APIs (e.g. `zero_grad()` or
 `step()`) by wrapping our Optax-Like API for traditional PyTorch users.
 ```python net = Net() # init loader = Loader() optimizer = torchopt.Adam
 (net.parameters()) xs, ys = next(loader) # get data pred = net(xs) # forward
 loss = F.cross_entropy(pred, ys) # compute loss optimizer.zero_grad() # zero
 gradients loss.backward() # backward optimizer.step() # step updates ``` ###
 Differentiable On top of the same optimization function as `torch.optim`, an
-important benefit of functional optimizer is that one can implement
+important benefit of the functional optimizer is that one can implement
 differentiable optimization easily. This is particularly helpful when the
-algorithm requires to differentiate through optimization updates (such as meta-
+algorithm requires differentiation through optimization updates (such as meta-
 learning practices). We take as the inputs the gradients and optimizer states,
 and use non-in-place operators to compute and output the updates. The processes
 can be automatically implemented, with the only need from users being to pass
-the argument `inplace=False` to the functions. Check out section [Explicit
-Gradient (EG)](#explicit-gradient-eg) functional API for example. -------------
-------------------------------------------------------------------- ## TorchOpt
-for Differentiable Optimization We design a bilevel-optimization updating
-scheme, which can be easily extended to realize various differentiable
-optimization processes.
+the argument `inplace=False` to the functions. Check out the section [Explicit
+Gradient](#explicit-gradient-eg) (EG)](#explicit-gradient-eg) functional API
+for example. ------------------------------------------------------------------
+-------------- ## TorchOpt for Differentiable Optimization We design a bilevel-
+optimization updating scheme, which can be easily extended to realize various
+differentiable optimization processes.
        [https://github.com/metaopt/torchopt/raw/HEAD/image/diffmode.png]
 As shown above, the scheme contains an outer level that has parameters $\phi$
 that can be learned end-to-end through the inner level parameters solution
 $\theta^{\prime}(\phi)$ by using the best-response derivatives $\partial
 \theta^{\prime}(\phi) / \partial \phi$. TorchOpt supports three differentiation
 modes. It can be seen that the key component of this algorithm is to calculate
 the best-response (BR) Jacobian. From the BR-based perspective, existing
 gradient methods can be categorized into three groups: explicit gradient over
 unrolled optimization, implicit differentiation, and zero-order gradient
-differentiation. ### Explicit Gradient (EG) The idea of explicit gradient is to
-treat the gradient step as a differentiable function and try to backpropagate
-through the unrolled optimization path. This differentiation mode is suitable
-for algorithms when the inner-level optimization solution is obtained by a few
-gradient steps, such as [MAML](https://arxiv.org/abs/1703.03400) and [MGRL]
-(https://arxiv.org/abs/1805.09801). TorchOpt offers both functional and object-
-oriented API for EG to fit different user applications. #### Functional API
-The functional API is to conduct optimization in a functional programming
-style. Note that we pass the argument `inplace=False` to the functions to make
-the optimization differentiable. Refer to the tutorial notebook [Functional
-Optimizer](tutorials/1_Functional_Optimizer.ipynb) for more guidances.
-```python # Define functional optimizer optimizer = torchopt.adam() # Define
-meta and inner parameters meta_params = ... fmodel, params = make_functional
-(model) # Initial state state = optimizer.init(params) for iter in range
-(iter_times): loss = inner_loss(fmodel, params, meta_params) grads =
-torch.autograd.grad(loss, params) # Apply non-inplace parameter update updates,
-state = optimizer.update(grads, state, inplace=False) params =
+differentiation. ### Explicit Gradient (EG) The idea of the explicit gradient
+is to treat the gradient step as a differentiable function and try to
+backpropagate through the unrolled optimization path. This differentiation mode
+is suitable for algorithms when the inner-level optimization solution is
+obtained by a few gradient steps, such as [MAML](https://arxiv.org/abs/
+1703.03400) and [MGRL](https://arxiv.org/abs/1805.09801). TorchOpt offers both
+functional and object-oriented API for EG to fit different user applications.
+#### Functional API  The functional API is to conduct optimization in a
+functional programming style. Note that we pass the argument `inplace=False` to
+the functions to make the optimization differentiable. Refer to the tutorial
+notebook [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb) for
+more guidance. ```python # Define functional optimizer optimizer =
+torchopt.adam() # Define meta and inner parameters meta_params = ... fmodel,
+params = make_functional(model) # Initial state state = optimizer.init(params)
+for iter in range(iter_times): loss = inner_loss(fmodel, params, meta_params)
+grads = torch.autograd.grad(loss, params) # Apply non-inplace parameter update
+updates, state = optimizer.update(grads, state, inplace=False) params =
 torchopt.apply_updates(params, updates) loss = outer_loss(fmodel, params,
 meta_params) meta_grads = torch.autograd.grad(loss, meta_params) ``` #### OOP
-API  TorchOpt also provides OOP API compatible with PyTorch programming style.
-Refer to the example and the tutorial notebook [Meta-Optimizer](tutorials/
-3_Meta_Optimizer.ipynb), [Stop Gradient](tutorials/4_Stop_Gradient.ipynb) for
-more guidances. ```python # Define meta and inner parameters meta_params = ...
-model = ... # Define differentiable optimizer optimizer = torchopt.MetaAdam
-(model) # a model instance as the argument instead of model.parameters() for
-iter in range(iter_times): # Perform inner update loss = inner_loss(model,
-meta_params) optimizer.step(loss) loss = outer_loss(model, meta_params)
-loss.backward() ``` ### Implicit Gradient (IG) By treating the solution
-$\theta^{\prime}$ as an implicit function of $\phi$, the idea of IG is to
-directly get analytical best-response derivatives $\partial \theta^{\prime}
-(\phi) / \partial \phi$ by [implicit function theorem](https://
+API  TorchOpt also provides OOP API compatible with the PyTorch programming
+style. Refer to the example and the tutorial notebook [Meta-Optimizer]
+(tutorials/3_Meta_Optimizer.ipynb), [Stop Gradient](tutorials/
+4_Stop_Gradient.ipynb) for more guidance. ```python # Define meta and inner
+parameters meta_params = ... model = ... # Define differentiable optimizer
+optimizer = torchopt.MetaAdam(model) # a model instance as the argument instead
+of model.parameters() for iter in range(iter_times): # Perform inner update
+loss = inner_loss(model, meta_params) optimizer.step(loss) loss = outer_loss
+(model, meta_params) loss.backward() ``` ### Implicit Gradient (IG) By treating
+the solution $\theta^{\prime}$ as an implicit function of $\phi$, the idea of
+IG is to directly get analytical best-response derivatives $\partial \theta^
+{\prime} (\phi) / \partial \phi$ by [implicit function theorem](https://
 en.wikipedia.org/wiki/Implicit_function_theorem). This is suitable for
 algorithms when the inner-level optimal solution is achieved ${\left. \frac
 {\partial F (\theta, \phi)}{\partial \theta} \right\rvert}_{\theta=\theta^
 {\prime}} = 0$ or reaches some stationary conditions $F (\theta^{\prime}, \phi)
 = 0$, such as [iMAML](https://arxiv.org/abs/1909.04630) and [DEQ](https://
 arxiv.org/abs/1909.01377). TorchOpt offers both functional and OOP APIs for
 supporting both [conjugate gradient-based](https://arxiv.org/abs/1909.04630)
 and [Neumann series-based](https://arxiv.org/abs/1911.02590) IG methods. Refer
 to the example [iMAML](https://github.com/waterhorse1/torchopt/tree/readme/
 examples/iMAML) and the notebook [Implicit Gradient](tutorials/
 5_Implicit_Differentiation.ipynb) for more guidance. #### Functional API  For
-implicit gradient, users need to define the stationary condition and TorchOpt
-provides the decorator to wrap the solve function for enabling implicit
-gradient computation. ```python # The stationary condition for the inner-loop
-def stationary(params, meta_params, data): # Stationary condition construction
-return stationary condition # Decorator for wrapping the function # Optionally
-specify the linear solver (conjugate gradient or Neumann series)
+the implicit gradient, users need to define the stationary condition and
+TorchOpt provides the decorator to wrap the solve function for enabling
+implicit gradient computation. ```python # The stationary condition for the
+inner-loop def stationary(params, meta_params, data): # Stationary condition
+construction return stationary condition # Decorator for wrapping the function
+# Optionally specify the linear solver (conjugate gradient or Neumann series)
 @torchopt.diff.implicit.custom_root(stationary, solve=linear_solver) def solve
 (params, meta_params, data): # Forward optimization process for params return
 output # Define params, meta_params and get data params, meta_prams, data =
 ..., ..., ... optimal_params = solve(params, meta_params, data) loss =
 outer_loss(optimal_params) meta_grads = torch.autograd.grad(loss, meta_params)
-``` #### OOP API  TorchOpt also offer an OOP API, users need to inherit from
-the class `torchopt.nn.ImplicitMetaGradientModule` to construct the inner-loop
-network. Users need to define the stationary condition/objective function and
-the inner-loop solve function to enable implicit gradient computation.
+``` #### OOP API  TorchOpt also offers an OOP API, which users need to inherit
+from the class `torchopt.nn.ImplicitMetaGradientModule` to construct the inner-
+loop network. Users need to define the stationary condition/objective function
+and the inner-loop solve function to enable implicit gradient computation.
 ```python # Inherited from the class ImplicitMetaGradientModule # Optionally
 specify the linear solver (conjugate gradient or Neumann series) class InnerNet
 (ImplicitMetaGradientModule, linear_solve=linear_solver): def __init__(self,
 meta_param): super().__init__() self.meta_param = meta_param ... def forward
 (self, batch): # Forward process ... def optimality(self, batch, labels): #
 Stationary condition construction for calculating implicit gradient # NOTE: If
 this method is not implemented, it will be automatically # derived from the
@@ -170,28 +170,28 @@
 process is non-differentiable or one wants to eliminate the heavy computation
 burdens in the previous two modes (brought by Hessian), one can choose Zero-
 order Differentiation (ZD). ZD typically gets gradients based on zero-order
 estimation, such as finite-difference, or [Evolutionary Strategy](https://
 arxiv.org/abs/1703.03864). Instead of optimizing the objective $F$, ES
 optimizes a smoothed objective. TorchOpt provides both functional and OOP APIs
 for the ES method. Refer to the tutorial notebook [Zero-order Differentiation]
-(tutorials/6_Zero_Order_Differentiation.ipynb) for more guidances. ####
+(tutorials/6_Zero_Order_Differentiation.ipynb) for more guidance. ####
 Functional API  For zero-order differentiation, users need to define the
 forward pass calculation and the noise sampling procedure. TorchOpt provides
 the decorator to wrap the forward function for enabling zero-order
 differentiation. ```python # Customize the noise sampling function in ES def
 distribution(sample_shape): # Generate a batch of noise samples # NOTE: The
 distribution should be spherical symmetric and with a constant variance of 1.
 ... return noise_batch # Distribution can also be an instance of
 `torch.distributions.Distribution`, e.g., `torch.distributions.Normal(...)`
 distribution = torch.distributions.Normal(loc=0, scale=1) # Specify method and
 hyper-parameter of ES @torchopt.diff.zero_order(distribution, method) def
 forward(params, batch, labels): # Forward process ... return objective # the
-returned tensor should be a scalar tensor ``` #### OOP API  TorchOpt also offer
-an OOP API, users need to inherit from the class
+returned tensor should be a scalar tensor ``` #### OOP API  TorchOpt also
+offers an OOP API, which users need to inherit from the class
 `torchopt.nn.ZeroOrderGradientModule` to construct the network as an
 `nn.Module` following a classical PyTorch style. Users need to define the
 forward process zero-order gradient procedures `forward()` and a noise sampling
 function `sample()`. ```python # Inherited from the class
 ZeroOrderGradientModule # Optionally specify the `method` and/or `num_samples`
 and/or `sigma` used for sampling class Net(ZeroOrderGradientModule,
 method=method, num_samples=num_samples, sigma=sigma): def __init__(self, ...):
@@ -207,60 +207,61 @@
 the optimizer as a whole instead of separating it into several basic operators
 (e.g., `sqrt` and `div`). Therefore, by manually writing the forward and
 backward functions, we can perform the symbolic reduction. In addition, we can
 store some intermediate data that can be reused during the backpropagation. We
 write the accelerated functions in C++ OpenMP and CUDA, bind them by
 [`pybind11`](https://github.com/pybind/pybind11) to allow they can be called by
 Python, and then define the forward and backward behavior using
-`torch.autograd.Function`. Users can use by simply setting the
-`use_accelerated_op` flag as `True`. Refer to the corresponding sections in
-tutorials [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb) and
-[Meta-Optimizer](tutorials/3_Meta_Optimizer.ipynb) ```python optimizer =
-torchopt.MetaAdam(model, lr, use_accelerated_op=True) ``` ### Distributed
-Training `TorchOpt` provides distributed training features based on the PyTorch
-RPC module for better training speed and multi-node multi-GPU support.
-Different from the MPI-like parallelization paradigm, which uses multiple
-homogenous workers and requires carefully designed communication hooks, the RPC
-APIs allow users to build their optimization pipeline more flexibly.
-Experimental results show that we achieve an approximately linear relationship
-between the speed-up ratio and the number of workers. Check out the
-[Distributed Training Documentation](https://torchopt.readthedocs.io/en/latest/
-distributed/distributed.html) and [distributed MAML example](https://
-github.com/metaopt/torchopt/tree/main/examples/distributed/few-shot) for more
-specific guidance. ### OpTree We implement the *PyTree* to enable fast nested
-structure flattening using C++. The tree operations (e.g., flatten and
-unflatten) are very important in enabling functional and Just-In-Time (JIT)
-features of deep learning frameworks. By implementing it in C++, we can use
-some cache/memory-friendly structures (e.g., `absl::InlinedVector`) to improve
-the performance. For more guidance and comparison results, please refer to our
-open-source project [`OpTree`](https://github.com/metaopt/optree). ------------
--------------------------------------------------------------------- ##
-Visualization Complex gradient flow in meta-learning brings in a great
-challenge for managing the gradient flow and verifying the correctness of it.
-TorchOpt provides a visualization tool that draws variable (e.g., network
-parameters or meta-parameters) names on the gradient graph for better analysis.
-The visualization tool is modified from [`torchviz`](https://github.com/
-szagoruyko/pytorchviz). Refer to the example [visualization code](examples/
-visualize.py) and the tutorial notebook [Visualization](tutorials/
-2_Visualization.ipynb) for more details. The figure below show the
-visualization result. Compared with [`torchviz`](https://github.com/szagoruyko/
-pytorchviz), TorchOpt fuses the operations within the `Adam` together (orange)
-to reduce the complexity and provide simpler visualization.
+`torch.autograd.Function`. Users can use it by simply setting the
+`use_accelerated_op` flag as `True`. Refer to the corresponding sections in the
+tutorials [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb)]
+(tutorials/1_Functional_Optimizer.ipynb) and [Meta-Optimizer](tutorials/
+3_Meta_Optimizer.ipynb) ```python optimizer = torchopt.MetaAdam(model, lr,
+use_accelerated_op=True) ``` ### Distributed Training `TorchOpt` provides
+distributed training features based on the PyTorch RPC module for better
+training speed and multi-node multi-GPU support. Different from the MPI-like
+parallelization paradigm, which uses multiple homogeneous workers and requires
+carefully designed communication hooks, the RPC APIs allow users to build their
+optimization pipeline more flexibly. Experimental results show that we achieve
+an approximately linear relationship between the speed-up ratio and the number
+of workers. Check out the [Distributed Training Documentation](https://
+torchopt.readthedocs.io/en/latest/distributed/distributed.html) and
+[distributed MAML example](https://github.com/metaopt/torchopt/tree/main/
+examples/distributed/few-shot) for more specific guidance. ### OpTree We
+implement the *PyTree* to enable fast nested structure flattening using C++.
+The tree operations (e.g., flatten and unflatten) are very important in
+enabling functional and Just-In-Time (JIT) features of deep learning
+frameworks. By implementing it in C++, we can use some cache/memory-friendly
+structures (e.g., `absl::InlinedVector`) to improve the performance. For more
+guidance and comparison results, please refer to our open-source project
+[`OpTree`](https://github.com/metaopt/optree). --------------------------------
+------------------------------------------------ ## Visualization Complex
+gradient flow in meta-learning brings in a great challenge for managing the
+gradient flow and verifying its correctness of it. TorchOpt provides a
+visualization tool that draws variable (e.g., network parameters or meta-
+parameters) names on the gradient graph for better analysis. The visualization
+tool is modified from [`torchviz`](https://github.com/szagoruyko/pytorchviz).
+Refer to the example [visualization code](examples/visualize.py) and the
+tutorial notebook [Visualization](tutorials/2_Visualization.ipynb) for more
+details. The figure below shows the visualization result. Compared with
+[`torchviz`](https://github.com/szagoruyko/pytorchviz), TorchOpt fuses the
+operations within the `Adam` together (orange) to reduce the complexity and
+provide simpler visualization.
  [https://github.com/metaopt/torchopt/raw/HEAD/image/torchviz-vs-torchopt.jpg]
 -------------------------------------------------------------------------------
 - ## Examples In the [`examples`](examples) directory, we offer several
-examples of functional optimizers and light-weight meta-learning examples with
+examples of functional optimizers and lightweight meta-learning examples with
 TorchOpt. - [Model-Agnostic Meta-Learning (MAML) - Supervised Learning](https:/
 /arxiv.org/abs/1703.03400) (ICML 2017) - [Learning to Reweight Examples for
 Robust Deep Learning](https://arxiv.org/abs/1803.09050) (ICML 2018) - [Model-
 Agnostic Meta-Learning (MAML) - Reinforcement Learning](https://arxiv.org/abs/
 1703.03400) (ICML 2017) - [Meta-Gradient Reinforcement Learning (MGRL)](https:/
 /arxiv.org/abs/1805.09801) (NeurIPS 2018) - [Learning through opponent learning
 process (LOLA)](https://arxiv.org/abs/1709.04326) (AAMAS 2018) - [Meta-Learning
-with Implicit Gradients](https://arxiv.org/abs/1909.04630) (NeurIPS 2019) Also
+with Implicit Gradients](https://arxiv.org/abs/1909.04630) (NeurIPS 2019) Also,
 check [`examples`](examples) for more distributed/visualization/functorch-
 compatible examples. ----------------------------------------------------------
 ---------------------- ## Installation Requirements - PyTorch - (Optional) For
 visualizing computation graphs - [Graphviz](https://graphviz.org/download) (for
 Linux users use `apt/yum install graphviz` or `conda install -c anaconda
 python-graphviz`) **Please follow the instructions at
 pytorch.org> to install PyTorch in your Python environment first.** Then run
```

### Comparing `torchopt-0.7.0/include/adam_op/adam_op.h` & `torchopt-0.7.1/include/adam_op/adam_op.h`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/include/adam_op/adam_op_impl_cpu.h` & `torchopt-0.7.1/include/adam_op/adam_op_impl_cpu.h`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/include/adam_op/adam_op_impl_cuda.cuh` & `torchopt-0.7.1/include/adam_op/adam_op_impl_cuda.cuh`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/include/common.h` & `torchopt-0.7.1/include/common.h`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/include/utils.h` & `torchopt-0.7.1/include/utils.h`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/setup.py` & `torchopt-0.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,64 +81,62 @@
         else:
             build_args.append('--parallel')
 
         build_args.extend(['--target', ext.target, '--'])
 
         try:
             os.chdir(build_temp)
-            self.spawn([cmake, ext.source_dir] + cmake_args)
+            self.spawn([cmake, ext.source_dir, *cmake_args])
             if not self.dry_run:
-                self.spawn([cmake, '--build', '.'] + build_args)
+                self.spawn([cmake, '--build', '.', *build_args])
         finally:
             os.chdir(HERE)
 
 
 CIBUILDWHEEL = os.getenv('CIBUILDWHEEL', '0') == '1'
 LINUX = platform.system() == 'Linux'
 MACOS = platform.system() == 'Darwin'
 WINDOWS = platform.system() == 'Windows'
-ext_kwargs = dict(
-    cmdclass={'build_ext': cmake_build_ext},
-    ext_modules=[
+ext_kwargs = {
+    'cmdclass': {'build_ext': cmake_build_ext},
+    'ext_modules': [
         CMakeExtension(
             'torchopt._C',
             source_dir=HERE,
             optional=not (LINUX and CIBUILDWHEEL),
-        )
+        ),
     ],
-)
+}
 
 TORCHOPT_NO_EXTENSIONS = (
     bool(os.getenv('TORCHOPT_NO_EXTENSIONS', '')) or WINDOWS or (MACOS and CIBUILDWHEEL)
 )
 if TORCHOPT_NO_EXTENSIONS:
     ext_kwargs.clear()
 
 
 VERSION_CONTENT = None
 
 try:
     if not version.__release__:
         try:
-            VERSION_CONTENT = VERSION_FILE.read_text(encoding='UTF-8')
+            VERSION_CONTENT = VERSION_FILE.read_text(encoding='utf-8')
             VERSION_FILE.write_text(
                 data=re.sub(
                     r"""__version__\s*=\s*('[^']+'|"[^"]+")""",
-                    f"__version__ = '{version.__version__}'",
+                    f'__version__ = {version.__version__!r}',
                     string=VERSION_CONTENT,
                 ),
-                encoding='UTF-8',
+                encoding='utf-8',
             )
         except OSError:
             VERSION_CONTENT = None
 
     setup(
         name='torchopt',
         version=version.__version__,
-        package_data={'sharedlib': ['*.so', '*.pyd']},
-        include_package_data=True,
         **ext_kwargs,
     )
 finally:
     if VERSION_CONTENT is not None:
-        with VERSION_FILE.open(mode='wt', encoding='UTF-8', newline='') as file:
+        with VERSION_FILE.open(mode='wt', encoding='utf-8', newline='') as file:
             file.write(VERSION_CONTENT)
```

### Comparing `torchopt-0.7.0/src/CMakeLists.txt` & `torchopt-0.7.1/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/src/adam_op/adam_op.cpp` & `torchopt-0.7.1/src/adam_op/adam_op.cpp`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/src/adam_op/adam_op_impl_cpu.cpp` & `torchopt-0.7.1/src/adam_op/adam_op_impl_cpu.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,17 @@
                                  const other_t inv_one_minus_pow_b2,
                                  const other_t eps,
                                  const other_t eps_root,
                                  const size_t n,
                                  scalar_t *__restrict__ updates_ptr,
                                  scalar_t *__restrict__ mu_ptr,
                                  scalar_t *__restrict__ nu_ptr) {
-#pragma omp parallel for num_threads(std::min( \
-    n / MIN_NUMEL_USE_OMP, static_cast <size_t>(omp_get_num_procs()))) if (n > MIN_NUMEL_USE_OMP)
+#pragma omp parallel for num_threads(   \
+        std::min(n / MIN_NUMEL_USE_OMP, \
+                     static_cast<size_t>(omp_get_num_procs()))) if (n > MIN_NUMEL_USE_OMP)
   for (size_t tid = 0; tid < n; ++tid) {
     const scalar_t updates = updates_ptr[tid];
     const scalar_t mu = mu_ptr[tid];
     const scalar_t nu = nu_ptr[tid];
 
     const scalar_t mu_out = b1 * mu + (1 - b1) * updates;
     const scalar_t nu_out = b2 * nu + (1 - b2) * updates * updates;
@@ -91,16 +92,17 @@
 
 template <typename scalar_t, typename other_t>
 void adamForwardMuCPUKernel(const scalar_t *__restrict__ updates_ptr,
                             const scalar_t *__restrict__ mu_ptr,
                             const other_t b1,
                             const size_t n,
                             scalar_t *__restrict__ mu_out_ptr) {
-#pragma omp parallel for num_threads(std::min( \
-    n / MIN_NUMEL_USE_OMP, static_cast <size_t>(omp_get_num_procs()))) if (n > MIN_NUMEL_USE_OMP)
+#pragma omp parallel for num_threads(   \
+        std::min(n / MIN_NUMEL_USE_OMP, \
+                     static_cast<size_t>(omp_get_num_procs()))) if (n > MIN_NUMEL_USE_OMP)
   for (size_t tid = 0; tid < n; ++tid) {
     const scalar_t updates = updates_ptr[tid];
     const scalar_t mu = mu_ptr[tid];
     const scalar_t mu_out = b1 * mu + (1 - b1) * updates;
     mu_out_ptr[tid] = mu_out;
   }
 }
@@ -124,16 +126,17 @@
 
 template <typename scalar_t, typename other_t>
 void adamForwardNuCPUKernel(const scalar_t *__restrict__ updates_ptr,
                             const scalar_t *__restrict__ nu_ptr,
                             const other_t b2,
                             const size_t n,
                             scalar_t *__restrict__ nu_out_ptr) {
-#pragma omp parallel for num_threads(std::min( \
-    n / MIN_NUMEL_USE_OMP, static_cast <size_t>(omp_get_num_procs()))) if (n > MIN_NUMEL_USE_OMP)
+#pragma omp parallel for num_threads(   \
+        std::min(n / MIN_NUMEL_USE_OMP, \
+                     static_cast<size_t>(omp_get_num_procs()))) if (n > MIN_NUMEL_USE_OMP)
   for (size_t tid = 0; tid < n; ++tid) {
     const scalar_t updates = updates_ptr[tid];
     const scalar_t nu = nu_ptr[tid];
 
     const scalar_t nu_out = b2 * nu + (1 - b2) * updates * updates;
     nu_out_ptr[tid] = nu_out;
   }
@@ -161,16 +164,17 @@
                                  const scalar_t *__restrict__ new_nu_ptr,
                                  const other_t inv_one_minus_pow_b1,
                                  const other_t inv_one_minus_pow_b2,
                                  const other_t eps,
                                  const other_t eps_root,
                                  const size_t n,
                                  scalar_t *__restrict__ updates_out_ptr) {
-#pragma omp parallel for num_threads(std::min( \
-    n / MIN_NUMEL_USE_OMP, static_cast <size_t>(omp_get_num_procs()))) if (n > MIN_NUMEL_USE_OMP)
+#pragma omp parallel for num_threads(   \
+        std::min(n / MIN_NUMEL_USE_OMP, \
+                     static_cast<size_t>(omp_get_num_procs()))) if (n > MIN_NUMEL_USE_OMP)
   for (size_t tid = 0; tid < n; ++tid) {
     const scalar_t new_mu = new_mu_ptr[tid];
     const scalar_t new_nu = new_nu_ptr[tid];
     const scalar_t mu_hat = new_mu * inv_one_minus_pow_b1;
     const scalar_t nu_hat = new_nu * inv_one_minus_pow_b2;
     updates_out_ptr[tid] = mu_hat / (sqrt(nu_hat + eps_root) + eps);
   }
@@ -206,16 +210,17 @@
 
 template <typename scalar_t, typename other_t>
 void adamBackwardMuCPUKernel(const scalar_t *__restrict__ dmu_ptr,
                              const other_t b1,
                              const size_t n,
                              scalar_t *__restrict__ dupdates_out_ptr,
                              scalar_t *__restrict__ dmu_out_ptr) {
-#pragma omp parallel for num_threads(std::min( \
-    n / MIN_NUMEL_USE_OMP, static_cast <size_t>(omp_get_num_procs()))) if (n > MIN_NUMEL_USE_OMP)
+#pragma omp parallel for num_threads(   \
+        std::min(n / MIN_NUMEL_USE_OMP, \
+                     static_cast<size_t>(omp_get_num_procs()))) if (n > MIN_NUMEL_USE_OMP)
   for (size_t tid = 0; tid < n; ++tid) {
     const scalar_t dmu = dmu_ptr[tid];
 
     dupdates_out_ptr[tid] = (1 - b1) * dmu;
     dmu_out_ptr[tid] = b1 * dmu;
   }
 }
@@ -242,16 +247,17 @@
 template <typename scalar_t, typename other_t>
 void adamBackwardNuCPUKernel(const scalar_t *__restrict__ dnu_ptr,
                              const scalar_t *__restrict__ updates_ptr,
                              const other_t b2,
                              const size_t n,
                              scalar_t *__restrict__ dupdates_out_ptr,
                              scalar_t *__restrict__ dnu_out_ptr) {
-#pragma omp parallel for num_threads(std::min( \
-    n / MIN_NUMEL_USE_OMP, static_cast <size_t>(omp_get_num_procs()))) if (n > MIN_NUMEL_USE_OMP)
+#pragma omp parallel for num_threads(   \
+        std::min(n / MIN_NUMEL_USE_OMP, \
+                     static_cast<size_t>(omp_get_num_procs()))) if (n > MIN_NUMEL_USE_OMP)
   for (size_t tid = 0; tid < n; ++tid) {
     const scalar_t dnu = dnu_ptr[tid];
     const scalar_t updates = updates_ptr[tid];
 
     dupdates_out_ptr[tid] = 2 * (1 - b2) * updates * dnu;
     dnu_out_ptr[tid] = b2 * dnu;
   }
@@ -282,16 +288,17 @@
                                   const scalar_t *__restrict__ updates_ptr,
                                   const scalar_t *__restrict__ new_mu_ptr,
                                   const other_t one_minus_pow_b1,
                                   const other_t inv_one_minus_pow_b2,
                                   const size_t n,
                                   scalar_t *__restrict__ dnew_mu_out_ptr,
                                   scalar_t *__restrict__ dnew_nu_out_ptr) {
-#pragma omp parallel for num_threads(std::min( \
-    n / MIN_NUMEL_USE_OMP, static_cast <size_t>(omp_get_num_procs()))) if (n > MIN_NUMEL_USE_OMP)
+#pragma omp parallel for num_threads(   \
+        std::min(n / MIN_NUMEL_USE_OMP, \
+                     static_cast<size_t>(omp_get_num_procs()))) if (n > MIN_NUMEL_USE_OMP)
   for (size_t tid = 0; tid < n; ++tid) {
     const scalar_t dupdates = dupdates_ptr[tid];
     const scalar_t updates = updates_ptr[tid];
     const scalar_t new_mu = new_mu_ptr[tid];
 
     if (new_mu == 0) {
       dnew_mu_out_ptr[tid] = 0;
```

### Comparing `torchopt-0.7.0/src/adam_op/adam_op_impl_cuda.cu` & `torchopt-0.7.1/src/adam_op/adam_op_impl_cuda.cu`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/src/extension.cpp` & `torchopt-0.7.1/src/extension.cpp`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/tests/test_accelerated_op.py` & `torchopt-0.7.1/tests/test_accelerated_op.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,15 +99,18 @@
 
         grads = torch.autograd.grad(loss, params, allow_unused=True)
         updates, optim_state = optim.update(grads, optim_state, params=params, inplace=inplace)
         params = torchopt.apply_updates(params, updates, inplace=inplace)
 
         grads = torch.autograd.grad(loss_ref, params_ref, allow_unused=True)
         updates, optim_state_ref = optim_ref.update(
-            grads, optim_state_ref, params=params, inplace=inplace
+            grads,
+            optim_state_ref,
+            params=params,
+            inplace=inplace,
         )
         params_ref = torchopt.apply_updates(params_ref, updates, inplace=inplace)
 
     helpers.assert_pytree_all_close(params, params_ref)
 
 
 @helpers.parametrize(
@@ -150,44 +153,56 @@
         inner_opt_state = inner_optimizer.init(params)
         with torch.enable_grad():
             # Temporarily enable gradient computation for conducting the optimization
             for _ in range(inner_update):
                 pred = f(params, b, x)
                 inner_loss = F.cross_entropy(pred, y)  # compute loss
                 grads = torch.autograd.grad(
-                    inner_loss, params, allow_unused=True
+                    inner_loss,
+                    params,
+                    allow_unused=True,
                 )  # compute gradients
                 updates, inner_opt_state = inner_optimizer.update(
-                    grads, inner_opt_state, inplace=False
+                    grads,
+                    inner_opt_state,
+                    inplace=False,
                 )  # get updates
                 params = torchopt.apply_updates(params, updates, inplace=False)
         return (params, b)
 
     for xs, ys in loader:
         xs = xs.to(dtype=dtype)
         data = (xs, ys, fmodel, buffers)
         data_ref = (xs, ys, fmodel_ref, buffers_ref)
 
         params_prime, buffers_prime = maml_inner_solver(params, data, use_accelerated_op=True)
         params_prime_ref, buffers_prime_ref = maml_inner_solver(
-            params_ref, data_ref, use_accelerated_op=False
+            params_ref,
+            data_ref,
+            use_accelerated_op=False,
         )
 
         pred = fmodel(params_prime, buffers_prime, xs)
         pred_ref = fmodel_ref(params_prime_ref, buffers_prime_ref, xs)
         outer_loss = F.cross_entropy(pred, ys)
         outer_loss_ref = F.cross_entropy(pred_ref, ys)
 
         grads = torch.autograd.grad(outer_loss, params, allow_unused=True)
         updates, outer_optim_state = outer_optim.update(
-            grads, outer_optim_state, params=params, inplace=inplace
+            grads,
+            outer_optim_state,
+            params=params,
+            inplace=inplace,
         )
         params = torchopt.apply_updates(params, updates, inplace=inplace)
 
         grads = torch.autograd.grad(outer_loss_ref, params_ref, allow_unused=True)
         updates, outer_optim_state_ref = outer_optim_ref.update(
-            grads, outer_optim_state_ref, params=params, inplace=inplace
+            grads,
+            outer_optim_state_ref,
+            params=params,
+            inplace=inplace,
         )
         params_ref = torchopt.apply_updates(params_ref, updates, inplace=inplace)
 
         torchopt.stop_gradient(model)
         torchopt.stop_gradient(model_ref)
```

### Comparing `torchopt-0.7.0/tests/test_alias.py` & `torchopt-0.7.1/tests/test_alias.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,64 @@
 import functorch
 import pytest
 import torch
 import torch.nn.functional as F
 
 import helpers
 import torchopt
+from torchopt import pytree
 from torchopt.alias.utils import _set_use_chain_flat
+from torchopt.typing import TensorTree
+
+
+@helpers.parametrize(
+    optimizer=[
+        torchopt.sgd,
+        torchopt.adam,
+        torchopt.adamw,
+        torchopt.rmsprop,
+    ],
+    tensortree=[
+        {},
+        (),
+        [],
+        (None,),
+        {'a': (), 'b': {'c': []}, 'd': None},
+    ],
+    maximize=[False, True],
+    inplace=[True, False],
+    use_chain_flat=[True, False],
+)
+def test_empty(
+    optimizer: Callable,
+    tensortree: TensorTree,
+    maximize: bool,
+    inplace: bool,
+    use_chain_flat: bool,
+) -> None:
+    _set_use_chain_flat(use_chain_flat)
+
+    params = pytree.tree_map(lambda x: x, tensortree)
+    grads = pytree.tree_map(lambda x: x, tensortree)
+
+    optim = optimizer(1e-3, maximize=maximize)
+    optim_state = optim.init(params)
+    updates, optim_state = optim.update(grads, optim_state, params=params, inplace=inplace)
+    _ = torchopt.apply_updates(params, updates)
+
+    try:
+        optim = optimizer(1e-3, maximize=maximize, use_accelerated_op=True)
+    except TypeError:
+        pass
+    else:
+        optim_state = optim.init(params)
+        updates, optim_state = optim.update(grads, optim_state, params=params, inplace=inplace)
+        _ = torchopt.apply_updates(params, updates)
+
+    _set_use_chain_flat(True)
 
 
 @helpers.parametrize(
     dtype=[torch.float64, torch.float32],
     lr=[1e-2, 1e-3, 1e-4],
     momentum=[0.0, 0.1],
     dampening=[0.0, 0.5],
@@ -218,35 +267,45 @@
         inner_opt_state = inner_optimizer.init(params)
         with torch.enable_grad():
             # Temporarily enable gradient computation for conducting the optimization
             for _ in range(inner_update):
                 pred = f(params, b, x)
                 inner_loss = F.cross_entropy(pred, y)  # compute loss
                 grads = torch.autograd.grad(
-                    inner_loss, params, allow_unused=True
+                    inner_loss,
+                    params,
+                    allow_unused=True,
                 )  # compute gradients
                 updates, inner_opt_state = inner_optimizer.update(
-                    grads, inner_opt_state, params=params, inplace=False
+                    grads,
+                    inner_opt_state,
+                    params=params,
+                    inplace=False,
                 )  # get updates
                 params = torchopt.apply_updates(params, updates, inplace=False)
         return (params, b)
 
     for xs, ys in loader:
         xs = xs.to(dtype=dtype)
         data = (xs, ys, fmodel, buffers)
 
         params_prime, buffers_prime = maml_inner_solver_torchopt(
-            params, data, use_accelerated_op=True
+            params,
+            data,
+            use_accelerated_op=True,
         )
         pred = fmodel(params_prime, buffers_prime, xs)
         outer_loss = F.cross_entropy(pred, ys)
 
         grads = torch.autograd.grad(outer_loss, params, allow_unused=True)
         updates, outer_optim_state = outer_optim.update(
-            grads, outer_optim_state, params=params, inplace=inplace
+            grads,
+            outer_optim_state,
+            params=params,
+            inplace=inplace,
         )
         params = torchopt.apply_updates(params, updates, inplace=inplace)
 
         torchopt.stop_gradient(model)
 
     _set_use_chain_flat(True)
 
@@ -377,14 +436,78 @@
         pred = fmodel(params, buffers, xs)
         pred_ref = model_ref(xs)
         loss = F.cross_entropy(pred, ys)
         loss_ref = F.cross_entropy(pred_ref, ys)
 
         grads = torch.autograd.grad(loss, params, allow_unused=True)
         updates, optim_state = optim.update(grads, optim_state, params=params, inplace=inplace)
+        params = torchopt.apply_updates(params, updates, inplace=inplace)
+
+        optim_ref.zero_grad()
+        loss_ref.backward()
+        optim_ref.step()
+
+    helpers.assert_model_all_close((params, buffers), model_ref, model_base, dtype=dtype)
+    _set_use_chain_flat(True)
+
+
+@helpers.parametrize(
+    dtype=[torch.float64],
+    lr=[1e-2, 1e-3, 1e-4],
+    lr_decay=[0.0, 1e-2],
+    initial_accumulator_value=[0.0, 1e-1],
+    eps=[1e-8],
+    inplace=[True, False],
+    weight_decay=[0.0, 1e-2],
+    maximize=[False, True],
+    use_chain_flat=[True, False],
+)
+def test_adagrad(
+    dtype: torch.dtype,
+    lr: float,
+    lr_decay: float,
+    initial_accumulator_value: float,
+    eps: float,
+    inplace: bool,
+    weight_decay: float,
+    maximize: bool,
+    use_chain_flat: bool,
+) -> None:
+    _set_use_chain_flat(use_chain_flat)
+
+    model, model_ref, model_base, loader = helpers.get_models(device='cpu', dtype=dtype)
+
+    fmodel, params, buffers = functorch.make_functional_with_buffers(model)
+    optim = torchopt.adagrad(
+        lr=lr,
+        lr_decay=lr_decay,
+        weight_decay=weight_decay,
+        initial_accumulator_value=initial_accumulator_value,
+        eps=eps,
+        maximize=maximize,
+    )
+    optim_state = optim.init(params)
+    optim_ref = torch.optim.Adagrad(
+        model_ref.parameters(),
+        lr=lr,
+        lr_decay=lr_decay,
+        weight_decay=weight_decay,
+        initial_accumulator_value=initial_accumulator_value,
+        eps=eps,
+        maximize=maximize,
+    )
+    for xs, ys in loader:
+        xs = xs.to(dtype=dtype)
+        pred = fmodel(params, buffers, xs)
+        pred_ref = model_ref(xs)
+        loss = F.cross_entropy(pred, ys)
+        loss_ref = F.cross_entropy(pred_ref, ys)
+
+        grads = torch.autograd.grad(loss, params, allow_unused=True)
+        updates, optim_state = optim.update(grads, optim_state, params=params, inplace=inplace)
         params = torchopt.apply_updates(params, updates, inplace=inplace)
 
         optim_ref.zero_grad()
         loss_ref.backward()
         optim_ref.step()
 
     helpers.assert_model_all_close((params, buffers), model_ref, model_base, dtype=dtype)
```

### Comparing `torchopt-0.7.0/tests/test_clip.py` & `torchopt-0.7.1/tests/test_clip.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/tests/test_combine.py` & `torchopt-0.7.1/tests/test_combine.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,21 +31,23 @@
         torchopt.base.ChainedGradientTransformation,
     )
 
     _set_use_chain_flat(False)
     adam = torchopt.adam()
     assert isinstance(adam, torchopt.base.ChainedGradientTransformation)
     assert isinstance(
-        adam.chain(torchopt.base.identity()), torchopt.base.ChainedGradientTransformation
+        adam.chain(torchopt.base.identity()),
+        torchopt.base.ChainedGradientTransformation,
     )
     assert adam.chain(torchopt.base.identity()) == adam
     assert torchopt.base.identity().chain(adam) == adam
     assert torchopt.chain(torchopt.base.identity(), adam, torchopt.base.identity()) == adam
     _set_use_chain_flat(True)
 
     assert isinstance(adam, torchopt.base.GradientTransformation)
     assert isinstance(
-        adam.chain(torchopt.base.identity()), torchopt.base.ChainedGradientTransformation
+        adam.chain(torchopt.base.identity()),
+        torchopt.base.ChainedGradientTransformation,
     )
     assert adam.chain(torchopt.base.identity()) == adam
     assert torchopt.base.identity().chain(adam) == adam
     assert torchopt.chain(torchopt.base.identity(), adam, torchopt.base.identity()) == adam
```

### Comparing `torchopt-0.7.0/tests/test_hook.py` & `torchopt-0.7.1/tests/test_hook.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/tests/test_implicit.py` & `torchopt-0.7.1/tests/test_implicit.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,36 +12,45 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from __future__ import annotations
 
 import copy
+import re
 from collections import OrderedDict
 from types import FunctionType
 
 import functorch
-import jax
-import jax.numpy as jnp
-import jaxopt
 import numpy as np
-import optax
 import pytest
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.types
 from torch.utils import data
 
 import helpers
 import torchopt
 from torchopt import pytree
 from torchopt.diff.implicit import ImplicitMetaGradientModule
 
 
+try:
+    import jax
+    import jax.numpy as jnp
+    import jaxopt
+    import optax
+
+    HAS_JAX = True
+except ImportError:
+    jax = jnp = jaxopt = optax = None
+    HAS_JAX = False
+
+
 BATCH_SIZE = 8
 NUM_UPDATES = 3
 
 MODEL_NUM_INPUTS = 10
 MODEL_NUM_CLASSES = 10
 
 
@@ -62,22 +71,23 @@
     def func(params, x):
         return x @ params['weight'] + params['bias']
 
     params = OrderedDict(
         [
             ('weight', jnp.ones((MODEL_NUM_INPUTS, MODEL_NUM_CLASSES), dtype=dtype)),
             ('bias', jnp.zeros((MODEL_NUM_CLASSES,), dtype=dtype)),
-        ]
+        ],
     )
     return func, params
 
 
 @torch.no_grad()
 def get_model_torch(
-    device: torch.types.Device = None, dtype: torch.dtype = torch.float32
+    device: torch.types.Device | None = None,
+    dtype: torch.dtype = torch.float32,
 ) -> tuple[nn.Module, data.DataLoader]:
     helpers.seed_everything(seed=42)
 
     model = FcNet(MODEL_NUM_INPUTS, MODEL_NUM_CLASSES).to(dtype=dtype)
 
     if device is not None:
         model = model.to(device=torch.device(device))
@@ -99,27 +109,29 @@
     NUM_UPDATES = 4
     dataset = data.TensorDataset(
         torch.randn((BATCH_SIZE * NUM_UPDATES, MODEL_NUM_INPUTS)),
         torch.randn((BATCH_SIZE * NUM_UPDATES,)),
         torch.randn((BATCH_SIZE * NUM_UPDATES, MODEL_NUM_INPUTS)),
         torch.randn((BATCH_SIZE * NUM_UPDATES,)),
     )
-    loader = data.DataLoader(dataset, BATCH_SIZE, shuffle=False)
-
-    return loader
+    return data.DataLoader(dataset, BATCH_SIZE, shuffle=False)
 
 
+@pytest.mark.skipif(not HAS_JAX, reason='JAX is not installed')
 @helpers.parametrize(
     dtype=[torch.float64, torch.float32],
     lr=[1e-3, 1e-4],
     inner_lr=[2e-2, 2e-3],
     inner_update=[20, 50, 100],
 )
 def test_imaml_solve_normal_cg(
-    dtype: torch.dtype, lr: float, inner_lr: float, inner_update: int
+    dtype: torch.dtype,
+    lr: float,
+    inner_lr: float,
+    inner_update: int,
 ) -> None:
     np_dtype = helpers.dtype_torch2numpy(dtype)
 
     jax_model, jax_params = get_model_jax(dtype=np_dtype)
     model, loader = get_model_torch(device='cpu', dtype=dtype)
 
     fmodel, params = functorch.make_functional(model)
@@ -131,16 +143,15 @@
 
     def imaml_objective_torchopt(params, meta_params, data):
         x, y, f = data
         y_pred = f(params, x)
         regularization_loss = 0
         for p1, p2 in zip(params, meta_params):
             regularization_loss += 0.5 * torch.sum(torch.square(p1 - p2))
-        loss = F.cross_entropy(y_pred, y) + regularization_loss
-        return loss
+        return F.cross_entropy(y_pred, y) + regularization_loss
 
     @torchopt.diff.implicit.custom_root(
         functorch.grad(imaml_objective_torchopt, argnums=0),
         argnums=1,
         has_aux=True,
         solve=torchopt.linear_solve.solve_normal_cg(),
     )
@@ -187,28 +198,28 @@
         def compute_loss(params, meta_params, x, y):
             pred = jax_model(params, x)
             loss = jnp.mean(optax.softmax_cross_entropy_with_integer_labels(pred, y))
             # Compute regularization loss
             regularization_loss = 0
             for p1, p2 in zip(params.values(), meta_params.values()):
                 regularization_loss += 0.5 * jnp.sum(jnp.square(p1 - p2))
-            final_loss = loss + regularization_loss
-            return final_loss
+            return loss + regularization_loss
 
-        for i in range(inner_update):
+        for _ in range(inner_update):
             grads = jax.grad(compute_loss)(params, meta_params, x, y)  # compute gradients
             updates, opt_state = optimizer.update(grads, opt_state)  # get updates
             params = optax.apply_updates(params, updates)
         return params, (0, {'a': 1, 'b': 2})
 
     for xs, ys in loader:
         xs = xs.to(dtype=dtype)
         data = (xs, ys, fmodel)
         inner_params = pytree.tree_map(
-            lambda t: t.clone().detach_().requires_grad_(requires_grad=t.requires_grad), params
+            lambda t: t.clone().detach_().requires_grad_(requires_grad=t.requires_grad),
+            params,
         )
         optimal_inner_params, aux = inner_solver_torchopt(inner_params, params, data)
         assert aux == (0, {'a': 1, 'b': 2})
         outer_loss = fmodel(optimal_inner_params, xs).mean()
 
         grads = torch.autograd.grad(outer_loss, params)
         updates, optim_state = optim.update(grads, optim_state)
@@ -216,28 +227,28 @@
 
         xs = xs.numpy()
         ys = ys.numpy()
 
         def outer_level(p, xs, ys):
             optimal_params, aux = inner_solver_jax(copy.deepcopy(p), p, xs, ys)
             assert aux == (0, {'a': 1, 'b': 2})
-            outer_loss = jax_model(optimal_params, xs).mean()
-            return outer_loss
+            return jax_model(optimal_params, xs).mean()
 
         grads_jax = jax.grad(outer_level, argnums=0)(jax_params, xs, ys)
         updates_jax, optim_state_jax = optim_jax.update(grads_jax, optim_state_jax)  # get updates
         jax_params = optax.apply_updates(jax_params, updates_jax)
 
     jax_params_as_tensor = tuple(
         nn.Parameter(torch.tensor(np.asarray(jax_params[j]), dtype=dtype)) for j in jax_params
     )
 
     helpers.assert_pytree_all_close(params, jax_params_as_tensor)
 
 
+@pytest.mark.skipif(not HAS_JAX, reason='JAX is not installed')
 @helpers.parametrize(
     dtype=[torch.float64, torch.float32],
     lr=[1e-3, 1e-4],
     inner_lr=[2e-2, 2e-3],
     inner_update=[20, 50, 100],
     ns=[False, True],
 )
@@ -262,16 +273,15 @@
 
     def imaml_objective_torchopt(params, meta_params, data):
         x, y, f = data
         y_pred = f(params, x)
         regularization_loss = 0
         for p1, p2 in zip(params, meta_params):
             regularization_loss += 0.5 * torch.sum(torch.square(p1 - p2))
-        loss = F.cross_entropy(y_pred, y) + regularization_loss
-        return loss
+        return F.cross_entropy(y_pred, y) + regularization_loss
 
     @torchopt.diff.implicit.custom_root(
         functorch.grad(imaml_objective_torchopt, argnums=0),
         argnums=1,
         solve=torchopt.linear_solve.solve_inv(ns=ns),
     )
     def inner_solver_torchopt(params, meta_params, data):
@@ -316,55 +326,55 @@
         def compute_loss(params, meta_params, x, y):
             pred = jax_model(params, x)
             loss = jnp.mean(optax.softmax_cross_entropy_with_integer_labels(pred, y))
             # Compute regularization loss
             regularization_loss = 0
             for p1, p2 in zip(params.values(), meta_params.values()):
                 regularization_loss += 0.5 * jnp.sum(jnp.square(p1 - p2))
-            final_loss = loss + regularization_loss
-            return final_loss
+            return loss + regularization_loss
 
-        for i in range(inner_update):
+        for _ in range(inner_update):
             grads = jax.grad(compute_loss)(params, meta_params, x, y)  # compute gradients
             updates, opt_state = optimizer.update(grads, opt_state)  # get updates
             params = optax.apply_updates(params, updates)
         return params
 
     for xs, ys in loader:
         xs = xs.to(dtype=dtype)
         data = (xs, ys, fmodel)
         inner_params = pytree.tree_map(
-            lambda t: t.clone().detach_().requires_grad_(requires_grad=t.requires_grad), params
+            lambda t: t.clone().detach_().requires_grad_(requires_grad=t.requires_grad),
+            params,
         )
         optimal_inner_params = inner_solver_torchopt(inner_params, params, data)
         outer_loss = fmodel(optimal_inner_params, xs).mean()
 
         grads = torch.autograd.grad(outer_loss, params)
         updates, optim_state = optim.update(grads, optim_state)
         params = torchopt.apply_updates(params, updates)
 
         xs = xs.numpy()
         ys = ys.numpy()
 
         def outer_level(p, xs, ys):
             optimal_params = inner_solver_jax(copy.deepcopy(p), p, xs, ys)
-            outer_loss = jax_model(optimal_params, xs).mean()
-            return outer_loss
+            return jax_model(optimal_params, xs).mean()
 
         grads_jax = jax.grad(outer_level, argnums=0)(jax_params, xs, ys)
         updates_jax, optim_state_jax = optim_jax.update(grads_jax, optim_state_jax)  # get updates
         jax_params = optax.apply_updates(jax_params, updates_jax)
 
     jax_params_as_tensor = tuple(
         nn.Parameter(torch.tensor(np.asarray(jax_params[j]), dtype=dtype)) for j in jax_params
     )
 
     helpers.assert_pytree_all_close(params, jax_params_as_tensor)
 
 
+@pytest.mark.skipif(not HAS_JAX, reason='JAX is not installed')
 @helpers.parametrize(
     dtype=[torch.float64, torch.float32],
     lr=[1e-3, 1e-4],
     inner_lr=[2e-2, 2e-3],
     inner_update=[20, 50, 100],
 )
 def test_imaml_module(dtype: torch.dtype, lr: float, inner_lr: float, inner_update: int) -> None:
@@ -428,18 +438,17 @@
         def compute_loss(params, meta_params, x, y):
             pred = jax_model(params, x)
             loss = jnp.mean(optax.softmax_cross_entropy_with_integer_labels(pred, y))
             # Compute regularization loss
             regularization_loss = 0
             for p1, p2 in zip(params.values(), meta_params.values()):
                 regularization_loss += 0.5 * jnp.sum(jnp.square(p1 - p2))
-            final_loss = loss + regularization_loss
-            return final_loss
+            return loss + regularization_loss
 
-        for i in range(inner_update):
+        for _ in range(inner_update):
             grads = jax.grad(compute_loss)(params, meta_params, x, y)  # compute gradients
             updates, opt_state = optimizer.update(grads, opt_state)  # get updates
             params = optax.apply_updates(params, updates)
         return params, (0, {'a': 1, 'b': 2})
 
     for xs, ys in loader:
         xs = xs.to(dtype=dtype)
@@ -454,28 +463,28 @@
 
         xs = xs.numpy()
         ys = ys.numpy()
 
         def outer_level(p, xs, ys):
             optimal_params, aux = inner_solver_jax(copy.deepcopy(p), p, xs, ys)
             assert aux == (0, {'a': 1, 'b': 2})
-            outer_loss = jax_model(optimal_params, xs).mean()
-            return outer_loss
+            return jax_model(optimal_params, xs).mean()
 
         grads_jax = jax.grad(outer_level, argnums=0)(jax_params, xs, ys)
         updates_jax, optim_state_jax = optim_jax.update(grads_jax, optim_state_jax)  # get updates
         jax_params = optax.apply_updates(jax_params, updates_jax)
 
     jax_params_as_tensor = tuple(
         nn.Parameter(torch.tensor(np.asarray(jax_params[j]), dtype=dtype)) for j in jax_params
     )
 
     helpers.assert_pytree_all_close(tuple(model.parameters()), jax_params_as_tensor)
 
 
+@pytest.mark.skipif(not HAS_JAX, reason='JAX is not installed')
 @helpers.parametrize(
     dtype=[torch.float64, torch.float32],
     lr=[1e-3, 1e-4],
 )
 def test_rr_solve_cg(
     dtype: torch.dtype,
     lr: float,
@@ -559,25 +568,25 @@
         ys = jnp.array(ys.numpy(), dtype=np_dtype)
         xq = jnp.array(xq.numpy(), dtype=np_dtype)
         yq = jnp.array(yq.numpy(), dtype=np_dtype)
 
         def outer_level(params_jax, l2reg_jax, xs, ys, xq, yq):
             w_fit = ridge_solver_jax_cg(params_jax, l2reg_jax, xs, ys)
             y_pred = xq @ w_fit
-            loss_value = jnp.mean(jnp.square(y_pred - yq))
-            return loss_value
+            return jnp.mean(jnp.square(y_pred - yq))
 
         grads_jax = jax.grad(outer_level, argnums=1)(init_params_jax, l2reg_jax, xs, ys, xq, yq)
         updates_jax, optim_state_jax = optim_jax.update(grads_jax, optim_state_jax)  # get updates
         l2reg_jax = optax.apply_updates(l2reg_jax, updates_jax)
 
     l2reg_jax_as_tensor = torch.tensor(np.asarray(l2reg_jax), dtype=dtype)
     helpers.assert_all_close(l2reg_torch, l2reg_jax_as_tensor)
 
 
+@pytest.mark.skipif(not HAS_JAX, reason='JAX is not installed')
 @helpers.parametrize(
     dtype=[torch.float64, torch.float32],
     lr=[1e-3, 1e-4],
     ns=[True, False],
 )
 def test_rr_solve_inv(
     dtype: torch.dtype,
@@ -664,16 +673,196 @@
         ys = jnp.array(ys.numpy(), dtype=np_dtype)
         xq = jnp.array(xq.numpy(), dtype=np_dtype)
         yq = jnp.array(yq.numpy(), dtype=np_dtype)
 
         def outer_level(params_jax, l2reg_jax, xs, ys, xq, yq):
             w_fit = ridge_solver_jax_inv(params_jax, l2reg_jax, xs, ys)
             y_pred = xq @ w_fit
-            loss_value = jnp.mean(jnp.square(y_pred - yq))
-            return loss_value
+            return jnp.mean(jnp.square(y_pred - yq))
 
         grads_jax = jax.grad(outer_level, argnums=1)(init_params_jax, l2reg_jax, xs, ys, xq, yq)
         updates_jax, optim_state_jax = optim_jax.update(grads_jax, optim_state_jax)  # get updates
         l2reg_jax = optax.apply_updates(l2reg_jax, updates_jax)
 
     l2reg_jax_as_tensor = torch.tensor(np.asarray(l2reg_jax), dtype=dtype)
     helpers.assert_all_close(l2reg_torch, l2reg_jax_as_tensor)
+
+
+def test_module_empty_parameters() -> None:
+    class EmptyParameters(ImplicitMetaGradientModule):
+        def __init__(self, x):
+            super().__init__()
+            self.x = x
+
+        def objective(self):
+            return self.x.mean()
+
+        def solve(self):
+            pass
+
+    model = EmptyParameters(torch.zeros(8))
+    with pytest.raises(RuntimeError, match='The module has no parameters.'):
+        model.solve()
+
+    model = EmptyParameters(torch.zeros(8))
+    model.register_parameter('y', torch.zeros(8, requires_grad=True))
+    with pytest.raises(RuntimeError, match='The module has no meta-parameters.'):
+        model.solve()
+
+    model = EmptyParameters(torch.zeros(8, requires_grad=True))
+    with pytest.raises(RuntimeError, match='The module has no parameters.'):
+        model.solve()
+
+    model = EmptyParameters(torch.zeros(8, requires_grad=True))
+    with pytest.raises(RuntimeError, match='The module has no parameters.'):
+        model.optimality()
+
+    model = EmptyParameters(torch.zeros(8))
+    model.register_parameter('y', torch.zeros(8, requires_grad=True))
+    with pytest.raises(RuntimeError, match='The module has no meta-parameters.'):
+        model.optimality()
+
+    model = EmptyParameters(torch.zeros(8, requires_grad=True))
+    model.register_parameter('y', torch.zeros(8, requires_grad=True))
+    model.solve()
+
+    model = EmptyParameters(nn.Linear(8, 8).eval())
+    with pytest.raises(RuntimeError, match='The module has no meta-parameters.'):
+        model.solve()
+
+    model = EmptyParameters(nn.Linear(8, 8))
+    model.register_parameter('y', torch.zeros(8, requires_grad=True))
+    model.solve()
+
+
+def test_module_enable_implicit_gradients_twice() -> None:
+    class MyModule1(torchopt.nn.ImplicitMetaGradientModule):
+        def objective(self):
+            return torch.tensor(0.0)
+
+        def solve(self):
+            pass
+
+    from torchopt.diff.implicit.nn.module import (
+        enable_implicit_gradients,
+        make_optimality_from_objective,
+    )
+
+    with pytest.raises(
+        TypeError,
+        match='Implicit gradients are already enabled for the `solve` method.',
+    ):
+        enable_implicit_gradients(MyModule1)
+
+    class MyModule2(torchopt.nn.ImplicitMetaGradientModule):
+        def optimality(self):
+            return torch.tensor(0.0)
+
+        def solve(self):
+            pass
+
+    with pytest.raises(
+        TypeError,
+        match='The objective function is not defined.',
+    ):
+        make_optimality_from_objective(MyModule2)
+
+
+def test_module_abstract_methods() -> None:
+    class MyModule1(torchopt.nn.ImplicitMetaGradientModule):
+        def objective(self):
+            return torch.tensor(0.0)
+
+    with pytest.raises(TypeError, match="Can't instantiate abstract class"):
+        MyModule1()
+
+    with pytest.raises(
+        TypeError,
+        match=re.escape(
+            'ImplicitMetaGradientModule requires either an optimality() method or an objective() method',
+        ),
+    ):
+
+        class MyModule2(torchopt.nn.ImplicitMetaGradientModule):
+            def solve(self):
+                pass
+
+    class MyModule3(torchopt.nn.ImplicitMetaGradientModule):
+        def optimality(self):
+            return ()
+
+        def solve(self):
+            pass
+
+    with pytest.raises(
+        TypeError,
+        match=re.escape('method optimality() must not be a staticmethod.'),
+    ):
+
+        class MyModule4(torchopt.nn.ImplicitMetaGradientModule):
+            @staticmethod
+            def optimality():
+                return ()
+
+            def solve(self):
+                pass
+
+    with pytest.raises(
+        TypeError,
+        match=re.escape('method optimality() must not be a classmethod.'),
+    ):
+
+        class MyModule5(torchopt.nn.ImplicitMetaGradientModule):
+            @classmethod
+            def optimality(self):
+                return ()
+
+            def solve(self):
+                pass
+
+    with pytest.raises(
+        TypeError,
+        match=re.escape('method optimality() must be callable.'),
+    ):
+
+        class MyModule6(torchopt.nn.ImplicitMetaGradientModule):
+            optimality = 0
+
+            def solve(self):
+                pass
+
+    with pytest.raises(
+        TypeError,
+        match=re.escape('method objective() must not be a staticmethod.'),
+    ):
+
+        class MyModule7(torchopt.nn.ImplicitMetaGradientModule):
+            @staticmethod
+            def objective():
+                return ()
+
+            def solve(self):
+                pass
+
+    with pytest.raises(
+        TypeError,
+        match=re.escape('method objective() must not be a classmethod.'),
+    ):
+
+        class MyModule8(torchopt.nn.ImplicitMetaGradientModule):
+            @classmethod
+            def objective(self):
+                return ()
+
+            def solve(self):
+                pass
+
+    with pytest.raises(
+        TypeError,
+        match=re.escape('method objective() must be callable.'),
+    ):
+
+        class MyModule9(torchopt.nn.ImplicitMetaGradientModule):
+            objective = 0
+
+            def solve(self):
+                pass
```

### Comparing `torchopt-0.7.0/tests/test_import.py` & `torchopt-0.7.1/tests/test_import.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,24 +21,25 @@
     torchopt.accelerated_op.is_available
     torchopt.accelerated_op_available
     from torchopt.accelerated_op import is_available
     from torchopt.accelerated_op.adam_op import AdamOp
 
 
 def test_alias_import() -> None:
+    torchopt.adagrad
     torchopt.adam
     torchopt.adamw
     torchopt.rmsprop
     torchopt.sgd
     torchopt.alias.adam
     torchopt.alias.adamw
     torchopt.alias.rmsprop
     torchopt.alias.sgd
-    from torchopt import adam, adamw, rmsprop, sgd
-    from torchopt.alias import adam, adamw, rmsprop, sgd
+    from torchopt import adagrad, adam, adamw, rmsprop, sgd
+    from torchopt.alias import adagrad, adam, adamw, rmsprop, sgd
 
 
 def test_diff_import() -> None:
     torchopt.diff.implicit
     torchopt.diff.implicit.custom_root
     torchopt.diff.implicit.ImplicitMetaGradientModule
     torchopt.diff.implicit.nn.ImplicitMetaGradientModule
@@ -103,54 +104,66 @@
     torchopt.nn.ImplicitMetaGradientModule
     torchopt.nn.ZeroOrderGradientModule
     from torchopt.nn import ImplicitMetaGradientModule, MetaGradientModule, ZeroOrderGradientModule
 
 
 def test_optim_import() -> None:
     torchopt.FuncOptimizer
+    torchopt.MetaAdaGrad
+    torchopt.MetaAdagrad
     torchopt.MetaAdam
     torchopt.MetaAdamW
     torchopt.MetaRMSProp
     torchopt.MetaRMSprop
     torchopt.MetaSGD
+    torchopt.AdaGrad
+    torchopt.Adagrad
     torchopt.Adam
     torchopt.AdamW
     torchopt.Optimizer
     torchopt.RMSProp
     torchopt.RMSprop
     torchopt.SGD
+    torchopt.optim.meta.MetaAdaGrad
+    torchopt.optim.meta.MetaAdagrad
     torchopt.optim.meta.MetaAdam
     torchopt.optim.meta.MetaAdamW
     torchopt.optim.meta.MetaRMSProp
     torchopt.optim.meta.MetaRMSprop
     torchopt.optim.meta.MetaSGD
     torchopt.optim.Adam
     torchopt.optim.AdamW
     torchopt.optim.Optimizer
     torchopt.optim.RMSProp
     torchopt.optim.RMSprop
     torchopt.optim.SGD
     torchopt.optim.func.FuncOptimizer
     from torchopt import (
         SGD,
+        AdaGrad,
+        Adagrad,
         Adam,
         AdamW,
         FuncOptimizer,
+        MetaAdaGrad,
+        MetaAdagrad,
         MetaAdam,
         MetaAdamW,
         MetaOptimizer,
-        MetaRMSProp,
         MetaRMSprop,
+        MetaRMSProp,
         MetaSGD,
         Optimizer,
         RMSProp,
     )
     from torchopt.optim import SGD, Adam, AdamW, FuncOptimizer, Optimizer, RMSProp
     from torchopt.optim.func import FuncOptimizer
     from torchopt.optim.meta import (
+        MetaAdaGrad,
+        MetaAdagrad,
         MetaAdam,
         MetaAdamW,
         MetaOptimizer,
         MetaRMSProp,
         MetaRMSprop,
         MetaSGD,
     )
```

### Comparing `torchopt-0.7.0/tests/test_linalg.py` & `torchopt-0.7.1/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/tests/test_meta_optim.py` & `torchopt-0.7.1/tests/test_meta_optim.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/tests/test_nn.py` & `torchopt-0.7.1/tests/test_nn.py`

 * *Files 22% similar despite different names*

```diff
@@ -65,77 +65,149 @@
     m = torchopt.nn.MetaGradientModule(x)
     m.x = x
     m.y = y
     m.z = z
 
     assert m._meta_parameters['x'] is x
     assert m._parameters['y'] is y
-    assert hasattr(m, 'z') and m.z is z and 'z' not in m._buffers
+    assert (
+        hasattr(m, 'z')
+        and m.z is z
+        and 'z' not in m._meta_parameters
+        and 'z' not in m._parameters
+        and 'z' not in m._buffers
+    )
 
     del m.x
     object.__setattr__(m, 'x', x)
     assert hasattr(m, 'x') and m.x is x and 'x' not in m._meta_parameters
     m.x = x
     assert m._meta_parameters['x'] is x
 
     m.register_buffer('b', None)
     assert m.b is None
     m.b = b
     assert m.b is b and 'b' in m._buffers
 
+    m = torchopt.nn.MetaGradientModule(x, b)
+
+    with pytest.raises(
+        TypeError,
+        match=re.escape('parameter name should be a string. Got bytes'),
+    ):
+        m.register_meta_parameter(b'x', x)
+
+    with pytest.raises(
+        KeyError,
+        match=re.escape("parameter name can't contain '.'"),
+    ):
+        m.register_meta_parameter('x.x', x)
+
+    with pytest.raises(
+        KeyError,
+        match=re.escape("parameter name can't be empty string ''"),
+    ):
+        m.register_meta_parameter('', x)
+
+    m.register_buffer('z', None)
+    with pytest.raises(
+        KeyError,
+        match=re.escape("attribute 'z' already exists"),
+    ):
+        m.register_meta_parameter('z', x)
+
+    with pytest.raises(
+        ValueError,
+        match=re.escape(
+            "cannot assign Tensor that is a meta-parameter to parameter 'x'. "
+            'Use self.register_meta_parameter() instead.',
+        ),
+    ):
+        m.register_parameter('x', x)
+
+    m.x = x
+    with pytest.raises(
+        KeyError,
+        match=re.escape("attribute 'x' already exists"),
+    ):
+        m.register_parameter('x', x)
+
+    with pytest.raises(
+        TypeError,
+        match=re.escape('parameter name should be a string. Got bytes'),
+    ):
+        m.register_parameter(b'y', y)
+
+    with pytest.raises(
+        KeyError,
+        match=re.escape("parameter name can't contain '.'"),
+    ):
+        m.register_parameter('y.x', y)
+
+    with pytest.raises(
+        KeyError,
+        match=re.escape("parameter name can't be empty string ''"),
+    ):
+        m.register_parameter('', y)
+
 
 def test_no_super_init() -> None:
     class NoSuper1(torchopt.nn.MetaGradientModule):
-        def __init__(self, x):
+        def __init__(self, x) -> None:
             self.x = x
 
     with pytest.raises(
-        AttributeError, match=re.escape('cannot assign parameters before Module.__init__() call')
+        AttributeError,
+        match=re.escape('cannot assign parameters before Module.__init__() call'),
     ):
         NoSuper1(torch.tensor(1.0, requires_grad=True))
 
     class NoSuper2(torchopt.nn.MetaGradientModule):
-        def __init__(self):
+        def __init__(self) -> None:
             self.x = torch.tensor(1.0, requires_grad=True)
 
     with pytest.raises(
-        AttributeError, match=re.escape('cannot assign parameters before Module.__init__() call')
+        AttributeError,
+        match=re.escape('cannot assign parameters before Module.__init__() call'),
     ):
         NoSuper2()
 
     class NoSuper3(torchopt.nn.MetaGradientModule):
-        def __init__(self):
+        def __init__(self) -> None:
             self.register_buffer('x', torch.tensor(1.0))
 
     with pytest.raises(
-        AttributeError, match=re.escape('cannot assign buffer before Module.__init__() call')
+        AttributeError,
+        match=re.escape('cannot assign buffer before Module.__init__() call'),
     ):
         NoSuper3()
 
     class NoSuper4(torchopt.nn.MetaGradientModule):
-        def __init__(self):
+        def __init__(self) -> None:
             self.x = torch.tensor(1.0, requires_grad=False)
 
     NoSuper4()  # no error
 
     class NoSuper5(torchopt.nn.MetaGradientModule):
-        def __init__(self, x):
+        def __init__(self, x) -> None:
             self.x = x
 
     with pytest.raises(
-        AttributeError, match=re.escape('cannot assign module before Module.__init__() call')
+        AttributeError,
+        match=re.escape('cannot assign module before Module.__init__() call'),
     ):
         NoSuper5(nn.Linear(1, 1))
 
     class NoSuper6(torchopt.nn.MetaGradientModule):
-        def __init__(self):
+        def __init__(self) -> None:
             self.x = nn.Linear(1, 1)
 
     with pytest.raises(
-        AttributeError, match=re.escape('cannot assign module before Module.__init__() call')
+        AttributeError,
+        match=re.escape('cannot assign module before Module.__init__() call'),
     ):
         NoSuper6()
 
 
 def test_add_meta_module() -> None:
     meta_module = helpers.get_model()
     fc = nn.Linear(1, 1)
```

### Comparing `torchopt-0.7.0/tests/test_optim.py` & `torchopt-0.7.1/tests/test_optim.py`

 * *Files 11% similar despite different names*

```diff
@@ -267,14 +267,71 @@
 
     helpers.assert_model_all_close(model, model_ref, model_base, dtype=dtype)
 
 
 @helpers.parametrize(
     dtype=[torch.float64],
     lr=[1e-2, 1e-3, 1e-4],
+    lr_decay=[0.0, 1e-2],
+    initial_accumulator_value=[0.0, 1e-1],
+    eps=[1e-8],
+    weight_decay=[0.0, 1e-2],
+    maximize=[False, True],
+)
+def test_AdaGrad(
+    dtype: torch.dtype,
+    lr: float,
+    lr_decay: float,
+    initial_accumulator_value: float,
+    eps: float,
+    weight_decay: float,
+    maximize: bool,
+) -> None:
+    model, model_ref, model_base, loader = helpers.get_models(device='cpu', dtype=dtype)
+
+    optim = torchopt.AdaGrad(
+        model.parameters(),
+        lr=lr,
+        lr_decay=lr_decay,
+        weight_decay=weight_decay,
+        initial_accumulator_value=initial_accumulator_value,
+        eps=eps,
+        maximize=maximize,
+    )
+    optim_ref = torch.optim.Adagrad(
+        model_ref.parameters(),
+        lr=lr,
+        lr_decay=lr_decay,
+        weight_decay=weight_decay,
+        initial_accumulator_value=initial_accumulator_value,
+        eps=eps,
+        maximize=maximize,
+    )
+
+    for xs, ys in loader:
+        xs = xs.to(dtype=dtype)
+        pred = model(xs)
+        pred_ref = model_ref(xs)
+        loss = F.cross_entropy(pred, ys)
+        loss_ref = F.cross_entropy(pred_ref, ys)
+
+        optim.zero_grad()
+        loss.backward()
+        optim.step()
+
+        optim_ref.zero_grad()
+        loss_ref.backward()
+        optim_ref.step()
+
+    helpers.assert_model_all_close(model, model_ref, model_base, dtype=dtype)
+
+
+@helpers.parametrize(
+    dtype=[torch.float64],
+    lr=[1e-2, 1e-3, 1e-4],
     alpha=[0.9, 0.99],
     eps=[1e-8],
     momentum=[0.0, 0.1],
     centered=[False, True],
     weight_decay=[0.0, 1e-2],
 )
 def test_RMSProp(
@@ -326,45 +383,48 @@
     helpers.assert_model_all_close(model, model_ref, model_base, dtype=dtype)
 
 
 @helpers.parametrize(
     dtype=[torch.float64, torch.float32],
     lr=[1e-2, 1e-3],
     optimizers=[
-        (torchopt.sgd, torch.optim.SGD),
-        (torchopt.adam, torch.optim.Adam),
-        (torchopt.adamw, torch.optim.AdamW),
-        (torchopt.rmsprop, torch.optim.RMSprop),
+        (torchopt.sgd, torch.optim.SGD, {}),
+        (torchopt.adam, torch.optim.Adam, {}),
+        (torchopt.adamw, torch.optim.AdamW, {}),
+        (torchopt.adagrad, torch.optim.Adagrad, {'eps': 1e-8}),
+        (torchopt.rmsprop, torch.optim.RMSprop, {}),
     ],
     inplace=[True, False],
     weight_decay=[0.0, 1e-2],
 )
 def test_FuncOptimizer(
     dtype: torch.dtype,
     lr: float,
     optimizers: tuple[Callable, torch.optim.Optimizer],
     inplace: bool,
     weight_decay: float,
 ) -> None:
     model, model_ref, model_base, loader = helpers.get_models(device='cpu', dtype=dtype)
 
-    torchopt_optimizer, torch_optimizer = optimizers
+    torchopt_optimizer, torch_optimizer, optimizer_kwargs = optimizers
 
     fmodel, params, buffers = functorch.make_functional_with_buffers(model)
     optim = torchopt.FuncOptimizer(
         torchopt_optimizer(
             lr=lr,
             weight_decay=weight_decay,
+            **optimizer_kwargs,
         ),
         inplace=inplace,
     )
     optim_ref = torch_optimizer(
         model_ref.parameters(),
         lr,
         weight_decay=weight_decay,
+        **optimizer_kwargs,
     )
 
     for xs, ys in loader:
         xs = xs.to(dtype=dtype)
         pred = fmodel(params, buffers, xs)
         pred_ref = model_ref(xs)
         loss = F.cross_entropy(pred, ys)
```

### Comparing `torchopt-0.7.0/tests/test_pytree.py` & `torchopt-0.7.1/tests/test_pytree.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,42 +173,45 @@
     tensor_a_complex = torch.randn(20, dtype=torch.cfloat)
     tensor_b_complex = torch.randn(20, dtype=torch.cfloat)
     expected = torch.vdot(tensor_a_complex, tensor_b_complex).real
     actual = torch.tensor(pytree.tree_vdot_real(tensor_a_complex, tensor_b_complex))
     helpers.assert_pytree_all_close(actual, expected)
 
     tree_a_complex, tree_b_complex = pytree.tree_map(
-        lambda x: torch.randn(x.size(), dtype=torch.cfloat), (tree_a, tree_b)
+        lambda x: torch.randn(x.size(), dtype=torch.cfloat),
+        (tree_a, tree_b),
     )
     expected = (
         torch.vdot(tree_a_complex[0].contiguous().view(-1), tree_b_complex[0].contiguous().view(-1))
         + torch.vdot(
-            tree_a_complex[1].contiguous().view(-1), tree_b_complex[1].contiguous().view(-1)
+            tree_a_complex[1].contiguous().view(-1),
+            tree_b_complex[1].contiguous().view(-1),
         )
     ).real
     actual = torch.tensor(pytree.tree_vdot_real(tree_a_complex, tree_b_complex))
     helpers.assert_all_close(actual, expected)
 
 
 @helpers.parametrize(
     tree_name=[
         'tree_a',
         'tree_b',
         'tree_a_dict',
         'tree_b_dict',
         'tensor_a',
         'tensor_b',
-    ]
+    ],
 )
 def test_tree_wait(tree_name: str) -> None:
     tree = globals()[tree_name]
 
     future_tree = pytree.tree_map(lambda x: torch.futures.Future(), tree)
     new_future_tree = pytree.tree_map(
-        lambda fut: fut.then(lambda f: torch.square(f.wait()) + 1.0), future_tree
+        lambda fut: fut.then(lambda f: torch.square(f.wait()) + 1.0),
+        future_tree,
     )
     pytree.tree_map_(lambda fut, x: fut.set_result(x), future_tree, tree)
 
     expected = pytree.tree_map(lambda x: torch.square(x) + 1.0, tree)
     actual = pytree.tree_wait(new_future_tree)
     assert all(fut.done() for fut in pytree.tree_leaves(new_future_tree))
     helpers.assert_pytree_all_close(actual, expected)
```

### Comparing `torchopt-0.7.0/tests/test_transform.py` & `torchopt-0.7.1/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/tests/test_utils.py` & `torchopt-0.7.1/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     for param_dict in state_dict.params:
         for k, v in param_dict.items():
             assert v.is_meta
             assert v.grad_fn.next_functions[0][0].next_functions[0][0].variable is fc._parameters[k]
 
     state_dict = torchopt.extract_state_dict(fc, by='deepcopy', device=torch.device('meta'))
     for param_dict in state_dict.params:
-        for k, v in param_dict.items():
+        for v in param_dict.values():
             assert v.is_meta
             assert v.grad_fn is None
 
     state_dict = torchopt.extract_state_dict(fc, by='reference')
     for param_dict in state_dict.params:
         for k, v in param_dict.items():
             assert v is fc._parameters[k]
```

### Comparing `torchopt-0.7.0/torchopt/_C/adam_op.pyi` & `torchopt-0.7.1/torchopt/_C/adam_op.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 # pylint: disable=all
 
-from __future__ import annotations
-
 import torch
 
 def forward_(
     updates: torch.Tensor,
     mu: torch.Tensor,
     nu: torch.Tensor,
     b1: float,
@@ -37,18 +35,24 @@
     b1: float,
     b2: float,
     eps: float,
     eps_root: float,
     count: int,
 ) -> torch.Tensor: ...
 def backward_mu(
-    dmu: torch.Tensor, updates: torch.Tensor, mu: torch.Tensor, b1: float
+    dmu: torch.Tensor,
+    updates: torch.Tensor,
+    mu: torch.Tensor,
+    b1: float,
 ) -> tuple[torch.Tensor, torch.Tensor]: ...
 def backward_nu(
-    dnu: torch.Tensor, updates: torch.Tensor, nu: torch.Tensor, b2: float
+    dnu: torch.Tensor,
+    updates: torch.Tensor,
+    nu: torch.Tensor,
+    b2: float,
 ) -> tuple[torch.Tensor, torch.Tensor]: ...
 def backward_updates(
     dupdates: torch.Tensor,
     updates: torch.Tensor,
     new_mu: torch.Tensor,
     new_nu: torch.Tensor,
     b1: float,
```

### Comparing `torchopt-0.7.0/torchopt/__init__.py` & `torchopt-0.7.1/torchopt/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,21 +29,23 @@
     optim,
     pytree,
     schedule,
     typing,
     visual,
 )
 from torchopt.accelerated_op import is_available as accelerated_op_available
-from torchopt.alias import adam, adamw, rmsprop, sgd
+from torchopt.alias import adagrad, adam, adamw, rmsprop, sgd
 from torchopt.clip import clip_grad_norm
 from torchopt.combine import chain
 from torchopt.hook import register_hook
-from torchopt.optim import SGD, Adam, AdamW, Optimizer, RMSProp, RMSprop
+from torchopt.optim import SGD, AdaGrad, Adagrad, Adam, AdamW, Optimizer, RMSProp, RMSprop
 from torchopt.optim.func import FuncOptimizer
 from torchopt.optim.meta import (
+    MetaAdaGrad,
+    MetaAdagrad,
     MetaAdam,
     MetaAdamW,
     MetaOptimizer,
     MetaRMSProp,
     MetaRMSprop,
     MetaSGD,
 )
@@ -59,30 +61,35 @@
 from torchopt.version import __version__
 
 
 __all__ = [
     'accelerated_op_available',
     'adam',
     'adamw',
+    'adagrad',
     'rmsprop',
     'sgd',
     'clip_grad_norm',
     'nan_to_num',
     'register_hook',
     'chain',
     'Optimizer',
     'SGD',
     'Adam',
     'AdamW',
+    'AdaGrad',
+    'Adagrad',
     'RMSProp',
     'RMSprop',
     'MetaOptimizer',
     'MetaSGD',
     'MetaAdam',
     'MetaAdamW',
+    'MetaAdaGrad',
+    'MetaAdagrad',
     'MetaRMSProp',
     'MetaRMSprop',
     'FuncOptimizer',
     'apply_updates',
     'extract_state_dict',
     'recover_state_dict',
     'stop_gradient',
```

### Comparing `torchopt-0.7.0/torchopt/accelerated_op/__init__.py` & `torchopt-0.7.1/torchopt/accelerated_op/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,9 +39,9 @@
         for device in devices:
             device = torch.device(device)
             if device.type == 'cuda' and not torch.cuda.is_available():
                 return False
             updates = torch.tensor(1.0, device=device)
             op(updates, updates, updates, 1)
         return True
-    except Exception:  # pylint: disable=broad-except
+    except Exception:  # noqa: BLE001 # pylint: disable=broad-except
         return False
```

### Comparing `torchopt-0.7.0/torchopt/accelerated_op/_src/__init__.py` & `torchopt-0.7.1/torchopt/accelerated_op/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/torchopt/accelerated_op/_src/adam_op.py` & `torchopt-0.7.1/torchopt/accelerated_op/_src/adam_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     count: int,
 ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
     """Adam forward inplace."""
     mu = mu.mul_(b1).add_(updates, alpha=1.0 - b1)
     nu = nu.mul_(b2).addcmul_(updates, updates, value=1.0 - b2)
     updates.copy_(
         mu.div(1.0 - pow(b1, count)).div_(
-            nu.div(1.0 - pow(b2, count)).add_(eps_root).sqrt_().add_(eps)
-        )
+            nu.div(1.0 - pow(b2, count)).add_(eps_root).sqrt_().add_(eps),
+        ),
     )
     return updates, mu, nu
 
 
 def forward_mu(
     updates: torch.Tensor,
     mu: torch.Tensor,
@@ -67,15 +67,15 @@
     b2: float,
     eps: float,
     eps_root: float,
     count: int,
 ) -> torch.Tensor:
     """Adam forward updates."""
     return new_mu.div(1.0 - pow(b1, count)).div_(
-        new_nu.div(1.0 - pow(b2, count)).add_(eps_root).sqrt_().add_(eps)
+        new_nu.div(1.0 - pow(b2, count)).add_(eps_root).sqrt_().add_(eps),
     )
 
 
 def backward_mu(
     dmu: torch.Tensor,
     updates: torch.Tensor,
     mu: torch.Tensor,
```

### Comparing `torchopt-0.7.0/torchopt/accelerated_op/adam_op.py` & `torchopt-0.7.1/torchopt/accelerated_op/adam_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,22 @@
         def backward(ctx: Any, *args: Any) -> Any:
             # pylint: disable-next=line-too-long
             """Define a formula for differentiating the operation with backward mode automatic differentiation (alias to the :meth:`vjp` function)."""
             dupdates = args[0]
             updates, new_mu, new_nu = ctx.saved_tensors
             b1, b2, _, eps_root, count = ctx.others
             result = adam_op.backward_updates(
-                dupdates, updates, new_mu, new_nu, b1, b2, eps_root, count
+                dupdates,
+                updates,
+                new_mu,
+                new_nu,
+                b1,
+                b2,
+                eps_root,
+                count,
             )
             return result[0], result[1], None
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         b1: float = 0.9,
```

### Comparing `torchopt-0.7.0/torchopt/alias/__init__.py` & `torchopt-0.7.1/torchopt/alias/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 MetaOPT Team. All Rights Reserved.
+# Copyright 2022-2023 MetaOPT Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -27,14 +27,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 r"""The aliases of preset :class:`GradientTransformation`\s for optimizers."""
 
+from torchopt.alias.adagrad import adagrad
 from torchopt.alias.adam import adam
 from torchopt.alias.adamw import adamw
 from torchopt.alias.rmsprop import rmsprop
 from torchopt.alias.sgd import sgd
 
 
-__all__ = ['adam', 'adamw', 'rmsprop', 'sgd']
+__all__ = ['adagrad', 'adam', 'adamw', 'rmsprop', 'sgd']
```

### Comparing `torchopt-0.7.0/torchopt/alias/adam.py` & `torchopt-0.7.1/torchopt/alias/adam.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     """Create a functional version of the Adam optimizer.
 
     Adam is an SGD variant with learning rate adaptation. The *learning rate* used for each weight
     is computed from estimates of first- and second-order moments of the gradients (using suitable
     exponential moving averages).
 
     References:
-        - Kingma et al, 2014: https://arxiv.org/abs/1412.6980
+        - Kingma et al., 2014: https://arxiv.org/abs/1412.6980
 
     Args:
         lr (float or callable, optional): This is a fixed global scaling factor or a learning rate
             scheduler. (default: :const:`1e-3`)
         betas (tuple of float, optional): Coefficients used for computing running averages of
             gradient and its square. (default: :const:`(0.9, 0.999)`)
         eps (float, optional): A small constant applied to denominator outside of the square root
@@ -92,32 +92,29 @@
         The corresponding :class:`GradientTransformation` instance.
 
     See Also:
         The functional optimizer wrapper :class:`torchopt.FuncOptimizer`.
     """
     b1, b2 = betas  # pylint: disable=invalid-name
     # pylint: disable=unneeded-not
-    if not (callable(lr) or 0.0 <= lr):  # pragma: no cover
+    if not (callable(lr) or lr >= 0.0):  # pragma: no cover
         raise ValueError(f'Invalid learning rate: {lr}')
-    if not 0.0 <= eps:  # pragma: no cover
+    if not eps >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid epsilon value: {eps}')
     if not 0.0 <= b1 < 1.0:  # pragma: no cover
         raise ValueError(f'Invalid beta parameter at index 0: {b1}')
     if not 0.0 <= b2 < 1.0:  # pragma: no cover
         raise ValueError(f'Invalid beta parameter at index 1: {b2}')
-    if not 0.0 <= weight_decay:  # pragma: no cover
+    if not weight_decay >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid weight_decay value: {weight_decay}')
     # pylint: enable=unneeded-not
 
     chain_fn = chain
     flip_sign_and_add_weight_decay_fn = flip_sign_and_add_weight_decay
-    if use_accelerated_op:
-        adam_scaler_fn = scale_by_accelerated_adam
-    else:
-        adam_scaler_fn = scale_by_adam
+    adam_scaler_fn = scale_by_accelerated_adam if use_accelerated_op else scale_by_adam
     scale_by_neg_lr_fn = scale_by_neg_lr
 
     if _get_use_chain_flat():  # default behavior
         chain_fn = chain_fn.flat  # type: ignore[attr-defined]
         flip_sign_and_add_weight_decay_fn = flip_sign_and_add_weight_decay_fn.flat  # type: ignore[attr-defined]
         adam_scaler_fn = adam_scaler_fn.flat  # type: ignore[attr-defined]
         scale_by_neg_lr_fn = scale_by_neg_lr_fn.flat  # type: ignore[attr-defined]
```

### Comparing `torchopt-0.7.0/torchopt/alias/adamw.py` & `torchopt-0.7.1/torchopt/alias/adamw.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,27 +65,27 @@
 
     AdamW uses weight decay to regularize learning towards small weights, as
     this leads to better generalization. In SGD you can also use L2 regularization
     to implement this as an additive loss term, however L2 regularization
     does not behave as intended for adaptive gradient algorithms such as Adam.
 
     References:
-        - Loshchilov et al, 2019: https://arxiv.org/abs/1711.05101
+        - Loshchilov et al., 2019: https://arxiv.org/abs/1711.05101
 
     Args:
         lr (float or callable, optional): This is a fixed global scaling factor or a learning rate
             scheduler. (default: :const:`1e-3`)
         betas (tuple of float, optional): Coefficients used for computing running averages of
             gradient and its square. (default: :const:`(0.9, 0.999)`)
         eps (float, optional): A small constant applied to denominator outside of the square root
             (as in the Adam paper) to avoid dividing by zero when rescaling.
             (default: :const:`1e-8`)
         weight_decay (float, optional): Strength of the weight decay regularization. Note that this
             weight decay is multiplied with the learning rate. This is consistent with other
-            frameworks such as PyTorch, but different from (Loshchilov et al, 2019) where the weight
+            frameworks such as PyTorch, but different from (Loshchilov et al., 2019) where the weight
             decay is only multiplied with the "schedule multiplier", but not the base learning rate.
             (default: :const:`1e-2`)
         eps_root (float, optional): A small constant applied to denominator inside the square root
             (as in RMSProp), to avoid dividing by zero when rescaling. This is needed for example
             when computing (meta-)gradients through Adam. (default: :const:`0.0`)
         mask (tree of Tensor, callable, or None, optional):
             A tree with same structure as (or a prefix of) the params pytree, or a function that
@@ -105,32 +105,29 @@
         The corresponding :class:`GradientTransformation` instance.
 
     See Also:
         The functional optimizer wrapper :class:`torchopt.FuncOptimizer`.
     """
     b1, b2 = betas  # pylint: disable=invalid-name
     # pylint: disable=unneeded-not
-    if not (callable(lr) or 0.0 <= lr):  # pragma: no cover
+    if not (callable(lr) or lr >= 0.0):  # pragma: no cover
         raise ValueError(f'Invalid learning rate: {lr}')
-    if not 0.0 <= eps:  # pragma: no cover
+    if not eps >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid epsilon value: {eps}')
     if not 0.0 <= b1 < 1.0:  # pragma: no cover
         raise ValueError(f'Invalid beta parameter at index 0: {b1}')
     if not 0.0 <= b2 < 1.0:  # pragma: no cover
         raise ValueError(f'Invalid beta parameter at index 1: {b2}')
-    if not 0.0 <= weight_decay:  # pragma: no cover
+    if not weight_decay >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid weight_decay value: {weight_decay}')
     # pylint: enable=unneeded-not
 
     chain_fn = chain
     flip_sign_and_add_weight_decay_fn = flip_sign_and_add_weight_decay
-    if use_accelerated_op:
-        adam_scaler_fn = scale_by_accelerated_adam
-    else:
-        adam_scaler_fn = scale_by_adam
+    adam_scaler_fn = scale_by_accelerated_adam if use_accelerated_op else scale_by_adam
     add_decayed_weights_fn = add_decayed_weights
     scale_by_neg_lr_fn = scale_by_neg_lr
 
     if _get_use_chain_flat():  # default behavior
         chain_fn = chain_fn.flat  # type: ignore[attr-defined]
         flip_sign_and_add_weight_decay_fn = flip_sign_and_add_weight_decay_fn.flat  # type: ignore[attr-defined]
         adam_scaler_fn = adam_scaler_fn.flat  # type: ignore[attr-defined]
```

### Comparing `torchopt-0.7.0/torchopt/alias/rmsprop.py` & `torchopt-0.7.1/torchopt/alias/rmsprop.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,32 +92,29 @@
     Returns:
         The corresponding :class:`GradientTransformation` instance.
 
     See Also:
         The functional optimizer wrapper :class:`torchopt.FuncOptimizer`.
     """
     # pylint: disable=unneeded-not
-    if not (callable(lr) or 0.0 <= lr):  # pragma: no cover
+    if not (callable(lr) or lr >= 0.0):  # pragma: no cover
         raise ValueError(f'Invalid learning rate: {lr}')
-    if not 0.0 <= alpha:  # pragma: no cover
+    if not alpha >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid alpha value: {alpha}')
-    if not 0.0 <= eps:  # pragma: no cover
+    if not eps >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid epsilon value: {eps}')
-    if not 0.0 <= momentum:  # pragma: no cover
+    if not momentum >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid momentum value: {momentum}')
-    if not 0.0 <= weight_decay:  # pragma: no cover
+    if not weight_decay >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid weight_decay value: {weight_decay}')
     # pylint: enable=unneeded-not
 
     chain_fn = chain
     flip_sign_and_add_weight_decay_fn = flip_sign_and_add_weight_decay
-    if centered:
-        rmsprop_scaler_fn = scale_by_stddev
-    else:
-        rmsprop_scaler_fn = scale_by_rms
+    rmsprop_scaler_fn = scale_by_stddev if centered else scale_by_rms
     trace_fn = trace
     scale_by_neg_lr_fn = scale_by_neg_lr
 
     if _get_use_chain_flat():  # default behavior
         chain_fn = chain_fn.flat  # type: ignore[attr-defined]
         flip_sign_and_add_weight_decay_fn = flip_sign_and_add_weight_decay_fn.flat  # type: ignore[attr-defined]
         rmsprop_scaler_fn = rmsprop_scaler_fn.flat  # type: ignore[attr-defined]
```

### Comparing `torchopt-0.7.0/torchopt/alias/sgd.py` & `torchopt-0.7.1/torchopt/alias/sgd.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     """Create a functional version of the canonical Stochastic Gradient Descent optimizer.
 
     This implements stochastic gradient descent. It also includes support for momentum, and nesterov
     acceleration, as these are standard practice when using stochastic gradient descent to train
     deep neural networks.
 
     References:
-        - Sutskever et al, 2013: http://proceedings.mlr.press/v28/sutskever13.pdf
+        - Sutskever et al., 2013: http://proceedings.mlr.press/v28/sutskever13.pdf
 
     Args:
         lr (float or callable): This is a fixed global scaling factor or a learning rate
             scheduler.
         momentum (float, optional): The decay rate used by the momentum term. The momentum is not
             used when it is set to :const:`0.0`. (default: :const:`0.0`)
         weight_decay (float, optional): Weight decay, add L2 penalty to parameters.
@@ -81,19 +81,19 @@
     Returns:
         The corresponding :class:`GradientTransformation` instance.
 
     See Also:
         The functional optimizer wrapper :class:`torchopt.FuncOptimizer`.
     """
     # pylint: disable=unneeded-not
-    if not (callable(lr) or 0.0 <= lr):  # pragma: no cover
+    if not (callable(lr) or lr >= 0.0):  # pragma: no cover
         raise ValueError(f'Invalid learning rate: {lr}')
-    if not 0.0 <= momentum:  # pragma: no cover
+    if not momentum >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid momentum value: {momentum}')
-    if not 0.0 <= weight_decay:  # pragma: no cover
+    if not weight_decay >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid weight_decay value: {weight_decay}')
     if nesterov and (momentum <= 0.0 or dampening != 0.0):  # pragma: no cover
         raise ValueError('Nesterov momentum requires a momentum and zero dampening')
     # pylint: enable=unneeded-not
 
     chain_fn = chain
     flip_sign_and_add_weight_decay_fn = flip_sign_and_add_weight_decay
```

### Comparing `torchopt-0.7.0/torchopt/alias/utils.py` & `torchopt-0.7.1/torchopt/alias/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 # limitations under the License.
 r"""Utilities for the aliases of preset :class:`GradientTransformation`\s for optimizers."""
 
 from __future__ import annotations
 
 import threading
 
+import torch
+
 from torchopt import pytree
 from torchopt.base import EmptyState, GradientTransformation, identity
 from torchopt.transform import scale, scale_by_schedule
 from torchopt.transform.utils import tree_map_flat, tree_map_flat_
-from torchopt.typing import OptState, Params, ScalarOrSchedule, Updates
+from torchopt.typing import Numeric, OptState, Params, ScalarOrSchedule, Updates
 
 
 __all__ = ['flip_sign_and_add_weight_decay', 'scale_by_neg_lr']
 
 
 __USE_CHAIN_FLAT_LOCK = threading.Lock()
 __USE_CHAIN_FLAT = True
@@ -39,44 +41,46 @@
 
 def _get_use_chain_flat() -> bool:  # only used for testing purposes
     with __USE_CHAIN_FLAT_LOCK:
         return __USE_CHAIN_FLAT
 
 
 def flip_sign_and_add_weight_decay(
-    weight_decay: float = 0.0, maximize=False
+    weight_decay: float = 0.0,
+    maximize: bool = False,
 ) -> GradientTransformation:
     """Flip the sign of the updates and adds weight decay."""
     return _flip_sign_and_add_weight_decay(
         weight_decay=weight_decay,
         maximize=maximize,
         already_flattened=False,
     )
 
 
 def _flip_sign_and_add_weight_decay_flat(
-    weight_decay: float = 0.0, maximize=False
+    weight_decay: float = 0.0,
+    maximize: bool = False,
 ) -> GradientTransformation:
     """Flip the sign of the updates and adds weight decay."""
     return _flip_sign_and_add_weight_decay(
         weight_decay=weight_decay,
         maximize=maximize,
         already_flattened=True,
     )
 
 
 def _flip_sign_and_add_weight_decay(
     weight_decay: float = 0.0,
-    maximize=False,
+    maximize: bool = False,
     *,
     already_flattened: bool = False,
 ) -> GradientTransformation:
     """Flip the sign of the updates and adds weight decay."""
     # pylint: disable-next=unneeded-not
-    if not 0.0 <= weight_decay:  # pragma: no cover
+    if not weight_decay >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid weight_decay value: {weight_decay}')
 
     if not maximize and weight_decay == 0.0:
         return identity()
 
     if already_flattened:
         tree_map = tree_map_flat
@@ -100,24 +104,24 @@
             assert params is not None, (
                 'Parameters are required for weight decay. '
                 'Call `update(updates, state, params=params)` instead.'
             )
 
             if inplace:
 
-                def f(g, p):
+                def f(g: torch.Tensor, p: torch.Tensor) -> torch.Tensor:
                     if g.requires_grad:
                         return g.add_(p, alpha=weight_decay)
                     return g.add_(p.data, alpha=weight_decay)
 
                 updates = tree_map_(f, updates, params)
 
             else:
 
-                def f(g, p):
+                def f(g: torch.Tensor, p: torch.Tensor) -> torch.Tensor:
                     return g.add(p, alpha=weight_decay)
 
                 updates = tree_map(f, updates, params)
 
             return updates, state
 
     else:  # gradient ascent
@@ -128,22 +132,22 @@
                 state: OptState,
                 *,
                 params: Params | None = None,  # pylint: disable=unused-argument
                 inplace: bool = True,
             ) -> tuple[Updates, OptState]:
                 if inplace:
 
-                    def f(g):
+                    def f(g: torch.Tensor) -> torch.Tensor:
                         return g.neg_()
 
                     updates = tree_map_(f, updates)
 
                 else:
 
-                    def f(g):
+                    def f(g: torch.Tensor) -> torch.Tensor:
                         return g.neg()
 
                     updates = tree_map(f, updates)
 
                 return updates, state
 
         else:
@@ -158,24 +162,24 @@
                 assert params is not None, (
                     'Parameters are required for weight decay. '
                     'Call `update(updates, state, params=params)` instead.'
                 )
 
                 if inplace:
 
-                    def f(g, p):
+                    def f(g: torch.Tensor, p: torch.Tensor) -> torch.Tensor:
                         if g.requires_grad:
                             return g.neg_().add_(p, alpha=weight_decay)
                         return g.neg_().add_(p.data, alpha=weight_decay)
 
                     updates = tree_map_(f, updates, params)
 
                 else:
 
-                    def f(g, p):
+                    def f(g: torch.Tensor, p: torch.Tensor) -> torch.Tensor:
                         return g.neg().add_(p, alpha=weight_decay)
 
                     updates = tree_map(f, updates, params)
 
                 return updates, state
 
     return GradientTransformation(init_fn, update_fn)
@@ -190,21 +194,25 @@
     return _scale_by_neg_lr(lr=lr, already_flattened=False)
 
 
 def _scale_by_neg_lr_flat(lr: ScalarOrSchedule) -> GradientTransformation:
     return _scale_by_neg_lr(lr=lr, already_flattened=True)
 
 
-def _scale_by_neg_lr(lr: ScalarOrSchedule, *, already_flattened=False) -> GradientTransformation:
-    if not (callable(lr) or 0.0 <= lr):  # pragma: no cover
+def _scale_by_neg_lr(
+    lr: ScalarOrSchedule,
+    *,
+    already_flattened: bool = False,
+) -> GradientTransformation:
+    if not (callable(lr) or lr >= 0.0):  # pragma: no cover
         raise ValueError(f'Invalid learning rate: {lr}')
 
     if callable(lr):
 
-        def schedule_wrapper(count):
+        def schedule_wrapper(count: Numeric) -> Numeric:
             return -lr(count)  # type: ignore[operator]
 
         return scale_by_schedule.impl(  # type: ignore[attr-defined]
             schedule_wrapper,
             already_flattened=already_flattened,
         )
     return scale.impl(-lr, already_flattened=already_flattened)  # type: ignore[attr-defined]
```

### Comparing `torchopt-0.7.0/torchopt/base.py` & `torchopt-0.7.1/torchopt/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,18 @@
 # ==============================================================================
 """The base classes for gradient transformation."""
 
 from __future__ import annotations
 
 import itertools
 from abc import abstractmethod
-from typing import TYPE_CHECKING, Callable, NamedTuple
-from typing_extensions import Protocol  # Python 3.8+
+from typing import TYPE_CHECKING, Callable, NamedTuple, Protocol
 
 
-if TYPE_CHECKING:  # pragma: no cover
+if TYPE_CHECKING:
     from torchopt.typing import OptState, Params, Updates
 
 
 __all__ = [
     'EmptyState',
     'UninitializedState',
     'GradientTransformation',
@@ -164,15 +163,15 @@
         """Create a new chained gradient transformation."""
         transformations = tuple(
             itertools.chain.from_iterable(
                 t.transformations
                 if isinstance(t, ChainedGradientTransformation)
                 else ((t,) if not isinstance(t, IdentityGradientTransformation) else ())
                 for t in transformations
-            )
+            ),
         )
 
         if len(transformations) == 0:
             transformations = (IdentityGradientTransformation(),)
 
         init_fns, update_fns = tuple(zip(*transformations))
 
@@ -185,15 +184,15 @@
             *,
             params: Params | None = None,
             inplace: bool = True,
         ) -> tuple[Updates, OptState]:
             if len(update_fns) != len(state):
                 raise ValueError(
                     'The number of updates and states has to be the same in chain! Make sure you'
-                    'have called init first!'
+                    'have called init first!',
                 )
             new_state = []
             for s, fn in zip(state, update_fns):  # pylint: disable=invalid-name
                 updates, new_s = fn(updates, s, params=params, inplace=inplace)
                 new_state.append(new_s)
             return updates, tuple(new_state)
 
@@ -232,15 +231,15 @@
         """Serialize the chained gradient transformation."""
         return ChainedGradientTransformation, (self.transformations,)
 
 
 class IdentityGradientTransformation(GradientTransformation):
     """A gradient transformation that does nothing."""
 
-    def __new__(cls):
+    def __new__(cls) -> IdentityGradientTransformation:
         """Create a new gradient transformation that does nothing."""
         return super().__new__(cls, init=cls.init_fn, update=cls.update_fn)
 
     @staticmethod
     def init_fn(params: Params) -> OptState:  # pylint: disable=unused-argument
         """Return empty state."""
         return EmptyState()
```

### Comparing `torchopt-0.7.0/torchopt/clip.py` & `torchopt-0.7.1/torchopt/clip.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,29 +74,29 @@
                     torch.stack([torch.norm(p, norm_type).to(device) for p in available_updates]),
                     norm_type,
                 )
             if error_if_nonfinite and torch.logical_or(total_norm.isnan(), total_norm.isinf()):
                 raise RuntimeError(
                     f'The total norm of order {norm_type} for gradients from `parameters` is '
                     f'non-finite, so it cannot be clipped. To disable this error and scale the '
-                    f'gradients by the non-finite norm anyway, set `error_if_nonfinite=False`'
+                    f'gradients by the non-finite norm anyway, set `error_if_nonfinite=False`',
                 )
         clip_coefficient = max_norm / (float(total_norm) + 1e-6)
         # Note: multiplying by the clamped coefficient is redundant when the coefficient is
         # clamped to 1, but doing so avoids a `if clip_coefficient < 1:` conditional which
         # can require a CPU <=> device synchronization when the gradients do not reside in
         # CPU memory.
         clip_coefficient_clamped = min(clip_coefficient, 1.0)
         if inplace:
 
-            def f(g):
+            def f(g: torch.Tensor) -> torch.Tensor:
                 return g.mul_(clip_coefficient_clamped)
 
         else:
 
-            def f(g):
+            def f(g: torch.Tensor) -> torch.Tensor:
                 return g.mul(clip_coefficient_clamped)
 
         new_updates = pytree.tree_map(f, updates)
         return new_updates, state
 
     return GradientTransformation(init_fn, update_fn)
```

### Comparing `torchopt-0.7.0/torchopt/combine.py` & `torchopt-0.7.1/torchopt/combine.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,34 +70,28 @@
             ``(init_fn, update_fn)`` tuples.
 
     Returns:
         A single ``(init_fn, update_fn)`` tuple.
     """
     if len(transformations) == 0:
         return identity()
-    if len(transformations) == 1:
-        inner = transformations[0]
-    else:
-        inner = chain(*transformations)
+    inner = transformations[0] if len(transformations) == 1 else chain(*transformations)
 
     def init_fn(params: Params) -> OptState:
         return inner.init(pytree.tree_leaves(params, none_is_leaf=True))
 
     def update_fn(
         updates: Updates,
         state: OptState,
         *,
         params: Params | None = None,
         inplace: bool = True,
     ) -> tuple[Updates, OptState]:
         flat_updates, treespec = pytree.tree_flatten(updates, none_is_leaf=True)
-        if params is not None:
-            flat_params = pytree.tree_leaves(params, none_is_leaf=True)
-        else:
-            flat_params = None
+        flat_params = pytree.tree_leaves(params, none_is_leaf=True) if params is not None else None
 
         flat_updates, state = inner.update(flat_updates, state, params=flat_params, inplace=inplace)
         updates: Updates
         updates = pytree.tree_unflatten(treespec, flat_updates)
         return updates, state
 
     return GradientTransformation(init_fn, update_fn)
```

### Comparing `torchopt-0.7.0/torchopt/diff/__init__.py` & `torchopt-0.7.1/torchopt/diff/__init__.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/torchopt/diff/implicit/__init__.py` & `torchopt-0.7.1/torchopt/diff/implicit/__init__.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/torchopt/diff/implicit/decorator.py` & `torchopt-0.7.1/torchopt/diff/implicit/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 def _root_vjp(
     optimality_fn: Callable[..., TensorOrTensors],
     solution: TupleOfTensors,
     args: Args,
     grad_outputs: TupleOfTensors,
     output_is_tensor: bool,
     argnums: tuple[int, ...],
-    solve: Callable[..., TensorOrTensors] = linear_solve.solve_normal_cg(),
+    solve: Callable[..., TensorOrTensors],
 ) -> TupleOfOptionalTensors:
     if output_is_tensor:
 
         def optimality_cond(solution: TupleOfTensors) -> TensorOrTensors:
             return optimality_fn(solution[0], *args)
 
     else:
@@ -119,26 +119,28 @@
     # The solution of A^T u = v, where
     # A = jacobian(optimality_fn, argnums=0)
     # v = -grad_outputs.
     v: TupleOfTensors = pytree.tree_map(torch.neg, grad_outputs)  # type: ignore[arg-type,assignment]
     u: TupleOfTensors = solve(matvec, v)  # type: ignore[assignment]
 
     masked_optimality_fn = MaskedOptimalityFn(
-        optimality_fn, solution, output_is_tensor, argnums, *args
+        optimality_fn,
+        solution,
+        output_is_tensor,
+        argnums,
+        *args,
     )
 
     _, optimality_vjp_fn, *_ = functorch.vjp(
-        masked_optimality_fn, *masked_optimality_fn.post_filled
+        masked_optimality_fn,
+        *masked_optimality_fn.post_filled,
     )
 
     output: TupleOfTensors
-    if output_is_tensor:
-        output = optimality_vjp_fn(u[0])
-    else:
-        output = optimality_vjp_fn(u)
+    output = optimality_vjp_fn(u[0]) if output_is_tensor else optimality_vjp_fn(u)
 
     # Prepend None as the vjp for init_params.
     true_output: ListOfOptionalTensors = [None]
     for idx in range(masked_optimality_fn.len_args):
         if idx + 1 in argnums:  # plus 1 because we exclude the first argument
             true_output.append(output[idx])
         else:
@@ -157,15 +159,17 @@
 def _signature_bind(signature: inspect.Signature, *args: Any, **kwargs: Any) -> tuple[Args, KwArgs]:
     bound = signature.bind(*args, **kwargs)
     bound.apply_defaults()
     return bound.args, bound.kwargs
 
 
 def _signature_bind_and_match(
-    signature: inspect.Signature, *args: Any, **kwargs: Any
+    signature: inspect.Signature,
+    *args: Any,
+    **kwargs: Any,
 ) -> tuple[Args, KwArgs, Callable[[Args], tuple[Args, KwArgs]]]:
     # We want to bind *args and **kwargs based on the provided signature, but also to associate the
     # resulting positional arguments back. To achieve this, we lift arguments to a triple:
     #
     #   (was_kwarg, ref, value)
     #
     # where ref is an index position (int) if the original argument was from *args and a dictionary
@@ -175,23 +179,23 @@
 
     args = [(False, i, v) for i, v in enumerate(args)]
     kwargs = {k: (True, k, v) for (k, v) in kwargs.items()}
     bound = signature.bind(*args, **kwargs)
 
     mapping = [(was_kwarg, ref) for was_kwarg, ref, _ in bound.args]
 
-    def map_args_back(out_args):
+    def map_args_back(out_args: Args) -> tuple[Args, KwArgs]:
         src_args = [None] * len(args)
         src_kwargs = {}
         for (was_kwarg, ref), out_arg in zip(mapping, out_args):
             if was_kwarg:
                 src_kwargs[ref] = out_arg
             else:
                 src_args[ref] = out_arg
-        return src_args, src_kwargs
+        return tuple(src_args), src_kwargs
 
     out_args = tuple(v for _, _, v in bound.args)
     out_kwargs = {k: v for k, (_, _, v) in bound.kwargs.items()}
     return out_args, out_kwargs, map_args_back
 
 
 def _split_tensor_and_others(
@@ -255,15 +259,16 @@
         kwarg_keys: Sequence[str],
         args_signs: tuple[tuple[int, int, type[tuple] | type[list] | None], ...],
     ) -> type[Function]:
         # pylint: disable-next=missing-class-docstring,abstract-method
         class ImplicitMetaGradient(Function):
             @staticmethod
             def forward(  # type: ignore[override] # pylint: disable=arguments-differ
-                ctx: Any, *flat_args: Any
+                ctx: Any,
+                *flat_args: Any,
             ) -> tuple[Any, ...]:
                 output, aux, output_is_tensor = None, None, False
 
                 args = []
                 for offset, nargs, arg_seq_type in args_signs:
                     if arg_seq_type is not None:
                         args.append(arg_seq_type(flat_args[offset : offset + nargs]))
@@ -274,25 +279,25 @@
                 args, kwargs = _extract_kwargs(kwarg_keys, args)
                 output = solver_fn(*args, **kwargs)
                 if has_aux:
                     if not (isinstance(output, tuple) and len(output) == 2):
                         raise RuntimeError(
                             f'custom_root(optimality_fn)(solver_fn)(*args): output of function '
                             f'solver_fn should be a tuple: (output, aux) if has_aux is True. '
-                            f'Got {output}'
+                            f'Got {output}',
                         )
                     output, aux = output
                 if isinstance(output, torch.Tensor):
                     output_is_tensor = True
                     output = (output,)
                 elif not (isinstance(output, tuple) and all(map(torch.is_tensor, output))):
                     raise RuntimeError(
                         f'custom_root(optimality_fn)(solver_fn)(*args): output of function '
                         f'solver_fn should be a torch.Tensor or a tuple of torch.Tensor. '
-                        f'Got {output}'
+                        f'Got {output}',
                     )
                 output = tuple(t.data for t in output)
 
                 (
                     args_treespec,
                     args_is_tensor_mask,
                     args_tensors,
@@ -305,68 +310,75 @@
                 ctx.save_for_backward(*output, *args_tensors)
                 ctx.output_is_tensor = output_is_tensor
 
                 return (*output, aux, output_is_tensor, type(output))
 
             @staticmethod
             def backward(  # pylint: disable=too-many-locals
-                ctx: Any, *grad_outputs: Any
+                ctx: Any,
+                *grad_outputs: Any,
             ) -> TupleOfTensors:
                 grad_outputs: TupleOfTensors = grad_outputs[:-3]
 
                 saved_tensors = ctx.saved_tensors
                 output = saved_tensors[: len(grad_outputs)]
                 args_tensors = saved_tensors[len(grad_outputs) :]
                 args_treespec = ctx.args_treespec
                 args_is_tensor_mask = ctx.args_is_tensor_mask
                 args_non_tensors = ctx.args_non_tensors
                 args = _merge_tensor_and_others(
-                    args_treespec, args_is_tensor_mask, args_tensors, args_non_tensors
+                    args_treespec,
+                    args_is_tensor_mask,
+                    args_tensors,
+                    args_non_tensors,
                 )
 
                 args, kwargs = _extract_kwargs(kwarg_keys, args)
 
                 bound_args, bound_kwargs, map_args_back = _signature_bind_and_match(
-                    reference_signature, *args, **kwargs  # type: ignore[arg-type]
+                    reference_signature,  # type: ignore[arg-type]
+                    *args,
+                    **kwargs,
                 )
                 if bound_kwargs:
                     raise TypeError(
                         f'keyword arguments to solver_fn could not be resolved to positional '
                         f'arguments based on the signature {reference_signature}. This can '
                         f'happen under custom_root if optimality_fn takes catch-all **kwargs, or '
                         f'under custom_fixed_point if fixed_point_fn takes catch-all **kwargs, '
-                        f'both of which are currently unsupported.'
+                        f'both of which are currently unsupported.',
                     )
 
                 # Compute VJPs w.r.t. args.
                 vjps = _root_vjp(
                     optimality_fn=optimality_fn,
                     solution=output,
                     args=bound_args[1:],
                     grad_outputs=grad_outputs,
                     output_is_tensor=ctx.output_is_tensor,
                     argnums=argnums,
                     solve=solve,
                 )
 
                 args_vjps, kwargs_vjps = map_args_back(vjps)
-                ordered_vjps = tuple(args_vjps) + tuple(kwargs_vjps[k] for k in kwargs.keys())
+                ordered_vjps = tuple(args_vjps) + tuple(kwargs_vjps[k] for k in kwargs)
                 true_vjps = []
                 for (_, _, arg_seq_type), vjp in zip(args_signs, ordered_vjps):
                     if arg_seq_type is not None:
                         true_vjps.extend(vjp)
                     else:
                         true_vjps.append(vjp)
                 return tuple(true_vjps)
 
         return ImplicitMetaGradient
 
     @functools.wraps(solver_fn)
     def wrapped_solver_fn(
-        *args: Any, **kwargs: Any
+        *args: Any,
+        **kwargs: Any,
     ) -> TensorOrTensors | tuple[TensorOrTensors, Any]:
         args, kwargs = _signature_bind(solver_fn_signature, *args, **kwargs)
         keys, vals = list(kwargs.keys()), list(kwargs.values())
 
         args_signs: list[tuple[int, int, type[tuple] | type[list] | None]] = []
         flat_args: list[Any] = []
         args_offset = 0
@@ -375,50 +387,47 @@
                 if isinstance(arg, torch.Tensor):
                     args_signs.append((args_offset, 1, None))  # start position, None
                     flat_args.append(arg)
                     args_offset += 1
                 elif isinstance(arg, (tuple, list)) and all(map(torch.is_tensor, arg)):
                     nargs = len(arg)
                     args_signs.append(
-                        (args_offset, nargs, type(arg))  # start position, sequence type
+                        (args_offset, nargs, type(arg)),  # start position, sequence type
                     )
                     flat_args.extend(arg)
                     args_offset += nargs
                 else:
                     raise RuntimeError(
                         'custom_root(optimality_fn)(solver_fn)(*args): argument of function '
                         'solver_fn specified with `argnums` should be a torch.Tensor or a tuple of '
-                        'torch.Tensor'
+                        'torch.Tensor',
                     )
             else:
                 args_signs.append((args_offset, 1, None))  # start position, None
                 flat_args.append(arg)
                 args_offset += 1
 
         args_signs = tuple(args_signs)
         flat_args = tuple(flat_args)
 
         result = make_custom_vjp_solver_fn(solver_fn, keys, args_signs).apply(*flat_args, *vals)
         *output, aux, output_is_tensor, output_type = result
-        if output_is_tensor:
-            output = output[0]
-        else:
-            output = output_type(output)
+        output = output[0] if output_is_tensor else output_type(output)
         if has_aux:
             return output, aux
         return output
 
     return wrapped_solver_fn
 
 
 def custom_root(
     optimality_fn: Callable[..., TensorOrTensors],
     argnums: int | tuple[int, ...],
     has_aux: bool = False,
-    solve: Callable[..., TensorOrTensors] = linear_solve.solve_normal_cg(),
+    solve: Callable[..., TensorOrTensors] | None = None,
 ) -> Callable[
     [Callable[..., TensorOrTensors | tuple[TensorOrTensors, Any]]],
     Callable[..., TensorOrTensors | tuple[TensorOrTensors, Any]],
 ]:
     """Return a decorator for adding implicit differentiation to a root solver.
 
     This wrapper should be used as a decorator:
@@ -461,14 +470,17 @@
     """
     if isinstance(argnums, int):
         assert argnums != 0
         argnums = (argnums,)
     else:
         assert 0 not in argnums
 
+    if solve is None:
+        solve = linear_solve.solve_normal_cg()
+
     return functools.partial(
         _custom_root,
         optimality_fn=optimality_fn,
         solve=solve,
         argnums=argnums,
         has_aux=has_aux,
     )
```

### Comparing `torchopt-0.7.0/torchopt/diff/implicit/nn/__init__.py` & `torchopt-0.7.1/torchopt/diff/implicit/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/torchopt/diff/implicit/nn/module.py` & `torchopt-0.7.1/torchopt/diff/implicit/nn/module.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 # pylint: disable=redefined-builtin
 
 from __future__ import annotations
 
 import abc
 import functools
+import inspect
 import itertools
 from typing import Any, Iterable
 
 import functorch
 import torch
 
 from torchopt.diff.implicit.decorator import custom_root
@@ -32,203 +33,216 @@
 from torchopt.typing import LinearSolver, TupleOfTensors
 
 
 __all__ = ['ImplicitMetaGradientModule']
 
 
 def _stateless_objective_fn(
-    __flat_params: TupleOfTensors,
-    __flat_meta_params: TupleOfTensors,
-    __params_names: Iterable[str],
-    __meta_params_names: Iterable[str],
+    flat_params: TupleOfTensors,
+    flat_meta_params: TupleOfTensors,
+    params_names: Iterable[str],
+    meta_params_names: Iterable[str],
     self: ImplicitMetaGradientModule,
-    *input,
-    **kwargs,
+    /,
+    *input: Any,
+    **kwargs: Any,
 ) -> torch.Tensor:
     with reparametrize(
         self,
         itertools.chain(
-            zip(__params_names, __flat_params),
-            zip(__meta_params_names, __flat_meta_params),
+            zip(params_names, flat_params),
+            zip(meta_params_names, flat_meta_params),
         ),
     ):
         return self.objective(*input, **kwargs)
 
 
 def _stateless_optimality_fn(
-    __flat_params: TupleOfTensors,
-    __flat_meta_params: TupleOfTensors,
-    __params_names: Iterable[str],
-    __meta_params_names: Iterable[str],
+    flat_params: TupleOfTensors,
+    flat_meta_params: TupleOfTensors,
+    params_names: Iterable[str],
+    meta_params_names: Iterable[str],
     self: ImplicitMetaGradientModule,
-    *input,
-    **kwargs,
+    /,
+    *input: Any,
+    **kwargs: Any,
 ) -> TupleOfTensors:
     with reparametrize(
         self,
         itertools.chain(
-            zip(__params_names, __flat_params),
-            zip(__meta_params_names, __flat_meta_params),
+            zip(params_names, flat_params),
+            zip(meta_params_names, flat_meta_params),
         ),
     ):
         return self.optimality(*input, **kwargs)
 
 
 def make_optimality_from_objective(
     cls: type[ImplicitMetaGradientModule],
 ) -> type[ImplicitMetaGradientModule]:
-    """Derives the optimality function of the objective function."""
-    if (
-        getattr(cls, 'objective', ImplicitMetaGradientModule.objective)
-        is ImplicitMetaGradientModule.objective
-    ):
+    """Derive the optimality function of the objective function."""
+    static_super_objective = inspect.getattr_static(ImplicitMetaGradientModule, 'objective')
+    static_cls_objective = inspect.getattr_static(cls, 'objective', static_super_objective)
+    if static_cls_objective is static_super_objective:
         raise TypeError('The objective function is not defined.')
 
-    def optimality(self: ImplicitMetaGradientModule, *input, **kwargs) -> TupleOfTensors:
-        params_names, flat_params = tuple(zip(*self.named_parameters()))
-        meta_params_names, flat_meta_params = tuple(zip(*self.named_meta_parameters()))
+    def optimality(self: ImplicitMetaGradientModule, *input: Any, **kwargs: Any) -> TupleOfTensors:
+        named_params = tuple(self.named_parameters())
+        named_meta_params = tuple(self.named_meta_parameters())
+        if len(named_params) == 0:
+            raise RuntimeError('The module has no parameters.')
+        if len(named_meta_params) == 0:
+            raise RuntimeError('The module has no meta-parameters.')
+        params_names, flat_params = tuple(zip(*named_params))
+        meta_params_names, flat_meta_params = tuple(zip(*named_meta_params))
 
         objective_grad_fn = functorch.grad(_stateless_objective_fn, argnums=0)
-        flat_grads = objective_grad_fn(
+        return objective_grad_fn(
             flat_params,
             flat_meta_params,
             params_names,
             meta_params_names,
             self,
             *input,
             **kwargs,
         )
-        return flat_grads
 
-    cls.optimality = optimality  # type: ignore[assignment]
+    cls.optimality = optimality  # type: ignore[method-assign]
     return cls
 
 
 def enable_implicit_gradients(
     cls: type[ImplicitMetaGradientModule],
 ) -> type[ImplicitMetaGradientModule]:
     """Enable implicit gradients for the :func:`solve` method."""
     cls_solve = cls.solve
     if getattr(cls_solve, '__implicit_gradients_enabled__', False):
         raise TypeError('Implicit gradients are already enabled for the `solve` method.')
 
-    if cls.linear_solve is not None:
-        solve_kwargs = {'solve': cls.linear_solve}
-    else:
-        solve_kwargs = {}
+    solve_kwargs = {'solve': cls.linear_solve} if cls.linear_solve is not None else {}
 
     @custom_root(_stateless_optimality_fn, argnums=1, has_aux=True, **solve_kwargs)
     def stateless_solver_fn(
         # pylint: disable=unused-argument
-        __flat_params: TupleOfTensors,
-        __flat_meta_params: TupleOfTensors,
-        __params_names: Iterable[str],
-        __meta_params_names: Iterable[str],
+        flat_params: TupleOfTensors,
+        flat_meta_params: TupleOfTensors,
+        params_names: Iterable[str],
+        meta_params_names: Iterable[str],
         # pylint: enable=unused-argument
         self: ImplicitMetaGradientModule,
-        *input,
-        **kwargs,
+        /,
+        *input: Any,
+        **kwargs: Any,
     ) -> tuple[TupleOfTensors, Any]:
         """Solve the optimization problem."""
         output = cls_solve(self, *input, **kwargs)
         flat_optimal_params = tuple(p.detach_() for p in self.parameters())
         return flat_optimal_params, output
 
     @functools.wraps(cls_solve)
-    def wrapped(self: ImplicitMetaGradientModule, *input, **kwargs) -> Any:
+    def wrapped(self: ImplicitMetaGradientModule, *input: Any, **kwargs: Any) -> Any:
         """Solve the optimization problem."""
-        params_names, flat_params = tuple(zip(*self.named_parameters()))
-        meta_params_names, flat_meta_params = tuple(zip(*self.named_meta_parameters()))
+        named_params = tuple(self.named_parameters())
+        named_meta_params = tuple(self.named_meta_parameters())
+        if len(named_params) == 0:
+            raise RuntimeError('The module has no parameters.')
+        if len(named_meta_params) == 0:
+            raise RuntimeError('The module has no meta-parameters.')
+        params_names, flat_params = tuple(zip(*named_params))
+        meta_params_names, flat_meta_params = tuple(zip(*named_meta_params))
 
         flat_optimal_params, output = stateless_solver_fn(
             flat_params,
             flat_meta_params,
             params_names,
             meta_params_names,
             self,
             *input,
             **kwargs,
         )
         swap_state(self, zip(params_names, flat_optimal_params))
         return output
 
     wrapped.__implicit_gradients_enabled__ = True  # type: ignore[attr-defined]
-    cls.solve = wrapped  # type: ignore[assignment]
+    cls.solve = wrapped  # type: ignore[method-assign]
     return cls
 
 
-class ImplicitMetaGradientModule(MetaGradientModule):
+class ImplicitMetaGradientModule(MetaGradientModule, metaclass=abc.ABCMeta):
     """The base class for differentiable implicit meta-gradient models."""
 
     _custom_optimality: bool
     _custom_objective: bool
     linear_solve: LinearSolver | None
 
     def __init_subclass__(cls, linear_solve: LinearSolver | None = None) -> None:
         """Validate and initialize the subclass."""
         super().__init_subclass__()
         cls.linear_solve = linear_solve
 
-        optimality = getattr(cls, 'optimality', ImplicitMetaGradientModule.optimality)
-        objective = getattr(cls, 'objective', ImplicitMetaGradientModule.objective)
-        cls._custom_optimality = optimality is not ImplicitMetaGradientModule.optimality
-        cls._custom_objective = objective is not ImplicitMetaGradientModule.objective
+        static_super_optimality = inspect.getattr_static(ImplicitMetaGradientModule, 'optimality')
+        static_super_objective = inspect.getattr_static(ImplicitMetaGradientModule, 'objective')
+        static_cls_optimality = inspect.getattr_static(cls, 'optimality')
+        static_cls_objective = inspect.getattr_static(cls, 'objective')
+        cls._custom_optimality = static_cls_optimality is not static_super_optimality
+        cls._custom_objective = static_cls_objective is not static_super_objective
 
         if cls._custom_optimality:
-            if isinstance(optimality, staticmethod):
+            if isinstance(static_cls_optimality, staticmethod):
                 raise TypeError('method optimality() must not be a staticmethod.')
-            if isinstance(optimality, classmethod):
+            if isinstance(static_cls_optimality, classmethod):
                 raise TypeError('method optimality() must not be a classmethod.')
-            if not callable(optimality):
+            if not callable(static_cls_optimality):
                 raise TypeError('method optimality() must be callable.')
         elif not cls._custom_objective:
             raise TypeError(
-                'ImplicitMetaGradientModule requires either an optimality() method or an objective() method'
+                'ImplicitMetaGradientModule requires either an optimality() method or an objective() method',
             )
         else:
-            if isinstance(objective, staticmethod):
+            if isinstance(static_cls_objective, staticmethod):
                 raise TypeError('method objective() must not be a staticmethod.')
-            if isinstance(objective, classmethod):
+            if isinstance(static_cls_objective, classmethod):
                 raise TypeError('method objective() must not be a classmethod.')
-            if not callable(objective):
+            if not callable(static_cls_objective):
                 raise TypeError('method objective() must be callable.')
 
             make_optimality_from_objective(cls)
 
         enable_implicit_gradients(cls)
 
     @abc.abstractmethod
-    def solve(self, *input, **kwargs) -> Any:
+    def solve(self, *input: Any, **kwargs: Any) -> Any:
         """Solve the inner optimization problem.
 
         .. warning::
             For gradient-based optimization methods, the parameter inputs should be explicitly
             specified in the :func:`torch.autograd.backward` function as argument ``inputs``.
             Otherwise, if not provided, the gradient is accumulated into all the leaf Tensors
             (including the meta-parameters) that were used to compute the objective output.
             Alternatively, please use :func:`torch.autograd.grad` instead.
 
-        Example::
+        Examples:
+            .. code-block:: python
 
-            def solve(self, batch, labels):
-                parameters = tuple(self.parameters())
-                optimizer = torch.optim.Adam(parameters, lr=1e-3)
-                with torch.enable_grad():
-                    for _ in range(100):
-                        loss = self.objective(batch, labels)
-                        optimizer.zero_grad()
-                        # Only update the `.grad` attribute for parameters
-                        # and leave the meta-parameters unchanged
-                        loss.backward(inputs=parameters)
-                        optimizer.step()
-                return self
+                def solve(self, batch, labels):
+                    parameters = tuple(self.parameters())
+                    optimizer = torch.optim.Adam(parameters, lr=1e-3)
+                    with torch.enable_grad():
+                        for _ in range(100):
+                            loss = self.objective(batch, labels)
+                            optimizer.zero_grad()
+                            # Only update the `.grad` attribute for parameters
+                            # and leave the meta-parameters unchanged
+                            loss.backward(inputs=parameters)
+                            optimizer.step()
+                    return self
         """
         raise NotImplementedError  # update parameters
 
-    def optimality(self, *input, **kwargs) -> TupleOfTensors:
+    def optimality(self, *input: Any, **kwargs: Any) -> TupleOfTensors:
         r"""Compute the optimality residual.
 
         This method stands for the optimality residual to the optimal parameters after solving the
         inner optimization problem (:meth:`solve`), i.e.:
 
         .. code-block:: python
 
@@ -263,15 +277,15 @@
         Returns:
             A tuple of tensors, the optimality residual to the optimal parameters after solving the
             inner optimization problem. The returned tensors should correspond to the outputs of
             `tuple(self.parameters())`.
         """  # pylint: disable=line-too-long
         raise NotImplementedError
 
-    def objective(self, *input, **kwargs) -> torch.Tensor:
+    def objective(self, *input: Any, **kwargs: Any) -> torch.Tensor:
         """Compute the objective function value.
 
         This method is used to calculate the :meth:`optimality` if it is not implemented.
         Otherwise, this method is optional.
 
         Returns:
             A scalar tensor (``dim=0``), the objective function value.
```

### Comparing `torchopt-0.7.0/torchopt/diff/zero_order/__init__.py` & `torchopt-0.7.1/torchopt/diff/zero_order/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,25 +12,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Zero-Order Gradient."""
 
 import sys as _sys
 from types import ModuleType as _ModuleType
+from typing import Any, Callable
+
+import torch
 
 from torchopt.diff.zero_order import nn
 from torchopt.diff.zero_order.decorator import zero_order
 from torchopt.diff.zero_order.nn import ZeroOrderGradientModule
 
 
 __all__ = ['zero_order', 'ZeroOrderGradientModule']
 
 
 class _CallableModule(_ModuleType):  # pylint: disable=too-few-public-methods
-    def __call__(self, *args, **kwargs):
+    def __call__(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Callable[[Callable[..., torch.Tensor]], Callable[..., torch.Tensor]]:
         return self.zero_order(*args, **kwargs)
 
 
 # Replace entry in sys.modules for this module with an instance of _CallableModule
 _modself = _sys.modules[__name__]
 _modself.__class__ = _CallableModule
 del _sys, _ModuleType, _modself, _CallableModule
```

### Comparing `torchopt-0.7.0/torchopt/diff/zero_order/decorator.py` & `torchopt-0.7.1/torchopt/diff/zero_order/decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 """Zero-Order Gradient Estimation."""
 
 from __future__ import annotations
 
 import functools
-from typing import Any, Callable, Sequence
-from typing_extensions import Literal  # Python 3.8+
+from typing import Any, Callable, Literal, Sequence
 from typing_extensions import TypeAlias  # Python 3.10+
 
 import torch
 from torch.autograd import Function
 
 from torchopt import pytree
 from torchopt.typing import ListOfTensors, Numeric, Samplable, SampleFunc, TupleOfOptionalTensors
@@ -31,26 +30,29 @@
 class WrappedSamplable(Samplable):  # pylint: disable=too-few-public-methods
     """A wrapper that wraps a sample function to a :class:`Samplable` object."""
 
     def __init__(self, sample_fn: SampleFunc) -> None:
         """Wrap a sample function to make it a :class:`Samplable` object."""
         self.sample_fn = sample_fn
 
-    def sample(self, sample_shape: torch.Size = torch.Size()) -> torch.Tensor | Sequence[Numeric]:
+    def sample(
+        self,
+        sample_shape: torch.Size = torch.Size(),  # noqa: B008
+    ) -> torch.Tensor | Sequence[Numeric]:
         # pylint: disable-next=line-too-long
         """Generate a sample_shape shaped sample or sample_shape shaped batch of samples if the distribution parameters are batched."""
         return self.sample_fn(sample_shape)
 
 
 def _zero_order_naive(  # pylint: disable=too-many-statements
     fn: Callable[..., torch.Tensor],
     distribution: Samplable,
     argnums: tuple[int, ...],
     num_samples: int,
-    sigma: Numeric,
+    sigma: float,
 ) -> Callable[..., torch.Tensor]:
     @functools.wraps(fn)
     def apply(*args: Any) -> torch.Tensor:  # pylint: disable=too-many-statements
         diff_params = [args[argnum] for argnum in argnums]
         flat_diff_params: list[Any]
         flat_diff_params, diff_params_treespec = pytree.tree_flatten(diff_params)  # type: ignore[arg-type]
 
@@ -85,15 +87,16 @@
                 ctx.save_for_backward(*flat_diff_params, *tensors)
                 ctx.len_args = len(args)
                 ctx.len_params = len(flat_diff_params)
                 return output
 
             @staticmethod
             def backward(  # pylint: disable=too-many-locals
-                ctx: Any, *grad_outputs: Any
+                ctx: Any,
+                *grad_outputs: Any,
             ) -> TupleOfOptionalTensors:
                 saved_tensors = ctx.saved_tensors
                 flat_diff_params = saved_tensors[: ctx.len_params]
                 tensors = saved_tensors[ctx.len_params :]
                 non_tensors = ctx.non_tensors
 
                 flat_args = []
@@ -105,26 +108,30 @@
                         tensors_counter += 1
                     else:
                         flat_args.append(non_tensors[non_tensors_counter])
                         non_tensors_counter += 1
 
                 args: list[Any] = pytree.tree_unflatten(ctx.args_treespec, flat_args)  # type: ignore[assignment]
 
-                def add_perturbation(tensor, noises):
-                    return tensor.add(noises, alpha=sigma)
+                def add_perturbation(
+                    tensor: torch.Tensor,
+                    noise: torch.Tensor | Numeric,
+                ) -> torch.Tensor:
+                    return tensor.add(noise, alpha=sigma)
 
                 param_grads: ListOfTensors = [0.0 for _ in range(len(flat_diff_params))]  # type: ignore[misc]
 
                 for _ in range(num_samples):
                     noises = [distribution.sample(sample_shape=p.shape) for p in flat_diff_params]
                     flat_noisy_params = [
-                        add_perturbation(t, n) for t, n in zip(flat_diff_params, noises)
+                        add_perturbation(t, n) for t, n in zip(flat_diff_params, noises)  # type: ignore[arg-type]
                     ]
                     noisy_params: list[Any] = pytree.tree_unflatten(  # type: ignore[assignment]
-                        diff_params_treespec, flat_noisy_params
+                        diff_params_treespec,
+                        flat_noisy_params,
                     )
 
                     for argnum, noisy_param in zip(argnums, noisy_params):
                         args[argnum] = noisy_param
 
                     output = fn(*args)
                     weighted_grad = grad_outputs[0].mul(output).mul_(1 / sigma)
@@ -143,15 +150,15 @@
 
 
 def _zero_order_forward(  # pylint: disable=too-many-statements
     fn: Callable[..., torch.Tensor],
     distribution: Samplable,
     argnums: tuple[int, ...],
     num_samples: int,
-    sigma: Numeric,
+    sigma: float,
 ) -> Callable[..., torch.Tensor]:
     @functools.wraps(fn)
     def apply(*args: Any) -> torch.Tensor:  # pylint: disable=too-many-statements
         diff_params = [args[argnum] for argnum in argnums]
         flat_diff_params: list[Any]
         flat_diff_params, diff_params_treespec = pytree.tree_flatten(diff_params)  # type: ignore[arg-type]
 
@@ -186,15 +193,16 @@
                 ctx.save_for_backward(*flat_diff_params, *tensors, output)
                 ctx.len_args = len(args)
                 ctx.len_params = len(flat_diff_params)
                 return output
 
             @staticmethod
             def backward(  # pylint: disable=too-many-locals
-                ctx: Any, *grad_outputs: Any
+                ctx: Any,
+                *grad_outputs: Any,
             ) -> TupleOfOptionalTensors:
                 saved_tensors = ctx.saved_tensors
                 flat_diff_params = saved_tensors[: ctx.len_params]
                 tensors = saved_tensors[ctx.len_params : -1]
                 output = saved_tensors[-1]
                 non_tensors = ctx.non_tensors
 
@@ -207,26 +215,27 @@
                         tensors_counter += 1
                     else:
                         flat_args.append(non_tensors[non_tensors_counter])
                         non_tensors_counter += 1
 
                 args: list[Any] = pytree.tree_unflatten(ctx.args_treespec, flat_args)  # type: ignore[assignment]
 
-                def add_perturbation(tensor, noises):
-                    return tensor.add(noises, alpha=sigma)
+                def add_perturbation(tensor: torch.Tensor, noise: torch.Tensor) -> torch.Tensor:
+                    return tensor.add(noise, alpha=sigma)
 
                 param_grads: ListOfTensors = [0.0 for _ in range(len(flat_diff_params))]  # type: ignore[misc]
 
                 for _ in range(num_samples):
                     noises = [distribution.sample(sample_shape=p.shape) for p in flat_diff_params]
                     flat_noisy_params = [
-                        add_perturbation(t, n) for t, n in zip(flat_diff_params, noises)
+                        add_perturbation(t, n) for t, n in zip(flat_diff_params, noises)  # type: ignore[arg-type]
                     ]
                     noisy_params: list[Any] = pytree.tree_unflatten(  # type: ignore[assignment]
-                        diff_params_treespec, flat_noisy_params
+                        diff_params_treespec,
+                        flat_noisy_params,
                     )
 
                     for argnum, noisy_param in zip(argnums, noisy_params):
                         args[argnum] = noisy_param
 
                     noisy_output = fn(*args)
                     output = noisy_output - output
@@ -246,15 +255,15 @@
 
 
 def _zero_order_antithetic(  # pylint: disable=too-many-statements
     fn: Callable[..., torch.Tensor],
     distribution: Samplable,
     argnums: tuple[int, ...],
     num_samples: int,
-    sigma: Numeric,
+    sigma: float,
 ) -> Callable[..., torch.Tensor]:
     @functools.wraps(fn)
     def apply(*args: Any) -> torch.Tensor:  # pylint: disable=too-many-statements
         diff_params = [args[argnum] for argnum in argnums]
         flat_diff_params: list[Any]
         flat_diff_params, diff_params_treespec = pytree.tree_flatten(diff_params)  # type: ignore[arg-type]
 
@@ -288,15 +297,18 @@
                     raise RuntimeError('`output` must be a scalar tensor.')
                 ctx.save_for_backward(*flat_diff_params, *tensors)
                 ctx.len_args = len(args)
                 ctx.len_params = len(flat_diff_params)
                 return output
 
             @staticmethod
-            def backward(ctx: Any, *grad_outputs: Any):  # pylint: disable=too-many-locals
+            def backward(  # pylint: disable=too-many-locals
+                ctx: Any,
+                *grad_outputs: Any,
+            ) -> TupleOfOptionalTensors:
                 saved_tensors = ctx.saved_tensors
                 flat_diff_params = saved_tensors[: ctx.len_params]
                 tensors = saved_tensors[ctx.len_params :]
                 non_tensors = ctx.non_tensors
 
                 flat_args = []
                 tensors_counter = 0
@@ -309,31 +321,35 @@
                         flat_args.append(non_tensors[non_tensors_counter])
                         non_tensors_counter += 1
 
                 args: list[Any] = pytree.tree_unflatten(ctx.args_treespec, flat_args)  # type: ignore[assignment]
 
                 param_grads: ListOfTensors = [0.0 for _ in range(len(flat_diff_params))]  # type: ignore[misc]
 
-                def get_output(add_perturbation_fn, noises) -> torch.Tensor:
+                def get_output(
+                    add_perturbation_fn: Callable,
+                    noises: Sequence[torch.Tensor | Numeric],
+                ) -> torch.Tensor:
                     flat_noisy_params = [
                         add_perturbation_fn(t, n, alpha=sigma)
                         for t, n in zip(flat_diff_params, noises)
                     ]
                     noisy_params: list[Any] = pytree.tree_unflatten(  # type: ignore[assignment]
-                        diff_params_treespec, flat_noisy_params
+                        diff_params_treespec,
+                        flat_noisy_params,
                     )
 
                     for argnum, noisy_param in zip(argnums, noisy_params):
                         args[argnum] = noisy_param
 
                     return fn(*args)
 
                 for _ in range(num_samples):
                     noises = [distribution.sample(sample_shape=p.shape) for p in flat_diff_params]
-                    output = get_output(torch.add, noises) - get_output(torch.sub, noises)
+                    output = get_output(torch.add, noises) - get_output(torch.sub, noises)  # type: ignore[arg-type]
                     weighted_grad = grad_outputs[0].mul(output).mul_(0.5 / sigma)
 
                     for i, noise in enumerate(noises):
                         param_grads[i] += weighted_grad * noise
 
                 for i in range(len(flat_diff_params)):
                     param_grads[i] /= num_samples
@@ -349,15 +365,15 @@
 
 
 def zero_order(
     distribution: SampleFunc | Samplable,
     method: Method = 'naive',
     argnums: int | tuple[int, ...] = (0,),
     num_samples: int = 1,
-    sigma: Numeric = 1.0,
+    sigma: float = 1.0,
 ) -> Callable[[Callable[..., torch.Tensor]], Callable[..., torch.Tensor]]:
     """Return a decorator for applying zero-order differentiation.
 
     Args:
         distribution (callable or Samplable): A samplable object that has method
             ``samplable.sample(sample_shape)`` or a function that takes the shape as input and
             returns a shaped batch of samples. This is used to sample perturbations from the given
@@ -365,15 +381,15 @@
         method (str, optional): The algorithm to use. The currently supported algorithms are
             :const:`'naive'`, :const:`'forward'`, and :const:`'antithetic'`.
             (default: :const:`'naive'`)
         argnums (int or tuple of int, optional): Specifies arguments to compute gradients with
             respect to. (default: :const:`0`)
         num_samples (int, optional): The number of sample to get the averaged estimated gradient.
             (default: :const:`1`)
-        sigma (float or Tensor, optional): The standard deviation of the perturbation.
+        sigma (float, optional): The standard deviation of the perturbation.
             (default: :const:`1.0`)
 
     Returns:
         A function decorator that enables zero-order gradient estimation.
     """
     assert method in ('naive', 'forward', 'antithetic')
     if method == 'naive':
```

### Comparing `torchopt-0.7.0/torchopt/diff/zero_order/nn/__init__.py` & `torchopt-0.7.1/torchopt/diff/zero_order/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/torchopt/diff/zero_order/nn/module.py` & `torchopt-0.7.1/torchopt/diff/zero_order/nn/module.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # pylint: disable=redefined-builtin
 
 from __future__ import annotations
 
 import abc
 import functools
-from typing import Sequence
+from typing import Any, Sequence
 
 import torch
 import torch.nn as nn
 
 from torchopt.diff.zero_order.decorator import Method, Samplable, zero_order
 from torchopt.nn.stateless import reparametrize
 from torchopt.typing import Numeric, TupleOfTensors
@@ -33,67 +33,71 @@
 __all__ = ['ZeroOrderGradientModule']
 
 
 def enable_zero_order_gradients(
     cls: type[ZeroOrderGradientModule],
     method: Method = 'naive',
     num_samples: int = 1,
-    sigma: Numeric = 1.0,
+    sigma: float = 1.0,
 ) -> type[ZeroOrderGradientModule]:
     """Enable zero-order gradient estimation for the :func:`forward` method."""
     cls_forward = cls.forward
     if getattr(cls_forward, '__zero_order_gradients_enabled__', False):
         raise TypeError(
-            'Zero-order gradient estimation is already enabled for the `forward` method.'
+            'Zero-order gradient estimation is already enabled for the `forward` method.',
         )
 
     @functools.wraps(cls_forward)
-    def wrapped(self: ZeroOrderGradientModule, *input, **kwargs) -> torch.Tensor:
+    def wrapped(self: ZeroOrderGradientModule, *input: Any, **kwargs: Any) -> torch.Tensor:
         """Do the forward pass calculation."""
-        params_names, flat_params = tuple(zip(*self.named_parameters()))
+        named_params = tuple(self.named_parameters())
+        if len(named_params) == 0:
+            raise RuntimeError('The module has no parameters.')
+        params_names, flat_params = tuple(zip(*named_params))
 
         @zero_order(self.sample, argnums=0, method=method, num_samples=num_samples, sigma=sigma)
         def forward_fn(
             __flat_params: TupleOfTensors,
-            *input,
-            **kwargs,
+            *input: Any,
+            **kwargs: Any,
         ) -> torch.Tensor:
             with reparametrize(self, zip(params_names, __flat_params)):
                 return cls_forward(self, *input, **kwargs)
 
         return forward_fn(flat_params, *input, **kwargs)
 
     wrapped.__zero_order_gradients_enabled__ = True  # type: ignore[attr-defined]
-    cls.forward = wrapped  # type: ignore[assignment]
+    cls.forward = wrapped  # type: ignore[method-assign]
     return cls
 
 
 class ZeroOrderGradientModule(nn.Module, Samplable):
     """The base class for zero-order gradient models."""
 
     def __init_subclass__(  # pylint: disable=arguments-differ
         cls,
         method: Method = 'naive',
         num_samples: int = 1,
-        sigma: Numeric = 1.0,
+        sigma: float = 1.0,
     ) -> None:
         """Validate and initialize the subclass."""
         super().__init_subclass__()
         enable_zero_order_gradients(
             cls,
             method=method,
             num_samples=num_samples,
             sigma=sigma,
         )
 
     @abc.abstractmethod
-    def forward(self, *args, **kwargs) -> torch.Tensor:
+    def forward(self, *args: Any, **kwargs: Any) -> torch.Tensor:
         """Do the forward pass of the model."""
         raise NotImplementedError
 
     @abc.abstractmethod
     def sample(
-        self, sample_shape: torch.Size = torch.Size()  # pylint: disable=unused-argument
+        self,
+        sample_shape: torch.Size = torch.Size(),  # noqa: B008 # pylint: disable=unused-argument
     ) -> torch.Tensor | Sequence[Numeric]:
         # pylint: disable-next=line-too-long
         """Generate a sample_shape shaped sample or sample_shape shaped batch of samples if the distribution parameters are batched."""
         raise NotImplementedError
```

### Comparing `torchopt-0.7.0/torchopt/distributed/__init__.py` & `torchopt-0.7.1/torchopt/distributed/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # ==============================================================================
 """Distributed utilities."""
 
 import torch.distributed as dist
 import torch.distributed.rpc as rpc
 
 from torchopt.distributed import api, autograd, world
-from torchopt.distributed.api import *
-from torchopt.distributed.world import *
+from torchopt.distributed.api import *  # noqa: F403
+from torchopt.distributed.world import *  # noqa: F403
 
 
 __all__ = ['is_available', *api.__all__, *world.__all__]
 
 
 def is_available() -> bool:
     """Check if the distributed module is available."""
```

### Comparing `torchopt-0.7.0/torchopt/distributed/api.py` & `torchopt-0.7.1/torchopt/distributed/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,18 +50,15 @@
     'remote_sync_call',
     'parallelize',
     'parallelize_async',
     'parallelize_sync',
 ]
 
 
-if rpc.is_available():
-    UNSET_RPC_TIMEOUT = rpc.api.UNSET_RPC_TIMEOUT
-else:
-    UNSET_RPC_TIMEOUT = -1.0
+UNSET_RPC_TIMEOUT = rpc.api.UNSET_RPC_TIMEOUT if rpc.is_available() else -1.0
 
 
 T = TypeVar('T')
 U = TypeVar('U')
 Args = Tuple[Any, ...]
 KwArgs = Dict[str, Any]
 PartitionFunction = Callable[..., Sequence[Tuple[int, Optional[Args], Optional[KwArgs]]]]
@@ -130,15 +127,15 @@
         for arg in flat_args:
             if isinstance(arg, torch.Tensor):
                 if batch_size is None:
                     batch_size = arg.shape[self.dim]
                 elif batch_size != arg.shape[self.dim]:  # type: ignore[unreachable]
                     raise ValueError(
                         f'Batch size mismatch on dim={self.dim}. '
-                        f'Expected {batch_size}, got {arg.shape[self.dim]} (shape: {arg.shape}).'
+                        f'Expected {batch_size}, got {arg.shape[self.dim]} (shape: {arg.shape}).',
                     )
 
         if batch_size is None:
             return [(get_world_rank(), args, kwargs.copy())]
 
         dim_slices: list[int | slice]
         batch_slices: list[tuple[int | slice | Ellipsis.__class__, ...]]  # type: ignore[name-defined]
```

### Comparing `torchopt-0.7.0/torchopt/distributed/autograd.py` & `torchopt-0.7.1/torchopt/distributed/autograd.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,22 +27,22 @@
 
 __all__ = ['is_available', 'context']
 
 
 LOCK = Lock()
 
 
-def is_available():
+def is_available() -> bool:
     """Check if distributed autograd module is available."""
     return autograd.is_available()
 
 
 if is_available():
     # pylint: disable-next=unused-import,ungrouped-imports
-    from torch.distributed.autograd import DistAutogradContext, get_gradients
+    from torch.distributed.autograd import DistAutogradContext, get_gradients  # noqa: F401
 
     def backward(
         autograd_ctx_id: int,
         tensors: TensorOrTensors,
         retain_graph: bool = False,
         inputs: TensorOrTensors | None = None,
     ) -> None:
@@ -65,15 +65,15 @@
         if inputs is not None:
             if isinstance(inputs, torch.Tensor):
                 inputs = (inputs,)
             elif len(inputs) == 0:
                 raise RuntimeError("'inputs' argument to backward() cannot be empty.")
             else:
                 inputs = tuple(inputs)
-            if not all(map(lambda t: t.requires_grad, inputs)):
+            if not all(t.requires_grad for t in inputs):
                 raise RuntimeError('One of the differentiated Tensors does not require grad')
 
         roots = [tensors] if isinstance(tensors, torch.Tensor) else list(tensors)
         autograd.backward(autograd_ctx_id, roots=roots, retain_graph=retain_graph)
 
         all_local_grads = autograd.get_gradients(autograd_ctx_id)
         if inputs is not None:
@@ -107,28 +107,28 @@
                 (default: :data:`False`)
             allow_unused (bool, optional): If :data:`False`, specifying inputs that were not used
                 when computing outputs (and therefore their grad is always zero) is an error.
                 (default: :data:`False`)
         """
         outputs = [outputs] if isinstance(outputs, torch.Tensor) else list(outputs)
         inputs = (inputs,) if isinstance(inputs, torch.Tensor) else tuple(inputs)
-        if not all(map(lambda t: t.requires_grad, inputs)):
+        if not all(t.requires_grad for t in inputs):
             raise RuntimeError('One of the differentiated Tensors does not require grad')
 
         autograd.backward(autograd_ctx_id, roots=outputs, retain_graph=retain_graph)
 
         all_local_grads = autograd.get_gradients(autograd_ctx_id)
         grads = []
         for p in inputs:
             try:
                 grads.append(all_local_grads[p])
             except KeyError as ex:
                 if not allow_unused:
                     raise RuntimeError(
                         'One of the differentiated Tensors appears to not have been used in the '
-                        'graph. Set allow_unused=True if this is the desired behavior.'
+                        'graph. Set allow_unused=True if this is the desired behavior.',
                     ) from ex
                 grads.append(None)  # type: ignore[arg-type]
 
         return tuple(grads)
 
     __all__.extend(['DistAutogradContext', 'get_gradients', 'backward', 'grad'])
```

### Comparing `torchopt-0.7.0/torchopt/distributed/world.py` & `torchopt-0.7.1/torchopt/distributed/world.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     _WORKER_NAME_FORMAT = worker_name_format
 
     def wrapper(func: F) -> F:
         world_info = get_world_info()
 
         @record
         @functools.wraps(func)
-        def wrapped(*args, **kwargs):
+        def wrapped(*args: Any, **kwargs: Any) -> Any:
             rpc.init_rpc(
                 name=world_info.worker_name,
                 rank=world_info.rank,
                 world_size=world_info.world_size,
                 backend=backend,
                 rpc_backend_options=rpc_backend_options,
             )
@@ -189,15 +189,15 @@
 def __on_ranks(ranks: Iterable[int], inverse: bool = False) -> Callable[[F], F]:
     ranks = frozenset(ranks)
 
     def wrapper(func: F) -> F:
         world_rank = get_world_info().world_rank
 
         @functools.wraps(func)
-        def wrapped(*args, **kwargs):
+        def wrapped(*args: Any, **kwargs: Any) -> Any:
             if inverse:
                 if world_rank not in ranks:
                     return func(*args, **kwargs)
             elif world_rank in ranks:
                 return func(*args, **kwargs)
             return None
 
@@ -207,15 +207,15 @@
 
 
 def on_rank(*ranks: int) -> Callable[[F], F]:
     """Return a decorator to mark a function to be executed only on given ranks."""
     return __on_ranks(ranks=ranks, inverse=False)
 
 
-def not_on_rank(*ranks) -> Callable[[F], F]:
+def not_on_rank(*ranks: int) -> Callable[[F], F]:
     """Return a decorator to mark a function to be executed only on non given ranks."""
     return __on_ranks(ranks=ranks, inverse=True)
 
 
 def rank_all(func: F) -> F:
     """Return a decorator to mark a function to be executed on all ranks."""
     return func
```

### Comparing `torchopt-0.7.0/torchopt/hook.py` & `torchopt-0.7.1/torchopt/hook.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,26 +30,28 @@
 
 def zero_nan_hook(g: torch.Tensor) -> torch.Tensor:
     """Replace ``nan`` with zero."""
     return g.nan_to_num(nan=0.0)
 
 
 def nan_to_num_hook(
-    nan: float = 0.0, posinf: float | None = None, neginf: float | None = None
+    nan: float = 0.0,
+    posinf: float | None = None,
+    neginf: float | None = None,
 ) -> Callable[[torch.Tensor], torch.Tensor]:
     """Return a ``nan`` to num hook to replace ``nan`` / ``+inf`` / ``-inf`` with the given numbers."""
 
     def hook(g: torch.Tensor) -> torch.Tensor:
         """Replace ``nan`` / ``+inf`` / ``-inf`` with the given numbers."""
         return g.nan_to_num(nan=nan, posinf=posinf, neginf=neginf)
 
     return hook
 
 
-def register_hook(hook) -> GradientTransformation:
+def register_hook(hook: Callable[[torch.Tensor], torch.Tensor | None]) -> GradientTransformation:
     """Stateless identity transformation that leaves input gradients untouched.
 
     This function passes through the *gradient updates* unchanged.
 
     Returns:
         An ``(init_fn, update_fn)`` tuple.
     """
@@ -60,14 +62,14 @@
     def update_fn(
         updates: Updates,
         state: OptState,
         *,
         params: Params | None = None,  # pylint: disable=unused-argument
         inplace: bool = True,  # pylint: disable=unused-argument
     ) -> tuple[Updates, OptState]:
-        def f(g):
+        def f(g: torch.Tensor) -> torch.utils.hooks.RemovableHandle:
             return g.register_hook(hook)
 
         pytree.tree_map_(f, updates)
         return updates, state
 
     return GradientTransformation(init_fn, update_fn)
```

### Comparing `torchopt-0.7.0/torchopt/linalg/__init__.py` & `torchopt-0.7.1/torchopt/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/torchopt/linalg/cg.py` & `torchopt-0.7.1/torchopt/linalg/cg.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,20 +66,22 @@
 ) -> TensorTree:
     # https://en.wikipedia.org/wiki/Conjugate_gradient_method#The_preconditioned_conjugate_gradient_method
 
     # tolerance handling uses the "non-legacy" behavior of `scipy.sparse.linalg.cg`
     b2 = tree_vdot_real(b, b)
     atol2 = max(rtol**2 * b2, atol**2)
 
-    def cond_fn(value):
+    def cond_fn(value: tuple[TensorTree, TensorTree, float, TensorTree, int]) -> bool:
         _, r, gamma, _, k = value
         rs = gamma if M is _identity else tree_vdot_real(r, r)
         return rs > atol2 and k < maxiter
 
-    def body_fn(value):
+    def body_fn(
+        value: tuple[TensorTree, TensorTree, float, TensorTree, int],
+    ) -> tuple[TensorTree, TensorTree, float, TensorTree, int]:
         x, r, gamma, p, k = value
         Ap = A(p)
         alpha = gamma / tree_vdot_real(p, Ap)
         x_ = pytree.tree_map(lambda a, b: a.add(b, alpha=alpha), x, p)
         r_ = pytree.tree_map(lambda a, b: a.sub(b, alpha=alpha), r, Ap)
         z_ = M(r_)
         gamma_ = tree_vdot_real(r_, z_)
@@ -121,21 +123,19 @@
     if M is None:
         M = _identity
     A = normalize_matvec(A)
     M = normalize_matvec(M)
 
     if cat_shapes(x0) != cat_shapes(b):
         raise ValueError(
-            f'Tensors in x0 and b must have matching shapes: {cat_shapes(x0)} vs. {cat_shapes(b)}.'
+            f'Tensors in x0 and b must have matching shapes: {cat_shapes(x0)} vs. {cat_shapes(b)}.',
         )
 
     isolve_solve = partial(_isolve_solve, x0=x0, rtol=rtol, atol=atol, maxiter=maxiter, M=M)
-
-    x = isolve_solve(A, b)
-    return x
+    return isolve_solve(A, b)
 
 
 def cg(
     A: TensorTree | Callable[[TensorTree], TensorTree],
     b: TensorTree,
     x0: TensorTree | None = None,
     *,
```

### Comparing `torchopt-0.7.0/torchopt/linalg/ns.py` & `torchopt-0.7.1/torchopt/linalg/ns.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,20 +108,20 @@
             v = pytree.tree_sub(v, matvec(v))
             # inv_A_hat_b = inv_A_hat_b + v
             inv_A_hat_b = pytree.tree_add(inv_A_hat_b, v)
 
     return inv_A_hat_b
 
 
-def _ns_inv(A: torch.Tensor, maxiter: int, alpha: float | None = None):
+def _ns_inv(A: torch.Tensor, maxiter: int, alpha: float | None = None) -> torch.Tensor:
     """Use Neumann Series iteration to solve ``A^{-1}``."""
     if A.ndim != 2 or A.shape[0] != A.shape[1]:
         raise ValueError(f'`A` must be a square matrix, but has shape: {A.shape}')
 
-    I = torch.eye(*A.shape, out=torch.empty_like(A))
+    I = torch.eye(*A.shape, out=torch.empty_like(A))  # noqa: E741
     inv_A_hat = torch.zeros_like(A)
     if alpha is not None:
         # A^{-1} = a [I - (I - a A)]^{-1} = a [I + (I - a A) + (I - a A)^2 + (I - a A)^3 + ...]
         M = I - alpha * A
         for rank in range(maxiter):
             inv_A_hat = inv_A_hat + torch.linalg.matrix_power(M, rank)
         inv_A_hat = alpha * inv_A_hat
```

### Comparing `torchopt-0.7.0/torchopt/linalg/utils.py` & `torchopt-0.7.1/torchopt/linalg/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 def cat_shapes(tree: TensorTree) -> tuple[int, ...]:
     """Concatenate the shapes of the leaves of a tree of tensors."""
     leaves = pytree.tree_leaves(tree)
     return tuple(itertools.chain.from_iterable(tuple(leaf.shape) for leaf in leaves))
 
 
 def normalize_matvec(
-    matvec: TensorTree | Callable[[TensorTree], TensorTree]
+    matvec: TensorTree | Callable[[TensorTree], TensorTree],
 ) -> Callable[[TensorTree], TensorTree]:
     """Normalize an argument for computing matrix-vector product."""
     if callable(matvec):
         return matvec
 
     mat_flat, treespec = pytree.tree_flatten(matvec)
     for mat in mat_flat:
@@ -44,14 +44,14 @@
             raise TypeError(f'Linear operator must be a square matrix, but has shape: {mat.shape}')
 
     def _matvec(x: TensorTree) -> TensorTree:
         x_flat = pytree.tree_leaves(x)
         if len(x_flat) != len(mat_flat):
             raise ValueError(
                 f'`x` must have the same number of leaves as `matvec`, '
-                f'but has {len(x_flat)} leaves and `matvec` has {len(mat_flat)} leaves'
+                f'but has {len(x_flat)} leaves and `matvec` has {len(mat_flat)} leaves',
             )
 
         y_flat = map(torch.matmul, mat_flat, x_flat)
         return pytree.tree_unflatten(treespec, y_flat)
 
     return _matvec
```

### Comparing `torchopt-0.7.0/torchopt/linear_solve/__init__.py` & `torchopt-0.7.1/torchopt/linear_solve/__init__.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/torchopt/linear_solve/cg.py` & `torchopt-0.7.1/torchopt/linear_solve/cg.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,30 +32,30 @@
 """Linear algebra solver for ``A x = b`` using conjugate gradient."""
 
 # pylint: disable=invalid-name
 
 from __future__ import annotations
 
 import functools
-from typing import Callable
+from typing import Any, Callable
 
 from torchopt import linalg
 from torchopt.linear_solve.utils import make_ridge_matvec
-from torchopt.typing import TensorTree
+from torchopt.typing import LinearSolver, TensorTree
 
 
 __all__ = ['solve_cg']
 
 
 def _solve_cg(
     matvec: Callable[[TensorTree], TensorTree],  # (x) -> A @ x
     b: TensorTree,
     ridge: float | None = None,
     init: TensorTree | None = None,
-    **kwargs,
+    **kwargs: Any,
 ) -> TensorTree:
     """Solve ``A x = b`` using conjugate gradient.
 
     This assumes that ``A`` is a hermitian, positive definite matrix.
 
     Args:
         matvec (callable): A function that returns the product between ``A`` and a vector.
@@ -74,15 +74,15 @@
         # i.e. (x) -> (A + ridge * I) @ x
         matvec = make_ridge_matvec(matvec, ridge=ridge)
 
     # Returns solution for `(A + ridge * I) @ x = b`.
     return linalg.cg(matvec, b, x0=init, **kwargs)
 
 
-def solve_cg(**kwargs):
+def solve_cg(**kwargs: Any) -> LinearSolver:
     """Return a solver function to solve ``A x = b`` using conjugate gradient.
 
     This assumes that ``A`` is a hermitian, positive definite matrix.
 
     Args:
         ridge (float or None, optional): Optional ridge regularization. If provided, solves the
             equation for ``A x + ridge x = b``. (default: :data:`None`)
@@ -94,20 +94,18 @@
     Returns:
         A solver function with signature ``(matvec, b) -> x`` that solves ``A x = b`` using
         conjugate gradient where ``matvec(v) = A v``.
 
     See Also:
         Conjugate gradient iteration :func:`torchopt.linalg.cg`.
 
-    Example::
-
+    Examples:
         >>> A = {'a': torch.eye(5, 5), 'b': torch.eye(3, 3)}
         >>> x = {'a': torch.randn(5), 'b': torch.randn(3)}
         >>> def matvec(x: TensorTree) -> TensorTree:
         ...     return {'a': A['a'] @ x['a'], 'b': A['b'] @ x['b']}
         >>> b = matvec(x)
         >>> solver = solve_cg(init={'a': torch.zeros(5), 'b': torch.zeros(3)})
         >>> x_hat = solver(matvec, b)
         >>> assert torch.allclose(x_hat['a'], x['a']) and torch.allclose(x_hat['b'], x['b'])
-
     """
     return functools.partial(_solve_cg, **kwargs)
```

### Comparing `torchopt-0.7.0/torchopt/linear_solve/inv.py` & `torchopt-0.7.1/torchopt/linear_solve/inv.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,32 +32,32 @@
 """Linear algebra solver for ``A x = b`` using matrix inversion."""
 
 # pylint: disable=invalid-name
 
 from __future__ import annotations
 
 import functools
-from typing import Callable
+from typing import Any, Callable
 
 import torch
 
 from torchopt import linalg, pytree
 from torchopt.linear_solve.utils import make_ridge_matvec, materialize_matvec
-from torchopt.typing import TensorTree
+from torchopt.typing import LinearSolver, TensorTree
 
 
 __all__ = ['solve_inv']
 
 
 def _solve_inv(
     matvec: Callable[[TensorTree], TensorTree],  # (x) -> A @ x
     b: TensorTree,
     ridge: float | None = None,
     ns: bool = False,
-    **kwargs,
+    **kwargs: Any,
 ) -> TensorTree:
     """Solve ``A x = b`` using matrix inversion.
 
     If ``ns = False``, this assumes the matrix ``A`` is a constant matrix and will materialize it
     in memory.
 
     Args:
@@ -87,15 +87,15 @@
     if ns:
         return linalg.ns(matvec, b, **kwargs)
 
     A, _, tree_ravel, tree_unravel = materialize_matvec(matvec, b)
     return tree_unravel(pytree.tree_map(torch.linalg.solve, A, tree_ravel(b)))
 
 
-def solve_inv(**kwargs):
+def solve_inv(**kwargs: Any) -> LinearSolver:
     """Return a solver function to solve ``A x = b`` using matrix inversion.
 
     If ``ns = False``, this assumes the matrix ``A`` is a constant matrix and will materialize it
     in memory.
 
     Args:
         ridge (float or None, optional): Optional ridge regularization. If provided, solves the
@@ -109,20 +109,18 @@
     Returns:
         A solver function with signature ``(matvec, b) -> x`` that solves ``A x = b`` using matrix
         inversion where ``matvec(v) = A v``.
 
     See Also:
         Neumann Series matrix inversion approximation :func:`torchopt.linalg.ns`.
 
-    Example::
-
+    Examples:
         >>> A = {'a': torch.eye(5, 5), 'b': torch.eye(3, 3)}
         >>> x = {'a': torch.randn(5), 'b': torch.randn(3)}
         >>> def matvec(x: TensorTree) -> TensorTree:
         ...     return {'a': A['a'] @ x['a'], 'b': A['b'] @ x['b']}
         >>> b = matvec(x)
         >>> solver = solve_inv(ns=True, maxiter=10)
         >>> x_hat = solver(matvec, b)
         >>> assert torch.allclose(x_hat['a'], x['a']) and torch.allclose(x_hat['b'], x['b'])
-
     """
     return functools.partial(_solve_inv, **kwargs)
```

### Comparing `torchopt-0.7.0/torchopt/linear_solve/normal_cg.py` & `torchopt-0.7.1/torchopt/linear_solve/normal_cg.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,30 +32,30 @@
 """Linear algebra solver for ``A^T A x = A^T b`` using conjugate gradient."""
 
 # pylint: disable=invalid-name
 
 from __future__ import annotations
 
 import functools
-from typing import Callable
+from typing import Any, Callable
 
 from torchopt import linalg
 from torchopt.linear_solve.utils import make_normal_matvec, make_ridge_matvec, make_rmatvec
-from torchopt.typing import TensorTree
+from torchopt.typing import LinearSolver, TensorTree
 
 
 __all__ = ['solve_normal_cg']
 
 
 def _solve_normal_cg(
     matvec: Callable[[TensorTree], TensorTree],  # (x) -> A @ x
     b: TensorTree,
     ridge: float | None = None,
     init: TensorTree | None = None,
-    **kwargs,
+    **kwargs: Any,
 ) -> TensorTree:
     """Solve the normal equation ``A^T A x = A^T b`` using conjugate gradient.
 
     This can be used to solve ``A x = b`` using conjugate gradient when ``A`` is not hermitian,
     positive definite.
 
     Args:
@@ -67,18 +67,15 @@
             conjugate gradient. If :data:`None`, uses zero initialization. (default: :data:`None`)
         **kwargs: Additional keyword arguments for the conjugate gradient solver
             :func:`torchopt.linalg.cg`.
 
     Returns:
         The solution with the same structure as ``b``.
     """
-    if init is None:
-        example_x = b  # This assumes that matvec is a square linear operator.
-    else:
-        example_x = init
+    example_x = b if init is None else init
 
     rmatvec = make_rmatvec(matvec, example_x)  # (x) -> A.T @ x
     normal_matvec = make_normal_matvec(matvec)  # (x) -> A.T @ A @ x
 
     if ridge is not None:
         #      (x) -> A.T @ A @ x + ridge * x
         # i.e. (x) -> (A.T @ A + ridge * I) @ x
@@ -86,15 +83,15 @@
 
     rhs = rmatvec(b)  # A.T @ b
 
     # Returns solution for `(A.T @ A + ridge * I) @ x = A.T @ b`.
     return linalg.cg(normal_matvec, rhs, x0=init, **kwargs)
 
 
-def solve_normal_cg(**kwargs):
+def solve_normal_cg(**kwargs: Any) -> LinearSolver:
     """Return a solver function to solve ``A^T A x = A^T b`` using conjugate gradient.
 
     This can be used to solve ``A x = b`` using conjugate gradient when ``A`` is not hermitian,
     positive definite.
 
     Args:
         ridge (float or None, optional): Optional ridge regularization. If provided, solves the
@@ -107,20 +104,18 @@
     Returns:
         A solver function with signature ``(matvec, b) -> x`` that solves ``A^T A x = A^T b`` using
         conjugate gradient where ``matvec(v) = A v``.
 
     See Also:
         Conjugate gradient iteration :func:`torchopt.linalg.cg`.
 
-    Example::
-
+    Examples:
         >>> A = {'a': torch.randn(5, 5), 'b': torch.randn(3, 3)}
         >>> x = {'a': torch.randn(5), 'b': torch.randn(3)}
         >>> def matvec(x: TensorTree) -> TensorTree:
         ...     return {'a': A['a'] @ x['a'], 'b': A['b'] @ x['b']}
         >>> b = matvec(x)
         >>> solver = solve_normal_cg(init={'a': torch.zeros(5), 'b': torch.zeros(3)})
         >>> x_hat = solver(matvec, b)
         >>> assert torch.allclose(x_hat['a'], x['a']) and torch.allclose(x_hat['b'], x['b'])
-
     """
     return functools.partial(_solve_normal_cg, **kwargs)
```

### Comparing `torchopt-0.7.0/torchopt/linear_solve/utils.py` & `torchopt-0.7.1/torchopt/linear_solve/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,49 +38,52 @@
 import functorch
 
 from torchopt import pytree
 from torchopt.typing import TensorTree
 
 
 def make_rmatvec(
-    matvec: Callable[[TensorTree], TensorTree], example_x: TensorTree
+    matvec: Callable[[TensorTree], TensorTree],
+    example_x: TensorTree,
 ) -> Callable[[TensorTree], TensorTree]:
     """Return a function that computes ``rmatvec(y) = A.T @ y`` from ``matvec(x) = A @ x``."""
     _, vjp, *_ = functorch.vjp(matvec, example_x)
 
     return lambda y: vjp(y)[0]
 
 
 def make_normal_matvec(
-    matvec: Callable[[TensorTree], TensorTree]
+    matvec: Callable[[TensorTree], TensorTree],
 ) -> Callable[[TensorTree], TensorTree]:
     """Return a function that computes ``normal_matvec(y) = A.T @ A @ y`` from ``matvec(x) = A @ x``."""
 
     def normal_matvec(y: TensorTree) -> TensorTree:
         """Compute ``A.T @ A @ y`` from ``matvec(x) = A @ x``."""
         matvec_y, vjp, *_ = functorch.vjp(matvec, y)
         return vjp(matvec_y)[0]
 
     return normal_matvec
 
 
 def make_ridge_matvec(
-    matvec: Callable[[TensorTree], TensorTree], ridge: float = 0.0
+    matvec: Callable[[TensorTree], TensorTree],
+    ridge: float = 0.0,
 ) -> Callable[[TensorTree], TensorTree]:
     """Return a function that computes ``ridge_matvec(y) = A.T @ A @ y + ridge * y`` from ``matvec(x) = A @ x``."""
 
     def ridge_matvec(y: TensorTree) -> TensorTree:
         """Compute ``A.T @ A @ v + ridge * v`` from ``matvec(x) = A @ x``."""
         return pytree.tree_add_scalar_mul(matvec(y), y, alpha=ridge)
 
     return ridge_matvec
 
 
 def materialize_matvec(
-    matvec: Callable[[TensorTree], TensorTree], x: TensorTree
+    matvec: Callable[[TensorTree], TensorTree],
+    x: TensorTree,
 ) -> tuple[
     TensorTree,
     Callable[[TensorTree], TensorTree],
     Callable[[TensorTree], TensorTree],
     Callable[[TensorTree], TensorTree],
 ]:
     """Materialize the matrix ``A`` used in ``matvec(x) = A @ x``."""
```

### Comparing `torchopt-0.7.0/torchopt/nn/__init__.py` & `torchopt-0.7.1/torchopt/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/torchopt/nn/module.py` & `torchopt-0.7.1/torchopt/nn/module.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 class MetaGradientModule(nn.Module):  # pylint: disable=abstract-method
     """Base class for neural network modules that hold meta-parameters and meta-modules."""
 
     _meta_inputs: MetaInputsContainer
     _meta_parameters: TensorContainer
     _meta_modules: dict[str, nn.Module | None]
 
-    def __new__(cls, *args, **kwargs) -> MetaGradientModule:
+    def __new__(cls, *args: Any, **kwargs: Any) -> MetaGradientModule:
         """Create a new module instance."""
         instance = super().__new__(cls)
         flat_args: list[Any]
         flat_args = pytree.tree_leaves((args, kwargs))  # type: ignore[arg-type]
         meta_parameters = {x for x in flat_args if isinstance(x, torch.Tensor) and x.requires_grad}
         meta_modules = {x for x in flat_args if isinstance(x, nn.Module) and x.training}
         for meta_module in tuple(meta_modules):
@@ -52,15 +52,15 @@
             meta_modules.update(meta_module.modules())
 
         instance._meta_inputs = MetaInputsContainer(meta_parameters, meta_modules)
         instance._meta_parameters: TensorContainer = OrderedDict()  # type: ignore[misc]
         instance._meta_modules: dict[str, nn.Module | None] = OrderedDict()  # type: ignore[misc]
         return instance
 
-    def __init__(self, *args, **kwargs) -> None:  # pylint: disable=unused-argument
+    def __init__(self, *args: Any, **kwargs: Any) -> None:  # pylint: disable=unused-argument
         """Initialize a new module instance."""
         super().__init__()
 
     def __getattr__(self, name: str) -> torch.Tensor | nn.Module:
         """Get an attribute of the module."""
         if '_parameters' in self.__dict__:
             _parameters = self.__dict__['_parameters']
@@ -84,30 +84,30 @@
                 return _meta_modules[name]
         raise AttributeError(f"'{type(self).__name__}' object has no attribute '{name}'")
 
     # pylint: disable-next=too-many-branches,too-many-statements
     def __setattr__(self, name: str, value: torch.Tensor | nn.Module) -> None:
         """Set an attribute of the module."""
 
-        def remove_from(*dicts_or_sets):
+        def remove_from(*dicts_or_sets: dict[str, Any] | set[str]) -> None:
             for dict_or_set in dicts_or_sets:
                 if name in dict_or_set:
                     if isinstance(dict_or_set, dict):
                         del dict_or_set[name]
                     else:
                         dict_or_set.discard(name)
 
         params = self.__dict__.get('_parameters')
         meta_params = self.__dict__.get('_meta_parameters')
         if isinstance(value, torch.Tensor) and value.requires_grad:
             if params is None:
                 raise AttributeError('cannot assign parameters before Module.__init__() call')
             if meta_params is None:
                 raise AttributeError(
-                    'cannot assign meta-parameters before MetaGradientModule.__init__() call'
+                    'cannot assign meta-parameters before MetaGradientModule.__init__() call',
                 )
             remove_from(
                 self.__dict__,
                 self._buffers,
                 self._modules,
                 self._non_persistent_buffers_set,
                 self._meta_parameters,
@@ -117,33 +117,33 @@
                 self.register_meta_parameter(name, value)
             else:
                 self.register_parameter(name, value)
         elif params is not None and name in params:
             if value is not None:
                 raise TypeError(
                     f"cannot assign '{torch.typename(value)}' as parameter '{name}' "
-                    f'(torch.Tensor or None expected)'
+                    f'(torch.Tensor or None expected)',
                 )
             self.register_parameter(name, value)  # type: ignore[unreachable]
         elif meta_params is not None and name in meta_params:
             if value is not None:
                 raise TypeError(
                     f"cannot assign '{torch.typename(value)}' as meta-parameter '{name}' "
-                    f'(torch.Tensor or None expected)'
+                    f'(torch.Tensor or None expected)',
                 )
             self.register_meta_parameter(name, value)  # type: ignore[unreachable]
         else:
             modules = self.__dict__.get('_modules')
             meta_modules = self.__dict__.get('_meta_modules')
             if isinstance(value, nn.Module):
                 if modules is None:
                     raise AttributeError('cannot assign module before Module.__init__() call')
                 if meta_modules is None:
                     raise AttributeError(
-                        'cannot assign module before MetaGradientModule.__init__() call'
+                        'cannot assign module before MetaGradientModule.__init__() call',
                     )
                 remove_from(
                     self.__dict__,
                     self._parameters,
                     self._buffers,
                     self._non_persistent_buffers_set,
                     self._meta_parameters,
@@ -153,24 +153,24 @@
                     meta_modules[name] = value
                 else:
                     modules[name] = value
             elif modules is not None and name in modules:
                 if value is not None:
                     raise TypeError(
                         f"cannot assign '{torch.typename(value)}' as child module '{name}' "
-                        f'(torch.nn.Module or None expected)'
+                        f'(torch.nn.Module or None expected)',
                     )
                 modules[name] = value  # type: ignore[unreachable]
             else:
                 buffers = self.__dict__.get('_buffers')
                 if buffers is not None and name in buffers:
                     if value is not None and not isinstance(value, torch.Tensor):
                         raise TypeError(
                             f"cannot assign '{torch.typename(value)}' as buffer '{name}' "
-                            f'(torch.Tensor or None expected)'
+                            f'(torch.Tensor or None expected)',
                         )
                     buffers[name] = value
                 else:
                     object.__setattr__(self, name, value)
 
     def __delattr__(self, name: str) -> None:
         """Delete an attribute of the module."""
@@ -214,24 +214,24 @@
         if param is None:
             self._parameters[name] = None
             return
 
         if not isinstance(param, torch.Tensor):
             raise TypeError(
                 f"cannot assign '{torch.typename(param)}' object to parameter '{name}' "
-                f'(torch.Tensor or None required)'
+                f'(torch.Tensor or None required)',
             )
         if not param.requires_grad:
             raise ValueError(
-                f"cannot assign Tensor that `requires_grad=False` to parameter '{name}'"
+                f"cannot assign Tensor that `requires_grad=False` to parameter '{name}'",
             )
         if param in self._meta_inputs.meta_parameters:
             raise ValueError(
                 f"cannot assign Tensor that is a meta-parameter to parameter '{name}'. "
-                f'Use self.register_meta_parameter() instead.'
+                f'Use self.register_meta_parameter() instead.',
             )
 
         self._parameters[name] = param  # type: ignore
 
     def register_meta_parameter(self, name: str, param: torch.Tensor | None) -> None:
         r"""Add a meta-parameter to the module.
 
@@ -242,15 +242,15 @@
                 module using the given name.
             param (Tensor or None): The meta-parameter to be added to the module. If :data:`None`,
                 then operations that run on meta-parameters, such as ``cuda``, are ignored. If
                 :data:`None`, the meta-parameter is **not** included in the module's ``state_dict``.
         """
         if '_meta_parameters' not in self.__dict__:
             raise AttributeError(
-                'cannot assign meta-parameter before MetaGradientModule.__init__() call'
+                'cannot assign meta-parameter before MetaGradientModule.__init__() call',
             )
         if not isinstance(name, str):
             raise TypeError(f'meta-parameter name should be a string. Got {torch.typename(name)}')
         if '.' in name:
             raise KeyError("meta-parameter name can't contain '.'")
         if name == '':
             raise KeyError("meta-parameter name can't be empty string ''")
@@ -260,19 +260,19 @@
         if param is None:
             self._meta_parameters[name] = None
             return
 
         if not isinstance(param, torch.Tensor):
             raise TypeError(
                 f"cannot assign '{torch.typename(param)}' object to meta-parameter '{name}' "
-                f'(torch.Tensor or None required)'
+                f'(torch.Tensor or None required)',
             )
         if not param.requires_grad:
             raise ValueError(
-                f"cannot assign Tensor that `requires_grad=False` to meta-parameter '{name}'"
+                f"cannot assign Tensor that `requires_grad=False` to meta-parameter '{name}'",
             )
 
         self._meta_parameters[name] = param
 
     def add_module(self, name: str, module: nn.Module | None) -> None:
         r"""Add a child module to the current module.
 
@@ -292,15 +292,15 @@
         if '.' in name:
             raise KeyError(f"module name can't contain '.', got: '{name}'")
         if name == '':
             raise KeyError("module name can't be empty string ''")
         if module in self._meta_inputs.meta_modules:
             raise ValueError(
                 f"cannot add module that is a meta-module to module '{name}'. "
-                f'Use self.add_meta_module() instead.'
+                f'Use self.add_meta_module() instead.',
             )
 
         self._modules[name] = module
 
     def register_module(self, name: str, module: nn.Module | None) -> None:
         r"""Alias for :func:`add_module`."""
         self.add_module(name, module)
@@ -341,46 +341,44 @@
             recurse (bool, optional): If :data:`True`, then yields parameters of this module and
                 all submodules. Otherwise, yields only meta-parameters that are direct members of
                 this module. (default: :data:`True`)
 
         Yields:
             Parameter: module meta-parameter
 
-        Example::
-
+        Examples:
             >>> for param in model.meta_parameters():
             >>>     print(type(param), param.size())
             <class 'torch.Tensor'> (20L,)
             <class 'torch.Tensor'> (20L, 1L, 5L, 5L)
-
         """
         for _, meta_param in self.named_meta_parameters(recurse=recurse):
             yield meta_param
 
     def named_meta_parameters(
-        self, prefix: str = '', recurse: bool = True
+        self,
+        prefix: str = '',
+        recurse: bool = True,
     ) -> Iterator[tuple[str, torch.Tensor]]:
         r"""Return an iterator over module meta-parameters, yielding both the name of the meta-parameter as well as the meta-parameter itself.
 
         Args:
             prefix (str, optional): The prefix to prepend to all meta-parameter names.
                 (default: :const:`''`)
             recurse (bool, optional): if :data:`True`, then yields meta-parameters of this module
                 and all submodules. Otherwise, yields only meta-parameters that are direct members
                 of this module. (default: :data:`True`)
 
         Yields:
             (string, Parameter): Tuple containing the name and parameter
 
-        Example::
-
+        Examples:
             >>> for name, meta_param in self.named_meta_parameters():
             >>>    if name in ['bias']:
             >>>        print(meta_param.size())
-
         """  # pylint: disable=line-too-long
         memo = set()
         for name, param in getattr(self, '_meta_parameters', {}).items():
             if param is None or param in memo:
                 continue
             memo.add(param)
             yield prefix + name, param
@@ -401,20 +399,18 @@
 
     def named_meta_children(self) -> Iterator[tuple[str, nn.Module]]:
         r"""Return an iterator over immediate children meta-modules, yielding both the name of the meta-module as well as the meta-module itself.
 
         Yields:
             (string, Module): Tuple containing a name and child meta-module
 
-        Example::
-
+        Examples:
             >>> for name, meta_module in model.named_meta_children():
             >>>     if name in ['conv4', 'conv5']:
             >>>         print(meta_module)
-
         """  # pylint: disable=line-too-long
         memo = set()
         for name, meta_module in self._meta_modules.items():
             if meta_module is not None and meta_module not in memo:
                 memo.add(meta_module)
                 yield name, meta_module
 
@@ -427,15 +423,18 @@
         Note:
             Duplicate meta-modules are returned only once.
         """
         for _, meta_module in self.named_meta_modules():
             yield meta_module
 
     def named_meta_modules(
-        self, memo: set[nn.Module] | None = None, prefix: str = '', remove_duplicate: bool = True
+        self,
+        memo: set[nn.Module] | None = None,
+        prefix: str = '',
+        remove_duplicate: bool = True,
     ) -> Iterator[tuple[str, nn.Module]]:
         r"""Return an iterator over all meta-modules in the network, yielding both the name of the meta-module as well as the meta-module itself.
 
         Args:
             memo (set of nn.Module or None, optional): A memory to store the set of meta-modules
                 already added to the result. If not provided, a new set will be created.
                 (default: :const:`None`)
```

### Comparing `torchopt-0.7.0/torchopt/nn/stateless.py` & `torchopt-0.7.1/torchopt/nn/stateless.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,18 +53,15 @@
             return submodule
 
     def recursive_setattr(path: str, value: torch.Tensor) -> torch.Tensor:
         """Set attribute recursively."""
         prefix, _, attr = path.rpartition('.')
         mod = get_submodule(prefix)
 
-        if allow_missing:
-            orig = getattr(mod, attr, MISSING)
-        else:
-            orig = getattr(mod, attr)
+        orig = getattr(mod, attr, MISSING) if allow_missing else getattr(mod, attr)
 
         # pylint: disable=protected-access
         if value is MISSING:
             delattr(mod, attr)
         elif hasattr(mod, '_parameters') and attr in mod._parameters:
             mod._parameters[attr] = value  # type: ignore[assignment]
         elif hasattr(mod, '_buffers') and attr in mod._buffers:
@@ -73,18 +70,15 @@
             mod._meta_parameters[attr] = value  # type: ignore[operator,index]
         else:
             setattr(mod, attr, value)
         # pylint: enable=protected-access
 
         return orig
 
-    orig_named_tensors = {
-        name: recursive_setattr(name, tensor) for name, tensor in named_tensors.items()
-    }
-    return orig_named_tensors
+    return {name: recursive_setattr(name, tensor) for name, tensor in named_tensors.items()}
 
 
 @contextlib.contextmanager
 def reparametrize(
     module: nn.Module,
     named_tensors: dict[str, torch.Tensor] | Iterable[tuple[str, torch.Tensor]],
     allow_missing: bool = False,
```

### Comparing `torchopt-0.7.0/torchopt/optim/__init__.py` & `torchopt-0.7.1/torchopt/optim/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 MetaOPT Team. All Rights Reserved.
+# Copyright 2022-2023 MetaOPT Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,13 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """object oriented optimizer implementations."""
 
 from torchopt.optim import meta
+from torchopt.optim.adagrad import AdaGrad, Adagrad
 from torchopt.optim.adam import Adam
 from torchopt.optim.adamw import AdamW
 from torchopt.optim.base import Optimizer
 from torchopt.optim.func import FuncOptimizer
 from torchopt.optim.rmsprop import RMSProp, RMSprop
 from torchopt.optim.sgd import SGD
```

### Comparing `torchopt-0.7.0/torchopt/optim/adam.py` & `torchopt-0.7.1/torchopt/optim/adam.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 MetaOPT Team. All Rights Reserved.
+# Copyright 2022-2023 MetaOPT Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -36,15 +36,15 @@
         - The differentiable meta-Adam optimizer: :class:`torchopt.MetaAdam`.
     """
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         params: Iterable[torch.Tensor],
-        lr: ScalarOrSchedule,
+        lr: ScalarOrSchedule = 1e-3,
         betas: tuple[float, float] = (0.9, 0.999),
         eps: float = 1e-8,
         weight_decay: float = 0.0,
         *,
         eps_root: float = 0.0,
         maximize: bool = False,
         use_accelerated_op: bool = False,
```

### Comparing `torchopt-0.7.0/torchopt/optim/adamw.py` & `torchopt-0.7.1/torchopt/optim/adamw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 MetaOPT Team. All Rights Reserved.
+# Copyright 2022-2023 MetaOPT Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -60,15 +60,15 @@
             betas (tuple of float, optional): Coefficients used for computing running averages of
                 gradient and its square. (default: :const:`(0.9, 0.999)`)
             eps (float, optional): A small constant applied to denominator outside of the square
                 root (as in the Adam paper) to avoid dividing by zero when rescaling.
                 (default: :const:`1e-8`)
             weight_decay (float, optional): Strength of the weight decay regularization. Note that
                 this weight decay is multiplied with the learning rate. This is consistent with
-                other frameworks such as PyTorch, but different from (Loshchilov et al, 2019) where
+                other frameworks such as PyTorch, but different from (Loshchilov et al., 2019) where
                 the weight decay is only multiplied with the "schedule multiplier", but not the base
                 learning rate. (default: :const:`1e-2`)
             eps_root (float, optional): A small constant applied to denominator inside the square
                 root (as in RMSProp), to avoid dividing by zero when rescaling. This is needed for
                 example when computing (meta-)gradients through Adam. (default: :const:`0.0`)
             mask (tree of Tensor, callable, or None, optional):
                 A tree with same structure as (or a prefix of) the params pytree, or a function that
```

### Comparing `torchopt-0.7.0/torchopt/optim/base.py` & `torchopt-0.7.1/torchopt/optim/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,20 +63,20 @@
 
         Args:
             set_to_none (bool, optional): Instead of setting to zero, set the ``grads`` to
                 :data:`None`. (default: :data:`False`)
         """
         if set_to_none:
 
-            def f(p):
+            def f(p: torch.Tensor) -> None:
                 p.grad = None
 
         else:
 
-            def f(p):
+            def f(p: torch.Tensor) -> None:
                 if p.grad is None:
                     return
                 if p.grad.grad_fn is not None:
                     p.grad.detach_()
                 else:
                     p.grad.requires_grad_(False)
                 p.grad.zero_()
@@ -106,15 +106,15 @@
                 the loss. Optional for most optimizers. (default: :data:`None`)
         """
         loss = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
-        def f(p):
+        def f(p: torch.Tensor) -> torch.Tensor | None:
             return p.grad
 
         for i, (params, state) in enumerate(zip(self.param_groups, self.state_groups)):
             if isinstance(state, UninitializedState):
                 state = self.impl.init(params)
             grads = pytree.tree_map(f, params)  # type: ignore[arg-type]
             updates, new_state = self.impl.update(grads, state, params=params, inplace=True)
```

### Comparing `torchopt-0.7.0/torchopt/optim/func/__init__.py` & `torchopt-0.7.1/torchopt/optim/func/__init__.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/torchopt/optim/func/base.py` & `torchopt-0.7.1/torchopt/optim/func/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 MetaOPT Team. All Rights Reserved.
+# Copyright 2022-2023 MetaOPT Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -30,14 +30,15 @@
     """A wrapper class to hold the functional optimizer.
 
     This wrapper makes it easier to maintain the optimizer states. The optimizer states are held by
     the wrapper internally. The wrapper provides a :meth:`step` function to compute the gradients
     and update the parameters.
 
     See Also:
+        - The functional AdaGrad optimizer: :func:`torchopt.adagrad`.
         - The functional Adam optimizer: :func:`torchopt.adam`.
         - The functional AdamW optimizer: :func:`torchopt.adamw`.
         - The functional RMSprop optimizer: :func:`torchopt.rmsprop`.
         - The functional SGD optimizer: :func:`torchopt.sgd`.
     """
 
     def __init__(self, impl: GradientTransformation, *, inplace: bool = False) -> None:
@@ -82,18 +83,20 @@
 
         if inplace is None:
             inplace = self.inplace
 
         # Step parameter only
         grads = torch.autograd.grad(loss, params, create_graph=True, allow_unused=True)
         updates, self.optim_state = self.impl.update(
-            grads, self.optim_state, params=params, inplace=inplace
+            grads,
+            self.optim_state,
+            params=params,
+            inplace=inplace,
         )
-        new_params = apply_updates(params, updates, inplace=inplace)
-        return new_params
+        return apply_updates(params, updates, inplace=inplace)
 
     def state_dict(self) -> OptState:
         """Extract the references of the optimizer states.
 
         Note that the states are references, so any in-place operations will change the states
         inside :class:`FuncOptimizer` at the same time.
         """
```

### Comparing `torchopt-0.7.0/torchopt/optim/meta/__init__.py` & `torchopt-0.7.1/torchopt/optim/meta/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 MetaOPT Team. All Rights Reserved.
+# Copyright 2022-2023 MetaOPT Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,12 +10,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Differentiable Meta-Optimizers."""
 
+from torchopt.optim.meta.adagrad import MetaAdaGrad, MetaAdagrad
 from torchopt.optim.meta.adam import MetaAdam
 from torchopt.optim.meta.adamw import MetaAdamW
 from torchopt.optim.meta.base import MetaOptimizer
 from torchopt.optim.meta.rmsprop import MetaRMSProp, MetaRMSprop
 from torchopt.optim.meta.sgd import MetaSGD
```

### Comparing `torchopt-0.7.0/torchopt/optim/meta/adam.py` & `torchopt-0.7.1/torchopt/optim/meta/adam.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/torchopt/optim/meta/adamw.py` & `torchopt-0.7.1/torchopt/optim/meta/adamw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 MetaOPT Team. All Rights Reserved.
+# Copyright 2022-2023 MetaOPT Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -60,15 +60,15 @@
             betas (tuple of float, optional): Coefficients used for computing running averages of
                 gradient and its square. (default: :const:`(0.9, 0.999)`)
             eps (float, optional): A small constant applied to denominator outside of the square
                 root (as in the Adam paper) to avoid dividing by zero when rescaling.
                 (default: :const:`1e-8`)
             weight_decay (float, optional): Strength of the weight decay regularization. Note that
                 this weight decay is multiplied with the learning rate. This is consistent with
-                other frameworks such as PyTorch, but different from (Loshchilov et al, 2019) where
+                other frameworks such as PyTorch, but different from (Loshchilov et al., 2019) where
                 the weight decay is only multiplied with the "schedule multiplier", but not the base
                 learning rate. (default: :const:`1e-2`)
             eps_root (float, optional): A small constant applied to denominator inside the square
                 root (as in RMSProp), to avoid dividing by zero when rescaling. This is needed for
                 example when computing (meta-)gradients through Adam. (default: :const:`0.0`)
             mask (tree of Tensor, callable, or None, optional):
                 A tree with same structure as (or a prefix of) the params pytree, or a function that
```

### Comparing `torchopt-0.7.0/torchopt/optim/meta/base.py` & `torchopt-0.7.1/torchopt/optim/meta/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         Args:
             loss (torch.Tensor): The loss that is used to compute the gradients to the network
                 parameters.
         """
         # Step parameter only
         for i, (param_container, state) in enumerate(
-            zip(self.param_containers_groups, self.state_groups)
+            zip(self.param_containers_groups, self.state_groups),
         ):
             flat_params: TupleOfTensors
             flat_params, container_treespec = pytree.tree_flatten_as_tuple(param_container)  # type: ignore[arg-type]
             if isinstance(state, UninitializedState):
                 state = self.impl.init(flat_params)
             grads = torch.autograd.grad(
                 loss,
@@ -85,15 +85,16 @@
                 state,
                 params=flat_params,
                 inplace=False,
             )
             self.state_groups[i] = new_state
             flat_new_params = apply_updates(flat_params, updates, inplace=False)
             new_params: ModuleTensorContainers = pytree.tree_unflatten(  # type: ignore[assignment]
-                container_treespec, flat_new_params
+                container_treespec,
+                flat_new_params,
             )
             for container, new_param in zip(param_container, new_params):
                 container.update(new_param)
 
     def add_param_group(self, module: nn.Module) -> None:
         """Add a param group to the optimizer's ``state_groups``."""
         params_container = extract_module_containers(module, with_buffers=False)[0]
```

### Comparing `torchopt-0.7.0/torchopt/optim/meta/rmsprop.py` & `torchopt-0.7.1/torchopt/optim/meta/rmsprop.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/torchopt/optim/meta/sgd.py` & `torchopt-0.7.1/torchopt/optim/meta/sgd.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/torchopt/optim/rmsprop.py` & `torchopt-0.7.1/torchopt/optim/rmsprop.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/torchopt/optim/sgd.py` & `torchopt-0.7.1/torchopt/optim/sgd.py`

 * *Files identical despite different names*

### Comparing `torchopt-0.7.0/torchopt/pytree.py` & `torchopt-0.7.1/torchopt/pytree.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,29 +98,33 @@
 
 def tree_add(*trees: PyTree[T]) -> PyTree[T]:
     """Tree addition over leaves."""
     return tree_map(acc_add, *trees)
 
 
 def tree_add_scalar_mul(
-    tree_x: TensorTree, tree_y: TensorTree, alpha: Scalar | None = None
+    tree_x: TensorTree,
+    tree_y: TensorTree,
+    alpha: Scalar | None = None,
 ) -> TensorTree:
     """Compute ``tree_x + alpha * tree_y``."""
     if alpha is None:
         return tree_map(lambda x, y: x.add(y), tree_x, tree_y)
     return tree_map(lambda x, y: x.add(y, alpha=alpha), tree_x, tree_y)
 
 
 def tree_sub(minuend_tree: PyTree[T], subtrahend_tree: PyTree[T]) -> PyTree[T]:
     """Tree subtraction over leaves."""
     return tree_map(operator.sub, minuend_tree, subtrahend_tree)
 
 
 def tree_sub_scalar_mul(
-    tree_x: TensorTree, tree_y: TensorTree, alpha: Scalar | None = None
+    tree_x: TensorTree,
+    tree_y: TensorTree,
+    alpha: Scalar | None = None,
 ) -> TensorTree:
     """Compute ``tree_x - alpha * tree_y``."""
     if alpha is None:
         return tree_map(lambda x, y: x.sub(y), tree_x, tree_y)
     return tree_map(lambda x, y: x.sub(y, alpha=alpha), tree_x, tree_y)
```

### Comparing `torchopt-0.7.0/torchopt/schedule/__init__.py` & `torchopt-0.7.1/torchopt/schedule/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 MetaOPT Team. All Rights Reserved.
+# Copyright 2022-2023 MetaOPT Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -27,11 +27,12 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Learning rate schedules."""
 
+from torchopt.schedule.exponential_decay import exponential_decay
 from torchopt.schedule.polynomial import linear_schedule, polynomial_schedule
 
 
-__all__ = ['polynomial_schedule', 'linear_schedule']
+__all__ = ['exponential_decay', 'polynomial_schedule', 'linear_schedule']
```

### Comparing `torchopt-0.7.0/torchopt/schedule/polynomial.py` & `torchopt-0.7.1/torchopt/schedule/polynomial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 MetaOPT Team. All Rights Reserved.
+# Copyright 2022-2023 MetaOPT Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -64,25 +64,25 @@
             annealing (before this many steps the scalar value is held fixed at ``init_value``).
             (default: :const:`0`)
 
     Returns:
         schedule:
             A function that maps step counts to values.
     """
-    if transition_steps <= 0:
+    if transition_steps <= 0:  # pragma: no cover
         logging.info(
             'A polynomial schedule was set with a non-positive `transition_steps` value; this '
-            'results in a constant schedule with value `init_value`.'
+            'results in a constant schedule with value `init_value`.',
         )
         return lambda count: init_value
 
-    if transition_begin < 0:
+    if transition_begin < 0:  # pragma: no cover
         logging.info(
             'An exponential schedule was set with a negative `transition_begin` value; this will '
-            'result in `transition_begin` falling back to `0`.'
+            'result in `transition_begin` falling back to `0`.',
         )
         transition_begin = 0
 
     def schedule(count: Numeric) -> Numeric:
         clip = torch.clamp if isinstance(count, torch.Tensor) else np.clip
         count = clip(count - transition_begin, 0, transition_steps)  # type: ignore[operator]
         frac = 1.0 - count / transition_steps
```

### Comparing `torchopt-0.7.0/torchopt/transform/__init__.py` & `torchopt-0.7.1/torchopt/transform/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,24 +32,26 @@
 """Preset transformations."""
 
 from torchopt.transform.add_decayed_weights import add_decayed_weights, masked
 from torchopt.transform.nan_to_num import nan_to_num
 from torchopt.transform.scale import scale
 from torchopt.transform.scale_by_adam import scale_by_accelerated_adam, scale_by_adam
 from torchopt.transform.scale_by_rms import scale_by_rms
+from torchopt.transform.scale_by_rss import scale_by_rss
 from torchopt.transform.scale_by_schedule import scale_by_schedule
 from torchopt.transform.scale_by_stddev import scale_by_stddev
 from torchopt.transform.trace import trace
 
 
 __all__ = [
     'trace',
     'scale',
     'scale_by_schedule',
     'add_decayed_weights',
     'masked',
     'scale_by_adam',
     'scale_by_accelerated_adam',
+    'scale_by_rss',
     'scale_by_rms',
     'scale_by_stddev',
     'nan_to_num',
 ]
```

### Comparing `torchopt-0.7.0/torchopt/transform/add_decayed_weights.py` & `torchopt-0.7.1/torchopt/transform/add_decayed_weights.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 # ==============================================================================
 """Preset transformations for adding weight decay to updates."""
 
 from __future__ import annotations
 
 from typing import Any, Callable, NamedTuple
 
+import torch
+
 from torchopt import pytree
 from torchopt.base import EmptyState, GradientTransformation, identity
 from torchopt.transform.utils import tree_map_flat, tree_map_flat_
 from torchopt.typing import OptState, Params, Updates
 
 
 __all__ = ['masked', 'add_decayed_weights']
@@ -99,20 +101,20 @@
 
 def _masked(
     inner: GradientTransformation,
     mask: OptState | Callable[[Params], OptState] | None = None,
     *,
     already_flattened: bool = False,
 ) -> GradientTransformation:
-    if already_flattened:
+    if already_flattened:  # noqa: SIM108
         tree_map = tree_map_flat
     else:
         tree_map = pytree.tree_map  # type: ignore[assignment]
 
-    def tree_mask(params, mask_tree):
+    def tree_mask(params: Params, mask_tree: OptState) -> Params:
         return tree_map(lambda p, m: p if m else MaskedNode(), params, mask_tree)
 
     def init_fn(params: Params) -> OptState:
         mask_tree = mask(params) if callable(mask) else mask
         masked_params = tree_mask(params, mask_tree)
         return MaskedState(inner_state=inner.init(masked_params))
 
@@ -124,19 +126,25 @@
         inplace: bool = True,
     ) -> tuple[Updates, OptState]:
         mask_tree = mask(updates) if callable(mask) else mask
         masked_updates = tree_mask(updates, mask_tree)
         masked_params = None if params is None else tree_mask(params, mask_tree)
 
         new_masked_updates, new_inner_state = inner.update(
-            masked_updates, state.inner_state, params=masked_params, inplace=inplace
+            masked_updates,
+            state.inner_state,
+            params=masked_params,
+            inplace=inplace,
         )
 
         new_updates = tree_map(
-            lambda old_u, new_u, m: new_u if m else old_u, updates, new_masked_updates, mask_tree
+            lambda old_u, new_u, m: new_u if m else old_u,
+            updates,
+            new_masked_updates,
+            mask_tree,
         )
         return new_updates, MaskedState(inner_state=new_inner_state)
 
     return GradientTransformation(init_fn, update_fn)
 
 
 masked.flat = _masked_flat  # type: ignore[attr-defined]
@@ -184,15 +192,15 @@
 def _add_decayed_weights(
     weight_decay: float = 0.0,
     mask: OptState | Callable[[Params], OptState] | None = None,
     *,
     already_flattened: bool = False,
 ) -> GradientTransformation:
     # pylint: disable-next=unneeded-not
-    if not 0.0 <= weight_decay:  # pragma: no cover
+    if not weight_decay >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid weight_decay value: {weight_decay}')
 
     if weight_decay == 0.0 and mask is None:
         return identity()
 
     if already_flattened:
         tree_map = tree_map_flat
@@ -214,24 +222,24 @@
         assert params is not None, (
             'Parameters are required for weight decay. '
             'Call `update(updates, state, params=params)` instead.'
         )
 
         if inplace:
 
-            def f(g, p):
+            def f(g: torch.Tensor, p: torch.Tensor) -> torch.Tensor:
                 if g.requires_grad:
                     return g.add_(p, alpha=weight_decay)
                 return g.add_(p.data, alpha=weight_decay)
 
             updates = tree_map_(f, updates, params)
 
         else:
 
-            def f(g, p):
+            def f(g: torch.Tensor, p: torch.Tensor) -> torch.Tensor:
                 return g.add(p, alpha=weight_decay)
 
             updates = tree_map(f, updates, params)
 
         return updates, state
 
     # If mask is not `None`, apply mask to the gradient transformation.
```

### Comparing `torchopt-0.7.0/torchopt/transform/nan_to_num.py` & `torchopt-0.7.1/torchopt/transform/nan_to_num.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Preset transformations that replaces updates with non-finite values to the given numbers."""
 
 from __future__ import annotations
 
+import torch
+
 from torchopt import pytree
 from torchopt.base import EmptyState, GradientTransformation
 from torchopt.typing import OptState, Params, Updates
 
 
 def nan_to_num(
     nan: float = 0.0,
@@ -40,19 +42,19 @@
         state: OptState,
         *,
         params: Params | None = None,  # pylint: disable=unused-argument
         inplace: bool = True,
     ) -> tuple[Updates, OptState]:
         if inplace:
 
-            def f(g):
+            def f(g: torch.Tensor) -> torch.Tensor:
                 return g.nan_to_num_(nan=nan, posinf=posinf, neginf=neginf)
 
         else:
 
-            def f(g):
+            def f(g: torch.Tensor) -> torch.Tensor:
                 return g.nan_to_num(nan=nan, posinf=posinf, neginf=neginf)
 
         new_updates = pytree.tree_map(f, updates)
         return new_updates, state
 
     return GradientTransformation(init_fn, update_fn)
```

### Comparing `torchopt-0.7.0/torchopt/transform/scale.py` & `torchopt-0.7.1/torchopt/transform/scale.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Preset transformation for scaling updates by learning rate."""
 
 from __future__ import annotations
 
+import torch
+
 from torchopt import pytree
 from torchopt.base import EmptyState, GradientTransformation
 from torchopt.transform.utils import tree_map_flat, tree_map_flat_
 from torchopt.typing import OptState, Params, Updates
 
 
 __all__ = ['scale']
@@ -81,22 +83,22 @@
         state: OptState,
         *,
         params: Params | None = None,  # pylint: disable=unused-argument
         inplace: bool = True,
     ) -> tuple[Updates, OptState]:
         if inplace:
 
-            def f(g):
+            def f(g: torch.Tensor) -> torch.Tensor:
                 return g.mul_(step_size)
 
             updates = tree_map_(f, updates)
 
         else:
 
-            def f(g):
+            def f(g: torch.Tensor) -> torch.Tensor:
                 return g.mul(step_size)
 
             updates = tree_map(f, updates)
 
         return updates, state
 
     return GradientTransformation(init_fn, update_fn)
```

### Comparing `torchopt-0.7.0/torchopt/transform/scale_by_adam.py` & `torchopt-0.7.1/torchopt/transform/scale_by_adam.py`

 * *Files 18% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     decay: float,
     count: OptState,
     *,
     already_flattened: bool = False,
 ) -> Updates:
     """Perform bias correction. This becomes a no-op as count goes to infinity."""
 
-    def f(t, c):  # pylint: disable=invalid-name
+    def f(t: torch.Tensor, c: torch.Tensor) -> torch.Tensor:  # pylint: disable=invalid-name
         return t.div(1 - pow(decay, c))
 
     if already_flattened:
         return tree_map_flat(f, moment, count)
     return pytree.tree_map(f, moment, count)
 
 
@@ -83,15 +83,15 @@
     eps: float = 1e-8,
     eps_root: float = 0.0,
     moment_requires_grad: bool = False,
 ) -> GradientTransformation:
     """Rescale updates according to the Adam algorithm.
 
     References:
-        [Kingma et al, 2014](https://arxiv.org/abs/1412.6980)
+        - Kingma et al., 2014: https://arxiv.org/abs/1412.6980
 
     Args:
         b1 (float, optional): Decay rate for the exponentially weighted average of grads.
             (default: :const:`0.9`)
         b2 (float, optional): Decay rate for the exponentially weighted average of squared grads.
             (default: :const:`0.999`)
         eps (float, optional): Term added to the denominator to improve numerical stability.
@@ -138,65 +138,86 @@
     eps: float = 1e-8,
     eps_root: float = 0.0,
     moment_requires_grad: bool = False,
     *,
     already_flattened: bool = False,
 ) -> GradientTransformation:
     # pylint: disable=unneeded-not
-    if not 0.0 <= eps:  # pragma: no cover
+    if not eps >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid epsilon value: {eps}')
     if not 0.0 <= b1 < 1.0:  # pragma: no cover
         raise ValueError(f'Invalid beta parameter at index 0: {b1}')
     if not 0.0 <= b2 < 1.0:  # pragma: no cover
         raise ValueError(f'Invalid beta parameter at index 1: {b2}')
     # pylint: enable=unneeded-not
 
-    if already_flattened:
+    if already_flattened:  # noqa: SIM108
         tree_map = tree_map_flat
     else:
         tree_map = pytree.tree_map  # type: ignore[assignment]
 
     def init_fn(params: Params) -> OptState:
         zero = tree_map(  # count init
-            lambda t: torch.zeros(1, dtype=torch.int64, device=t.device).squeeze_(), params
+            lambda t: torch.zeros(1, dtype=torch.int64, device=t.device).squeeze_(),
+            params,
         )
         mu = tree_map(  # first moment
-            lambda t: torch.zeros_like(t, requires_grad=moment_requires_grad), params
+            lambda t: torch.zeros_like(t, requires_grad=moment_requires_grad),
+            params,
         )
         nu = tree_map(  # second moment
-            lambda t: torch.zeros_like(t, requires_grad=moment_requires_grad), params
+            lambda t: torch.zeros_like(t, requires_grad=moment_requires_grad),
+            params,
         )
         return ScaleByAdamState(mu=mu, nu=nu, count=zero)
 
     def update_fn(
         updates: Updates,
         state: OptState,
         *,
         params: Params | None = None,  # pylint: disable=unused-argument
         inplace: bool = True,
     ) -> tuple[Updates, OptState]:
         mu = update_moment.impl(  # type: ignore[attr-defined]
-            updates, state.mu, b1, order=1, inplace=inplace, already_flattened=already_flattened
+            updates,
+            state.mu,
+            b1,
+            order=1,
+            inplace=inplace,
+            already_flattened=already_flattened,
         )
         nu = update_moment.impl(  # type: ignore[attr-defined]
-            updates, state.nu, b2, order=2, inplace=inplace, already_flattened=already_flattened
+            updates,
+            state.nu,
+            b2,
+            order=2,
+            inplace=inplace,
+            already_flattened=already_flattened,
         )
         # pylint: disable=line-too-long
         count_inc = inc_count.impl(updates, state.count, already_flattened=already_flattened)  # type: ignore[attr-defined]
         mu_hat = _bias_correction(mu, b1, count_inc, already_flattened=already_flattened)
         nu_hat = _bias_correction(nu, b2, count_inc, already_flattened=already_flattened)
 
         if inplace:
 
-            def f(g, m, v):  # pylint: disable=unused-argument
+            def f(
+                g: torch.Tensor,  # pylint: disable=unused-argument
+                m: torch.Tensor,
+                v: torch.Tensor,
+            ) -> torch.Tensor:
                 return m.div_(v.add_(eps_root).sqrt_().add(eps))
 
         else:
 
-            def f(g, m, v):  # pylint: disable=unused-argument
+            def f(
+                g: torch.Tensor,  # pylint: disable=unused-argument
+                m: torch.Tensor,
+                v: torch.Tensor,
+            ) -> torch.Tensor:
                 return m.div(v.add(eps_root).sqrt_().add(eps))
 
         updates = tree_map(f, updates, mu_hat, nu_hat)
         return updates, ScaleByAdamState(mu=mu, nu=nu, count=count_inc)
 
     return GradientTransformation(init_fn, update_fn)
 
@@ -213,15 +234,15 @@
     moment_requires_grad: bool = False,
 ) -> GradientTransformation:
     """Rescale updates according to the Adam algorithm.
 
     This function is accelerated by using some fused accelerated operators.
 
     References:
-        [Kingma et al, 2014](https://arxiv.org/abs/1412.6980)
+        - Kingma et al., 2014: https://arxiv.org/abs/1412.6980
 
     Args:
         b1 (float, optional): Decay rate for the exponentially weighted average of grads.
             (default: :const:`0.9`)
         b2 (float, optional): Decay rate for the exponentially weighted average of squared grads.
             (default: :const:`0.999`)
         eps (float, optional): Term added to the denominator to improve numerical stability.
@@ -268,15 +289,15 @@
     eps: float = 1e-8,
     eps_root: float = 0.0,
     moment_requires_grad: bool = False,
     *,
     already_flattened: bool = False,
 ) -> GradientTransformation:
     # pylint: disable=unneeded-not
-    if not 0.0 <= eps:  # pragma: no cover
+    if not eps >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid epsilon value: {eps}')
     if not 0.0 <= b1 < 1.0:  # pragma: no cover
         raise ValueError(f'Invalid beta parameter at index 0: {b1}')
     if not 0.0 <= b2 < 1.0:  # pragma: no cover
         raise ValueError(f'Invalid beta parameter at index 1: {b2}')
     # pylint: enable=unneeded-not
 
@@ -289,51 +310,113 @@
             *,
             params: Params | None = None,  # pylint: disable=unused-argument
             inplace: bool = True,
         ) -> tuple[Updates, OptState]:
             count_inc = inc_count.impl(updates, state.count, already_flattened=True)  # type: ignore[attr-defined]
 
             op = AdamOp(b1=b1, b2=b2, eps=eps, eps_root=eps_root, inplace=inplace)
-            out = tree_map_flat(op, state.mu, state.nu, updates, count_inc)
 
-            new_mu, new_nu, new_updates = tuple(zip(*out))  # transpose
+            def op_fn(
+                mu: torch.Tensor | None,
+                nu: torch.Tensor | None,
+                update: torch.Tensor | None,
+                count: torch.Tensor | None,
+            ) -> tuple[torch.Tensor | None, torch.Tensor | None, torch.Tensor | None]:
+                if mu is None:
+                    return (None, None, None)
+                return op(mu, nu, update, count)  # type: ignore[arg-type]
+
+            out = tree_map_flat(
+                op_fn,
+                state.mu,
+                state.nu,
+                updates,
+                count_inc,
+                none_is_leaf=True,
+            )
+
+            if len(out) == 0:
+                new_mu, new_nu, new_updates = (), (), ()
+            else:
+                new_mu, new_nu, new_updates = tuple(zip(*out))  # transpose
+
+            new_mu, new_nu, new_updates = (
+                new if type(new) is type(old) else type(old)(new)
+                for new, old in (
+                    (new_mu, state.mu),
+                    (new_nu, state.nu),
+                    (new_updates, updates),
+                )
+            )
+
             return new_updates, ScaleByAdamState(mu=new_mu, nu=new_nu, count=count_inc)
 
     else:
         tree_map = pytree.tree_map  # type: ignore[assignment]
 
         def update_fn(
             updates: Updates,
             state: OptState,
             *,
             params: Params | None = None,  # pylint: disable=unused-argument
             inplace: bool = True,
         ) -> tuple[Updates, OptState]:
             count_inc = inc_count.impl(updates, state.count, already_flattened=False)  # type: ignore[attr-defined]
 
-            treespec = pytree.tree_structure(updates, none_is_leaf=True)
-
-            op = AdamOp(b1=b1, b2=b2, eps=eps, eps_root=eps_root, inplace=inplace)
-            out = pytree.tree_map(op, state.mu, state.nu, updates, count_inc)
-
             new_mu: Updates
             new_nu: Updates
             new_updates: Updates
-            new_mu, new_nu, new_updates = pytree.tree_transpose(treespec, TRIPLE_PYTREE_SPEC, out)  # type: ignore[misc]
+
+            treespec = pytree.tree_structure(updates, none_is_leaf=True)
+            if treespec.num_leaves > 0:
+                op = AdamOp(b1=b1, b2=b2, eps=eps, eps_root=eps_root, inplace=inplace)
+
+                def op_fn(
+                    mu: torch.Tensor | None,
+                    nu: torch.Tensor | None,
+                    update: torch.Tensor | None,
+                    count: torch.Tensor | None,
+                ) -> tuple[torch.Tensor | None, torch.Tensor | None, torch.Tensor | None]:
+                    if mu is None:
+                        return (None, None, None)
+                    return op(mu, nu, update, count)  # type: ignore[arg-type]
+
+                out = pytree.tree_map(
+                    op_fn,
+                    state.mu,
+                    state.nu,
+                    updates,
+                    count_inc,
+                    none_is_leaf=True,
+                )
+
+                new_mu, new_nu, new_updates = pytree.tree_transpose(  # type: ignore[misc]
+                    treespec,
+                    TRIPLE_PYTREE_SPEC,
+                    out,
+                )
+            else:
+                new_mu = pytree.tree_unflatten(treespec, ())
+                new_nu = pytree.tree_unflatten(treespec, ())
+                new_updates = pytree.tree_unflatten(treespec, ())
+
             return new_updates, ScaleByAdamState(mu=new_mu, nu=new_nu, count=count_inc)
 
     def init_fn(params: Params) -> OptState:
         zero = tree_map(  # count init
-            lambda t: torch.zeros(1, dtype=torch.int64, device=t.device).squeeze_(), params
+            lambda t: torch.zeros(1, dtype=torch.int64, device=t.device).squeeze_(),
+            params,
         )
         mu = tree_map(  # first moment
-            lambda t: torch.zeros_like(t, requires_grad=moment_requires_grad), params
+            lambda t: torch.zeros_like(t, requires_grad=moment_requires_grad),
+            params,
         )
         nu = tree_map(  # second moment
-            lambda t: torch.zeros_like(t, requires_grad=moment_requires_grad), params
+            lambda t: torch.zeros_like(t, requires_grad=moment_requires_grad),
+            params,
         )
         return ScaleByAdamState(mu=mu, nu=nu, count=zero)
 
     return GradientTransformation(init_fn, update_fn)
 
 
 scale_by_accelerated_adam.flat = _scale_by_accelerated_adam_flat  # type: ignore[attr-defined]
```

### Comparing `torchopt-0.7.0/torchopt/transform/scale_by_rms.py` & `torchopt-0.7.1/torchopt/transform/scale_by_rms.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     alpha: float = 0.9,
     eps: float = 1e-8,
     initial_scale: float = 0.0,
 ) -> GradientTransformation:
     """Rescale updates by the root of the exp. moving avg of the square.
 
     References:
-        [Hinton](www.cs.toronto.edu/~tijmen/csc321/slides/lecture_slides_lec6.pdf)
+        - Tieleman and Hinton, 2012: http://www.cs.toronto.edu/~hinton/coursera/lecture6/lec6.pdf
 
     Args:
         alpha (float, optional): Decay rate for the exponentially weighted average of squared grads.
             (default: :const:`0.9`)
         eps (float, optional): Term added to the denominator to improve numerical stability.
             (default: :const:`1e-8`)
         initial_scale (float, optional): Initial value for second moment. (default: :const:`0.0`)
@@ -97,17 +97,17 @@
     alpha: float = 0.9,
     eps: float = 1e-8,
     initial_scale: float = 0.0,
     *,
     already_flattened: bool = False,
 ) -> GradientTransformation:
     # pylint: disable=unneeded-not
-    if not 0.0 <= alpha:  # pragma: no cover
+    if not alpha >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid alpha value: {alpha}')
-    if not 0.0 <= eps:  # pragma: no cover
+    if not eps >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid epsilon value: {eps}')
     # pylint: enable=unneeded-not
 
     if already_flattened:
         tree_map = tree_map_flat
         tree_map_ = tree_map_flat_
     else:
@@ -122,27 +122,32 @@
         updates: Updates,
         state: OptState,
         *,
         params: Params | None = None,  # pylint: disable=unused-argument
         inplace: bool = True,
     ) -> tuple[Updates, OptState]:
         nu = update_moment.impl(  # type: ignore[attr-defined]
-            updates, state.nu, alpha, order=2, inplace=inplace, already_flattened=already_flattened
+            updates,
+            state.nu,
+            alpha,
+            order=2,
+            inplace=inplace,
+            already_flattened=already_flattened,
         )
 
         if inplace:
 
-            def f(g, n):  # pylint: disable=invalid-name
+            def f(g: torch.Tensor, n: torch.Tensor) -> torch.Tensor:  # pylint: disable=invalid-name
                 return g.div_(n.sqrt().add_(eps))
 
             updates = tree_map_(f, updates, nu)
 
         else:
 
-            def f(g, n):  # pylint: disable=invalid-name
+            def f(g: torch.Tensor, n: torch.Tensor) -> torch.Tensor:  # pylint: disable=invalid-name
                 return g.div(n.sqrt().add(eps))
 
             updates = tree_map(f, updates, nu)
 
         return updates, ScaleByRmsState(nu=nu)
 
     return GradientTransformation(init_fn, update_fn)
```

### Comparing `torchopt-0.7.0/torchopt/transform/scale_by_schedule.py` & `torchopt-0.7.1/torchopt/transform/scale_by_schedule.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from typing import NamedTuple
 
 import torch
 
 from torchopt import pytree
 from torchopt.base import GradientTransformation
 from torchopt.transform.utils import inc_count, tree_map_flat, tree_map_flat_
-from torchopt.typing import OptState, Params, Schedule, SequenceOfTensors, Updates
+from torchopt.typing import Numeric, OptState, Params, Schedule, SequenceOfTensors, Updates
 
 
 __all__ = ['scale_by_schedule']
 
 
 class ScaleByScheduleState(NamedTuple):
     """Maintain count for scale scheduling."""
@@ -79,49 +79,50 @@
         tree_map_ = tree_map_flat_
     else:
         tree_map = pytree.tree_map  # type: ignore[assignment]
         tree_map_ = pytree.tree_map_  # type: ignore[assignment]
 
     def init_fn(params: Params) -> OptState:
         zero = tree_map(  # count init
-            lambda t: torch.zeros(1, dtype=torch.int64, device=t.device).squeeze_(), params
+            lambda t: torch.zeros(1, dtype=torch.int64, device=t.device).squeeze_(),
+            params,
         )
         return ScaleByScheduleState(count=zero)
 
     def update_fn(
         updates: Updates,
         state: OptState,
         *,
         params: Params | None = None,  # pylint: disable=unused-argument
         inplace: bool = True,
     ) -> tuple[Updates, OptState]:
         if inplace:
 
-            def f(g, c):  # pylint: disable=invalid-name
+            def f(g: torch.Tensor, c: Numeric) -> torch.Tensor:  # pylint: disable=invalid-name
                 step_size = step_size_fn(c)
                 return g.mul_(step_size)
 
             updates = tree_map_(f, updates, state.count)
 
         else:
 
-            def f(g, c):  # pylint: disable=invalid-name
+            def f(g: torch.Tensor, c: Numeric) -> torch.Tensor:  # pylint: disable=invalid-name
                 step_size = step_size_fn(c)
                 return g.mul(step_size)
 
             updates = tree_map(f, updates, state.count)
 
         return (
             updates,
             ScaleByScheduleState(
                 count=inc_count.impl(  # type: ignore[attr-defined]
                     updates,
                     state.count,
                     already_flattened=already_flattened,
-                )
+                ),
             ),
         )
 
     return GradientTransformation(init_fn, update_fn)
 
 
 scale_by_schedule.flat = _scale_by_schedule_flat  # type: ignore[attr-defined]
```

### Comparing `torchopt-0.7.0/torchopt/transform/scale_by_stddev.py` & `torchopt-0.7.1/torchopt/transform/scale_by_stddev.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     alpha: float = 0.9,
     eps: float = 1e-8,
     initial_scale: float = 0.0,
 ) -> GradientTransformation:
     """Rescale updates by the root of the centered exponential moving average of squares.
 
     References:
-        [Hinton](www.cs.toronto.edu/~tijmen/csc321/slides/lecture_slides_lec6.pdf)
+        - Tieleman and Hinton, 2012: http://www.cs.toronto.edu/~hinton/coursera/lecture6/lec6.pdf
 
     Args:
         alpha (float, optional): Decay rate for the exponentially weighted average of squared grads.
             (default: :const:`0.9`)
         eps (float, optional): Term added to the denominator to improve numerical stability.
             (default: :const:`1e-8`)
         initial_scale (float, optional): Initial value for second moment. (default: :const:`0.0`)
@@ -100,17 +100,17 @@
     alpha: float = 0.9,
     eps: float = 1e-8,
     initial_scale: float = 0.0,
     *,
     already_flattened: bool = False,
 ) -> GradientTransformation:
     # pylint: disable=unneeded-not
-    if not 0.0 <= alpha:  # pragma: no cover
+    if not alpha >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid alpha value: {alpha}')
-    if not 0.0 <= eps:  # pragma: no cover
+    if not eps >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid epsilon value: {eps}')
     # pylint: enable=unneeded-not
 
     if already_flattened:
         tree_map = tree_map_flat
         tree_map_ = tree_map_flat_
     else:
@@ -126,30 +126,40 @@
         updates: Updates,
         state: OptState,
         *,
         params: Params | None = None,  # pylint: disable=unused-argument
         inplace: bool = True,
     ) -> tuple[Updates, OptState]:
         mu = update_moment.impl(  # type: ignore[attr-defined]
-            updates, state.mu, alpha, order=1, inplace=inplace, already_flattened=already_flattened
+            updates,
+            state.mu,
+            alpha,
+            order=1,
+            inplace=inplace,
+            already_flattened=already_flattened,
         )
         nu = update_moment.impl(  # type: ignore[attr-defined]
-            updates, state.nu, alpha, order=2, inplace=inplace, already_flattened=already_flattened
+            updates,
+            state.nu,
+            alpha,
+            order=2,
+            inplace=inplace,
+            already_flattened=already_flattened,
         )
 
         if inplace:
 
-            def f(g, m, n):
+            def f(g: torch.Tensor, m: torch.Tensor, n: torch.Tensor) -> torch.Tensor:
                 return g.div_(n.addcmul(m, m, value=-1.0).sqrt_().add(eps))
 
             updates = tree_map_(f, updates, mu, nu)
 
         else:
 
-            def f(g, m, n):
+            def f(g: torch.Tensor, m: torch.Tensor, n: torch.Tensor) -> torch.Tensor:
                 return g.div(n.addcmul(m, m, value=-1.0).sqrt_().add(eps))
 
             updates = tree_map(f, updates, mu, nu)
 
         return updates, ScaleByRStdDevState(mu=mu, nu=nu)
 
     return GradientTransformation(init_fn, update_fn)
```

### Comparing `torchopt-0.7.0/torchopt/transform/trace.py` & `torchopt-0.7.1/torchopt/transform/trace.py`

 * *Files 13% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     dampening: float = 0.0,
     nesterov: bool = False,
     moment_requires_grad: bool = False,
     *,
     already_flattened: bool = False,
 ) -> GradientTransformation:
     # pylint: disable=unneeded-not
-    if not 0.0 <= momentum:  # pragma: no cover
+    if not momentum >= 0.0:  # pragma: no cover
         raise ValueError(f'Invalid momentum value: {momentum}')
     if nesterov and (momentum <= 0.0 or dampening != 0.0):  # pragma: no cover
         raise ValueError('Nesterov momentum requires a momentum and zero dampening')
     # pylint: enable=unneeded-not
 
     if momentum == 0.0:
         return identity()
@@ -125,16 +125,17 @@
     else:
         tree_map = pytree.tree_map  # type: ignore[assignment]
         tree_map_ = pytree.tree_map_  # type: ignore[assignment]
 
     def init_fn(params: Params) -> OptState:
         return TraceState(
             trace=tree_map(
-                lambda t: torch.zeros_like(t, requires_grad=moment_requires_grad), params
-            )
+                lambda t: torch.zeros_like(t, requires_grad=moment_requires_grad),
+                params,
+            ),
         )
 
     first_call = True
 
     def update_fn(
         updates: Updates,
         state: OptState,
@@ -143,55 +144,55 @@
         inplace: bool = True,
     ) -> tuple[Updates, OptState]:
         nonlocal first_call
 
         if nesterov:
             if inplace:
 
-                def f1(g, t):
+                def f1(g: torch.Tensor, t: torch.Tensor) -> torch.Tensor:
                     if first_call:
                         return t.add_(g)
                     return t.mul_(momentum).add_(g)
 
-                def f2(g, t):
+                def f2(g: torch.Tensor, t: torch.Tensor) -> torch.Tensor:
                     return g.add_(t, alpha=momentum)
 
                 new_trace = tree_map(f1, updates, state.trace)
                 updates = tree_map_(f2, updates, new_trace)
 
             else:
 
-                def f1(g, t):
+                def f1(g: torch.Tensor, t: torch.Tensor) -> torch.Tensor:
                     if first_call:
                         return t.add(g)
                     return t.mul(momentum).add_(g)
 
-                def f2(g, t):
+                def f2(g: torch.Tensor, t: torch.Tensor) -> torch.Tensor:
                     return g.add(t, alpha=momentum)
 
                 new_trace = tree_map(f1, updates, state.trace)
                 updates = tree_map(f2, updates, new_trace)
 
         else:
             if inplace:
 
-                def f(g, t):
+                def f(g: torch.Tensor, t: torch.Tensor) -> torch.Tensor:
                     if first_call:
                         return t.add_(g)
                     return t.mul_(momentum).add_(g, alpha=1.0 - dampening)
 
-                def copy_(g, t):
+                def copy_(g: torch.Tensor, t: torch.Tensor) -> torch.Tensor:
                     return g.copy_(t)
 
                 new_trace = tree_map(f, updates, state.trace)
                 updates = tree_map_(copy_, updates, new_trace)
 
             else:
 
-                def f(g, t):
+                def f(g: torch.Tensor, t: torch.Tensor) -> torch.Tensor:
                     if first_call:
                         return t.add(g)
                     return t.mul(momentum).add_(g, alpha=1.0 - dampening)
 
                 new_trace = tree_map(f, updates, state.trace)
                 updates = tree_map(torch.clone, new_trace)
```

### Comparing `torchopt-0.7.0/torchopt/transform/utils.py` & `torchopt-0.7.1/torchopt/transform/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     none_is_leaf: bool = False,
 ) -> Sequence[Any]:
     """Apply a function to each element of a flattened list."""
     if none_is_leaf:
         fn = func
     else:
 
-        def fn(x, *xs):
+        def fn(x: Any | None, *xs: Any) -> Any | None:
             return func(x, *xs) if x is not None else None
 
     return flat_arg.__class__(map(fn, flat_arg, *flat_args))  # type: ignore[call-arg]
 
 
 def tree_map_flat_(
     func: Callable,
@@ -72,15 +72,15 @@
     none_is_leaf: bool = False,
 ) -> Sequence[Any]:
     """Apply a function to each element of a flattened list and return the original list."""
     if none_is_leaf:
         fn = func
     else:
 
-        def fn(x, *xs):
+        def fn(x: Any | None, *xs: Any) -> Any | None:
             return func(x, *xs) if x is not None else None
 
     flat_results = map(fn, flat_arg, *flat_args)
     deque(flat_results, maxlen=0)  # consume and exhaust the iterable
     return flat_arg
 
 
@@ -107,15 +107,15 @@
 
 def _inc_count(
     updates: Updates,
     count: TensorTree,
     *,
     already_flattened: bool = False,
 ) -> TensorTree:
-    def f(c, g):  # pylint: disable=invalid-name
+    def f(c: torch.Tensor, g: torch.Tensor | None) -> torch.Tensor:  # pylint: disable=invalid-name
         return c + (c != INT64_MAX).to(torch.int64) if g is not None else c
 
     if already_flattened:
         return tree_map_flat(f, count, updates, none_is_leaf=True)
     return pytree.tree_map(f, count, updates, none_is_leaf=True)
 
 
@@ -163,39 +163,63 @@
 def _update_moment(
     updates: Updates,
     moments: TensorTree,
     decay: float,
     *,
     order: int,
     inplace: bool = True,
-    already_flattened=False,
+    already_flattened: bool = False,
 ) -> TensorTree:
     assert order in (1, 2)
 
     if inplace:
         if order == 2:
+            if decay != 1.0:
+
+                def f(g: torch.Tensor | None, t: torch.Tensor) -> torch.Tensor:
+                    return t.mul_(decay).addcmul_(g, g, value=1 - decay) if g is not None else t
+
+            else:
 
-            def f(g, t):
-                return t.mul_(decay).addcmul_(g, g, value=1 - decay) if g is not None else t
+                def f(g: torch.Tensor | None, t: torch.Tensor) -> torch.Tensor:
+                    return t.addcmul_(g, g) if g is not None else t
 
         else:
+            if decay != 1.0:
+
+                def f(g: torch.Tensor | None, t: torch.Tensor) -> torch.Tensor:
+                    return t.mul_(decay).add_(g, alpha=1 - decay) if g is not None else t
+
+            else:
 
-            def f(g, t):
-                return t.mul_(decay).add_(g, alpha=1 - decay) if g is not None else t
+                def f(g: torch.Tensor | None, t: torch.Tensor) -> torch.Tensor:
+                    return t.add_(g) if g is not None else t
 
     else:
         if order == 2:
+            if decay != 1.0:
 
-            def f(g, t):
-                return t.mul(decay).addcmul_(g, g, value=1 - decay) if g is not None else t
+                def f(g: torch.Tensor | None, t: torch.Tensor) -> torch.Tensor:
+                    return t.mul(decay).addcmul_(g, g, value=1 - decay) if g is not None else t
+
+            else:
+
+                def f(g: torch.Tensor | None, t: torch.Tensor) -> torch.Tensor:
+                    return t.addcmul(g, g) if g is not None else t
 
         else:
+            if decay != 1.0:
+
+                def f(g: torch.Tensor | None, t: torch.Tensor) -> torch.Tensor:
+                    return t.mul(decay).add_(g, alpha=1 - decay) if g is not None else t
+
+            else:
 
-            def f(g, t):
-                return t.mul(decay).add_(g, alpha=1 - decay) if g is not None else t
+                def f(g: torch.Tensor | None, t: torch.Tensor) -> torch.Tensor:
+                    return t.add(g) if g is not None else t
 
     if already_flattened:
         return tree_map_flat(f, updates, moments, none_is_leaf=True)
     return pytree.tree_map(f, updates, moments, none_is_leaf=True)
 
 
 update_moment.flat = _update_moment_flat  # type: ignore[attr-defined]
```

### Comparing `torchopt-0.7.0/torchopt/typing.py` & `torchopt-0.7.1/torchopt/typing.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,17 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Typing utilities."""
 
 import abc
-from typing import Callable, Dict, List, Optional, Sequence, Tuple, TypeVar, Union
+from typing import (
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Protocol,
+    Sequence,
+    Tuple,
+    TypeVar,
+    Union,
+    runtime_checkable,
+)
 from typing_extensions import TypeAlias  # Python 3.10+
-from typing_extensions import Protocol, runtime_checkable  # Python 3.8+
 
 import torch
 import torch.distributed.rpc as rpc
 from optree.typing import PyTree, PyTreeTypeVar
 from torch import Tensor
 from torch.distributions import Distribution
 from torch.futures import Future
@@ -122,15 +132,16 @@
 
 @runtime_checkable
 class Samplable(Protocol):  # pylint: disable=too-few-public-methods
     """Abstract protocol class that supports sampling."""
 
     @abc.abstractmethod
     def sample(
-        self, sample_shape: Size = Size()  # pylint: disable=unused-argument
+        self,
+        sample_shape: Size = Size(),  # noqa: B008 # pylint: disable=unused-argument
     ) -> Union[Tensor, Sequence[Numeric]]:
         # pylint: disable-next=line-too-long
         """Generate a sample_shape shaped sample or sample_shape shaped batch of samples if the distribution parameters are batched."""
-        raise NotImplementedError  # pragma: no cover
+        raise NotImplementedError
 
 
 Samplable.register(Distribution)
```

### Comparing `torchopt-0.7.0/torchopt/update.py` & `torchopt-0.7.1/torchopt/update.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Helper functions for applying updates."""
 
+from __future__ import annotations
+
+import torch
+
 from torchopt import pytree
 from torchopt.typing import Params, Updates
 
 
 __all__ = ['apply_updates']
 
 
@@ -55,18 +59,18 @@
             (default: :data:`True`)
 
     Returns:
         Updated parameters, with same structure, shape and type as ``params``.
     """
     if inplace:
 
-        def f(p, u):
+        def f(p: torch.Tensor, u: torch.Tensor | None) -> torch.Tensor:
             if u is not None:
                 p.data.add_(u)
             return p
 
     else:
 
-        def f(p, u):
+        def f(p: torch.Tensor, u: torch.Tensor | None) -> torch.Tensor:
             return p.add(u) if u is not None else p
 
     return pytree.tree_map(f, params, updates)
```

### Comparing `torchopt-0.7.0/torchopt/utils.py` & `torchopt-0.7.1/torchopt/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,25 @@
 # ==============================================================================
 """Utilities for TorchOpt."""
 
 from __future__ import annotations
 
 import copy
 import itertools
-from typing import TYPE_CHECKING, NamedTuple, Sequence, cast, overload
-from typing_extensions import Literal  # Python 3.8+
+from typing import TYPE_CHECKING, Any, Literal, NamedTuple, Sequence, cast, overload
 from typing_extensions import TypeAlias  # Python 3.10+
 
 import torch
 import torch.nn as nn
 
 from torchopt import pytree
 from torchopt.typing import Device, ModuleTensorContainers, OptState, TensorContainer, TensorTree
 
 
-if TYPE_CHECKING:  # pragma: no cover
+if TYPE_CHECKING:
     from torchopt.optim.meta.base import MetaOptimizer
 
 
 __all__ = [
     'ModuleState',
     'stop_gradient',
     'extract_state_dict',
@@ -42,16 +41,16 @@
     'module_detach_',
 ]
 
 
 class ModuleState(NamedTuple):
     """Container for module state."""
 
-    params: tuple[dict[str, torch.Tensor], ...]
-    buffers: tuple[dict[str, torch.Tensor], ...]
+    params: tuple[TensorContainer, ...]
+    buffers: tuple[TensorContainer, ...]
     visual_contents: dict | None = None
     detach_buffers: bool = False
 
 
 CopyMode: TypeAlias = Literal['reference', 'copy', 'deepcopy', 'ref', 'clone', 'deepclone']
 
 
@@ -70,15 +69,15 @@
             detached from the computation graph, it could be a :class:`nn.Module`,
             :class:`torchopt.MetaOptimizer`, state of the :class:`torchopt.MetaOptimizer`, or just
             a plain list of tensors.
     """
     # pylint: disable-next=import-outside-toplevel
     from torchopt.optim.meta.base import MetaOptimizer
 
-    def fn_(obj):
+    def fn_(obj: Any) -> None:
         if isinstance(obj, torch.Tensor):
             requires_grad = obj.requires_grad
             obj.detach_().requires_grad_(requires_grad)
 
     if isinstance(target, ModuleState):
         true_target = cast(TensorTree, (target.params, target.buffers))
     elif isinstance(target, nn.Module):
@@ -94,29 +93,27 @@
 @overload
 def extract_state_dict(
     target: nn.Module,
     *,
     by: CopyMode = 'reference',
     device: Device | None = None,
     with_buffers: bool = True,
+    detach_buffers: bool = False,
     enable_visual: bool = False,
     visual_prefix: str = '',
 ) -> ModuleState:  # pragma: no cover
     ...
 
 
 @overload
 def extract_state_dict(
     target: MetaOptimizer,
     *,
     by: CopyMode = 'reference',
     device: Device | None = None,
-    with_buffers: bool = True,
-    enable_visual: bool = False,
-    visual_prefix: str = '',
 ) -> tuple[OptState, ...]:  # pragma: no cover
     ...
 
 
 # pylint: disable-next=too-many-branches,too-many-locals
 def extract_state_dict(
     target: nn.Module | MetaOptimizer,
@@ -181,15 +178,16 @@
 
         def clone(t: torch.Tensor) -> torch.Tensor:
             return t.clone().to(device=target_device)
 
         def clone_detach_(t: torch.Tensor) -> torch.Tensor:
             if isinstance(t, nn.Parameter):
                 return nn.Parameter(
-                    t.clone().to(device=target_device).detach_(), requires_grad=t.requires_grad
+                    t.clone().to(device=target_device).detach_(),
+                    requires_grad=t.requires_grad,
                 )
             return t.clone().to(device=target_device).detach_().requires_grad_(t.requires_grad)
 
     else:
 
         def reference(t: torch.Tensor) -> torch.Tensor:
             return t
@@ -217,93 +215,94 @@
                 if v.grad_fn is not None:
                     visual_contents.update({v.grad_fn: (visual_prefix + k, v)})
                 else:
                     visual_contents.update({v: visual_prefix + k})  # type: ignore[dict-item]
         else:
             visual_contents = None
 
-        params: list[dict[str, torch.Tensor]] = []
-        buffers: list[dict[str, torch.Tensor]] = []
+        params: list[TensorContainer] = []
+        buffers: list[TensorContainer] = []
         memo: set[nn.Module] = set()
 
-        def update_params(container):
+        def update_params(container: TensorContainer) -> None:
             if len(container) > 0:
                 params.append(
                     type(container)(
                         (k, replicate(v))
                         for k, v in container.items()
                         if isinstance(v, torch.Tensor)
-                    )
+                    ),
                 )
 
-        def update_buffers(container):
+        def update_buffers(container: TensorContainer) -> None:
             if len(container) > 0:
                 fn = clone_detach_ if detach_buffers else replicate
                 buffers.append(
                     type(container)(
                         (k, fn(v)) for k, v in container.items() if isinstance(v, torch.Tensor)
-                    )
+                    ),
                 )
 
         # pylint: disable=protected-access
-        update_params(target._parameters)
+        update_params(target._parameters)  # type: ignore[arg-type]
         if with_buffers:
             update_buffers(target._buffers)
         memo.add(target)
         for submodule in target.modules():
             if submodule in memo:
                 continue
-            update_params(submodule._parameters)
+            update_params(submodule._parameters)  # type: ignore[arg-type]
             if with_buffers:
                 update_buffers(submodule._buffers)
             memo.add(submodule)
 
         return ModuleState(
             params=tuple(params),
             buffers=tuple(buffers),
             visual_contents=visual_contents,
             detach_buffers=detach_buffers,
         )
 
-    elif isinstance(target, MetaOptimizer):
+    if isinstance(target, MetaOptimizer):
         state = target.state_dict()
 
-        def get_variable(t):
+        def get_variable(t: torch.Tensor | None) -> torch.Tensor | None:
             if isinstance(t, torch.Tensor):
                 return replicate(t)
             return t
 
         state = pytree.tree_map(get_variable, state)  # type: ignore[arg-type,assignment]
         return state
 
     raise RuntimeError(f'Unexpected class of {target}')
 
 
 def extract_module_containers(
-    module: nn.Module, with_buffers: bool = True
+    module: nn.Module,
+    with_buffers: bool = True,
 ) -> tuple[ModuleTensorContainers, ModuleTensorContainers]:
     """Extract the references to the containers of parameters and buffers from a module."""
     if isinstance(module, nn.Module):
         params: list[TensorContainer] = []
         buffers: list[TensorContainer] = []
         memo: set[nn.Module] = set()
 
-        def update_container(container, items):
+        def update_container(container: list[TensorContainer], items: TensorContainer) -> None:
             if len(items) > 0:
                 container.append(items)  # we need references to original dictionaries
 
         # pylint: disable=protected-access
-        update_container(params, module._parameters)
+        update_container(params, module._parameters)  # type: ignore[arg-type]
         if with_buffers:
             update_container(buffers, module._buffers)
         memo.add(module)
         for submodule in module.modules():
             if submodule in memo:
                 continue
-            update_container(params, submodule._parameters)
+            update_container(params, submodule._parameters)  # type: ignore[arg-type]
             if with_buffers:
                 update_container(buffers, submodule._buffers)
             memo.add(submodule)
         return tuple(params), tuple(buffers)
 
     raise RuntimeError(f'Unexpected class of {module}')
 
@@ -449,15 +448,16 @@
 
         def clone(t: torch.Tensor) -> torch.Tensor:
             return t.clone().to(device=target_device)
 
         def clone_detach_(t: torch.Tensor) -> torch.Tensor:
             if isinstance(t, nn.Parameter):
                 return nn.Parameter(
-                    t.clone().to(device=target_device).detach_(), requires_grad=t.requires_grad
+                    t.clone().to(device=target_device).detach_(),
+                    requires_grad=t.requires_grad,
                 )
             return t.clone().to(device=target_device).detach_().requires_grad_(t.requires_grad)
 
     else:
 
         def reference(t: torch.Tensor) -> torch.Tensor:
             return t
```

### Comparing `torchopt-0.7.0/torchopt/version.py` & `torchopt-0.7.1/torchopt/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """TorchOpt: a high-performance optimizer library built upon PyTorch."""
 
-__version__ = '0.7.0'
+__version__ = '0.7.1'
 __license__ = 'Apache License, Version 2.0'
 __author__ = 'TorchOpt Contributors'
 __release__ = True
 
 if not __release__:
     import os
     import subprocess
 
     try:
         prefix, sep, suffix = (
             subprocess.check_output(
-                ['git', 'describe', '--abbrev=7'],
+                ['git', 'describe', '--abbrev=7'],  # noqa: S603,S607
                 cwd=os.path.dirname(os.path.abspath(__file__)),
                 stderr=subprocess.DEVNULL,
                 text=True,
             )
             .strip()
             .lstrip('v')
             .replace('-', '.dev', 1)
```

### Comparing `torchopt-0.7.0/torchopt/visual.py` & `torchopt-0.7.1/torchopt/visual.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,33 +16,34 @@
 # https://github.com/szagoruyko/pytorchviz/blob/master/torchviz/dot.py
 # ==============================================================================
 """Computation graph visualization."""
 
 from __future__ import annotations
 
 from collections import namedtuple
-from typing import Generator, Iterable, Mapping, cast
+from typing import Any, Generator, Iterable, Mapping, cast
 
 import torch
 from graphviz import Digraph
 
-from torchopt.typing import TensorOrTensors
+from torchopt import pytree
+from torchopt.typing import TensorTree
 from torchopt.utils import ModuleState
 
 
 __all__ = ['make_dot', 'resize_graph']
 
 
 Node = namedtuple('Node', ('name', 'inputs', 'attr', 'op'))
 
 # Saved attrs for grad_fn (incl. saved variables) begin with `._saved_*`
 SAVED_PREFIX = '_saved_'
 
 
-def get_fn_name(fn, show_attrs, max_attr_chars):
+def get_fn_name(fn: Any, show_attrs: bool, max_attr_chars: int) -> str:
     """Return function name."""
     name = str(type(fn).__name__)
     if not show_attrs:
         return name
     attrs = {}
     for attr in dir(fn):
         if not attr.startswith(SAVED_PREFIX):
@@ -59,24 +60,24 @@
         return name
     max_attr_chars = max(max_attr_chars, 3)
     col1width = max(map(len, attrs))
     col2width = min(max(len(str(v)) for v in attrs.values()), max_attr_chars)
     sep = '-' * max(col1width + col2width + 2, len(name))
     attrstr = '%-' + str(col1width) + 's: %' + str(col2width) + 's'
 
-    def truncate(s):  # pylint: disable=invalid-name
+    def truncate(s: str) -> str:  # pylint: disable=invalid-name
         return s[: col2width - 3] + '...' if len(s) > col2width else s
 
     params = '\n'.join(attrstr % (k, truncate(str(v))) for (k, v) in attrs.items())
     return name + '\n' + sep + '\n' + params
 
 
 # pylint: disable-next=too-many-branches,too-many-statements,too-many-locals
 def make_dot(
-    var: TensorOrTensors,
+    var: TensorTree,
     params: (
         Mapping[str, torch.Tensor]
         | ModuleState
         | Generator
         | Iterable[Mapping[str, torch.Tensor] | ModuleState | Generator]
         | None
     ) = None,
@@ -138,28 +139,28 @@
         'ranksep': '0.1',
         'height': '0.2',
         'fontname': 'monospace',
     }
     dot = Digraph(node_attr=node_attr, graph_attr={'size': '12,12'})
     seen = set()
 
-    def size_to_str(size):
+    def size_to_str(size: tuple[int, ...]) -> str:
         return '(' + (', ').join(map(str, size)) + ')'
 
-    def get_var_name(var, name=None):
+    def get_var_name(var: torch.Tensor, name: str | None = None) -> str:
         if not name:
             name = param_map[var] if var in param_map else ''
         return f'{name}\n{size_to_str(var.size())}'
 
-    def get_var_name_with_flag(var):
+    def get_var_name_with_flag(var: torch.Tensor) -> str | None:
         if var in param_map:
             return f'{param_map[var][0]}\n{size_to_str(param_map[var][1].size())}'
         return None
 
-    def add_nodes(fn):  # pylint: disable=too-many-branches
+    def add_nodes(fn: Any) -> None:  # pylint: disable=too-many-branches
         assert not isinstance(fn, torch.Tensor)
         if fn in seen:
             return
         seen.add(fn)
 
         if show_saved:
             for attr in dir(fn):
@@ -206,33 +207,32 @@
         # working* as it was moved to ATen and Variable-Tensor merged
         # also note that this still works for custom autograd functions
         if hasattr(fn, 'saved_tensors'):
             for t in fn.saved_tensors:
                 dot.edge(str(id(t)), str(id(fn)))
                 dot.node(str(id(t)), get_var_name(t), fillcolor='orange')
 
-    def add_base_tensor(v, color='darkolivegreen1'):  # pylint: disable=invalid-name
+    def add_base_tensor(
+        v: torch.Tensor,  # pylint: disable=invalid-name
+        color: str = 'darkolivegreen1',
+    ) -> None:
         if v in seen:
             return
         seen.add(v)
         dot.node(str(id(v)), get_var_name(v), fillcolor=color)
         if v.grad_fn:
             add_nodes(v.grad_fn)
             dot.edge(str(id(v.grad_fn)), str(id(v)))
         # pylint: disable=protected-access
         if v._is_view():
-            add_base_tensor(v._base, color='darkolivegreen3')
+            add_base_tensor(v._base, color='darkolivegreen3')  # type: ignore[arg-type]
             dot.edge(str(id(v._base)), str(id(v)), style='dotted')
 
     # handle multiple outputs
-    if isinstance(var, (tuple, list)):
-        for v in var:  # pylint: disable=invalid-name
-            add_base_tensor(v)
-    else:
-        add_base_tensor(var)
+    pytree.tree_map_(add_base_tensor, var)
 
     resize_graph(dot)
 
     return dot
 
 
 def resize_graph(dot: Digraph, size_per_element: float = 0.5, min_size: float = 12.0) -> None:
```

### Comparing `torchopt-0.7.0/torchopt.egg-info/PKG-INFO` & `torchopt-0.7.1/torchopt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: torchopt
-Version: 0.7.0
+Version: 0.7.1
 Summary: An efficient library for differentiable optimization for PyTorch.
 Author: TorchOpt Contributors
 Author-email: Jie Ren <jieren9806@gmail.com>, Xidong Feng <xidong.feng.20@ucl.ac.uk>, Bo Liu <benjaminliu.eecs@gmail.com>, Xuehai Pan <XuehaiPan@pku.edu.cn>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/metaopt/torchopt
 Project-URL: Repository, https://github.com/metaopt/torchopt
 Project-URL: Documentation, https://torchopt.readthedocs.io
 Project-URL: Bug Report, https://github.com/metaopt/torchopt/issues
 Keywords: PyTorch,functorch,JAX,Meta-Learning,Optimizer,Differentiable Optimizer,Functional Programming
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Environment :: GPU
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: lint
 Provides-Extra: test
 License-File: LICENSE
 
 <!-- markdownlint-disable first-line-h1 -->
 <!-- markdownlint-disable html -->
@@ -40,18 +39,18 @@
 
 <div align="center">
   <img src="https://github.com/metaopt/torchopt/raw/HEAD/image/logo-large.png" width="75%" />
 </div>
 
 <div align="center">
 
-  <a>![Python 3.7+](https://img.shields.io/badge/Python-3.7%2B-brightgreen.svg)</a>
+  <a>![Python 3.8+](https://img.shields.io/badge/Python-3.8%2B-brightgreen.svg)</a>
   <a href="https://pypi.org/project/torchopt">![PyPI](https://img.shields.io/pypi/v/torchopt?logo=pypi)</a>
   <a href="https://github.com/metaopt/torchopt/tree/HEAD/tests">![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/metaopt/torchopt/tests.yml?label=tests&logo=github)</a>
-  <a href="https://codecov.io/gh/metaopt/torchopt">![CodeCov](https://img.shields.io/codecov/c/gh/metaopt/torchopt)</a>
+  <a href="https://codecov.io/gh/metaopt/torchopt">![CodeCov](https://img.shields.io/codecov/c/github/metaopt/torchopt/main?logo=codecov)</a>
   <a href="https://torchopt.readthedocs.io">![Documentation Status](https://img.shields.io/readthedocs/torchopt?logo=readthedocs)</a>
   <a href="https://pepy.tech/project/torchopt">![Downloads](https://static.pepy.tech/personalized-badge/torchopt?period=total&left_color=grey&right_color=blue&left_text=downloads)</a>
   <a href="https://github.com/metaopt/torchopt/blob/HEAD/LICENSE">![License](https://img.shields.io/github/license/metaopt/torchopt?label=license&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0IiBmaWxsPSIjZmZmZmZmIj48cGF0aCBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik0xMi43NSAyLjc1YS43NS43NSAwIDAwLTEuNSAwVjQuNUg5LjI3NmExLjc1IDEuNzUgMCAwMC0uOTg1LjMwM0w2LjU5NiA1Ljk1N0EuMjUuMjUgMCAwMTYuNDU1IDZIMi4zNTNhLjc1Ljc1IDAgMTAwIDEuNUgzLjkzTC41NjMgMTUuMThhLjc2Mi43NjIgMCAwMC4yMS44OGMuMDguMDY0LjE2MS4xMjUuMzA5LjIyMS4xODYuMTIxLjQ1Mi4yNzguNzkyLjQzMy42OC4zMTEgMS42NjIuNjIgMi44NzYuNjJhNi45MTkgNi45MTkgMCAwMDIuODc2LS42MmMuMzQtLjE1NS42MDYtLjMxMi43OTItLjQzMy4xNS0uMDk3LjIzLS4xNTguMzEtLjIyM2EuNzUuNzUgMCAwMC4yMDktLjg3OEw1LjU2OSA3LjVoLjg4NmMuMzUxIDAgLjY5NC0uMTA2Ljk4NC0uMzAzbDEuNjk2LTEuMTU0QS4yNS4yNSAwIDAxOS4yNzUgNmgxLjk3NXYxNC41SDYuNzYzYS43NS43NSAwIDAwMCAxLjVoMTAuNDc0YS43NS43NSAwIDAwMC0xLjVIMTIuNzVWNmgxLjk3NGMuMDUgMCAuMS4wMTUuMTQuMDQzbDEuNjk3IDEuMTU0Yy4yOS4xOTcuNjMzLjMwMy45ODQuMzAzaC44ODZsLTMuMzY4IDcuNjhhLjc1Ljc1IDAgMDAuMjMuODk2Yy4wMTIuMDA5IDAgMCAuMDAyIDBhMy4xNTQgMy4xNTQgMCAwMC4zMS4yMDZjLjE4NS4xMTIuNDUuMjU2Ljc5LjRhNy4zNDMgNy4zNDMgMCAwMDIuODU1LjU2OCA3LjM0MyA3LjM0MyAwIDAwMi44NTYtLjU2OWMuMzM4LS4xNDMuNjA0LS4yODcuNzktLjM5OWEzLjUgMy41IDAgMDAuMzEtLjIwNi43NS43NSAwIDAwLjIzLS44OTZMMjAuMDcgNy41aDEuNTc4YS43NS43NSAwIDAwMC0xLjVoLTQuMTAyYS4yNS4yNSAwIDAxLS4xNC0uMDQzbC0xLjY5Ny0xLjE1NGExLjc1IDEuNzUgMCAwMC0uOTg0LS4zMDNIMTIuNzVWMi43NXpNMi4xOTMgMTUuMTk4YTUuNDE4IDUuNDE4IDAgMDAyLjU1Ny42MzUgNS40MTggNS40MTggMCAwMDIuNTU3LS42MzVMNC43NSA5LjM2OGwtMi41NTcgNS44M3ptMTQuNTEtLjAyNGMuMDgyLjA0LjE3NC4wODMuMjc1LjEyNi41My4yMjMgMS4zMDUuNDUgMi4yNzIuNDVhNS44NDYgNS44NDYgMCAwMDIuNTQ3LS41NzZMMTkuMjUgOS4zNjdsLTIuNTQ3IDUuODA3eiI+PC9wYXRoPjwvc3ZnPgo=)</a>
 </div>
 
 <p align="center">
   <a href="https://github.com/metaopt/torchopt#installation">Installation</a> |
@@ -66,15 +65,15 @@
 TorchOpt is:
 
 - **Comprehensive**: TorchOpt provides three differentiation modes - explicit differentiation, implicit differentiation, and zero-order differentiation for handling different differentiable optimization situations.
 - **Flexible**: TorchOpt provides both functional and objective-oriented API for users' different preferences. Users can implement differentiable optimization in JAX-like or PyTorch-like style.
 - **Efficient**: TorchOpt provides (1) CPU/GPU acceleration differentiable optimizer (2) RPC-based distributed training framework (3) Fast Tree Operations, to largely increase the training efficiency for bi-level optimization problems.
 
 Beyond differentiable optimization, TorchOpt can also be regarded as a functional optimizer that enables [JAX-like](https://github.com/google/jax) composable functional optimizer for PyTorch.
-With TorchOpt, users can easily conduct neural network optimization in PyTorch with functional style optimizer, similar to [Optax](https://github.com/deepmind/optax) in JAX.
+With TorchOpt, users can easily conduct neural network optimization in PyTorch with a functional style optimizer, similar to [Optax](https://github.com/deepmind/optax) in JAX.
 
 --------------------------------------------------------------------------------
 
 The README is organized as follows:
 
 - [TorchOpt as Functional Optimizer](#torchopt-as-functional-optimizer)
   - [Optax-Like API](#optax-like-api)
@@ -164,19 +163,19 @@
 optimizer.zero_grad()             # zero gradients
 loss.backward()                   # backward
 optimizer.step()                  # step updates
 ```
 
 ### Differentiable
 
-On top of the same optimization function as `torch.optim`, an important benefit of functional optimizer is that one can implement differentiable optimization easily.
-This is particularly helpful when the algorithm requires to differentiate through optimization updates (such as meta-learning practices).
+On top of the same optimization function as `torch.optim`, an important benefit of the functional optimizer is that one can implement differentiable optimization easily.
+This is particularly helpful when the algorithm requires differentiation through optimization updates (such as meta-learning practices).
 We take as the inputs the gradients and optimizer states, and use non-in-place operators to compute and output the updates.
 The processes can be automatically implemented, with the only need from users being to pass the argument `inplace=False` to the functions.
-Check out section [Explicit Gradient (EG)](#explicit-gradient-eg) functional API for example.
+Check out the section [Explicit Gradient](#explicit-gradient-eg) (EG)](#explicit-gradient-eg) functional API for example.
 
 --------------------------------------------------------------------------------
 
 ## TorchOpt for Differentiable Optimization
 
 We design a bilevel-optimization updating scheme, which can be easily extended to realize various differentiable optimization processes.
 
@@ -187,23 +186,23 @@
 As shown above, the scheme contains an outer level that has parameters $\phi$ that can be learned end-to-end through the inner level parameters solution $\theta^{\prime}(\phi)$ by using the best-response derivatives $\partial \theta^{\prime}(\phi) / \partial \phi$.
 TorchOpt supports three differentiation modes.
 It can be seen that the key component of this algorithm is to calculate the best-response (BR) Jacobian.
 From the BR-based perspective, existing gradient methods can be categorized into three groups: explicit gradient over unrolled optimization, implicit differentiation, and zero-order gradient differentiation.
 
 ### Explicit Gradient (EG)
 
-The idea of explicit gradient is to treat the gradient step as a differentiable function and try to backpropagate through the unrolled optimization path.
+The idea of the explicit gradient is to treat the gradient step as a differentiable function and try to backpropagate through the unrolled optimization path.
 This differentiation mode is suitable for algorithms when the inner-level optimization solution is obtained by a few gradient steps, such as [MAML](https://arxiv.org/abs/1703.03400) and [MGRL](https://arxiv.org/abs/1805.09801).
 TorchOpt offers both functional and object-oriented API for EG to fit different user applications.
 
 #### Functional API  <!-- omit in toc -->
 
 The functional API is to conduct optimization in a functional programming style.
 Note that we pass the argument `inplace=False` to the functions to make the optimization differentiable.
-Refer to the tutorial notebook [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb) for more guidances.
+Refer to the tutorial notebook [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb) for more guidance.
 
 ```python
 # Define functional optimizer
 optimizer = torchopt.adam()
 # Define meta and inner parameters
 meta_params = ...
 fmodel, params = make_functional(model)
@@ -219,16 +218,16 @@
 
 loss = outer_loss(fmodel, params, meta_params)
 meta_grads = torch.autograd.grad(loss, meta_params)
 ```
 
 #### OOP API  <!-- omit in toc -->
 
-TorchOpt also provides OOP API compatible with PyTorch programming style.
-Refer to the example and the tutorial notebook [Meta-Optimizer](tutorials/3_Meta_Optimizer.ipynb), [Stop Gradient](tutorials/4_Stop_Gradient.ipynb) for more guidances.
+TorchOpt also provides OOP API compatible with the PyTorch programming style.
+Refer to the example and the tutorial notebook [Meta-Optimizer](tutorials/3_Meta_Optimizer.ipynb), [Stop Gradient](tutorials/4_Stop_Gradient.ipynb) for more guidance.
 
 ```python
 # Define meta and inner parameters
 meta_params = ...
 model = ...
 # Define differentiable optimizer
 optimizer = torchopt.MetaAdam(model)  # a model instance as the argument instead of model.parameters()
@@ -247,15 +246,15 @@
 By treating the solution $\theta^{\prime}$ as an implicit function of $\phi$, the idea of IG is to directly get analytical best-response derivatives $\partial \theta^{\prime} (\phi) / \partial \phi$ by [implicit function theorem](https://en.wikipedia.org/wiki/Implicit_function_theorem).
 This is suitable for algorithms when the inner-level optimal solution is achieved ${\left. \frac{\partial F (\theta, \phi)}{\partial \theta} \right\rvert}_{\theta=\theta^{\prime}} = 0$ or reaches some stationary conditions $F (\theta^{\prime}, \phi) = 0$, such as [iMAML](https://arxiv.org/abs/1909.04630) and [DEQ](https://arxiv.org/abs/1909.01377).
 TorchOpt offers both functional and OOP APIs for supporting both [conjugate gradient-based](https://arxiv.org/abs/1909.04630) and [Neumann series-based](https://arxiv.org/abs/1911.02590) IG methods.
 Refer to the example [iMAML](https://github.com/waterhorse1/torchopt/tree/readme/examples/iMAML) and the notebook [Implicit Gradient](tutorials/5_Implicit_Differentiation.ipynb) for more guidance.
 
 #### Functional API  <!-- omit in toc -->
 
-For implicit gradient, users need to define the stationary condition and TorchOpt provides the decorator to wrap the solve function for enabling implicit gradient computation.
+For the implicit gradient, users need to define the stationary condition and TorchOpt provides the decorator to wrap the solve function for enabling implicit gradient computation.
 
 ```python
 # The stationary condition for the inner-loop
 def stationary(params, meta_params, data):
     # Stationary condition construction
     return stationary condition
 
@@ -272,15 +271,15 @@
 loss = outer_loss(optimal_params)
 
 meta_grads = torch.autograd.grad(loss, meta_params)
 ```
 
 #### OOP API  <!-- omit in toc -->
 
-TorchOpt also offer an OOP API, users need to inherit from the class `torchopt.nn.ImplicitMetaGradientModule` to construct the inner-loop network.
+TorchOpt also offers an OOP API, which users need to inherit from the class `torchopt.nn.ImplicitMetaGradientModule` to construct the inner-loop network.
 Users need to define the stationary condition/objective function and the inner-loop solve function to enable implicit gradient computation.
 
 ```python
 # Inherited from the class ImplicitMetaGradientModule
 # Optionally specify the linear solver (conjugate gradient or Neumann series)
 class InnerNet(ImplicitMetaGradientModule, linear_solve=linear_solver):
     def __init__(self, meta_param):
@@ -320,15 +319,15 @@
 
 ### Zero-order Differentiation (ZD)
 
 When the inner-loop process is non-differentiable or one wants to eliminate the heavy computation burdens in the previous two modes (brought by Hessian), one can choose Zero-order Differentiation (ZD).
 ZD typically gets gradients based on zero-order estimation, such as finite-difference, or [Evolutionary Strategy](https://arxiv.org/abs/1703.03864).
 Instead of optimizing the objective $F$, ES optimizes a smoothed objective.
 TorchOpt provides both functional and OOP APIs for the ES method.
-Refer to the tutorial notebook [Zero-order Differentiation](tutorials/6_Zero_Order_Differentiation.ipynb) for more guidances.
+Refer to the tutorial notebook [Zero-order Differentiation](tutorials/6_Zero_Order_Differentiation.ipynb) for more guidance.
 
 #### Functional API  <!-- omit in toc -->
 
 For zero-order differentiation, users need to define the forward pass calculation and the noise sampling procedure. TorchOpt provides the decorator to wrap the forward function for enabling zero-order differentiation.
 
 ```python
 # Customize the noise sampling function in ES
@@ -347,15 +346,15 @@
     # Forward process
     ...
     return objective  # the returned tensor should be a scalar tensor
 ```
 
 #### OOP API  <!-- omit in toc -->
 
-TorchOpt also offer an OOP API, users need to inherit from the class `torchopt.nn.ZeroOrderGradientModule` to construct the network as an `nn.Module` following a classical PyTorch style.
+TorchOpt also offers an OOP API, which users need to inherit from the class `torchopt.nn.ZeroOrderGradientModule` to construct the network as an `nn.Module` following a classical PyTorch style.
 Users need to define the forward process zero-order gradient procedures `forward()` and a noise sampling function `sample()`.
 
 ```python
 # Inherited from the class ZeroOrderGradientModule
 # Optionally specify the `method` and/or `num_samples` and/or `sigma` used for sampling
 class Net(ZeroOrderGradientModule, method=method, num_samples=num_samples, sigma=sigma):
     def __init__(self, ...):
@@ -388,65 +387,65 @@
 
 ### CPU/GPU accelerated differentiable optimizer
 
 We take the optimizer as a whole instead of separating it into several basic operators (e.g., `sqrt` and `div`).
 Therefore, by manually writing the forward and backward functions, we can perform the symbolic reduction.
 In addition, we can store some intermediate data that can be reused during the backpropagation.
 We write the accelerated functions in C++ OpenMP and CUDA, bind them by [`pybind11`](https://github.com/pybind/pybind11) to allow they can be called by Python, and then define the forward and backward behavior using `torch.autograd.Function`.
-Users can use by simply setting the `use_accelerated_op` flag as `True`.
-Refer to the corresponding sections in tutorials [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb) and [Meta-Optimizer](tutorials/3_Meta_Optimizer.ipynb)
+Users can use it by simply setting the `use_accelerated_op` flag as `True`.
+Refer to the corresponding sections in the tutorials [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb)](tutorials/1_Functional_Optimizer.ipynb) and [Meta-Optimizer](tutorials/3_Meta_Optimizer.ipynb)
 
 ```python
 optimizer = torchopt.MetaAdam(model, lr, use_accelerated_op=True)
 ```
 
 ### Distributed Training
 
 `TorchOpt` provides distributed training features based on the PyTorch RPC module for better training speed and multi-node multi-GPU support.
-Different from the MPI-like parallelization paradigm, which uses multiple homogenous workers and requires carefully designed communication hooks, the RPC APIs allow users to build their optimization pipeline more flexibly.
+Different from the MPI-like parallelization paradigm, which uses multiple homogeneous workers and requires carefully designed communication hooks, the RPC APIs allow users to build their optimization pipeline more flexibly.
 Experimental results show that we achieve an approximately linear relationship between the speed-up ratio and the number of workers.
 Check out the [Distributed Training Documentation](https://torchopt.readthedocs.io/en/latest/distributed/distributed.html) and [distributed MAML example](https://github.com/metaopt/torchopt/tree/main/examples/distributed/few-shot) for more specific guidance.
 
 ### OpTree
 
 We implement the *PyTree* to enable fast nested structure flattening using C++.
 The tree operations (e.g., flatten and unflatten) are very important in enabling functional and Just-In-Time (JIT) features of deep learning frameworks.
 By implementing it in C++, we can use some cache/memory-friendly structures (e.g., `absl::InlinedVector`) to improve the performance.
 For more guidance and comparison results, please refer to our open-source project [`OpTree`](https://github.com/metaopt/optree).
 
 --------------------------------------------------------------------------------
 
 ## Visualization
 
-Complex gradient flow in meta-learning brings in a great challenge for managing the gradient flow and verifying the correctness of it.
+Complex gradient flow in meta-learning brings in a great challenge for managing the gradient flow and verifying its correctness of it.
 TorchOpt provides a visualization tool that draws variable (e.g., network parameters or meta-parameters) names on the gradient graph for better analysis.
 The visualization tool is modified from [`torchviz`](https://github.com/szagoruyko/pytorchviz).
 Refer to the example [visualization code](examples/visualize.py) and the tutorial notebook [Visualization](tutorials/2_Visualization.ipynb) for more details.
 
-The figure below show the visualization result.
+The figure below shows the visualization result.
 Compared with [`torchviz`](https://github.com/szagoruyko/pytorchviz), TorchOpt fuses the operations within the `Adam` together (orange) to reduce the complexity and provide simpler visualization.
 
 <div align="center">
   <img src="https://github.com/metaopt/torchopt/raw/HEAD/image/torchviz-vs-torchopt.jpg" width="80%" />
 </div>
 
 --------------------------------------------------------------------------------
 
 ## Examples
 
-In the [`examples`](examples) directory, we offer several examples of functional optimizers and light-weight meta-learning examples with TorchOpt.
+In the [`examples`](examples) directory, we offer several examples of functional optimizers and lightweight meta-learning examples with TorchOpt.
 
 - [Model-Agnostic Meta-Learning (MAML) - Supervised Learning](https://arxiv.org/abs/1703.03400) (ICML 2017)
 - [Learning to Reweight Examples for Robust Deep Learning](https://arxiv.org/abs/1803.09050) (ICML 2018)
 - [Model-Agnostic Meta-Learning (MAML) - Reinforcement Learning](https://arxiv.org/abs/1703.03400) (ICML 2017)
 - [Meta-Gradient Reinforcement Learning (MGRL)](https://arxiv.org/abs/1805.09801) (NeurIPS 2018)
 - [Learning through opponent learning process (LOLA)](https://arxiv.org/abs/1709.04326) (AAMAS 2018)
 - [Meta-Learning with Implicit Gradients](https://arxiv.org/abs/1909.04630) (NeurIPS 2019)
 
-Also check [`examples`](examples) for more distributed/visualization/functorch-compatible examples.
+Also, check [`examples`](examples) for more distributed/visualization/functorch-compatible examples.
 
 --------------------------------------------------------------------------------
 
 ## Installation
 
 Requirements
```

#### html2text {}

```diff
@@ -1,40 +1,39 @@
-Metadata-Version: 2.1 Name: torchopt Version: 0.7.0 Summary: An efficient
+Metadata-Version: 2.1 Name: torchopt Version: 0.7.1 Summary: An efficient
 library for differentiable optimization for PyTorch. Author: TorchOpt
 Contributors Author-email: Jie Ren
 gmail.com>, Xidong Feng
 feng.20@ucl.ac.uk>, Bo Liu
 eecs@gmail.com>, Xuehai Pan
 pku.edu.cn> License: Apache License, Version 2.0 Project-URL: Homepage, https:/
 /github.com/metaopt/torchopt Project-URL: Repository, https://github.com/
 metaopt/torchopt Project-URL: Documentation, https://torchopt.readthedocs.io
 Project-URL: Bug Report, https://github.com/metaopt/torchopt/issues Keywords:
 PyTorch,functorch,JAX,Meta-Learning,Optimizer,Differentiable
 Optimizer,Functional Programming Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
-:: Linux Classifier: Operating System :: MacOS Classifier: Environment :: GPU
-Classifier: Environment :: GPU :: NVIDIA CUDA Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Education Classifier: Intended
-Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-lint Provides-Extra: test License-File: LICENSE
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: POSIX :: Linux Classifier: Operating System :: MacOS
+Classifier: Environment :: GPU Classifier: Environment :: GPU :: NVIDIA CUDA
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Education Classifier: Intended Audience :: Science/Research Classifier: Topic
+:: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Requires-Python: >=3.8 Description-Content-Type: text/
+markdown Provides-Extra: lint Provides-Extra: test License-File: LICENSE
       [https://github.com/metaopt/torchopt/raw/HEAD/image/logo-large.png]
- ![Python 3.7+](https://img.shields.io/badge/Python-3.7%2B-brightgreen.svg) !
+ ![Python 3.8+](https://img.shields.io/badge/Python-3.8%2B-brightgreen.svg) !
   [PyPI](https://img.shields.io/pypi/v/torchopt?logo=pypi) ![GitHub_Workflow
 Status](https://img.shields.io/github/actions/workflow/status/metaopt/torchopt/
 tests.yml?label=tests&logo=github) ![CodeCov](https://img.shields.io/codecov/c/
-     gh/metaopt/torchopt) ![Documentation_Status](https://img.shields.io/
- readthedocs/torchopt?logo=readthedocs) ![Downloads](https://static.pepy.tech/
-                              personalized-badge/
+  github/metaopt/torchopt/main?logo=codecov) ![Documentation_Status](https://
+  img.shields.io/readthedocs/torchopt?logo=readthedocs) ![Downloads](https://
+                     static.pepy.tech/personalized-badge/
  torchopt?period=total&left_color=grey&right_color=blue&left_text=downloads) !
            [License](https://img.shields.io/github/license/metaopt/
                     torchopt?label=license&logo=data:image/
 svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0IiBmaWxsPSIjZmZmZmZmIj48cGF0aCBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik0xMi43NSAyLjc1YS43NS43NSAwIDAwLTEuNSAwVjQuNUg5LjI3NmExLjc1IDEuNzUgMCAwMC0uOTg1LjMwM0w2LjU5NiA1Ljk1N0EuMjUuMjUgMCAwMTYuNDU1IDZIMi4zNTNhLjc1Ljc1IDAgMTAwIDEuNUgzLjkzTC41NjMgMTUuMThhLjc2Mi43NjIgMCAwMC4yMS44OGMuMDguMDY0LjE2MS4xMjUuMzA5LjIyMS4xODYuMTIxLjQ1Mi4yNzguNzkyLjQzMy42OC4zMTEgMS42NjIuNjIgMi44NzYuNjJhNi45MTkgNi45MTkgMCAwMDIuODc2LS42MmMuMzQtLjE1NS42MDYtLjMxMi43OTItLjQzMy4xNS0uMDk3LjIzLS4xNTguMzEtLjIyM2EuNzUuNzUgMCAwMC4yMDktLjg3OEw1LjU2OSA3LjVoLjg4NmMuMzUxIDAgLjY5NC0uMTA2Ljk4NC0uMzAzbDEuNjk2LTEuMTU0QS4yNS4yNSAwIDAxOS4yNzUgNmgxLjk3NXYxNC41SDYuNzYzYS43NS43NSAwIDAwMCAxLjVoMTAuNDc0YS43NS43NSAwIDAwMC0xLjVIMTIuNzVWNmgxLjk3NGMuMDUgMCAuMS4wMTUuMTQuMDQzbDEuNjk3IDEuMTU0Yy4yOS4xOTcuNjMzLjMwMy45ODQuMzAzaC44ODZsLTMuMzY4IDcuNjhhLjc1Ljc1IDAgMDAuMjMuODk2Yy4wMTIuMDA5IDAgMCAuMDAyIDBhMy4xNTQgMy4xNTQgMCAwMC4zMS4yMDZjLjE4NS4xMTIuNDUuMjU2Ljc5LjRhNy4zNDMgNy4zNDMgMCAwMDIuODU1LjU2OCA3LjM0MyA3LjM0MyAwIDAwMi44NTYtLjU2OWMuMzM4LS4xNDMuNjA0LS4yODcuNzktLjM5OWEzLjUgMy41IDAgMDAuMzEtLjIwNi43NS43NSAwIDAwLjIzLS44OTZMMjAuMDcgNy41aDEuNTc4YS43NS43NSAwIDAwMC0xLjVoLTQuMTAyYS4yNS4yNSAwIDAxLS4xNC0uMDQzbC0xLjY5Ny0xLjE1NGExLjc1IDEuNzUgMCAwMC0uOTg0LS4zMDNIMTIuNzVWMi43NXpNMi4xOTMgMTUuMTk4YTUuNDE4IDUuNDE4IDAgMDAyLjU1Ny42MzUgNS40MTggNS40MTggMCAwMDIuNTU3LS42MzVMNC43NSA5LjM2OGwtMi41NTcgNS44M3ptMTQuNTEtLjAyNGMuMDgyLjA0LjE3NC4wODMuMjc1LjEyNi41My4yMjMgMS4zMDUuNDUgMi4yNzIuNDVhNS44NDYgNS44NDYgMCAwMDIuNTQ3LS41NzZMMTkuMjUgOS4zNjdsLTIuNTQ3IDUuODA3eiI+PC9wYXRoPjwvc3ZnPgo=)
     Installation | Documentation | Tutorials | Examples | Paper | Citation
 **TorchOpt** is an efficient library for differentiable optimization built upon
 [PyTorch](https://pytorch.org). TorchOpt is: - **Comprehensive**: TorchOpt
@@ -45,141 +44,141 @@
 can implement differentiable optimization in JAX-like or PyTorch-like style. -
 **Efficient**: TorchOpt provides (1) CPU/GPU acceleration differentiable
 optimizer (2) RPC-based distributed training framework (3) Fast Tree
 Operations, to largely increase the training efficiency for bi-level
 optimization problems. Beyond differentiable optimization, TorchOpt can also be
 regarded as a functional optimizer that enables [JAX-like](https://github.com/
 google/jax) composable functional optimizer for PyTorch. With TorchOpt, users
-can easily conduct neural network optimization in PyTorch with functional style
-optimizer, similar to [Optax](https://github.com/deepmind/optax) in JAX. ------
--------------------------------------------------------------------------- The
-README is organized as follows: - [TorchOpt as Functional Optimizer](#torchopt-
-as-functional-optimizer) - [Optax-Like API](#optax-like-api) - [PyTorch-Like
-API](#pytorch-like-api) - [Differentiable](#differentiable) - [TorchOpt for
-Differentiable Optimization](#torchopt-for-differentiable-optimization) -
-[Explicit Gradient (EG)](#explicit-gradient-eg) - [Implicit Gradient (IG)]
-(#implicit-gradient-ig) - [Zero-order Differentiation (ZD)](#zero-order-
-differentiation-zd) - [High-Performance and Distributed Training](#high-
-performance-and-distributed-training) - [CPU/GPU accelerated differentiable
-optimizer](#cpugpu-accelerated-differentiable-optimizer) - [Distributed
-Training](#distributed-training) - [OpTree](#optree) - [Visualization]
-(#visualization) - [Examples](#examples) - [Installation](#installation) -
-[Changelog](#changelog) - [Citing TorchOpt](#citing-torchopt) - [The Team]
-(#the-team) - [License](#license) ---------------------------------------------
------------------------------------ ## TorchOpt as Functional Optimizer The
-design of TorchOpt follows the philosophy of functional programming. Aligned
-with [`functorch`](https://github.com/pytorch/functorch), users can conduct
-functional style programming with models, optimizers and training in PyTorch.
-We use the Adam optimizer as an example in the following illustration. You can
-also check out the tutorial notebook [Functional Optimizer](tutorials/
-1_Functional_Optimizer.ipynb) for more details. ### Optax-Like API For those
-users who prefer fully functional programming, we offer Optax-Like API by
-passing gradients and optimizer states to the optimizer function. Here is an
-example coupled with `functorch`: ```python class Net(nn.Module): ... class
-Loader(DataLoader): ... net = Net() # init loader = Loader() optimizer =
-torchopt.adam() model, params = functorch.make_functional(net) # use functorch
-extract network parameters opt_state = optimizer.init(params) # init optimizer
-xs, ys = next(loader) # get data pred = model(params, xs) # forward loss =
-F.cross_entropy(pred, ys) # compute loss grads = torch.autograd.grad(loss,
-params) # compute gradients updates, opt_state = optimizer.update(grads,
-opt_state) # get updates params = torchopt.apply_updates(params, updates) #
-update network parameters ``` We also provide a wrapper
-`torchopt.FuncOptimizer` to make maintaining the optimizer state easier:
-```python net = Net() # init loader = Loader() optimizer =
+can easily conduct neural network optimization in PyTorch with a functional
+style optimizer, similar to [Optax](https://github.com/deepmind/optax) in JAX.
+-------------------------------------------------------------------------------
+- The README is organized as follows: - [TorchOpt as Functional Optimizer]
+(#torchopt-as-functional-optimizer) - [Optax-Like API](#optax-like-api) -
+[PyTorch-Like API](#pytorch-like-api) - [Differentiable](#differentiable) -
+[TorchOpt for Differentiable Optimization](#torchopt-for-differentiable-
+optimization) - [Explicit Gradient (EG)](#explicit-gradient-eg) - [Implicit
+Gradient (IG)](#implicit-gradient-ig) - [Zero-order Differentiation (ZD)]
+(#zero-order-differentiation-zd) - [High-Performance and Distributed Training]
+(#high-performance-and-distributed-training) - [CPU/GPU accelerated
+differentiable optimizer](#cpugpu-accelerated-differentiable-optimizer) -
+[Distributed Training](#distributed-training) - [OpTree](#optree) -
+[Visualization](#visualization) - [Examples](#examples) - [Installation]
+(#installation) - [Changelog](#changelog) - [Citing TorchOpt](#citing-torchopt)
+- [The Team](#the-team) - [License](#license) ---------------------------------
+----------------------------------------------- ## TorchOpt as Functional
+Optimizer The design of TorchOpt follows the philosophy of functional
+programming. Aligned with [`functorch`](https://github.com/pytorch/functorch),
+users can conduct functional style programming with models, optimizers and
+training in PyTorch. We use the Adam optimizer as an example in the following
+illustration. You can also check out the tutorial notebook [Functional
+Optimizer](tutorials/1_Functional_Optimizer.ipynb) for more details. ### Optax-
+Like API For those users who prefer fully functional programming, we offer
+Optax-Like API by passing gradients and optimizer states to the optimizer
+function. Here is an example coupled with `functorch`: ```python class Net
+(nn.Module): ... class Loader(DataLoader): ... net = Net() # init loader =
+Loader() optimizer = torchopt.adam() model, params = functorch.make_functional
+(net) # use functorch extract network parameters opt_state = optimizer.init
+(params) # init optimizer xs, ys = next(loader) # get data pred = model(params,
+xs) # forward loss = F.cross_entropy(pred, ys) # compute loss grads =
+torch.autograd.grad(loss, params) # compute gradients updates, opt_state =
+optimizer.update(grads, opt_state) # get updates params =
+torchopt.apply_updates(params, updates) # update network parameters ``` We also
+provide a wrapper `torchopt.FuncOptimizer` to make maintaining the optimizer
+state easier: ```python net = Net() # init loader = Loader() optimizer =
 torchopt.FuncOptimizer(torchopt.adam()) # wrap with `torchopt.FuncOptimizer`
 model, params = functorch.make_functional(net) # use functorch extract network
 parameters for xs, ys in loader: # get data pred = model(params, xs) # forward
 loss = F.cross_entropy(pred, ys) # compute loss params = optimizer.step(loss,
 params) # update network parameters ``` ### PyTorch-Like API We also design a
 base class `torchopt.Optimizer` that has the same interface as
 `torch.optim.Optimizer`. We offer origin PyTorch APIs (e.g. `zero_grad()` or
 `step()`) by wrapping our Optax-Like API for traditional PyTorch users.
 ```python net = Net() # init loader = Loader() optimizer = torchopt.Adam
 (net.parameters()) xs, ys = next(loader) # get data pred = net(xs) # forward
 loss = F.cross_entropy(pred, ys) # compute loss optimizer.zero_grad() # zero
 gradients loss.backward() # backward optimizer.step() # step updates ``` ###
 Differentiable On top of the same optimization function as `torch.optim`, an
-important benefit of functional optimizer is that one can implement
+important benefit of the functional optimizer is that one can implement
 differentiable optimization easily. This is particularly helpful when the
-algorithm requires to differentiate through optimization updates (such as meta-
+algorithm requires differentiation through optimization updates (such as meta-
 learning practices). We take as the inputs the gradients and optimizer states,
 and use non-in-place operators to compute and output the updates. The processes
 can be automatically implemented, with the only need from users being to pass
-the argument `inplace=False` to the functions. Check out section [Explicit
-Gradient (EG)](#explicit-gradient-eg) functional API for example. -------------
-------------------------------------------------------------------- ## TorchOpt
-for Differentiable Optimization We design a bilevel-optimization updating
-scheme, which can be easily extended to realize various differentiable
-optimization processes.
+the argument `inplace=False` to the functions. Check out the section [Explicit
+Gradient](#explicit-gradient-eg) (EG)](#explicit-gradient-eg) functional API
+for example. ------------------------------------------------------------------
+-------------- ## TorchOpt for Differentiable Optimization We design a bilevel-
+optimization updating scheme, which can be easily extended to realize various
+differentiable optimization processes.
        [https://github.com/metaopt/torchopt/raw/HEAD/image/diffmode.png]
 As shown above, the scheme contains an outer level that has parameters $\phi$
 that can be learned end-to-end through the inner level parameters solution
 $\theta^{\prime}(\phi)$ by using the best-response derivatives $\partial
 \theta^{\prime}(\phi) / \partial \phi$. TorchOpt supports three differentiation
 modes. It can be seen that the key component of this algorithm is to calculate
 the best-response (BR) Jacobian. From the BR-based perspective, existing
 gradient methods can be categorized into three groups: explicit gradient over
 unrolled optimization, implicit differentiation, and zero-order gradient
-differentiation. ### Explicit Gradient (EG) The idea of explicit gradient is to
-treat the gradient step as a differentiable function and try to backpropagate
-through the unrolled optimization path. This differentiation mode is suitable
-for algorithms when the inner-level optimization solution is obtained by a few
-gradient steps, such as [MAML](https://arxiv.org/abs/1703.03400) and [MGRL]
-(https://arxiv.org/abs/1805.09801). TorchOpt offers both functional and object-
-oriented API for EG to fit different user applications. #### Functional API
-The functional API is to conduct optimization in a functional programming
-style. Note that we pass the argument `inplace=False` to the functions to make
-the optimization differentiable. Refer to the tutorial notebook [Functional
-Optimizer](tutorials/1_Functional_Optimizer.ipynb) for more guidances.
-```python # Define functional optimizer optimizer = torchopt.adam() # Define
-meta and inner parameters meta_params = ... fmodel, params = make_functional
-(model) # Initial state state = optimizer.init(params) for iter in range
-(iter_times): loss = inner_loss(fmodel, params, meta_params) grads =
-torch.autograd.grad(loss, params) # Apply non-inplace parameter update updates,
-state = optimizer.update(grads, state, inplace=False) params =
+differentiation. ### Explicit Gradient (EG) The idea of the explicit gradient
+is to treat the gradient step as a differentiable function and try to
+backpropagate through the unrolled optimization path. This differentiation mode
+is suitable for algorithms when the inner-level optimization solution is
+obtained by a few gradient steps, such as [MAML](https://arxiv.org/abs/
+1703.03400) and [MGRL](https://arxiv.org/abs/1805.09801). TorchOpt offers both
+functional and object-oriented API for EG to fit different user applications.
+#### Functional API  The functional API is to conduct optimization in a
+functional programming style. Note that we pass the argument `inplace=False` to
+the functions to make the optimization differentiable. Refer to the tutorial
+notebook [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb) for
+more guidance. ```python # Define functional optimizer optimizer =
+torchopt.adam() # Define meta and inner parameters meta_params = ... fmodel,
+params = make_functional(model) # Initial state state = optimizer.init(params)
+for iter in range(iter_times): loss = inner_loss(fmodel, params, meta_params)
+grads = torch.autograd.grad(loss, params) # Apply non-inplace parameter update
+updates, state = optimizer.update(grads, state, inplace=False) params =
 torchopt.apply_updates(params, updates) loss = outer_loss(fmodel, params,
 meta_params) meta_grads = torch.autograd.grad(loss, meta_params) ``` #### OOP
-API  TorchOpt also provides OOP API compatible with PyTorch programming style.
-Refer to the example and the tutorial notebook [Meta-Optimizer](tutorials/
-3_Meta_Optimizer.ipynb), [Stop Gradient](tutorials/4_Stop_Gradient.ipynb) for
-more guidances. ```python # Define meta and inner parameters meta_params = ...
-model = ... # Define differentiable optimizer optimizer = torchopt.MetaAdam
-(model) # a model instance as the argument instead of model.parameters() for
-iter in range(iter_times): # Perform inner update loss = inner_loss(model,
-meta_params) optimizer.step(loss) loss = outer_loss(model, meta_params)
-loss.backward() ``` ### Implicit Gradient (IG) By treating the solution
-$\theta^{\prime}$ as an implicit function of $\phi$, the idea of IG is to
-directly get analytical best-response derivatives $\partial \theta^{\prime}
-(\phi) / \partial \phi$ by [implicit function theorem](https://
+API  TorchOpt also provides OOP API compatible with the PyTorch programming
+style. Refer to the example and the tutorial notebook [Meta-Optimizer]
+(tutorials/3_Meta_Optimizer.ipynb), [Stop Gradient](tutorials/
+4_Stop_Gradient.ipynb) for more guidance. ```python # Define meta and inner
+parameters meta_params = ... model = ... # Define differentiable optimizer
+optimizer = torchopt.MetaAdam(model) # a model instance as the argument instead
+of model.parameters() for iter in range(iter_times): # Perform inner update
+loss = inner_loss(model, meta_params) optimizer.step(loss) loss = outer_loss
+(model, meta_params) loss.backward() ``` ### Implicit Gradient (IG) By treating
+the solution $\theta^{\prime}$ as an implicit function of $\phi$, the idea of
+IG is to directly get analytical best-response derivatives $\partial \theta^
+{\prime} (\phi) / \partial \phi$ by [implicit function theorem](https://
 en.wikipedia.org/wiki/Implicit_function_theorem). This is suitable for
 algorithms when the inner-level optimal solution is achieved ${\left. \frac
 {\partial F (\theta, \phi)}{\partial \theta} \right\rvert}_{\theta=\theta^
 {\prime}} = 0$ or reaches some stationary conditions $F (\theta^{\prime}, \phi)
 = 0$, such as [iMAML](https://arxiv.org/abs/1909.04630) and [DEQ](https://
 arxiv.org/abs/1909.01377). TorchOpt offers both functional and OOP APIs for
 supporting both [conjugate gradient-based](https://arxiv.org/abs/1909.04630)
 and [Neumann series-based](https://arxiv.org/abs/1911.02590) IG methods. Refer
 to the example [iMAML](https://github.com/waterhorse1/torchopt/tree/readme/
 examples/iMAML) and the notebook [Implicit Gradient](tutorials/
 5_Implicit_Differentiation.ipynb) for more guidance. #### Functional API  For
-implicit gradient, users need to define the stationary condition and TorchOpt
-provides the decorator to wrap the solve function for enabling implicit
-gradient computation. ```python # The stationary condition for the inner-loop
-def stationary(params, meta_params, data): # Stationary condition construction
-return stationary condition # Decorator for wrapping the function # Optionally
-specify the linear solver (conjugate gradient or Neumann series)
+the implicit gradient, users need to define the stationary condition and
+TorchOpt provides the decorator to wrap the solve function for enabling
+implicit gradient computation. ```python # The stationary condition for the
+inner-loop def stationary(params, meta_params, data): # Stationary condition
+construction return stationary condition # Decorator for wrapping the function
+# Optionally specify the linear solver (conjugate gradient or Neumann series)
 @torchopt.diff.implicit.custom_root(stationary, solve=linear_solver) def solve
 (params, meta_params, data): # Forward optimization process for params return
 output # Define params, meta_params and get data params, meta_prams, data =
 ..., ..., ... optimal_params = solve(params, meta_params, data) loss =
 outer_loss(optimal_params) meta_grads = torch.autograd.grad(loss, meta_params)
-``` #### OOP API  TorchOpt also offer an OOP API, users need to inherit from
-the class `torchopt.nn.ImplicitMetaGradientModule` to construct the inner-loop
-network. Users need to define the stationary condition/objective function and
-the inner-loop solve function to enable implicit gradient computation.
+``` #### OOP API  TorchOpt also offers an OOP API, which users need to inherit
+from the class `torchopt.nn.ImplicitMetaGradientModule` to construct the inner-
+loop network. Users need to define the stationary condition/objective function
+and the inner-loop solve function to enable implicit gradient computation.
 ```python # Inherited from the class ImplicitMetaGradientModule # Optionally
 specify the linear solver (conjugate gradient or Neumann series) class InnerNet
 (ImplicitMetaGradientModule, linear_solve=linear_solver): def __init__(self,
 meta_param): super().__init__() self.meta_param = meta_param ... def forward
 (self, batch): # Forward process ... def optimality(self, batch, labels): #
 Stationary condition construction for calculating implicit gradient # NOTE: If
 this method is not implemented, it will be automatically # derived from the
@@ -194,28 +193,28 @@
 process is non-differentiable or one wants to eliminate the heavy computation
 burdens in the previous two modes (brought by Hessian), one can choose Zero-
 order Differentiation (ZD). ZD typically gets gradients based on zero-order
 estimation, such as finite-difference, or [Evolutionary Strategy](https://
 arxiv.org/abs/1703.03864). Instead of optimizing the objective $F$, ES
 optimizes a smoothed objective. TorchOpt provides both functional and OOP APIs
 for the ES method. Refer to the tutorial notebook [Zero-order Differentiation]
-(tutorials/6_Zero_Order_Differentiation.ipynb) for more guidances. ####
+(tutorials/6_Zero_Order_Differentiation.ipynb) for more guidance. ####
 Functional API  For zero-order differentiation, users need to define the
 forward pass calculation and the noise sampling procedure. TorchOpt provides
 the decorator to wrap the forward function for enabling zero-order
 differentiation. ```python # Customize the noise sampling function in ES def
 distribution(sample_shape): # Generate a batch of noise samples # NOTE: The
 distribution should be spherical symmetric and with a constant variance of 1.
 ... return noise_batch # Distribution can also be an instance of
 `torch.distributions.Distribution`, e.g., `torch.distributions.Normal(...)`
 distribution = torch.distributions.Normal(loc=0, scale=1) # Specify method and
 hyper-parameter of ES @torchopt.diff.zero_order(distribution, method) def
 forward(params, batch, labels): # Forward process ... return objective # the
-returned tensor should be a scalar tensor ``` #### OOP API  TorchOpt also offer
-an OOP API, users need to inherit from the class
+returned tensor should be a scalar tensor ``` #### OOP API  TorchOpt also
+offers an OOP API, which users need to inherit from the class
 `torchopt.nn.ZeroOrderGradientModule` to construct the network as an
 `nn.Module` following a classical PyTorch style. Users need to define the
 forward process zero-order gradient procedures `forward()` and a noise sampling
 function `sample()`. ```python # Inherited from the class
 ZeroOrderGradientModule # Optionally specify the `method` and/or `num_samples`
 and/or `sigma` used for sampling class Net(ZeroOrderGradientModule,
 method=method, num_samples=num_samples, sigma=sigma): def __init__(self, ...):
@@ -231,60 +230,61 @@
 the optimizer as a whole instead of separating it into several basic operators
 (e.g., `sqrt` and `div`). Therefore, by manually writing the forward and
 backward functions, we can perform the symbolic reduction. In addition, we can
 store some intermediate data that can be reused during the backpropagation. We
 write the accelerated functions in C++ OpenMP and CUDA, bind them by
 [`pybind11`](https://github.com/pybind/pybind11) to allow they can be called by
 Python, and then define the forward and backward behavior using
-`torch.autograd.Function`. Users can use by simply setting the
-`use_accelerated_op` flag as `True`. Refer to the corresponding sections in
-tutorials [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb) and
-[Meta-Optimizer](tutorials/3_Meta_Optimizer.ipynb) ```python optimizer =
-torchopt.MetaAdam(model, lr, use_accelerated_op=True) ``` ### Distributed
-Training `TorchOpt` provides distributed training features based on the PyTorch
-RPC module for better training speed and multi-node multi-GPU support.
-Different from the MPI-like parallelization paradigm, which uses multiple
-homogenous workers and requires carefully designed communication hooks, the RPC
-APIs allow users to build their optimization pipeline more flexibly.
-Experimental results show that we achieve an approximately linear relationship
-between the speed-up ratio and the number of workers. Check out the
-[Distributed Training Documentation](https://torchopt.readthedocs.io/en/latest/
-distributed/distributed.html) and [distributed MAML example](https://
-github.com/metaopt/torchopt/tree/main/examples/distributed/few-shot) for more
-specific guidance. ### OpTree We implement the *PyTree* to enable fast nested
-structure flattening using C++. The tree operations (e.g., flatten and
-unflatten) are very important in enabling functional and Just-In-Time (JIT)
-features of deep learning frameworks. By implementing it in C++, we can use
-some cache/memory-friendly structures (e.g., `absl::InlinedVector`) to improve
-the performance. For more guidance and comparison results, please refer to our
-open-source project [`OpTree`](https://github.com/metaopt/optree). ------------
--------------------------------------------------------------------- ##
-Visualization Complex gradient flow in meta-learning brings in a great
-challenge for managing the gradient flow and verifying the correctness of it.
-TorchOpt provides a visualization tool that draws variable (e.g., network
-parameters or meta-parameters) names on the gradient graph for better analysis.
-The visualization tool is modified from [`torchviz`](https://github.com/
-szagoruyko/pytorchviz). Refer to the example [visualization code](examples/
-visualize.py) and the tutorial notebook [Visualization](tutorials/
-2_Visualization.ipynb) for more details. The figure below show the
-visualization result. Compared with [`torchviz`](https://github.com/szagoruyko/
-pytorchviz), TorchOpt fuses the operations within the `Adam` together (orange)
-to reduce the complexity and provide simpler visualization.
+`torch.autograd.Function`. Users can use it by simply setting the
+`use_accelerated_op` flag as `True`. Refer to the corresponding sections in the
+tutorials [Functional Optimizer](tutorials/1_Functional_Optimizer.ipynb)]
+(tutorials/1_Functional_Optimizer.ipynb) and [Meta-Optimizer](tutorials/
+3_Meta_Optimizer.ipynb) ```python optimizer = torchopt.MetaAdam(model, lr,
+use_accelerated_op=True) ``` ### Distributed Training `TorchOpt` provides
+distributed training features based on the PyTorch RPC module for better
+training speed and multi-node multi-GPU support. Different from the MPI-like
+parallelization paradigm, which uses multiple homogeneous workers and requires
+carefully designed communication hooks, the RPC APIs allow users to build their
+optimization pipeline more flexibly. Experimental results show that we achieve
+an approximately linear relationship between the speed-up ratio and the number
+of workers. Check out the [Distributed Training Documentation](https://
+torchopt.readthedocs.io/en/latest/distributed/distributed.html) and
+[distributed MAML example](https://github.com/metaopt/torchopt/tree/main/
+examples/distributed/few-shot) for more specific guidance. ### OpTree We
+implement the *PyTree* to enable fast nested structure flattening using C++.
+The tree operations (e.g., flatten and unflatten) are very important in
+enabling functional and Just-In-Time (JIT) features of deep learning
+frameworks. By implementing it in C++, we can use some cache/memory-friendly
+structures (e.g., `absl::InlinedVector`) to improve the performance. For more
+guidance and comparison results, please refer to our open-source project
+[`OpTree`](https://github.com/metaopt/optree). --------------------------------
+------------------------------------------------ ## Visualization Complex
+gradient flow in meta-learning brings in a great challenge for managing the
+gradient flow and verifying its correctness of it. TorchOpt provides a
+visualization tool that draws variable (e.g., network parameters or meta-
+parameters) names on the gradient graph for better analysis. The visualization
+tool is modified from [`torchviz`](https://github.com/szagoruyko/pytorchviz).
+Refer to the example [visualization code](examples/visualize.py) and the
+tutorial notebook [Visualization](tutorials/2_Visualization.ipynb) for more
+details. The figure below shows the visualization result. Compared with
+[`torchviz`](https://github.com/szagoruyko/pytorchviz), TorchOpt fuses the
+operations within the `Adam` together (orange) to reduce the complexity and
+provide simpler visualization.
  [https://github.com/metaopt/torchopt/raw/HEAD/image/torchviz-vs-torchopt.jpg]
 -------------------------------------------------------------------------------
 - ## Examples In the [`examples`](examples) directory, we offer several
-examples of functional optimizers and light-weight meta-learning examples with
+examples of functional optimizers and lightweight meta-learning examples with
 TorchOpt. - [Model-Agnostic Meta-Learning (MAML) - Supervised Learning](https:/
 /arxiv.org/abs/1703.03400) (ICML 2017) - [Learning to Reweight Examples for
 Robust Deep Learning](https://arxiv.org/abs/1803.09050) (ICML 2018) - [Model-
 Agnostic Meta-Learning (MAML) - Reinforcement Learning](https://arxiv.org/abs/
 1703.03400) (ICML 2017) - [Meta-Gradient Reinforcement Learning (MGRL)](https:/
 /arxiv.org/abs/1805.09801) (NeurIPS 2018) - [Learning through opponent learning
 process (LOLA)](https://arxiv.org/abs/1709.04326) (AAMAS 2018) - [Meta-Learning
-with Implicit Gradients](https://arxiv.org/abs/1909.04630) (NeurIPS 2019) Also
+with Implicit Gradients](https://arxiv.org/abs/1909.04630) (NeurIPS 2019) Also,
 check [`examples`](examples) for more distributed/visualization/functorch-
 compatible examples. ----------------------------------------------------------
 ---------------------- ## Installation Requirements - PyTorch - (Optional) For
 visualizing computation graphs - [Graphviz](https://graphviz.org/download) (for
 Linux users use `apt/yum install graphviz` or `conda install -c anaconda
 python-graphviz`) **Please follow the instructions at
 pytorch.org> to install PyTorch in your Python environment first.** Then run
```

### Comparing `torchopt-0.7.0/torchopt.egg-info/SOURCES.txt` & `torchopt-0.7.1/torchopt.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 torchopt.egg-info/top_level.txt
 torchopt/_C/adam_op.pyi
 torchopt/accelerated_op/__init__.py
 torchopt/accelerated_op/adam_op.py
 torchopt/accelerated_op/_src/__init__.py
 torchopt/accelerated_op/_src/adam_op.py
 torchopt/alias/__init__.py
+torchopt/alias/adagrad.py
 torchopt/alias/adam.py
 torchopt/alias/adamw.py
 torchopt/alias/rmsprop.py
 torchopt/alias/sgd.py
 torchopt/alias/utils.py
 torchopt/diff/__init__.py
 torchopt/diff/implicit/__init__.py
@@ -80,32 +81,36 @@
 torchopt/linear_solve/inv.py
 torchopt/linear_solve/normal_cg.py
 torchopt/linear_solve/utils.py
 torchopt/nn/__init__.py
 torchopt/nn/module.py
 torchopt/nn/stateless.py
 torchopt/optim/__init__.py
+torchopt/optim/adagrad.py
 torchopt/optim/adam.py
 torchopt/optim/adamw.py
 torchopt/optim/base.py
 torchopt/optim/rmsprop.py
 torchopt/optim/sgd.py
 torchopt/optim/func/__init__.py
 torchopt/optim/func/base.py
 torchopt/optim/meta/__init__.py
+torchopt/optim/meta/adagrad.py
 torchopt/optim/meta/adam.py
 torchopt/optim/meta/adamw.py
 torchopt/optim/meta/base.py
 torchopt/optim/meta/rmsprop.py
 torchopt/optim/meta/sgd.py
 torchopt/schedule/__init__.py
+torchopt/schedule/exponential_decay.py
 torchopt/schedule/polynomial.py
 torchopt/transform/__init__.py
 torchopt/transform/add_decayed_weights.py
 torchopt/transform/nan_to_num.py
 torchopt/transform/scale.py
 torchopt/transform/scale_by_adam.py
 torchopt/transform/scale_by_rms.py
+torchopt/transform/scale_by_rss.py
 torchopt/transform/scale_by_schedule.py
 torchopt/transform/scale_by_stddev.py
 torchopt/transform/trace.py
 torchopt/transform/utils.py
```

