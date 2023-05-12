# Comparing `tmp/pythie-serving-3.3.0.tar.gz` & `tmp/pythie-serving-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pythie-serving-3.3.0.tar", last modified: Fri Mar 10 12:59:24 2023, max compression
+gzip compressed data, was "dist/pythie-serving-3.4.0.tar", last modified: Fri May 12 11:47:57 2023, max compression
```

## Comparing `pythie-serving-3.3.0.tar` & `pythie-serving-3.4.0.tar`

### file list

```diff
@@ -1,681 +1,681 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/abstract_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/lightgbm_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/sklearn_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/table_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/jit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/jit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/jit/xla_activity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/jit/xla_activity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/jit/xla_compilation_cache_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/jit/xla_compilation_cache_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/lite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/lite/quantization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/lite/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/lite/quantization/quantization_info_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/lite/quantization/quantization_info_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/quantization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/quantization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/quantization/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/quantization/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/quantization/tensorflow/quantization_options_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/quantization/tensorflow/quantization_options_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tfrt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tfrt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tfrt/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tfrt/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tfrt/analysis/analysis_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tfrt/analysis/analysis_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tools/kernel_gen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tools/kernel_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tools/kernel_gen/compile_cache_item_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tools/kernel_gen/compile_cache_item_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2tensorrt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2tensorrt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2tensorrt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2tensorrt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2tensorrt/utils/trt_engine_instance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2tensorrt/utils/trt_engine_instance_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/host_compute_metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/host_compute_metadata_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/kernels/callback_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/kernels/callback_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/tf2xla_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/tf2xla_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/compile_options_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/compile_options_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/distributed/protocol_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15465 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/distributed/protocol_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/tpu_driver_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/tpu_driver_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/tpu_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/tpu_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/rpc/xla_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    33732 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/rpc/xla_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/backend_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/backend_config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/executable_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/executable_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/xla_framework_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/xla_framework_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/backend_configs_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/backend_configs_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/executable_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/executable_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/gpu_autotuning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/gpu_autotuning_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_execution_profile_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_execution_profile_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18137 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_profile_printer_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_profile_printer_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/test_compilation_environment_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/test_compilation_environment_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/stream_executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/stream_executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/stream_executor/dnn_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/stream_executor/dnn_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/tools/run_hlo_module_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/tools/run_hlo_module_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15439 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/xla_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/xla_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17049 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/xla_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/xla_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xrt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xrt/xrt_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xrt/xrt_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/dataset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/dataset_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/dispatcher_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    28122 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/dispatcher_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/export_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/export_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/journal_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/journal_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/worker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/worker_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/debug_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/debug_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/debugger_event_metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/debugger_event_metadata_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/example_parser_configuration_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/example_parser_configuration_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/example_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/example_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/feature_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/feature_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/allocation_description_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/allocation_description_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/api_def_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/api_def_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/attr_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/attr_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/cost_graph_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/cost_graph_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/dataset_metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/dataset_metadata_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/dataset_options_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/dataset_options_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/device_attributes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/device_attributes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/full_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/full_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/function_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/function_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/graph_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/graph_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/graph_transfer_info_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/graph_transfer_info_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/kernel_def_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/kernel_def_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/log_memory_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/log_memory_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/model_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/node_def_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/node_def_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/op_def_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/op_def_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/reader_base_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/reader_base_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/resource_handle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/resource_handle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/step_stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/step_stats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/summary_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/summary_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_description_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_description_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_shape_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_shape_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_slice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_slice_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/types_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/variable_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/variable_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/versions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/versions_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/default_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/default_types_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/serialization_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/serialization_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/serialization_test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/serialization_test_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/costs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/costs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/costs/op_performance_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/costs/op_performance_data_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/optimizers/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/optimizers/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/optimizers/inference/batch_op_rewriter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/optimizers/inference/batch_op_rewriter_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profile_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_analysis_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_analysis_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_options_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_options_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_service_monitor_result_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_service_monitor_result_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/diagnostics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/diagnostics_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/hardware_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/hardware_types_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/input_pipeline_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/input_pipeline_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/kernel_stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/kernel_stats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/memory_profile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/memory_profile_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/memory_viewer_preprocess_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/memory_viewer_preprocess_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_metrics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_metrics_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_profile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_profile_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_stats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/overview_page_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/overview_page_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/pod_stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/pod_stats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/pod_viewer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/pod_viewer_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/steps_db_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/steps_db_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_data_stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_data_stats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_function_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_function_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_stats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tfstreamz_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tfstreamz_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/trace_events_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/trace_events_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/xplane_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/xplane_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_options_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_options_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_output_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_output_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/autotuning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/autotuning_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/bfc_memory_map_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/bfc_memory_map_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/cluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/cluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/composite_tensor_variant_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/composite_tensor_variant_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/control_flow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/control_flow_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/conv_autotuning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/conv_autotuning_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/coordination_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/coordination_config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/coordination_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    34011 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/coordination_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/core_platform_payloads_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/core_platform_payloads_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/critical_section_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/critical_section_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/data_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/data_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/debug_event_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/debug_event_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/debug_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/debug_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/device_filters_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/device_filters_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/device_properties_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/device_properties_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/distributed_runtime_payloads_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/distributed_runtime_payloads_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/eager_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/eager_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/error_codes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/error_codes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/fingerprint_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/fingerprint_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/graph_debug_info_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/graph_debug_info_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/master_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/master_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/master_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    27112 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/master_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/meta_graph_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/meta_graph_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/named_tensor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/named_tensor_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/queue_runner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/queue_runner_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/remote_tensor_handle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/remote_tensor_handle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/replay_log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/replay_log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/rewriter_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/rewriter_config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saved_model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saved_model_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saved_object_graph_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saved_object_graph_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saver_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saver_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/service_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/service_config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/snapshot_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/snapshot_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/struct_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/struct_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tensor_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tensor_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tensorflow_server_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tensorflow_server_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/compilation_result_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/compilation_result_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/compile_metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/compile_metadata_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/dynamic_padding_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/dynamic_padding_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/optimization_parameters_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/optimization_parameters_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/topology_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/topology_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/tpu_embedding_configuration_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/tpu_embedding_configuration_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/trackable_object_graph_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/trackable_object_graph_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/transport_options_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/transport_options_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/verifier_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/verifier_config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/worker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/worker_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/worker_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29187 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/worker_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tfrt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tfrt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tfrt/fallback/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tfrt/fallback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tfrt/fallback/op_cost_map_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tfrt/fallback/op_cost_map_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compilation_cache_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compilation_cache_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compilation_cache_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compilation_cache_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compile_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_executable_info_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_executable_info_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/autotune_maps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/autotune_maps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/autotune_maps/autotune_map_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/autotune_maps/autotune_map_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/autotune_maps/conv_parameters_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/autotune_maps/conv_parameters_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/event_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/event_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/example_proto_fast_parsing_test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/example_proto_fast_parsing_test_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/memmapped_file_system_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/memmapped_file_system_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/quantization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/quantization/uniform_quant_ops_attr_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/quantization/uniform_quant_ops_attr_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/saved_tensor_slice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/saved_tensor_slice_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/test_log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/test_log_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/rpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/rpc/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/rpc/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/rpc/proto/tf_rpc_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/rpc/proto/tf_rpc_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/dtensor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/dtensor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/dtensor/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/dtensor/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/dtensor/proto/layout_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/dtensor/proto/layout_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/acceleration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/acceleration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/acceleration/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/acceleration/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/acceleration/configuration/configuration_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/acceleration/configuration/configuration_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/python/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/python/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/python/metrics/converter_error_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/python/metrics/converter_error_data_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/logging/toco_conversion_log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/logging/toco_conversion_log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/model_flags_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/model_flags_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/toco_flags_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/toco_flags_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/types_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/compatibility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/compatibility/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/compatibility/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/compatibility/protos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/compatibility/protos/compatibility_result_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/compatibility/protos/compatibility_result_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/evaluation_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/evaluation_config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/evaluation_stages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/evaluation_stages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/preprocessing_steps_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/preprocessing_steps_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/framework/cpp_shape_inference_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/framework/cpp_shape_inference_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/projector_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/projector_config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/saved_metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/saved_metadata_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/versions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/versions_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/kernel_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/kernel_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/kernel_tests/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/kernel_tests/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/kernel_tests/proto/test_example_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/kernel_tests/proto/test_example_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/tpu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/tpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/tpu/tensor_tracer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/tpu/tensor_tracer_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/training/checkpoint_state_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/training/checkpoint_state_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/util/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/util/protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/util/protobuf/compare_test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/util/protobuf/compare_test_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/security/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/security/fuzzing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/security/fuzzing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/security/fuzzing/checkpoint_reader_fuzz_input_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/security/fuzzing/checkpoint_reader_fuzz_input_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/proto_text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/proto_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/proto_text/test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/proto_text/test_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/protobuf/error_codes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/protobuf/error_codes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/protobuf/histogram_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/protobuf/histogram_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/classification_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/classification_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/get_model_metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/get_model_metadata_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/get_model_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/get_model_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/inference_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/inference_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/input_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/input_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/internal/serialized_input_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/internal/serialized_input_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/logging_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/logging_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_management_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_management_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/predict_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/predict_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/prediction_log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/prediction_log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/prediction_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/prediction_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/regression_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/regression_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/session_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/session_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/status_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/file_system_storage_path_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/file_system_storage_path_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/log_collector_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/log_collector_config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/logging_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/logging_config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/model_server_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/model_server_config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/monitoring_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/monitoring_config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/platform_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/platform_config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/ssl_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/ssl_config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/core/test_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/core/test_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/core/test_util/fake_loader_source_adapter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/core/test_util/fake_loader_source_adapter_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/model_servers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/model_servers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/model_servers/test_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/model_servers/test_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/model_servers/test_util/storage_path_error_injecting_source_adapter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/model_servers/test_util/storage_path_error_injecting_source_adapter_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/resources/resources_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/resources/resources_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/hashmap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/hashmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/hashmap/hashmap_source_adapter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/hashmap/hashmap_source_adapter_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/saved_model_bundle_source_adapter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/saved_model_bundle_source_adapter_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/session_bundle_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/session_bundle_config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/test_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/test_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/test_util/fake_thread_pool_factory_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/test_util/fake_thread_pool_factory_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/thread_pool_factory_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/thread_pool_factory_config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/session_bundle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/session_bundle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/session_bundle/oss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/session_bundle/oss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/session_bundle/oss/manifest_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/session_bundle/oss/manifest_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/sources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/sources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/sources/storage_path/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/sources/storage_path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/sources/storage_path/static_storage_path_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/sources/storage_path/static_storage_path_source_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/util/class_registration_test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/util/class_registration_test_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/treelite_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-10 12:59:12.000000 pythie-serving-3.3.0/src/pythie_serving/xgboost_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    48232 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 12:59:24.000000 pythie-serving-3.3.0/src/pythie_serving.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/abstract_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/lightgbm_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/sklearn_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/table_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/jit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/jit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/jit/xla_activity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/jit/xla_activity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/jit/xla_compilation_cache_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/jit/xla_compilation_cache_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/lite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/lite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/lite/quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/lite/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/lite/quantization/quantization_info_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/lite/quantization/quantization_info_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/quantization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/quantization/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/quantization/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/quantization/tensorflow/quantization_options_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/quantization/tensorflow/quantization_options_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tfrt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tfrt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tfrt/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tfrt/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tfrt/analysis/analysis_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tfrt/analysis/analysis_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tools/kernel_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tools/kernel_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tools/kernel_gen/compile_cache_item_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tools/kernel_gen/compile_cache_item_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2tensorrt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2tensorrt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2tensorrt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2tensorrt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2tensorrt/utils/trt_engine_instance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2tensorrt/utils/trt_engine_instance_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/host_compute_metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/host_compute_metadata_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/kernels/callback_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/kernels/callback_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/tf2xla_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/tf2xla_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/compile_options_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/compile_options_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/distributed/protocol_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15465 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/distributed/protocol_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/tpu_driver_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/tpu_driver_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/tpu_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/tpu_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/rpc/xla_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33732 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/rpc/xla_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/backend_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/backend_config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/executable_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/executable_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/xla_framework_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/xla_framework_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/backend_configs_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/backend_configs_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/executable_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/executable_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/gpu_autotuning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/gpu_autotuning_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_execution_profile_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_execution_profile_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18137 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_profile_printer_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_profile_printer_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/test_compilation_environment_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/test_compilation_environment_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/stream_executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/stream_executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/stream_executor/dnn_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/stream_executor/dnn_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/tools/run_hlo_module_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/tools/run_hlo_module_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15439 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/xla_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/xla_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17049 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/xla_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/xla_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xrt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xrt/xrt_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xrt/xrt_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/dataset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/dataset_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/dispatcher_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28122 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/dispatcher_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/export_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/export_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/journal_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/journal_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/worker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/worker_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/debug_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/debug_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/debugger_event_metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/debugger_event_metadata_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/example_parser_configuration_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/example_parser_configuration_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/example_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/example_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/feature_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/feature_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/allocation_description_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/allocation_description_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/api_def_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/api_def_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/attr_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/attr_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/cost_graph_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/cost_graph_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/dataset_metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/dataset_metadata_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/dataset_options_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/dataset_options_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/device_attributes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/device_attributes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/full_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/full_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/function_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/function_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/graph_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/graph_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/graph_transfer_info_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/graph_transfer_info_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/kernel_def_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/kernel_def_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/log_memory_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/log_memory_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/model_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/node_def_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/node_def_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/op_def_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/op_def_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/reader_base_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/reader_base_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/resource_handle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/resource_handle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/step_stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/step_stats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/summary_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/summary_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_description_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_description_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_shape_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_shape_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_slice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_slice_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/types_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/variable_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/variable_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/versions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/versions_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/default_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/default_types_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/serialization_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/serialization_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/serialization_test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/serialization_test_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/costs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/costs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/costs/op_performance_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/costs/op_performance_data_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/optimizers/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/optimizers/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/optimizers/inference/batch_op_rewriter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/optimizers/inference/batch_op_rewriter_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profile_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_analysis_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_analysis_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_options_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_options_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_service_monitor_result_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_service_monitor_result_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/diagnostics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/diagnostics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/hardware_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/hardware_types_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/input_pipeline_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/input_pipeline_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/kernel_stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/kernel_stats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/memory_profile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/memory_profile_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/memory_viewer_preprocess_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/memory_viewer_preprocess_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_metrics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_metrics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_profile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_profile_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_stats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/overview_page_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/overview_page_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/pod_stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/pod_stats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/pod_viewer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/pod_viewer_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/steps_db_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/steps_db_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_data_stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_data_stats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_function_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_function_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_stats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tfstreamz_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tfstreamz_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/trace_events_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/trace_events_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/xplane_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/xplane_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_options_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_options_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_output_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_output_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/autotuning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/autotuning_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/bfc_memory_map_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/bfc_memory_map_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/cluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/cluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/composite_tensor_variant_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/composite_tensor_variant_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/control_flow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/control_flow_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/conv_autotuning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/conv_autotuning_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/coordination_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/coordination_config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/coordination_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34011 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/coordination_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/core_platform_payloads_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/core_platform_payloads_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/critical_section_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/critical_section_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/data_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/data_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/debug_event_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/debug_event_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/debug_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/debug_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/device_filters_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/device_filters_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/device_properties_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/device_properties_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/distributed_runtime_payloads_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/distributed_runtime_payloads_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/eager_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/eager_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/error_codes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/error_codes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/fingerprint_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/fingerprint_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/graph_debug_info_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/graph_debug_info_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/master_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/master_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/master_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27112 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/master_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/meta_graph_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/meta_graph_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/named_tensor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/named_tensor_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/queue_runner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/queue_runner_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/remote_tensor_handle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/remote_tensor_handle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/replay_log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/replay_log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/rewriter_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/rewriter_config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saved_model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saved_model_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saved_object_graph_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saved_object_graph_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saver_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saver_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/service_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/service_config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/snapshot_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/snapshot_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/struct_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/struct_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tensor_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tensor_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tensorflow_server_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tensorflow_server_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/compilation_result_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/compilation_result_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/compile_metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/compile_metadata_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/dynamic_padding_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/dynamic_padding_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/optimization_parameters_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/optimization_parameters_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/topology_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/topology_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/tpu_embedding_configuration_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/tpu_embedding_configuration_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/trackable_object_graph_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/trackable_object_graph_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/transport_options_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/transport_options_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/verifier_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/verifier_config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/worker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/worker_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/worker_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29187 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/worker_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tfrt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tfrt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tfrt/fallback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tfrt/fallback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tfrt/fallback/op_cost_map_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tfrt/fallback/op_cost_map_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compilation_cache_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compilation_cache_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compilation_cache_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compilation_cache_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compile_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_executable_info_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_executable_info_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/autotune_maps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/autotune_maps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/autotune_maps/autotune_map_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/autotune_maps/autotune_map_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/autotune_maps/conv_parameters_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/autotune_maps/conv_parameters_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/event_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/event_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/example_proto_fast_parsing_test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/example_proto_fast_parsing_test_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/memmapped_file_system_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/memmapped_file_system_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/quantization/uniform_quant_ops_attr_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/quantization/uniform_quant_ops_attr_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/saved_tensor_slice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/saved_tensor_slice_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/test_log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/test_log_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/rpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/rpc/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/rpc/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/rpc/proto/tf_rpc_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/rpc/proto/tf_rpc_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/dtensor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/dtensor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/dtensor/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/dtensor/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/dtensor/proto/layout_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/dtensor/proto/layout_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/acceleration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/acceleration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/acceleration/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/acceleration/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/acceleration/configuration/configuration_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/acceleration/configuration/configuration_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/python/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/python/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/python/metrics/converter_error_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/python/metrics/converter_error_data_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/logging/toco_conversion_log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/logging/toco_conversion_log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/model_flags_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/model_flags_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/toco_flags_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/toco_flags_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/types_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/compatibility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/compatibility/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/compatibility/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/compatibility/protos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/compatibility/protos/compatibility_result_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/compatibility/protos/compatibility_result_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/evaluation_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/evaluation_config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/evaluation_stages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/evaluation_stages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/preprocessing_steps_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/preprocessing_steps_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/framework/cpp_shape_inference_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/framework/cpp_shape_inference_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/projector_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/projector_config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/saved_metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/saved_metadata_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/versions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/versions_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/kernel_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/kernel_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/kernel_tests/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/kernel_tests/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/kernel_tests/proto/test_example_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/kernel_tests/proto/test_example_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/tpu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/tpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/tpu/tensor_tracer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/tpu/tensor_tracer_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/training/checkpoint_state_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/training/checkpoint_state_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/util/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/util/protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/util/protobuf/compare_test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/util/protobuf/compare_test_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/security/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/security/fuzzing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/security/fuzzing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/security/fuzzing/checkpoint_reader_fuzz_input_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/security/fuzzing/checkpoint_reader_fuzz_input_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/proto_text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/proto_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/proto_text/test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/proto_text/test_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/protobuf/error_codes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/protobuf/error_codes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/protobuf/histogram_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/protobuf/histogram_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/classification_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/classification_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/get_model_metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/get_model_metadata_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/get_model_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/get_model_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/inference_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/inference_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/input_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/input_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/internal/serialized_input_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/internal/serialized_input_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/logging_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/logging_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_management_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_management_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/predict_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/predict_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/prediction_log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/prediction_log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/prediction_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/prediction_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/regression_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/regression_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/session_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/session_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/status_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/file_system_storage_path_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/file_system_storage_path_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/log_collector_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/log_collector_config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/logging_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/logging_config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/model_server_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/model_server_config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/monitoring_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/monitoring_config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/platform_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/platform_config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/ssl_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/ssl_config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/core/test_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/core/test_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/core/test_util/fake_loader_source_adapter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/core/test_util/fake_loader_source_adapter_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/model_servers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/model_servers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/model_servers/test_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/model_servers/test_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/model_servers/test_util/storage_path_error_injecting_source_adapter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/model_servers/test_util/storage_path_error_injecting_source_adapter_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/resources/resources_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/resources/resources_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/hashmap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/hashmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/hashmap/hashmap_source_adapter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/hashmap/hashmap_source_adapter_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/saved_model_bundle_source_adapter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/saved_model_bundle_source_adapter_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/session_bundle_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/session_bundle_config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/test_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/test_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/test_util/fake_thread_pool_factory_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/test_util/fake_thread_pool_factory_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/thread_pool_factory_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/thread_pool_factory_config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/session_bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/session_bundle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/session_bundle/oss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/session_bundle/oss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/session_bundle/oss/manifest_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/session_bundle/oss/manifest_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/sources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/sources/storage_path/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/sources/storage_path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/sources/storage_path/static_storage_path_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/sources/storage_path/static_storage_path_source_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/util/class_registration_test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/util/class_registration_test_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/treelite_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-12 11:47:47.000000 pythie-serving-3.4.0/src/pythie_serving/xgboost_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-12 11:47:56.000000 pythie-serving-3.4.0/src/pythie_serving.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    48232 2023-05-12 11:47:57.000000 pythie-serving-3.4.0/src/pythie_serving.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:47:56.000000 pythie-serving-3.4.0/src/pythie_serving.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 11:47:56.000000 pythie-serving-3.4.0/src/pythie_serving.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-12 11:47:56.000000 pythie-serving-3.4.0/src/pythie_serving.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-12 11:47:56.000000 pythie-serving-3.4.0/src/pythie_serving.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:47:56.000000 pythie-serving-3.4.0/src/pythie_serving.egg-info/zip-safe
```

### Comparing `pythie-serving-3.3.0/PKG-INFO` & `pythie-serving-3.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pythie-serving
-Version: 3.3.0
+Version: 3.4.0
 Summary: A GRPC server to serve model types using tensorflow-serving .proto services
 Home-page: https://gitlab.cayzn.com/wiremind/data-science/pythie-neos.git
 Author: wiremind data science team
 Author-email: data-science@wiremind.io
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Provides-Extra: serving
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: all
```

### Comparing `pythie-serving-3.3.0/README.md` & `pythie-serving-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/setup.py` & `pythie-serving-3.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     author="wiremind data science team",
     author_email="data-science@wiremind.io",
     url="https://gitlab.cayzn.com/wiremind/data-science/pythie-neos.git",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=True,
-    python_requires=">=3.10",
+    python_requires=">=3.11",
     install_requires=[
         "numpy~=1.23.0",
         "grpcio~=1.51",
         "protobuf~=4.22.0",
     ],
     # pip-compile setup.py --no-emit-index-url --upgrade --rebuild
     # pip-compile setup.py --no-emit-index-url --upgrade --extra serving -o pythie-serving-requirements.txt
@@ -56,12 +56,12 @@
     },
     entry_points={
         "console_scripts": [
             "pythie-serving=pythie_serving.run:run",
         ]
     },
     classifiers=[
-        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     ],
 )
```

### Comparing `pythie-serving-3.3.0/src/pythie_serving/abstract_wrapper.py` & `pythie-serving-3.4.0/src/pythie_serving/abstract_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc
 import logging
+import os
 import time
 from pathlib import Path
 from typing import Any, ClassVar, TypedDict
 
 import grpc
 import numpy as np
 from numpy.typing import NDArray
@@ -29,14 +30,15 @@
 
 
 class AbstractPythieServingPredictionServiceServicer(prediction_service_pb2_grpc.PredictionServiceServicer, abc.ABC):
     model_file_extension: ClassVar[str]
 
     def __init__(self, *, model_server_config: ModelServerConfig):
         self.logger = logging.getLogger("pythie_serving")
+        self.verbose = bool(os.environ.get("VERBOSE", True))
 
         self.model_map = {}
         for model_config in model_server_config.model_config_list.config:
             if not self._get_model_path(model_config).exists():
                 raise PythieServingException(f"Model file for {model_config.name} not found.")
             if not self._get_metadata_path(model_config).exists():
                 raise PythieServingException("Metadata file metadata.json not found ")
@@ -74,19 +76,20 @@
             predict_response = predict_pb2.PredictResponse(
                 model_spec=request.model_spec, outputs={"predictions": make_tensor_proto(pred)}
             )
         except Exception as e:
             self.logger.error(f"Failed to serve because: {e}")
             raise
         else:
-            duration = time.time() - start
-            self.logger.info(
-                f"Served model {request.model_spec.name}/{request.model_spec.signature_name}: "
-                f"{len(pred)} predictions in {duration:.2f} seconds ({len(pred) / duration:.2f} pred/sec) "
-            )
+            if self.verbose:
+                duration = time.time() - start
+                self.logger.info(
+                    f"Served model {request.model_spec.name}/{request.model_spec.signature_name}: "
+                    f"{len(pred)} predictions in {duration:.2f} seconds ({len(pred) / duration:.2f} pred/sec) "
+                )
             return predict_response
 
     @staticmethod
     def _parse_samples(request: predict_pb2.PredictRequest, model_specs: ModelSpecs) -> NDArray:
         nb_features = model_specs["nb_features"]
         request_inputs = request.inputs
 
@@ -98,15 +101,14 @@
                 f"Expected {features_names}, got {set(request_inputs)}."
             )
 
         nb_samples = request_inputs[features_names[0]].tensor_shape.dim[0].size
         samples = np.empty((nb_samples, nb_features), model_specs["samples_dtype"])
 
         for i, feature_name in enumerate(features_names):
-
             if request_inputs[feature_name].tensor_shape.dim[0].size != nb_samples:
                 raise PythieServingException(f"{feature_name} has invalid length.")
 
             nd_array = make_ndarray_from_tensor(request_inputs[feature_name])
 
             if len(nd_array.shape) != 2 or nd_array.shape[1] != 1:
                 raise PythieServingException("All input vectors should be 1D tensor")
```

### Comparing `pythie-serving-3.3.0/src/pythie_serving/lightgbm_wrapper.py` & `pythie-serving-3.4.0/src/pythie_serving/lightgbm_wrapper.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/run.py` & `pythie-serving-3.4.0/src/pythie_serving/run.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/server.py` & `pythie-serving-3.4.0/src/pythie_serving/server.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/sklearn_wrapper.py` & `pythie-serving-3.4.0/src/pythie_serving/sklearn_wrapper.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/table_wrapper.py` & `pythie-serving-3.4.0/src/pythie_serving/table_wrapper.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/jit/xla_activity_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/jit/xla_activity_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/jit/xla_compilation_cache_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/jit/xla_compilation_cache_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/lite/quantization/quantization_info_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/lite/quantization/quantization_info_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/quantization/tensorflow/quantization_options_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/quantization/tensorflow/quantization_options_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tfrt/analysis/analysis_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tfrt/analysis/analysis_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tools/kernel_gen/compile_cache_item_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/mlir/tools/kernel_gen/compile_cache_item_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2tensorrt/utils/trt_engine_instance_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2tensorrt/utils/trt_engine_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/host_compute_metadata_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/host_compute_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/kernels/callback_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/kernels/callback_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/tf2xla_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/tf2xla/tf2xla_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/compile_options_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/compile_options_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/distributed/protocol_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/distributed/protocol_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/distributed/protocol_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/pjrt/distributed/protocol_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/tpu_driver_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/tpu_driver_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/tpu_service_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/tpu_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/tpu_service_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/python/tpu_driver/tpu_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/rpc/xla_service_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/rpc/xla_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/rpc/xla_service_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/rpc/xla_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/backend_config_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/backend_config_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/executable_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/executable_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/xla_framework_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/cpu/xla_framework_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/backend_configs_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/backend_configs_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/executable_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/executable_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/gpu_autotuning_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/gpu/gpu_autotuning_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_execution_profile_data_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_execution_profile_data_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_profile_printer_data_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/hlo_profile_printer_data_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/test_compilation_environment_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/service/test_compilation_environment_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/stream_executor/dnn_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/stream_executor/dnn_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/tools/run_hlo_module_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/tools/run_hlo_module_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/xla_data_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/xla_data_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/xla_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xla/xla_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xrt/xrt_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/compiler/xrt/xrt_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/dataset_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/common_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/common_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/dispatcher_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/dispatcher_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/dispatcher_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/dispatcher_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/export_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/export_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/journal_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/journal_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/worker_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/worker_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/worker_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/data/service/worker_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/debug_service_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/debug_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/debug_service_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/debug_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/debugger_event_metadata_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/debug/debugger_event_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/example_parser_configuration_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/example_parser_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/example_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/example_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/feature_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/example/feature_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/allocation_description_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/allocation_description_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/api_def_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/api_def_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/attr_value_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/attr_value_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/cost_graph_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/cost_graph_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/dataset_metadata_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/dataset_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/dataset_options_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/dataset_options_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/device_attributes_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/device_attributes_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/full_type_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/full_type_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/function_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/function_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/graph_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/graph_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/graph_transfer_info_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/graph_transfer_info_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/kernel_def_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/kernel_def_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/log_memory_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/log_memory_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/model_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/model_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/node_def_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/node_def_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/op_def_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/op_def_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/reader_base_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/reader_base_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/resource_handle_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/resource_handle_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/step_stats_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/step_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/summary_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/summary_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_description_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_description_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_shape_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_shape_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_slice_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/tensor_slice_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/types_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/types_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/variable_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/variable_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/versions_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/framework/versions_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/default_types_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/default_types_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/serialization_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/serialization_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/serialization_test_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/function/trace_type/serialization_test_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/costs/op_performance_data_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/costs/op_performance_data_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/optimizers/inference/batch_op_rewriter_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/grappler/optimizers/inference/batch_op_rewriter_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profile_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profile_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_analysis_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_analysis_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_analysis_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_analysis_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_options_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_options_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_service_monitor_result_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_service_monitor_result_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_service_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_service_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/profiler_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/diagnostics_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/diagnostics_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/hardware_types_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/hardware_types_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/input_pipeline_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/input_pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/kernel_stats_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/kernel_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/memory_profile_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/memory_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/memory_viewer_preprocess_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/memory_viewer_preprocess_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_metrics_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_profile_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_stats_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/op_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/overview_page_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/overview_page_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/pod_stats_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/pod_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/pod_viewer_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/pod_viewer_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/steps_db_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/steps_db_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_data_stats_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_data_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_function_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_function_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_stats_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tf_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tfstreamz_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/tfstreamz_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/trace_events_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/trace_events_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/xplane_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/protobuf/xplane_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_log_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_log_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_options_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_options_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_output_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/profiler/tfprof_output_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/autotuning_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/autotuning_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/bfc_memory_map_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/bfc_memory_map_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/cluster_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/composite_tensor_variant_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/composite_tensor_variant_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/config_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/config_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/control_flow_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/control_flow_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/conv_autotuning_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/conv_autotuning_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/coordination_config_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/coordination_config_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/coordination_service_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/coordination_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/coordination_service_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/coordination_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/core_platform_payloads_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/core_platform_payloads_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/critical_section_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/critical_section_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/data_service_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/data_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/debug_event_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/debug_event_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/debug_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/debug_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/device_filters_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/device_filters_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/device_properties_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/device_properties_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/distributed_runtime_payloads_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/distributed_runtime_payloads_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/eager_service_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/eager_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/eager_service_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/eager_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/error_codes_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/error_codes_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/fingerprint_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/fingerprint_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/graph_debug_info_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/graph_debug_info_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/master_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/master_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/master_service_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/master_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/master_service_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/master_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/meta_graph_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/meta_graph_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/named_tensor_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/named_tensor_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/queue_runner_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/queue_runner_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/remote_tensor_handle_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/remote_tensor_handle_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/replay_log_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/replay_log_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/rewriter_config_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/rewriter_config_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saved_model_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saved_model_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saved_object_graph_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saved_object_graph_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saver_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/saver_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/service_config_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/service_config_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/snapshot_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/struct_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/struct_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tensor_bundle_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tensor_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tensorflow_server_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tensorflow_server_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/compilation_result_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/compilation_result_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/compile_metadata_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/compile_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/dynamic_padding_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/dynamic_padding_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/optimization_parameters_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/optimization_parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/topology_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/topology_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/tpu_embedding_configuration_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/tpu/tpu_embedding_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/trackable_object_graph_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/trackable_object_graph_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/transport_options_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/transport_options_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/verifier_config_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/verifier_config_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/worker_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/worker_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/worker_service_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/worker_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/worker_service_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/protobuf/worker_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tfrt/fallback/op_cost_map_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tfrt/fallback/op_cost_map_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compilation_cache_common_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compilation_cache_common_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compilation_cache_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compilation_cache_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compilation_cache_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compilation_cache_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compile_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_compile_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_executable_info_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/tpu/kernels/tpu_executable_info_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/autotune_maps/autotune_map_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/autotune_maps/autotune_map_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/autotune_maps/conv_parameters_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/autotune_maps/conv_parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/event_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/event_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/example_proto_fast_parsing_test_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/example_proto_fast_parsing_test_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/memmapped_file_system_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/memmapped_file_system_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/quantization/uniform_quant_ops_attr_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/quantization/uniform_quant_ops_attr_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/saved_tensor_slice_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/saved_tensor_slice_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/test_log_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/core/util/test_log_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/rpc/proto/tf_rpc_service_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/rpc/proto/tf_rpc_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/rpc/proto/tf_rpc_service_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/distribute/experimental/rpc/proto/tf_rpc_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/dtensor/proto/layout_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/dtensor/proto/layout_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/acceleration/configuration/configuration_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/experimental/acceleration/configuration/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/python/metrics/converter_error_data_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/python/metrics/converter_error_data_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/logging/toco_conversion_log_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/logging/toco_conversion_log_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/model_flags_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/model_flags_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/toco_flags_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/toco_flags_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/types_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/toco/types_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/compatibility/protos/compatibility_result_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/delegates/compatibility/protos/compatibility_result_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/evaluation_config_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/evaluation_config_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/evaluation_stages_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/evaluation_stages_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/preprocessing_steps_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/lite/tools/evaluation/proto/preprocessing_steps_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/framework/cpp_shape_inference_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/framework/cpp_shape_inference_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/projector_config_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/projector_config_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/saved_metadata_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/saved_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/versions_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/keras/protobuf/versions_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/kernel_tests/proto/test_example_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/kernel_tests/proto/test_example_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/tpu/tensor_tracer_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/tpu/tensor_tracer_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/training/checkpoint_state_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/training/checkpoint_state_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/python/util/protobuf/compare_test_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/python/util/protobuf/compare_test_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/security/fuzzing/checkpoint_reader_fuzz_input_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/security/fuzzing/checkpoint_reader_fuzz_input_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/proto_text/test_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tools/proto_text/test_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/protobuf/error_codes_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/protobuf/error_codes_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/protobuf/histogram_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow/tsl/protobuf/histogram_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/classification_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/classification_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/get_model_metadata_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/get_model_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/get_model_status_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/get_model_status_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/inference_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/inference_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/input_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/input_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/internal/serialized_input_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/internal/serialized_input_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/logging_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/logging_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_management_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_management_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_service_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_service_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/model_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/predict_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/predict_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/prediction_log_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/prediction_log_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/prediction_service_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/prediction_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/prediction_service_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/prediction_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/regression_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/regression_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/session_service_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/session_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/session_service_pb2_grpc.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/session_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/status_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/apis/status_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/file_system_storage_path_source_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/file_system_storage_path_source_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/log_collector_config_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/log_collector_config_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/logging_config_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/logging_config_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/model_server_config_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/model_server_config_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/monitoring_config_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/monitoring_config_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/platform_config_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/platform_config_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/ssl_config_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/config/ssl_config_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/core/test_util/fake_loader_source_adapter_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/core/test_util/fake_loader_source_adapter_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/model_servers/test_util/storage_path_error_injecting_source_adapter_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/model_servers/test_util/storage_path_error_injecting_source_adapter_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/resources/resources_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/resources/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/hashmap/hashmap_source_adapter_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/hashmap/hashmap_source_adapter_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/saved_model_bundle_source_adapter_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/saved_model_bundle_source_adapter_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/session_bundle_config_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/session_bundle_config_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/test_util/fake_thread_pool_factory_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/test_util/fake_thread_pool_factory_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/thread_pool_factory_config_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/servables/tensorflow/thread_pool_factory_config_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/session_bundle/oss/manifest_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/session_bundle/oss/manifest_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/sources/storage_path/static_storage_path_source_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/sources/storage_path/static_storage_path_source_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/util/class_registration_test_pb2.py` & `pythie-serving-3.4.0/src/pythie_serving/tensorflow_proto/tensorflow_serving/util/class_registration_test_pb2.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/treelite_wrapper.py` & `pythie-serving-3.4.0/src/pythie_serving/treelite_wrapper.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/utils.py` & `pythie-serving-3.4.0/src/pythie_serving/utils.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving/xgboost_wrapper.py` & `pythie-serving-3.4.0/src/pythie_serving/xgboost_wrapper.py`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving.egg-info/PKG-INFO` & `pythie-serving-3.4.0/src/pythie_serving.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pythie-serving
-Version: 3.3.0
+Version: 3.4.0
 Summary: A GRPC server to serve model types using tensorflow-serving .proto services
 Home-page: https://gitlab.cayzn.com/wiremind/data-science/pythie-neos.git
 Author: wiremind data science team
 Author-email: data-science@wiremind.io
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Provides-Extra: serving
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: all
```

### Comparing `pythie-serving-3.3.0/src/pythie_serving.egg-info/SOURCES.txt` & `pythie-serving-3.4.0/src/pythie_serving.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythie-serving-3.3.0/src/pythie_serving.egg-info/requires.txt` & `pythie-serving-3.4.0/src/pythie_serving.egg-info/requires.txt`

 * *Files identical despite different names*

