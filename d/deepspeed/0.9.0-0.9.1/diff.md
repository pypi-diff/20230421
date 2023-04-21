# Comparing `tmp/deepspeed-0.9.0.tar.gz` & `tmp/deepspeed-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepspeed-0.9.0.tar", last modified: Thu Apr 13 15:30:33 2023, max compression
+gzip compressed data, was "deepspeed-0.9.1.tar", last modified: Fri Apr 21 00:48:05 2023, max compression
```

## Comparing `deepspeed-0.9.0.tar` & `deepspeed-0.9.1.tar`

### file list

```diff
@@ -1,602 +1,602 @@
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.747389 deepspeed-0.9.0/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11357 2023-04-11 17:18:49.000000 deepspeed-0.9.0/LICENSE
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      290 2023-02-28 00:54:52.000000 deepspeed-0.9.0/MANIFEST.in
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27085 2023-04-13 15:30:33.747389 deepspeed-0.9.0/PKG-INFO
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    26202 2023-04-13 15:29:56.000000 deepspeed-0.9.0/README.md
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.577389 deepspeed-0.9.0/accelerator/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.0/accelerator/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4532 2023-04-11 17:18:49.000000 deepspeed-0.9.0/accelerator/abstract_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8029 2023-04-13 15:29:56.000000 deepspeed-0.9.0/accelerator/cuda_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3668 2023-04-11 17:18:49.000000 deepspeed-0.9.0/accelerator/real_accelerator.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.577389 deepspeed-0.9.0/bin/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.0/bin/deepspeed
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.0/bin/deepspeed.pt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.0/bin/ds
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      757 2022-08-05 18:43:48.000000 deepspeed-0.9.0/bin/ds_bench
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1869 2023-04-11 17:18:49.000000 deepspeed-0.9.0/bin/ds_elastic
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.0/bin/ds_report
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      680 2022-07-06 20:47:37.000000 deepspeed-0.9.0/bin/ds_ssh
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.0/bin/dsr
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:32.000000 deepspeed-0.9.0/build.txt
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.547389 deepspeed-0.9.0/csrc/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.577389 deepspeed-0.9.0/csrc/adagrad/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/adagrad/cpu_adagrad.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.577389 deepspeed-0.9.0/csrc/adam/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/adam/cpu_adam.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/adam/fused_adam_frontend.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/adam/multi_tensor_adam.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/adam/multi_tensor_apply.cuh
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.537389 deepspeed-0.9.0/csrc/aio/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.577389 deepspeed-0.9.0/csrc/aio/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/common/deepspeed_aio_common.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/common/deepspeed_aio_common.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/common/deepspeed_aio_types.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/common/deepspeed_aio_types.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/common/deepspeed_aio_utils.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/common/deepspeed_aio_utils.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.587389 deepspeed-0.9.0/csrc/aio/py_lib/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_aio_thread.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_aio_thread.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_pin_tensor.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_py_aio.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_py_aio.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_py_aio_handle.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_py_copy.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_py_copy.h
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/aio/py_lib/py_ds_aio.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.587389 deepspeed-0.9.0/csrc/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/common/custom_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.587389 deepspeed-0.9.0/csrc/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/StopWatch.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/Timer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/compat.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.0/csrc/includes/context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12108 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/conversion_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.0/csrc/includes/cpu_adagrad.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.0/csrc/includes/cpu_adam.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/custom_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/dequantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/dropout.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1178 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/ds_kernel_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/ds_transformer_cuda.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/feed_forward.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/gelu.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/gemm_test.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/general_kernels.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/memory_access_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/normalize_layer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/quantization.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17384 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/quantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      264 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/quantizer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/reduction_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/simd.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/softmax.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/strided_batch_gemm.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/includes/type_shim.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.587389 deepspeed-0.9.0/csrc/lamb/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/lamb/fused_lamb_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/lamb/fused_lamb_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.597389 deepspeed-0.9.0/csrc/quantization/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/quantization/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.0/csrc/quantization/fake_quantizer.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/quantization/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/quantization/quantize.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.597389 deepspeed-0.9.0/csrc/random_ltd/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/random_ltd/gather_scatter.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/random_ltd/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/random_ltd/slice_attn_masks.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/random_ltd/token_sort.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.597389 deepspeed-0.9.0/csrc/sparse_attention/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/sparse_attention/utils.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.537389 deepspeed-0.9.0/csrc/spatial/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.597389 deepspeed-0.9.0/csrc/spatial/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/spatial/csrc/opt_bias_add.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/spatial/csrc/pt_binding.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.597389 deepspeed-0.9.0/csrc/spatial/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      833 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/spatial/includes/spatial_cuda_layers.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.597389 deepspeed-0.9.0/csrc/transformer/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/transformer/cublas_wrappers.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.0/csrc/transformer/dropout_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.0/csrc/transformer/ds_transformer_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/transformer/gelu_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14532 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/transformer/general_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.537389 deepspeed-0.9.0/csrc/transformer/inference/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.597389 deepspeed-0.9.0/csrc/transformer/inference/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    16338 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6908 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/transformer/inference/csrc/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29045 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/transformer/inference/csrc/gelu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22685 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/transformer/inference/csrc/layer_norm.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    77643 2023-04-13 15:29:56.000000 deepspeed-0.9.0/csrc/transformer/inference/csrc/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/transformer/inference/csrc/relu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23789 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/transformer/inference/csrc/softmax.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29531 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/transformer/inference/csrc/transform.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.597389 deepspeed-0.9.0/csrc/transformer/inference/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10279 2023-04-13 15:29:56.000000 deepspeed-0.9.0/csrc/transformer/inference/includes/inference_context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17739 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/transformer/inference/includes/inference_cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8265 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/transformer/inference/includes/inference_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/transformer/normalize_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/transformer/softmax_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/transformer/transform_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.597389 deepspeed-0.9.0/csrc/utils/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.0/csrc/utils/flatten_unflatten.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.597389 deepspeed-0.9.0/deepspeed/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    13947 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.607389 deepspeed-0.9.0/deepspeed/accelerator/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/accelerator/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4532 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/accelerator/abstract_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8029 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/accelerator/cuda_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3668 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/accelerator/real_accelerator.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.607389 deepspeed-0.9.0/deepspeed/autotuning/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      129 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/autotuning/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    54204 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/autotuning/autotuner.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4633 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/autotuning/config.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.607389 deepspeed-0.9.0/deepspeed/autotuning/config_templates/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       48 2022-07-06 20:47:37.000000 deepspeed-0.9.0/deepspeed/autotuning/config_templates/template_zero0.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      113 2022-07-06 20:47:37.000000 deepspeed-0.9.0/deepspeed/autotuning/config_templates/template_zero1.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      237 2022-07-06 20:47:37.000000 deepspeed-0.9.0/deepspeed/autotuning/config_templates/template_zero2.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      485 2022-07-06 20:47:37.000000 deepspeed-0.9.0/deepspeed/autotuning/config_templates/template_zero3.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5945 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/autotuning/constants.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    15644 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/autotuning/scheduler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.607389 deepspeed-0.9.0/deepspeed/autotuning/tuner/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      235 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/autotuning/tuner/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2756 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/autotuning/tuner/base_tuner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1820 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/autotuning/tuner/cost_model.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1158 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/autotuning/tuner/index_based_tuner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5614 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/autotuning/tuner/model_based_tuner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2329 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/autotuning/tuner/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15054 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/autotuning/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.617389 deepspeed-0.9.0/deepspeed/checkpoint/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      561 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/checkpoint/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2335 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/checkpoint/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12009 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/checkpoint/deepspeed_checkpoint.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4674 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/checkpoint/reshape_3d_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7885 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/checkpoint/reshape_meg_2d.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2888 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/checkpoint/reshape_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4888 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/checkpoint/universal_checkpoint.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      936 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/checkpoint/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5316 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/checkpoint/zero_checkpoint.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.617389 deepspeed-0.9.0/deepspeed/comm/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2124 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/comm/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1416 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/comm/backend.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26108 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/comm/comm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      855 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/comm/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1256 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/comm/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10310 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/comm/torch.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4184 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/comm/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.617389 deepspeed-0.9.0/deepspeed/compression/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      243 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/compression/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    36034 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/compression/basic_layer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10519 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/compression/compress.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23240 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/compression/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4959 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/compression/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12303 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/compression/helper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8039 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/compression/scheduler.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7814 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/compression/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      733 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.617389 deepspeed-0.9.0/deepspeed/elasticity/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      383 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/elasticity/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4701 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/elasticity/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2452 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/elasticity/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7762 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/elasticity/elastic_agent.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17374 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/elasticity/elasticity.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      459 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/elasticity/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4793 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/env_report.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      756 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/git_version_info.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      790 2023-04-13 15:30:32.000000 deepspeed-0.9.0/deepspeed/git_version_info_installed.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.617389 deepspeed-0.9.0/deepspeed/inference/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/inference/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9506 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/inference/config.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    28924 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/inference/engine.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.617389 deepspeed-0.9.0/deepspeed/launcher/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/launcher/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      352 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/launcher/constants.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    19078 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/launcher/launch.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11952 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/launcher/multinode_runner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    23296 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/launcher/runner.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.617389 deepspeed-0.9.0/deepspeed/model_implementations/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      220 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/model_implementations/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.617389 deepspeed-0.9.0/deepspeed/model_implementations/diffusers/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/model_implementations/diffusers/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2792 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/model_implementations/diffusers/unet.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6025 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/model_implementations/diffusers/vae.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.627389 deepspeed-0.9.0/deepspeed/model_implementations/features/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/model_implementations/features/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      563 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/model_implementations/features/cuda_graph.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.627389 deepspeed-0.9.0/deepspeed/model_implementations/transformers/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/model_implementations/transformers/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3045 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/model_implementations/transformers/clip_encoder.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      388 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/model_implementations/transformers/ds_base.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      667 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/model_implementations/transformers/ds_bert.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      669 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/model_implementations/transformers/ds_bloom.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/model_implementations/transformers/ds_gpt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      682 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/model_implementations/transformers/ds_megatron_gpt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/model_implementations/transformers/ds_opt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7828 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/model_implementations/transformers/ds_transformer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.627389 deepspeed-0.9.0/deepspeed/module_inject/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      444 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/module_inject/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4815 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/module_inject/auto_tp.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.637389 deepspeed-0.9.0/deepspeed/module_inject/containers/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      838 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23292 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/base.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5756 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/base_moe.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3718 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/bert.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4762 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/bloom.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2807 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/clip.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3137 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/distil_bert.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.637389 deepspeed-0.9.0/deepspeed/module_inject/containers/features/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      181 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/features/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1206 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/features/megatron.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2486 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/features/meta_tensor.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2249 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/gpt2.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3833 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/gptj.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4107 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/gptneo.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5005 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/gptneox.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5045 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/megatron_gpt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3913 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/megatron_gpt_moe.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5660 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/opt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1732 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/unet.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1163 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/module_inject/containers/vae.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     4719 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/module_inject/inject.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3825 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/module_inject/layers.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14122 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/module_inject/load_checkpoint.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3107 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/module_inject/module_quantize.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7723 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/module_inject/policy.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    35947 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/module_inject/replace_module.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      930 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/module_inject/replace_policy.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1653 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/module_inject/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.637389 deepspeed-0.9.0/deepspeed/moe/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/moe/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1223 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/moe/experts.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6082 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/moe/layer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3529 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/moe/mappings.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20621 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/moe/sharded_moe.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5214 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/moe/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.637389 deepspeed-0.9.0/deepspeed/monitor/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/monitor/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2529 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/monitor/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2907 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/monitor/csv_monitor.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1604 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/monitor/monitor.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2227 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/monitor/tensorboard.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      754 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/monitor/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1150 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/monitor/wandb.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.637389 deepspeed-0.9.0/deepspeed/nebula/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/nebula/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1764 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/nebula/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2786 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/nebula/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.637389 deepspeed-0.9.0/deepspeed/ops/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      477 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.637389 deepspeed-0.9.0/deepspeed/ops/adagrad/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      141 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/adagrad/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5089 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/adagrad/cpu_adagrad.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.637389 deepspeed-0.9.0/deepspeed/ops/adam/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      169 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/adam/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8546 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/adam/cpu_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6878 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/adam/fused_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      429 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/adam/multi_tensor_apply.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.637389 deepspeed-0.9.0/deepspeed/ops/aio/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      136 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/aio/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.557389 deepspeed-0.9.0/deepspeed/ops/csrc/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.647389 deepspeed-0.9.0/deepspeed/ops/csrc/adagrad/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.647389 deepspeed-0.9.0/deepspeed/ops/csrc/adam/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/adam/cpu_adam.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/adam/multi_tensor_adam.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.557389 deepspeed-0.9.0/deepspeed/ops/csrc/aio/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.647389 deepspeed-0.9.0/deepspeed/ops/csrc/aio/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.657389 deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.657389 deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_test/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      359 2021-08-17 18:54:40.000000 deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_test/single_process_config.json
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.657389 deepspeed-0.9.0/deepspeed/ops/csrc/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/common/custom_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.667389 deepspeed-0.9.0/deepspeed/ops/csrc/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/StopWatch.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/Timer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/compat.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12108 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/conversion_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/cpu_adagrad.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/cpu_adam.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/custom_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/dequantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/dropout.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1178 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/ds_kernel_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/ds_transformer_cuda.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/feed_forward.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/gelu.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/gemm_test.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/general_kernels.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/memory_access_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/normalize_layer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/quantization.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17384 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/quantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      264 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/quantizer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/reduction_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/simd.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/softmax.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/strided_batch_gemm.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/includes/type_shim.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.667389 deepspeed-0.9.0/deepspeed/ops/csrc/lamb/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.667389 deepspeed-0.9.0/deepspeed/ops/csrc/quantization/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/quantization/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/ops/csrc/quantization/fake_quantizer.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/quantization/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/quantization/quantize.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.667389 deepspeed-0.9.0/deepspeed/ops/csrc/random_ltd/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/random_ltd/gather_scatter.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/random_ltd/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/random_ltd/token_sort.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.677389 deepspeed-0.9.0/deepspeed/ops/csrc/sparse_attention/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/sparse_attention/utils.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.557389 deepspeed-0.9.0/deepspeed/ops/csrc/spatial/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.677389 deepspeed-0.9.0/deepspeed/ops/csrc/spatial/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.677389 deepspeed-0.9.0/deepspeed/ops/csrc/spatial/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      833 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.677389 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/cublas_wrappers.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/dropout_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/gelu_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14532 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/general_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.557389 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.677389 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    16338 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6908 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29045 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22685 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    77643 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23789 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29531 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.687389 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10279 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17739 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8265 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/normalize_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/softmax_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/transformer/transform_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.687389 deepspeed-0.9.0/deepspeed/ops/csrc/utils/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/csrc/utils/flatten_unflatten.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.687389 deepspeed-0.9.0/deepspeed/ops/lamb/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      130 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/lamb/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7815 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/lamb/fused_lamb.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.697389 deepspeed-0.9.0/deepspeed/ops/op_builder/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/op_builder/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/op_builder/all_ops.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/op_builder/async_io.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28488 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/op_builder/builder.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/op_builder/cpu_adagrad.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/op_builder/cpu_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/op_builder/fused_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/op_builder/fused_lamb.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/op_builder/quantizer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/op_builder/random_ltd.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2965 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/op_builder/sparse_attn.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/op_builder/spatial_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/op_builder/stochastic_transformer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/op_builder/transformer.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2622 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/op_builder/transformer_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/op_builder/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.697389 deepspeed-0.9.0/deepspeed/ops/quantizer/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/quantizer/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1193 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/quantizer/quantizer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.697389 deepspeed-0.9.0/deepspeed/ops/random_ltd/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      191 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/random_ltd/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4901 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/random_ltd/dropping_utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.697389 deepspeed-0.9.0/deepspeed/ops/sparse_attention/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      467 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/sparse_attention/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3463 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    32948 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/sparse_attention/matmul.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11322 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/sparse_attention/softmax.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12300 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/sparse_attention/sparse_attention_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6746 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/sparse_attention/sparse_self_attention.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    42462 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/sparse_attention/sparsity_config.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.697389 deepspeed-0.9.0/deepspeed/ops/sparse_attention/trsrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1032 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/sparse_attention/trsrc/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6628 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/sparse_attention/trsrc/matmul.tr
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1923 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4047 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.697389 deepspeed-0.9.0/deepspeed/ops/transformer/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      413 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/transformer/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.697389 deepspeed-0.9.0/deepspeed/ops/transformer/inference/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      315 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      876 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/bias_add.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5612 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      236 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/diffusers_2d_transformer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9944 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/diffusers_attention.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4763 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/diffusers_transformer_block.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13928 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/ds_attention.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4585 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/ds_mlp.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18473 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/moe_inference.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.707389 deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      382 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      551 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/base.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1051 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1007 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/linear.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1273 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1424 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1215 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/residual_add.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1059 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/softmax.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1513 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/softmax_context.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      875 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4434 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/transformer/inference/triton_ops.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20600 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/ops/transformer/transformer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.707389 deepspeed-0.9.0/deepspeed/pipe/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      164 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/pipe/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.707389 deepspeed-0.9.0/deepspeed/profiling/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/profiling/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1708 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/profiling/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1098 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/profiling/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.707389 deepspeed-0.9.0/deepspeed/profiling/flops_profiler/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      120 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/profiling/flops_profiler/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47039 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/profiling/flops_profiler/profiler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.707389 deepspeed-0.9.0/deepspeed/runtime/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      192 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.717389 deepspeed-0.9.0/deepspeed/runtime/activation_checkpointing/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/activation_checkpointing/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    32764 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/activation_checkpointing/checkpointing.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3987 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/activation_checkpointing/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18459 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/bf16_optimizer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.717389 deepspeed-0.9.0/deepspeed/runtime/checkpoint_engine/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/checkpoint_engine/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      654 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4982 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1060 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.717389 deepspeed-0.9.0/deepspeed/runtime/comm/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/comm/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3698 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/comm/coalesced_collectives.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10062 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/comm/mpi.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7712 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/comm/nccl.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.717389 deepspeed-0.9.0/deepspeed/runtime/compression/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/compression/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      701 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/compression/cupy.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    39382 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/runtime/config.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8199 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/config_utils.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    12806 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.717389 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6081 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4701 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10025 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/curriculum_scheduler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.717389 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_routing/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_routing/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5638 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1282 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_routing/helper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4638 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_routing/scheduler.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      955 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_routing/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.717389 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_sampling/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_sampling/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    25015 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19160 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20614 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1756 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_sampling/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6977 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/dataloader.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5625 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/eigenvalue.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)   148945 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/runtime/engine.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.717389 deepspeed-0.9.0/deepspeed/runtime/fp16/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/fp16/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20052 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/fp16/fused_optimizer.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11093 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/runtime/fp16/loss_scaler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.727389 deepspeed-0.9.0/deepspeed/runtime/fp16/onebit/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      186 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/fp16/onebit/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15258 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/fp16/onebit/adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23085 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/fp16/onebit/lamb.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19112 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/fp16/onebit/zoadam.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18076 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/fp16/unfused_optimizer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19007 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/runtime/hybrid_engine.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    33557 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/lr_schedules.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.727389 deepspeed-0.9.0/deepspeed/runtime/pipe/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      195 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/pipe/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    56517 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/pipe/engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27186 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/pipe/module.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5477 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/pipe/p2p.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15546 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/pipe/schedule.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17167 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/pipe/topology.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1353 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/progressive_layer_drop.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     7699 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/quantize.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2416 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/sparse_tensor.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18177 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/state_dict_factory.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.727389 deepspeed-0.9.0/deepspeed/runtime/swap_tensor/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       95 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/swap_tensor/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1172 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/swap_tensor/aio_config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6282 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/swap_tensor/async_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      596 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/swap_tensor/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18967 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/swap_tensor/optimizer_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9654 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17684 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10793 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7734 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/swap_tensor/utils.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    35806 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/runtime/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/weight_quantizer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.727389 deepspeed-0.9.0/deepspeed/runtime/zero/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      423 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/zero/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9996 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/runtime/zero/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10926 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/zero/contiguous_memory_allocator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7784 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/runtime/zero/linear.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2931 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/zero/offload_config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    21889 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/runtime/zero/parameter_offload.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    69726 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/runtime/zero/partition_parameters.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22345 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/runtime/zero/partitioned_param_coordinator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)   112178 2023-04-13 15:29:56.000000 deepspeed-0.9.0/deepspeed/runtime/zero/stage3.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)   110183 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/zero/stage_1_and_2.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2727 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/zero/test.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11727 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/zero/tiling.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2931 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/runtime/zero/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.737389 deepspeed-0.9.0/deepspeed/utils/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      717 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/utils/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6096 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/utils/comms_logging.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4370 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/utils/debug.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      144 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/utils/exceptions.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15606 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/utils/groups.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3004 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/utils/init_on_device.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4375 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/utils/logging.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2041 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/utils/mixed_precision_linkage.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      499 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/utils/nvtx.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7997 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/utils/tensor_fragment.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8765 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/utils/timer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      200 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/utils/types.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18737 2023-04-11 17:18:49.000000 deepspeed-0.9.0/deepspeed/utils/zero_to_fp32.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.607389 deepspeed-0.9.0/deepspeed.egg-info/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27085 2023-04-13 15:30:32.000000 deepspeed-0.9.0/deepspeed.egg-info/PKG-INFO
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20079 2023-04-13 15:30:33.000000 deepspeed-0.9.0/deepspeed.egg-info/SOURCES.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        1 2023-04-13 15:30:32.000000 deepspeed-0.9.0/deepspeed.egg-info/dependency_links.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       85 2023-04-13 15:30:32.000000 deepspeed-0.9.0/deepspeed.egg-info/entry_points.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1094 2023-04-13 15:30:32.000000 deepspeed-0.9.0/deepspeed.egg-info/requires.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       10 2023-04-13 15:30:32.000000 deepspeed-0.9.0/deepspeed.egg-info/top_level.txt
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.737389 deepspeed-0.9.0/op_builder/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.0/op_builder/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.0/op_builder/all_ops.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.0/op_builder/async_io.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28488 2023-04-11 17:18:49.000000 deepspeed-0.9.0/op_builder/builder.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.0/op_builder/cpu_adagrad.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.0/op_builder/cpu_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.0/op_builder/fused_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.0/op_builder/fused_lamb.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.0/op_builder/quantizer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.0/op_builder/random_ltd.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2965 2023-04-11 17:18:49.000000 deepspeed-0.9.0/op_builder/sparse_attn.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.0/op_builder/spatial_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.0/op_builder/stochastic_transformer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.0/op_builder/transformer.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2622 2023-04-11 17:18:49.000000 deepspeed-0.9.0/op_builder/transformer_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.0/op_builder/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-13 15:30:33.747389 deepspeed-0.9.0/requirements/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        7 2022-07-06 20:47:37.000000 deepspeed-0.9.0/requirements/requirements-1bit-mpi.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       23 2022-07-06 20:47:37.000000 deepspeed-0.9.0/requirements/requirements-autotuning-ml.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        9 2022-07-06 20:47:37.000000 deepspeed-0.9.0/requirements/requirements-autotuning.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      232 2022-11-14 17:49:34.000000 deepspeed-0.9.0/requirements/requirements-dev.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       72 2023-02-28 00:54:52.000000 deepspeed-0.9.0/requirements/requirements-inf.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       85 2022-11-23 21:50:53.000000 deepspeed-0.9.0/requirements/requirements-readthedocs.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       36 2023-04-11 17:18:49.000000 deepspeed-0.9.0/requirements/requirements-sd.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       14 2022-07-06 20:47:37.000000 deepspeed-0.9.0/requirements/requirements-sparse_attn.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       72 2023-02-28 00:54:52.000000 deepspeed-0.9.0/requirements/requirements.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      148 2023-04-13 15:30:33.747389 deepspeed-0.9.0/setup.cfg
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11109 2023-04-11 17:18:49.000000 deepspeed-0.9.0/setup.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        6 2023-04-13 15:29:56.000000 deepspeed-0.9.0/version.txt
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.873510 deepspeed-0.9.1/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11357 2023-04-11 17:18:49.000000 deepspeed-0.9.1/LICENSE
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      290 2023-02-28 00:54:52.000000 deepspeed-0.9.1/MANIFEST.in
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27276 2023-04-21 00:48:05.873510 deepspeed-0.9.1/PKG-INFO
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    26393 2023-04-21 00:47:36.000000 deepspeed-0.9.1/README.md
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.473510 deepspeed-0.9.1/accelerator/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.1/accelerator/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4532 2023-04-11 17:18:49.000000 deepspeed-0.9.1/accelerator/abstract_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8029 2023-04-13 15:29:56.000000 deepspeed-0.9.1/accelerator/cuda_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3668 2023-04-11 17:18:49.000000 deepspeed-0.9.1/accelerator/real_accelerator.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.473510 deepspeed-0.9.1/bin/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.1/bin/deepspeed
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.1/bin/deepspeed.pt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.1/bin/ds
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      757 2022-08-05 18:43:48.000000 deepspeed-0.9.1/bin/ds_bench
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1869 2023-04-11 17:18:49.000000 deepspeed-0.9.1/bin/ds_elastic
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.1/bin/ds_report
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      680 2022-07-06 20:47:37.000000 deepspeed-0.9.1/bin/ds_ssh
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.1/bin/dsr
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:04.000000 deepspeed-0.9.1/build.txt
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.433510 deepspeed-0.9.1/csrc/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.473510 deepspeed-0.9.1/csrc/adagrad/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/adagrad/cpu_adagrad.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.473510 deepspeed-0.9.1/csrc/adam/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/adam/cpu_adam.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/adam/fused_adam_frontend.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/adam/multi_tensor_adam.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/adam/multi_tensor_apply.cuh
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.423510 deepspeed-0.9.1/csrc/aio/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.473510 deepspeed-0.9.1/csrc/aio/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_common.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_common.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_types.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_types.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_utils.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_utils.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.483510 deepspeed-0.9.1/csrc/aio/py_lib/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_aio_thread.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_aio_thread.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_pin_tensor.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_aio.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_aio.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_aio_handle.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_copy.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_copy.h
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/aio/py_lib/py_ds_aio.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.483510 deepspeed-0.9.1/csrc/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/common/custom_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.503510 deepspeed-0.9.1/csrc/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/StopWatch.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/Timer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/compat.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.1/csrc/includes/context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12223 2023-04-21 00:47:36.000000 deepspeed-0.9.1/csrc/includes/conversion_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.1/csrc/includes/cpu_adagrad.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.1/csrc/includes/cpu_adam.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/custom_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/dequantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/dropout.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1178 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/ds_kernel_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/ds_transformer_cuda.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/feed_forward.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/gelu.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/gemm_test.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/general_kernels.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/memory_access_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/normalize_layer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/quantization.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.1/csrc/includes/quantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      264 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/quantizer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/reduction_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/simd.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/softmax.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/strided_batch_gemm.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/includes/type_shim.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.503510 deepspeed-0.9.1/csrc/lamb/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/lamb/fused_lamb_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/lamb/fused_lamb_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.513510 deepspeed-0.9.1/csrc/quantization/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/quantization/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.1/csrc/quantization/fake_quantizer.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/quantization/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/quantization/quantize.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.513510 deepspeed-0.9.1/csrc/random_ltd/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/random_ltd/gather_scatter.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/random_ltd/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/random_ltd/slice_attn_masks.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/random_ltd/token_sort.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.523510 deepspeed-0.9.1/csrc/sparse_attention/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/sparse_attention/utils.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.433510 deepspeed-0.9.1/csrc/spatial/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.523510 deepspeed-0.9.1/csrc/spatial/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/spatial/csrc/opt_bias_add.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/spatial/csrc/pt_binding.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.523510 deepspeed-0.9.1/csrc/spatial/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      833 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/spatial/includes/spatial_cuda_layers.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.533510 deepspeed-0.9.1/csrc/transformer/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/cublas_wrappers.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.1/csrc/transformer/dropout_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.1/csrc/transformer/ds_transformer_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/gelu_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14532 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/general_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.433510 deepspeed-0.9.1/csrc/transformer/inference/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.543510 deepspeed-0.9.1/csrc/transformer/inference/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    16338 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6908 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/csrc/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29045 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/csrc/gelu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22685 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/csrc/layer_norm.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    77643 2023-04-21 00:47:36.000000 deepspeed-0.9.1/csrc/transformer/inference/csrc/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/csrc/relu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23789 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/csrc/softmax.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29531 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/csrc/transform.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.543510 deepspeed-0.9.1/csrc/transformer/inference/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10279 2023-04-13 15:29:56.000000 deepspeed-0.9.1/csrc/transformer/inference/includes/inference_context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17739 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/includes/inference_cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8265 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/inference/includes/inference_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/normalize_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/softmax_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/transformer/transform_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.543510 deepspeed-0.9.1/csrc/utils/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.1/csrc/utils/flatten_unflatten.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.553510 deepspeed-0.9.1/deepspeed/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    14304 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.553510 deepspeed-0.9.1/deepspeed/accelerator/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/accelerator/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4532 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/accelerator/abstract_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8029 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/accelerator/cuda_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3668 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/accelerator/real_accelerator.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.553510 deepspeed-0.9.1/deepspeed/autotuning/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      129 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    54204 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/autotuning/autotuner.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4633 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/config.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.573510 deepspeed-0.9.1/deepspeed/autotuning/config_templates/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       48 2022-07-06 20:47:37.000000 deepspeed-0.9.1/deepspeed/autotuning/config_templates/template_zero0.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      113 2022-07-06 20:47:37.000000 deepspeed-0.9.1/deepspeed/autotuning/config_templates/template_zero1.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      237 2022-07-06 20:47:37.000000 deepspeed-0.9.1/deepspeed/autotuning/config_templates/template_zero2.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      485 2022-07-06 20:47:37.000000 deepspeed-0.9.1/deepspeed/autotuning/config_templates/template_zero3.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5945 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/constants.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    15644 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/scheduler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.573510 deepspeed-0.9.1/deepspeed/autotuning/tuner/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      235 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/tuner/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2756 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/tuner/base_tuner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1820 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/tuner/cost_model.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1158 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/tuner/index_based_tuner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5614 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/tuner/model_based_tuner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2329 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/tuner/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15054 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/autotuning/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.583510 deepspeed-0.9.1/deepspeed/checkpoint/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      561 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/checkpoint/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2429 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/checkpoint/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12009 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/checkpoint/deepspeed_checkpoint.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4674 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/checkpoint/reshape_3d_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7885 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/checkpoint/reshape_meg_2d.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2888 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/checkpoint/reshape_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4888 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/checkpoint/universal_checkpoint.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      936 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/checkpoint/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5316 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/checkpoint/zero_checkpoint.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.583510 deepspeed-0.9.1/deepspeed/comm/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      137 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/comm/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1416 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/comm/backend.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26108 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/comm/comm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      855 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/comm/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1256 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/comm/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10257 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/comm/torch.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3684 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/comm/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.593510 deepspeed-0.9.1/deepspeed/compression/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      243 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/compression/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    36034 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/compression/basic_layer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10519 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/compression/compress.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23240 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/compression/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4959 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/compression/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12303 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/compression/helper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8039 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/compression/scheduler.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7814 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/compression/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      733 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.603510 deepspeed-0.9.1/deepspeed/elasticity/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      383 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/elasticity/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4701 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/elasticity/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2452 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/elasticity/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7762 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/elasticity/elastic_agent.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17374 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/elasticity/elasticity.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      459 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/elasticity/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4793 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/env_report.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      756 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/git_version_info.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      790 2023-04-21 00:48:04.000000 deepspeed-0.9.1/deepspeed/git_version_info_installed.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.603510 deepspeed-0.9.1/deepspeed/inference/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/inference/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9506 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/inference/config.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    28924 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/inference/engine.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.613510 deepspeed-0.9.1/deepspeed/launcher/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/launcher/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      352 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/launcher/constants.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    19078 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/launcher/launch.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11952 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/launcher/multinode_runner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    23296 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/launcher/runner.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.613510 deepspeed-0.9.1/deepspeed/model_implementations/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      220 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.613510 deepspeed-0.9.1/deepspeed/model_implementations/diffusers/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/diffusers/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2792 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/diffusers/unet.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6025 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/diffusers/vae.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.613510 deepspeed-0.9.1/deepspeed/model_implementations/features/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/features/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      563 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/features/cuda_graph.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.623510 deepspeed-0.9.1/deepspeed/model_implementations/transformers/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3045 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/clip_encoder.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      388 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_base.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      667 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_bert.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      669 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_bloom.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_gpt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      682 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_megatron_gpt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_opt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7828 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_transformer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.633510 deepspeed-0.9.1/deepspeed/module_inject/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      444 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4815 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/auto_tp.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.653510 deepspeed-0.9.1/deepspeed/module_inject/containers/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      838 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23292 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/base.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5756 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/base_moe.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3718 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/bert.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4762 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/bloom.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2807 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/clip.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3137 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/distil_bert.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.653510 deepspeed-0.9.1/deepspeed/module_inject/containers/features/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      181 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/features/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1206 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/features/megatron.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2486 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/features/meta_tensor.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2249 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/gpt2.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3833 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/gptj.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4107 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/gptneo.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5005 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/gptneox.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5045 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/megatron_gpt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3913 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/megatron_gpt_moe.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6283 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/opt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1732 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/unet.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1163 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/containers/vae.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     4719 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/inject.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3825 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/layers.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14122 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/load_checkpoint.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3107 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/module_quantize.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7723 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/policy.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    35947 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/module_inject/replace_module.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      930 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/replace_policy.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1653 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/module_inject/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.663510 deepspeed-0.9.1/deepspeed/moe/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/moe/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1223 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/moe/experts.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6082 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/moe/layer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3529 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/moe/mappings.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20621 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/moe/sharded_moe.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5214 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/moe/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.673510 deepspeed-0.9.1/deepspeed/monitor/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/monitor/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2529 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/monitor/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2907 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/monitor/csv_monitor.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1604 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/monitor/monitor.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2227 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/monitor/tensorboard.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      754 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/monitor/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1150 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/monitor/wandb.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.673510 deepspeed-0.9.1/deepspeed/nebula/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/nebula/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1764 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/nebula/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2786 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/nebula/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.673510 deepspeed-0.9.1/deepspeed/ops/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      477 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.673510 deepspeed-0.9.1/deepspeed/ops/adagrad/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      141 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/adagrad/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5089 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/adagrad/cpu_adagrad.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.683510 deepspeed-0.9.1/deepspeed/ops/adam/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      169 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/adam/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8546 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/adam/cpu_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6878 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/adam/fused_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      429 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/adam/multi_tensor_apply.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.683510 deepspeed-0.9.1/deepspeed/ops/aio/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      136 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/aio/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.453510 deepspeed-0.9.1/deepspeed/ops/csrc/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.683510 deepspeed-0.9.1/deepspeed/ops/csrc/adagrad/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.683510 deepspeed-0.9.1/deepspeed/ops/csrc/adam/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/adam/cpu_adam.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/adam/multi_tensor_adam.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.453510 deepspeed-0.9.1/deepspeed/ops/csrc/aio/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.693510 deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.693510 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.693510 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_test/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      359 2021-08-17 18:54:40.000000 deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_test/single_process_config.json
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.693510 deepspeed-0.9.1/deepspeed/ops/csrc/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/common/custom_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.693510 deepspeed-0.9.1/deepspeed/ops/csrc/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/StopWatch.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/Timer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/compat.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12223 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/conversion_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/cpu_adagrad.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/cpu_adam.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/custom_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/dequantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/dropout.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1178 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/ds_kernel_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/ds_transformer_cuda.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/feed_forward.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/gelu.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/gemm_test.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/general_kernels.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/memory_access_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/normalize_layer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/quantization.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/quantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      264 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/quantizer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/reduction_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/simd.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/softmax.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/strided_batch_gemm.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/includes/type_shim.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.693510 deepspeed-0.9.1/deepspeed/ops/csrc/lamb/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.703510 deepspeed-0.9.1/deepspeed/ops/csrc/quantization/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/quantization/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/csrc/quantization/fake_quantizer.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/quantization/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/quantization/quantize.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.703510 deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/gather_scatter.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/token_sort.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.703510 deepspeed-0.9.1/deepspeed/ops/csrc/sparse_attention/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/sparse_attention/utils.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.453510 deepspeed-0.9.1/deepspeed/ops/csrc/spatial/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.703510 deepspeed-0.9.1/deepspeed/ops/csrc/spatial/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.703510 deepspeed-0.9.1/deepspeed/ops/csrc/spatial/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      833 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.713510 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/cublas_wrappers.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/dropout_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/gelu_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14532 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/general_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.453510 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.713510 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    16338 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6908 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29045 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22685 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    77643 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23789 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29531 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.713510 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10279 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17739 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8265 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/normalize_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/softmax_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/transformer/transform_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.723510 deepspeed-0.9.1/deepspeed/ops/csrc/utils/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/csrc/utils/flatten_unflatten.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.723510 deepspeed-0.9.1/deepspeed/ops/lamb/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      130 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/lamb/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7815 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/lamb/fused_lamb.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.733510 deepspeed-0.9.1/deepspeed/ops/op_builder/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/all_ops.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/async_io.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28628 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/builder.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/cpu_adagrad.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/cpu_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/fused_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/fused_lamb.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/quantizer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/random_ltd.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/sparse_attn.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/spatial_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/stochastic_transformer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/transformer.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2622 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/transformer_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/op_builder/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.733510 deepspeed-0.9.1/deepspeed/ops/quantizer/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/quantizer/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1193 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/quantizer/quantizer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.743510 deepspeed-0.9.1/deepspeed/ops/random_ltd/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      191 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/random_ltd/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4901 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/random_ltd/dropping_utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.743510 deepspeed-0.9.1/deepspeed/ops/sparse_attention/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      467 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3463 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    32948 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/matmul.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11322 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/softmax.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12300 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/sparse_attention_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6746 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/sparse_self_attention.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    42462 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/sparsity_config.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.753510 deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1032 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6628 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/matmul.tr
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1923 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4047 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.753510 deepspeed-0.9.1/deepspeed/ops/transformer/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      413 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.763510 deepspeed-0.9.1/deepspeed/ops/transformer/inference/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      315 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      876 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/bias_add.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5612 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      236 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/diffusers_2d_transformer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9986 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/diffusers_attention.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4763 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/diffusers_transformer_block.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13928 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/ds_attention.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4585 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/ds_mlp.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18473 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/moe_inference.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.773510 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      382 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      551 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/base.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1227 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1007 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/linear.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1273 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1424 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1215 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/residual_add.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1059 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/softmax.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1513 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/softmax_context.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      875 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4434 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/inference/triton_ops.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20600 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/ops/transformer/transformer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.773510 deepspeed-0.9.1/deepspeed/pipe/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      164 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/pipe/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.773510 deepspeed-0.9.1/deepspeed/profiling/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/profiling/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1708 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/profiling/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1098 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/profiling/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.773510 deepspeed-0.9.1/deepspeed/profiling/flops_profiler/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      120 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/profiling/flops_profiler/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47039 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/profiling/flops_profiler/profiler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.793510 deepspeed-0.9.1/deepspeed/runtime/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      192 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.793510 deepspeed-0.9.1/deepspeed/runtime/activation_checkpointing/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/activation_checkpointing/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    32764 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/activation_checkpointing/checkpointing.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3987 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/activation_checkpointing/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18559 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/runtime/bf16_optimizer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.803510 deepspeed-0.9.1/deepspeed/runtime/checkpoint_engine/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/checkpoint_engine/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      654 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4982 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1060 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.803510 deepspeed-0.9.1/deepspeed/runtime/comm/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/comm/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3698 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/comm/coalesced_collectives.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10062 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/comm/mpi.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7712 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/comm/nccl.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.803510 deepspeed-0.9.1/deepspeed/runtime/compression/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/compression/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      701 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/compression/cupy.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    39382 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/config.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8199 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/config_utils.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    12806 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.803510 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6081 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4701 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10025 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/curriculum_scheduler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.813510 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5638 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1282 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/helper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4638 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/scheduler.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      955 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.813510 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    25015 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19160 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20614 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1756 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6977 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/dataloader.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5625 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/eigenvalue.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)   149903 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/runtime/engine.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.813510 deepspeed-0.9.1/deepspeed/runtime/fp16/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/fp16/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20052 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/fp16/fused_optimizer.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11093 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/fp16/loss_scaler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.823510 deepspeed-0.9.1/deepspeed/runtime/fp16/onebit/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      186 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/fp16/onebit/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15258 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/fp16/onebit/adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23085 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/fp16/onebit/lamb.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19112 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/fp16/onebit/zoadam.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18076 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/fp16/unfused_optimizer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19007 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/hybrid_engine.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    33557 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/lr_schedules.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.823510 deepspeed-0.9.1/deepspeed/runtime/pipe/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      195 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/pipe/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    56559 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/runtime/pipe/engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27186 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/pipe/module.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5477 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/pipe/p2p.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15546 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/pipe/schedule.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17167 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/pipe/topology.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1353 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/progressive_layer_drop.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     7699 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/quantize.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2416 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/sparse_tensor.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18177 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/state_dict_factory.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.833510 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       95 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1172 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/aio_config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6282 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/async_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      596 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18967 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/optimizer_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9654 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17684 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10793 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7734 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/swap_tensor/utils.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    35806 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/weight_quantizer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.843510 deepspeed-0.9.1/deepspeed/runtime/zero/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      423 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/zero/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9996 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/zero/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10926 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/zero/contiguous_memory_allocator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7784 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/zero/linear.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2931 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/zero/offload_config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    21889 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/zero/parameter_offload.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    71248 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/runtime/zero/partition_parameters.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22345 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/zero/partitioned_param_coordinator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)   112178 2023-04-13 15:29:56.000000 deepspeed-0.9.1/deepspeed/runtime/zero/stage3.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)   110183 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/zero/stage_1_and_2.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2727 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/zero/test.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11727 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/zero/tiling.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2931 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/runtime/zero/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.863510 deepspeed-0.9.1/deepspeed/utils/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      717 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6096 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/comms_logging.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4370 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/debug.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      144 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/exceptions.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15606 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/groups.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3004 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/init_on_device.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4375 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/logging.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2041 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/mixed_precision_linkage.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      499 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/nvtx.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7997 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/tensor_fragment.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8765 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/timer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      200 2023-04-11 17:18:49.000000 deepspeed-0.9.1/deepspeed/utils/types.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    24043 2023-04-21 00:47:36.000000 deepspeed-0.9.1/deepspeed/utils/zero_to_fp32.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.553510 deepspeed-0.9.1/deepspeed.egg-info/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27276 2023-04-21 00:48:04.000000 deepspeed-0.9.1/deepspeed.egg-info/PKG-INFO
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20079 2023-04-21 00:48:05.000000 deepspeed-0.9.1/deepspeed.egg-info/SOURCES.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        1 2023-04-21 00:48:04.000000 deepspeed-0.9.1/deepspeed.egg-info/dependency_links.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       85 2023-04-21 00:48:04.000000 deepspeed-0.9.1/deepspeed.egg-info/entry_points.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1124 2023-04-21 00:48:04.000000 deepspeed-0.9.1/deepspeed.egg-info/requires.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       10 2023-04-21 00:48:04.000000 deepspeed-0.9.1/deepspeed.egg-info/top_level.txt
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.873510 deepspeed-0.9.1/op_builder/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/all_ops.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/async_io.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28628 2023-04-21 00:47:36.000000 deepspeed-0.9.1/op_builder/builder.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/cpu_adagrad.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/cpu_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/fused_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/fused_lamb.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/quantizer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/random_ltd.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.1/op_builder/sparse_attn.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/spatial_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/stochastic_transformer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/transformer.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2622 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/transformer_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.1/op_builder/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-04-21 00:48:05.873510 deepspeed-0.9.1/requirements/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        7 2022-07-06 20:47:37.000000 deepspeed-0.9.1/requirements/requirements-1bit-mpi.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       23 2022-07-06 20:47:37.000000 deepspeed-0.9.1/requirements/requirements-autotuning-ml.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        9 2022-07-06 20:47:37.000000 deepspeed-0.9.1/requirements/requirements-autotuning.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      232 2022-11-14 17:49:34.000000 deepspeed-0.9.1/requirements/requirements-dev.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       72 2023-02-28 00:54:52.000000 deepspeed-0.9.1/requirements/requirements-inf.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       97 2023-04-21 00:47:36.000000 deepspeed-0.9.1/requirements/requirements-readthedocs.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       36 2023-04-11 17:18:49.000000 deepspeed-0.9.1/requirements/requirements-sd.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       14 2022-07-06 20:47:37.000000 deepspeed-0.9.1/requirements/requirements-sparse_attn.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       78 2023-04-21 00:47:36.000000 deepspeed-0.9.1/requirements/requirements.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      148 2023-04-21 00:48:05.873510 deepspeed-0.9.1/setup.cfg
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11318 2023-04-21 00:47:36.000000 deepspeed-0.9.1/setup.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        6 2023-04-13 15:30:43.000000 deepspeed-0.9.1/version.txt
```

### Comparing `deepspeed-0.9.0/LICENSE` & `deepspeed-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/PKG-INFO` & `deepspeed-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepspeed
-Version: 0.9.0
+Version: 0.9.1
 Summary: DeepSpeed library
 Home-page: http://deepspeed.ai
 Author: DeepSpeed Team
 Author-email: deepspeed-info@microsoft.com
 License: MIT
 Project-URL: Documentation, https://deepspeed.readthedocs.io
 Project-URL: Source, https://github.com/microsoft/DeepSpeed
@@ -121,15 +121,15 @@
 
 DeepSpeed has been integrated with several different popular open-source DL frameworks such as:
 
 |                                                                                                | Documentation                                |
 | ---------------------------------------------------------------------------------------------- | -------------------------------------------- |
 <img src="docs/assets/images/transformers-light.png#gh-light-mode-only" width="250px"><img src="docs/assets/images/transformers-dark.png#gh-dark-mode-only" width="250px"> | [Transformers with DeepSpeed](https://huggingface.co/docs/transformers/main/main_classes/deepspeed) |
 | <img src="docs/assets/images/accelerate-light.png#gh-light-mode-only" width="250px"><img src="docs/assets/images/accelerate-dark.png#gh-dark-mode-only" width="250px"> | [Accelerate with DeepSpeed](https://huggingface.co/docs/accelerate/usage_guides/deepspeed) |
-| <img src="docs/assets/images/lightning-light.svg#gh-light-mode-only" width="200px"><img src="docs/assets/images/lightning-dark.svg#gh-dark-mode-only" width="200px"> | [Lightning with DeepSpeed](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.strategies.DeepSpeedStrategy.html) |
+| <img src="docs/assets/images/lightning-light.svg#gh-light-mode-only" width="200px"><img src="docs/assets/images/lightning-dark.svg#gh-dark-mode-only" width="200px"> | [Lightning with DeepSpeed](https://lightning.ai/docs/pytorch/stable/advanced/model_parallel.html#deepspeed) |
 | <img src="docs/assets/images/mosaicml.svg" width="200px"> | [MosaicML with DeepSpeed](https://docs.mosaicml.com/en/latest/trainer/using_the_trainer.html?highlight=deepspeed#deepspeed-integration) |
 | <img src="docs/assets/images/determined.svg" width="225px"> | [Determined with DeepSpeed](https://docs.determined.ai/latest/training/apis-howto/deepspeed/overview.html) |
 
 ---
 
 # Build Pipeline Status
 
@@ -202,15 +202,20 @@
 | [Tutorials](https://www.deepspeed.ai/tutorials/)                                               |  Tutorials                                   |
 | [Blogs](https://www.deepspeed.ai/posts/)                                                       |  Blogs                                   |
 
 
 # Contributing
 DeepSpeed welcomes your contributions! Please see our
 [contributing](CONTRIBUTING.md) guide for more details on formatting, testing,
-etc.
+etc.<br/>
+Thanks so much to all of our amazing contributors!
+
+<a href="https://github.com/microsoft/DeepSpeed/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=microsoft/DeepSpeed&r="  width="800px"/>
+</a>
 
 ## Contributor License Agreement
 This project welcomes contributions and suggestions. Most contributions require you to
 agree to a Contributor License Agreement (CLA) declaring that you have the right to, and
 actually do, grant us the rights to use your contribution. For details, visit
 https://cla.opensource.microsoft.com.
```

### Comparing `deepspeed-0.9.0/README.md` & `deepspeed-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 DeepSpeed has been integrated with several different popular open-source DL frameworks such as:
 
 |                                                                                                | Documentation                                |
 | ---------------------------------------------------------------------------------------------- | -------------------------------------------- |
 <img src="docs/assets/images/transformers-light.png#gh-light-mode-only" width="250px"><img src="docs/assets/images/transformers-dark.png#gh-dark-mode-only" width="250px"> | [Transformers with DeepSpeed](https://huggingface.co/docs/transformers/main/main_classes/deepspeed) |
 | <img src="docs/assets/images/accelerate-light.png#gh-light-mode-only" width="250px"><img src="docs/assets/images/accelerate-dark.png#gh-dark-mode-only" width="250px"> | [Accelerate with DeepSpeed](https://huggingface.co/docs/accelerate/usage_guides/deepspeed) |
-| <img src="docs/assets/images/lightning-light.svg#gh-light-mode-only" width="200px"><img src="docs/assets/images/lightning-dark.svg#gh-dark-mode-only" width="200px"> | [Lightning with DeepSpeed](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.strategies.DeepSpeedStrategy.html) |
+| <img src="docs/assets/images/lightning-light.svg#gh-light-mode-only" width="200px"><img src="docs/assets/images/lightning-dark.svg#gh-dark-mode-only" width="200px"> | [Lightning with DeepSpeed](https://lightning.ai/docs/pytorch/stable/advanced/model_parallel.html#deepspeed) |
 | <img src="docs/assets/images/mosaicml.svg" width="200px"> | [MosaicML with DeepSpeed](https://docs.mosaicml.com/en/latest/trainer/using_the_trainer.html?highlight=deepspeed#deepspeed-integration) |
 | <img src="docs/assets/images/determined.svg" width="225px"> | [Determined with DeepSpeed](https://docs.determined.ai/latest/training/apis-howto/deepspeed/overview.html) |
 
 ---
 
 # Build Pipeline Status
 
@@ -173,15 +173,20 @@
 | [Tutorials](https://www.deepspeed.ai/tutorials/)                                               |  Tutorials                                   |
 | [Blogs](https://www.deepspeed.ai/posts/)                                                       |  Blogs                                   |
 
 
 # Contributing
 DeepSpeed welcomes your contributions! Please see our
 [contributing](CONTRIBUTING.md) guide for more details on formatting, testing,
-etc.
+etc.<br/>
+Thanks so much to all of our amazing contributors!
+
+<a href="https://github.com/microsoft/DeepSpeed/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=microsoft/DeepSpeed&r="  width="800px"/>
+</a>
 
 ## Contributor License Agreement
 This project welcomes contributions and suggestions. Most contributions require you to
 agree to a Contributor License Agreement (CLA) declaring that you have the right to, and
 actually do, grant us the rights to use your contribution. For details, visit
 https://cla.opensource.microsoft.com.
```

### Comparing `deepspeed-0.9.0/accelerator/abstract_accelerator.py` & `deepspeed-0.9.1/accelerator/abstract_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/accelerator/cuda_accelerator.py` & `deepspeed-0.9.1/accelerator/cuda_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/accelerator/real_accelerator.py` & `deepspeed-0.9.1/accelerator/real_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/bin/ds_bench` & `deepspeed-0.9.1/bin/ds_bench`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/bin/ds_elastic` & `deepspeed-0.9.1/bin/ds_elastic`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/bin/ds_ssh` & `deepspeed-0.9.1/bin/ds_ssh`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/adagrad/cpu_adagrad.cpp` & `deepspeed-0.9.1/csrc/adagrad/cpu_adagrad.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/adam/cpu_adam.cpp` & `deepspeed-0.9.1/csrc/adam/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/adam/fused_adam_frontend.cpp` & `deepspeed-0.9.1/csrc/adam/fused_adam_frontend.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/adam/multi_tensor_adam.cu` & `deepspeed-0.9.1/csrc/adam/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/adam/multi_tensor_apply.cuh` & `deepspeed-0.9.1/csrc/adam/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/common/deepspeed_aio_common.cpp` & `deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_common.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/common/deepspeed_aio_common.h` & `deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_common.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/common/deepspeed_aio_types.cpp` & `deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_types.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/common/deepspeed_aio_types.h` & `deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_types.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/common/deepspeed_aio_utils.cpp` & `deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/common/deepspeed_aio_utils.h` & `deepspeed-0.9.1/csrc/aio/common/deepspeed_aio_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_aio_thread.cpp` & `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_aio_thread.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_aio_thread.h` & `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_aio_thread.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_pin_tensor.cpp` & `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_pin_tensor.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_pin_tensor.h` & `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_pin_tensor.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_py_aio.cpp` & `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_py_aio.h` & `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_aio.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp` & `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_py_aio_handle.h` & `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_aio_handle.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_py_copy.cpp` & `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_copy.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/py_lib/deepspeed_py_copy.h` & `deepspeed-0.9.1/csrc/aio/py_lib/deepspeed_py_copy.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/aio/py_lib/py_ds_aio.cpp` & `deepspeed-0.9.1/csrc/aio/py_lib/py_ds_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/common/custom_cuda_kernel.cu` & `deepspeed-0.9.1/csrc/common/custom_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/StopWatch.h` & `deepspeed-0.9.1/csrc/includes/StopWatch.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/Timer.h` & `deepspeed-0.9.1/csrc/includes/Timer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/context.h` & `deepspeed-0.9.1/csrc/includes/context.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/conversion_utils.h` & `deepspeed-0.9.1/csrc/includes/conversion_utils.h`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,20 @@
 }
 #endif
 
 /*********************  To Half Conversions *********************/
 template <>
 DS_D_INLINE __half to(double val)
 {
+#ifdef __HIP_PLATFORM_HCC__
+    float val_f = __double2float_rn(val);
+    return __float2half(val_f);
+#else
     return __double2half(val);
+#endif
 }
 template <>
 DS_D_INLINE __half to(float val)
 {
     return __float2half(val);
 }
 template <>
```

### Comparing `deepspeed-0.9.0/csrc/includes/cpu_adagrad.h` & `deepspeed-0.9.1/csrc/includes/cpu_adagrad.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/cpu_adam.h` & `deepspeed-0.9.1/csrc/includes/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/cublas_wrappers.h` & `deepspeed-0.9.1/csrc/includes/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/custom_cuda_layers.h` & `deepspeed-0.9.1/csrc/includes/custom_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/dequantization_utils.h` & `deepspeed-0.9.1/csrc/includes/dequantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/dropout.h` & `deepspeed-0.9.1/csrc/includes/dropout.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/ds_kernel_utils.h` & `deepspeed-0.9.1/csrc/includes/ds_kernel_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/ds_transformer_cuda.h` & `deepspeed-0.9.1/csrc/includes/ds_transformer_cuda.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/feed_forward.h` & `deepspeed-0.9.1/csrc/includes/feed_forward.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/gelu.h` & `deepspeed-0.9.1/csrc/includes/gelu.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/gemm_test.h` & `deepspeed-0.9.1/csrc/includes/gemm_test.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/general_kernels.h` & `deepspeed-0.9.1/csrc/includes/general_kernels.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/memory_access_utils.h` & `deepspeed-0.9.1/csrc/includes/memory_access_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/normalize_layer.h` & `deepspeed-0.9.1/csrc/includes/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/quantization.h` & `deepspeed-0.9.1/csrc/includes/quantization.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/quantization_utils.h` & `deepspeed-0.9.1/csrc/includes/quantization_utils.h`

 * *Files 2% similar despite different names*

```diff
@@ -98,34 +98,34 @@
     float offset;
 
     DS_D_INLINE Params(float max, float min)
     {
         if (max == min) {
             scale = 1.0;
         } else {
-            scale = (1 << numBits) / (max - min);
+            scale = ((1 << numBits)) / (max - min);
         }
-        offset = -(1 << (numBits - 1)) - (min * scale);
+        offset = (max + min) / 2;
     }
 
     DS_D_INLINE int8_t quantize(__half val)
     {
         constexpr int32_t q_min = -(1 << (numBits - 1));
         constexpr int32_t q_max = (1 << (numBits - 1)) - 1;
 
-        float val_f = conversion::to<float>(val) * scale + offset;
+        float val_f = (conversion::to<float>(val) - offset) * scale;
         int32_t data_i32 = conversion::to<int32_t>(val_f);
         data_i32 = min(max(data_i32, q_min), q_max);
         return (int8_t)data_i32;
     }
 
     template <typename T>
     DS_D_INLINE T dequantize(int8_t val)
     {
-        const float val_deq_f = conversion::to<float>(val) * scale + offset;
+        const float val_deq_f = ((conversion::to<float>(val)) * scale) + offset;
         return conversion::to<__half>(val_deq_f);
     }
 
     DS_D_INLINE void store(float* params, int group_index)
     {
         // Codegen should turn this into stg.64
         const float store_scale = 1 / scale;
```

### Comparing `deepspeed-0.9.0/csrc/includes/reduction_utils.h` & `deepspeed-0.9.1/csrc/includes/reduction_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/simd.h` & `deepspeed-0.9.1/csrc/includes/simd.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/softmax.h` & `deepspeed-0.9.1/csrc/includes/softmax.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/strided_batch_gemm.h` & `deepspeed-0.9.1/csrc/includes/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/includes/type_shim.h` & `deepspeed-0.9.1/csrc/includes/type_shim.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/lamb/fused_lamb_cuda.cpp` & `deepspeed-0.9.1/csrc/lamb/fused_lamb_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/lamb/fused_lamb_cuda_kernel.cu` & `deepspeed-0.9.1/csrc/lamb/fused_lamb_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/quantization/dequantize.cu` & `deepspeed-0.9.1/csrc/quantization/dequantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/quantization/fake_quantizer.cu` & `deepspeed-0.9.1/csrc/quantization/fake_quantizer.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/quantization/pt_binding.cpp` & `deepspeed-0.9.1/csrc/quantization/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/quantization/quantize.cu` & `deepspeed-0.9.1/csrc/quantization/quantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/random_ltd/gather_scatter.cu` & `deepspeed-0.9.1/csrc/random_ltd/gather_scatter.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/random_ltd/pt_binding.cpp` & `deepspeed-0.9.1/csrc/random_ltd/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/random_ltd/slice_attn_masks.cu` & `deepspeed-0.9.1/csrc/random_ltd/slice_attn_masks.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/random_ltd/token_sort.cu` & `deepspeed-0.9.1/csrc/random_ltd/token_sort.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/sparse_attention/utils.cpp` & `deepspeed-0.9.1/csrc/sparse_attention/utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/spatial/csrc/opt_bias_add.cu` & `deepspeed-0.9.1/csrc/spatial/csrc/opt_bias_add.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/spatial/csrc/pt_binding.cpp` & `deepspeed-0.9.1/csrc/spatial/csrc/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/spatial/includes/spatial_cuda_layers.h` & `deepspeed-0.9.1/csrc/spatial/includes/spatial_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/cublas_wrappers.cu` & `deepspeed-0.9.1/csrc/transformer/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/dropout_kernels.cu` & `deepspeed-0.9.1/csrc/transformer/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/ds_transformer_cuda.cpp` & `deepspeed-0.9.1/csrc/transformer/ds_transformer_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/gelu_kernels.cu` & `deepspeed-0.9.1/csrc/transformer/gelu_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/general_kernels.cu` & `deepspeed-0.9.1/csrc/transformer/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu` & `deepspeed-0.9.1/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/inference/csrc/dequantize.cu` & `deepspeed-0.9.1/csrc/transformer/inference/csrc/dequantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/inference/csrc/gelu.cu` & `deepspeed-0.9.1/csrc/transformer/inference/csrc/gelu.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/inference/csrc/layer_norm.cu` & `deepspeed-0.9.1/csrc/transformer/inference/csrc/layer_norm.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/inference/csrc/pt_binding.cpp` & `deepspeed-0.9.1/csrc/transformer/inference/csrc/pt_binding.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -458,17 +458,17 @@
                        .dtype(query_key_value.options().dtype())
                        .layout(at::kStrided)
                        .device(at::kCUDA)
                        .requires_grad(false);
 
     T* workspace = (T*)InferenceContext::Instance().GetWorkSpace();
     size_t buf_size = bsz * seq_len * hidden_dim;
-    auto output = torch::from_blob(workspace + 3 * buf_size, {bsz, seq_len, hidden_dim}, options);
+    auto output = torch::from_blob(workspace + 4 * buf_size, {bsz, seq_len, hidden_dim}, options);
 
-    auto query_cont = workspace + 4 * buf_size;
+    auto query_cont = workspace + 5 * buf_size;
     size_t offset =
         10 * (hidden_dim * bsz * InferenceContext::Instance().GetMaxTokenLenght()) +
         layer_id * 2 * bsz * InferenceContext::Instance().GetMaxTokenLenght() * hidden_dim;
     unsigned all_tokens = soft_len;
     auto kv_cache = workspace + offset + (hidden_dim / heads) * (is_prompt ? 0 : soft_len - 1);
     size_t value_offset = bsz * InferenceContext::Instance().GetMaxTokenLenght() * hidden_dim;
```

### Comparing `deepspeed-0.9.0/csrc/transformer/inference/csrc/relu.cu` & `deepspeed-0.9.1/csrc/transformer/inference/csrc/relu.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/inference/csrc/softmax.cu` & `deepspeed-0.9.1/csrc/transformer/inference/csrc/softmax.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/inference/csrc/transform.cu` & `deepspeed-0.9.1/csrc/transformer/inference/csrc/transform.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/inference/includes/inference_context.h` & `deepspeed-0.9.1/csrc/transformer/inference/includes/inference_context.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/inference/includes/inference_cublas_wrappers.h` & `deepspeed-0.9.1/csrc/transformer/inference/includes/inference_cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/inference/includes/inference_cuda_layers.h` & `deepspeed-0.9.1/csrc/transformer/inference/includes/inference_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/normalize_kernels.cu` & `deepspeed-0.9.1/csrc/transformer/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/softmax_kernels.cu` & `deepspeed-0.9.1/csrc/transformer/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/transformer/transform_kernels.cu` & `deepspeed-0.9.1/csrc/transformer/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/csrc/utils/flatten_unflatten.cpp` & `deepspeed-0.9.1/csrc/utils/flatten_unflatten.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/__init__.py` & `deepspeed-0.9.1/deepspeed/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler
 from packaging import version as pkg_version
 
 from . import ops
 from . import module_inject
 
+from .accelerator import get_accelerator
 from .runtime.engine import DeepSpeedEngine, DeepSpeedOptimizerCallable, DeepSpeedSchedulerCallable
 from .runtime.engine import ADAM_OPTIMIZER, LAMB_OPTIMIZER
 from .runtime.hybrid_engine import DeepSpeedHybridEngine
 from .runtime.pipe.engine import PipelineEngine
 from .inference.engine import InferenceEngine
 from .inference.config import DeepSpeedInferenceConfig
 from .runtime.lr_schedules import add_tuning_arguments
@@ -46,14 +47,17 @@
 
 # Export version information
 __version__ = version
 __version_major__, __version_minor__, __version_patch__ = _parse_version(__version__)
 __git_hash__ = git_hash
 __git_branch__ = git_branch
 
+# Set to torch's distributed package or deepspeed.comm based inside DeepSpeedEngine init
+dist = None
+
 
 def initialize(args=None,
                model: torch.nn.Module = None,
                optimizer: Optional[Union[Optimizer, DeepSpeedOptimizerCallable]] = None,
                model_parameters: Optional[torch.nn.Module] = None,
                training_data: Optional[torch.utils.data.Dataset] = None,
                lr_scheduler: Optional[Union[_LRScheduler, DeepSpeedSchedulerCallable]] = None,
@@ -115,14 +119,19 @@
              ranks=[0])
 
     # Disable zero.Init context if it's currently enabled
     zero.partition_parameters.shutdown_init_context()
 
     assert model is not None, "deepspeed.initialize requires a model"
 
+    global dist
+    from deepspeed import comm as dist
+    dist_backend = get_accelerator().communication_backend_name()
+    dist.init_distributed(dist_backend=dist_backend, dist_init_required=dist_init_required)
+
     # Set config using config_params for backwards compat
     if config is None and config_params is not None:
         config = config_params
 
     # Check for deepscale_config for backwards compat
     if hasattr(args, "deepscale_config") and args.deepscale_config is not None:
         logger.warning("************ --deepscale_config is deprecated, please use --deepspeed_config ************")
```

### Comparing `deepspeed-0.9.0/deepspeed/accelerator/abstract_accelerator.py` & `deepspeed-0.9.1/deepspeed/accelerator/abstract_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/accelerator/cuda_accelerator.py` & `deepspeed-0.9.1/deepspeed/accelerator/cuda_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/accelerator/real_accelerator.py` & `deepspeed-0.9.1/deepspeed/accelerator/real_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/autotuning/autotuner.py` & `deepspeed-0.9.1/deepspeed/autotuning/autotuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
         self.results_dir = self.autotuning_config.results_dir
         if self.autotuning_config.overwrite and os.path.exists(self.results_dir):
             shutil.rmtree(self.results_dir, ignore_errors=True)
         if not os.path.exists(self.results_dir):
             try:
                 os.makedirs(self.results_dir, exist_ok=True)
-                logger.info(f"Created autotuning resutls directory: {self.exps_dir}")
+                logger.info(f"Created autotuning results directory: {self.exps_dir}")
             except:
                 logger.error(
                     f"Failed to create {self.results_dir}, please check `results_dir` in the autotuning config file is accessible by all the nodes in the job."
                 )
                 exit(-1)
 
         # set the active resource for the autotuner resource manager
```

### Comparing `deepspeed-0.9.0/deepspeed/autotuning/config.py` & `deepspeed-0.9.1/deepspeed/autotuning/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/autotuning/constants.py` & `deepspeed-0.9.1/deepspeed/autotuning/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/autotuning/scheduler.py` & `deepspeed-0.9.1/deepspeed/autotuning/scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/autotuning/tuner/base_tuner.py` & `deepspeed-0.9.1/deepspeed/autotuning/tuner/base_tuner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/autotuning/tuner/cost_model.py` & `deepspeed-0.9.1/deepspeed/autotuning/tuner/cost_model.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/autotuning/tuner/index_based_tuner.py` & `deepspeed-0.9.1/deepspeed/autotuning/tuner/index_based_tuner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/autotuning/tuner/model_based_tuner.py` & `deepspeed-0.9.1/deepspeed/autotuning/tuner/model_based_tuner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/autotuning/tuner/utils.py` & `deepspeed-0.9.1/deepspeed/autotuning/tuner/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/autotuning/utils.py` & `deepspeed-0.9.1/deepspeed/autotuning/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/checkpoint/__init__.py` & `deepspeed-0.9.1/deepspeed/checkpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/checkpoint/constants.py` & `deepspeed-0.9.1/deepspeed/checkpoint/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 #########################################
 # Module checkpoint keys
 #########################################
 PARAM = 'param'
 PARAM_SHAPES = 'param_shapes'
 BUFFER_NAMES = 'buffer_names'
+FROZEN_PARAM_SHAPES = 'frozen_param_shapes'
+FROZEN_PARAM_FRAGMENTS = 'frozen_param_fragments'
 
 #########################################
 # Checkpoint naming constants
 #########################################
 MODEL_FILE_PREFIX = 'mp_rank_'
 ZERO_FILE_PREFIX = 'zero_pp_rank_'
 OPTIM_FILE_SUFFIX = '_optim_states.pt'
```

### Comparing `deepspeed-0.9.0/deepspeed/checkpoint/deepspeed_checkpoint.py` & `deepspeed-0.9.1/deepspeed/checkpoint/deepspeed_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/checkpoint/reshape_3d_utils.py` & `deepspeed-0.9.1/deepspeed/checkpoint/reshape_3d_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/checkpoint/reshape_meg_2d.py` & `deepspeed-0.9.1/deepspeed/checkpoint/reshape_meg_2d.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/checkpoint/reshape_utils.py` & `deepspeed-0.9.1/deepspeed/checkpoint/reshape_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/checkpoint/universal_checkpoint.py` & `deepspeed-0.9.1/deepspeed/checkpoint/universal_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/checkpoint/utils.py` & `deepspeed-0.9.1/deepspeed/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/checkpoint/zero_checkpoint.py` & `deepspeed-0.9.1/deepspeed/checkpoint/zero_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/comm/backend.py` & `deepspeed-0.9.1/deepspeed/comm/backend.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/comm/comm.py` & `deepspeed-0.9.1/deepspeed/comm/comm.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/comm/config.py` & `deepspeed-0.9.1/deepspeed/comm/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/comm/constants.py` & `deepspeed-0.9.1/deepspeed/comm/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/comm/torch.py` & `deepspeed-0.9.1/deepspeed/comm/torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
         is initialized, standard torch.distributed.* can be used directly
         so no need to wrap all the functions. We can keep adding wrappers as
         needed.
     """
 
     def __init__(self, backend, timeout, init_method, rank=-1, world_size=-1, name='torch'):
         super(TorchBackend, self).__init__()
-        self.torch_version_before_18 = older_torch()
         self.all_gather_function = self.get_all_gather_function()
         self.reduce_scatter_function = self.get_reduce_scatter_function()
         self.initialized = True
         self.name = name
         # Future functionality to support ds.initialize() on a single GPU
         # The idea is to fake that dist backend is initialized even when
         # it is not so we can run on a single GPU without doing any init_process_group
```

### Comparing `deepspeed-0.9.0/deepspeed/comm/utils.py` & `deepspeed-0.9.1/deepspeed/comm/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,17 @@
 # Copyright (c) Microsoft Corporation.
 # SPDX-License-Identifier: Apache-2.0
 
 # DeepSpeed Team
 
 import os
-import torch
 import inspect
 from deepspeed.utils import get_caller_func
 
 
-def older_torch():
-    '''
-        Helper to lookup torch version. For versions less than 1.8, torch.dist
-        used torch.distributed.group.WORLD as the default group argument instead of None.
-        See more details at: https://github.com/pytorch/pytorch/pull/48767
-    '''
-    TORCH_MAJOR = int(torch.__version__.split('.')[0])
-    TORCH_MINOR = int(torch.__version__.split('.')[1])
-    if TORCH_MAJOR == 1 and TORCH_MINOR < 8:
-        return True
-    else:
-        return False
-
-
 def get_local_rank_from_launcher():
 
     # DeepSpeed launcher will set it so get from there
     rank = os.environ.get('LOCAL_RANK')
 
     if rank is None:
         rank = os.environ.get('OMPI_COMM_WORLD_LOCAL_RANK')
```

### Comparing `deepspeed-0.9.0/deepspeed/compression/basic_layer.py` & `deepspeed-0.9.1/deepspeed/compression/basic_layer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/compression/compress.py` & `deepspeed-0.9.1/deepspeed/compression/compress.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/compression/config.py` & `deepspeed-0.9.1/deepspeed/compression/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/compression/constants.py` & `deepspeed-0.9.1/deepspeed/compression/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/compression/helper.py` & `deepspeed-0.9.1/deepspeed/compression/helper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/compression/scheduler.py` & `deepspeed-0.9.1/deepspeed/compression/scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/compression/utils.py` & `deepspeed-0.9.1/deepspeed/compression/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/constants.py` & `deepspeed-0.9.1/deepspeed/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/elasticity/config.py` & `deepspeed-0.9.1/deepspeed/elasticity/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/elasticity/constants.py` & `deepspeed-0.9.1/deepspeed/elasticity/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/elasticity/elastic_agent.py` & `deepspeed-0.9.1/deepspeed/elasticity/elastic_agent.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/elasticity/elasticity.py` & `deepspeed-0.9.1/deepspeed/elasticity/elasticity.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/env_report.py` & `deepspeed-0.9.1/deepspeed/env_report.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/git_version_info.py` & `deepspeed-0.9.1/deepspeed/git_version_info.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/git_version_info_installed.py` & `deepspeed-0.9.1/deepspeed/git_version_info_installed.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-version='0.9.0'
+version='0.9.1'
 git_hash='unknown'
 git_branch='unknown'
 installed_ops={'async_io': False, 'cpu_adagrad': False, 'cpu_adam': False, 'fused_adam': False, 'fused_lamb': False, 'quantizer': False, 'random_ltd': False, 'sparse_attn': False, 'spatial_inference': False, 'transformer': False, 'stochastic_transformer': False, 'transformer_inference': False, 'utils': False}
 compatible_ops={'async_io': False, 'cpu_adagrad': True, 'cpu_adam': True, 'fused_adam': True, 'fused_lamb': True, 'quantizer': True, 'random_ltd': True, 'sparse_attn': False, 'spatial_inference': True, 'transformer': True, 'stochastic_transformer': True, 'transformer_inference': True, 'utils': True}
 torch_info={'version': '1.9', 'bf16_support': False, 'cuda_version': '10.2', 'nccl_version': '2.7', 'hip_version': '0.0'}
```

### Comparing `deepspeed-0.9.0/deepspeed/inference/config.py` & `deepspeed-0.9.1/deepspeed/inference/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/inference/engine.py` & `deepspeed-0.9.1/deepspeed/inference/engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/launcher/launch.py` & `deepspeed-0.9.1/deepspeed/launcher/launch.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/launcher/multinode_runner.py` & `deepspeed-0.9.1/deepspeed/launcher/multinode_runner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/launcher/runner.py` & `deepspeed-0.9.1/deepspeed/launcher/runner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/model_implementations/diffusers/unet.py` & `deepspeed-0.9.1/deepspeed/model_implementations/diffusers/unet.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/model_implementations/diffusers/vae.py` & `deepspeed-0.9.1/deepspeed/model_implementations/diffusers/vae.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/model_implementations/features/cuda_graph.py` & `deepspeed-0.9.1/deepspeed/model_implementations/features/cuda_graph.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/model_implementations/transformers/clip_encoder.py` & `deepspeed-0.9.1/deepspeed/model_implementations/transformers/clip_encoder.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/model_implementations/transformers/ds_bert.py` & `deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_bert.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/model_implementations/transformers/ds_bloom.py` & `deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_bloom.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/model_implementations/transformers/ds_gpt.py` & `deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_gpt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/model_implementations/transformers/ds_megatron_gpt.py` & `deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_megatron_gpt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/model_implementations/transformers/ds_opt.py` & `deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_opt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/model_implementations/transformers/ds_transformer.py` & `deepspeed-0.9.1/deepspeed/model_implementations/transformers/ds_transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/auto_tp.py` & `deepspeed-0.9.1/deepspeed/module_inject/auto_tp.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/__init__.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/base.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/base.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/base_moe.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/base_moe.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/bert.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/bert.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/bloom.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/bloom.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/clip.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/clip.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/distil_bert.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/distil_bert.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/features/megatron.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/features/megatron.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/features/meta_tensor.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/features/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/gpt2.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/gpt2.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/gptj.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/gptj.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/gptneo.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/gptneo.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/gptneox.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/gptneox.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/megatron_gpt.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/megatron_gpt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/megatron_gpt_moe.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/megatron_gpt_moe.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/opt.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/opt.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,26 +68,34 @@
                        prefix + param_names[i])
 
 
 class HFOPTLayerPolicy(TransformerPolicy):
     _orig_layer_class = None
 
     def __init__(self, client_module, inference=True, use_load_prefix=True):
-        super().__init__(inference,
-                         linear_layer=True,
-                         mlp_act_func_type=ActivationFuncType.ReLU,
-                         pre_attn_norm=True,
-                         use_load_prefix=use_load_prefix)
+        super().__init__(inference, linear_layer=True, pre_attn_norm=True, use_load_prefix=use_load_prefix)
         self.client_module = client_module
         try:
             import transformers
             HFOPTLayerPolicy._orig_layer_class = transformers.models.opt.modeling_opt.OPTDecoderLayer
         except:
             HFOPTLayerPolicy._orig_layer_class = None
 
+        if hasattr(TransformerPolicy, "hf_model_config") and hasattr(TransformerPolicy.hf_model_config,
+                                                                     "activation_function"):
+            if TransformerPolicy.hf_model_config.activation_function == "relu":
+                self.mlp_act_func_type == ActivationFuncType.ReLU
+            elif TransformerPolicy.hf_model_config.activation_function in ["gelu", "gelu_new"]:
+                self.mlp_act_func_type == ActivationFuncType.GELU
+            else:
+                raise ValueError("Unsupported activation function: {}".format(
+                    TransformerPolicy.hf_model_config.activation_function))
+        else:
+            self.mlp_act_func_type == ActivationFuncType.ReLU  # default
+
     def get_hidden_heads(self):
         return self.client_module.self_attn.embed_dim, \
                 self.client_module.self_attn.num_heads, \
                 self.client_module.self_attn_layer_norm.eps
 
     def get_q_k_v(self):
         return self.client_module.self_attn.q_proj.weight, \
```

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/unet.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/unet.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/containers/vae.py` & `deepspeed-0.9.1/deepspeed/module_inject/containers/vae.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/inject.py` & `deepspeed-0.9.1/deepspeed/module_inject/inject.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/layers.py` & `deepspeed-0.9.1/deepspeed/module_inject/layers.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/load_checkpoint.py` & `deepspeed-0.9.1/deepspeed/module_inject/load_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/module_quantize.py` & `deepspeed-0.9.1/deepspeed/module_inject/module_quantize.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/policy.py` & `deepspeed-0.9.1/deepspeed/module_inject/policy.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/replace_module.py` & `deepspeed-0.9.1/deepspeed/module_inject/replace_module.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/replace_policy.py` & `deepspeed-0.9.1/deepspeed/module_inject/replace_policy.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/module_inject/utils.py` & `deepspeed-0.9.1/deepspeed/module_inject/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/moe/experts.py` & `deepspeed-0.9.1/deepspeed/moe/experts.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/moe/layer.py` & `deepspeed-0.9.1/deepspeed/moe/layer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/moe/mappings.py` & `deepspeed-0.9.1/deepspeed/moe/mappings.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/moe/sharded_moe.py` & `deepspeed-0.9.1/deepspeed/moe/sharded_moe.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/moe/utils.py` & `deepspeed-0.9.1/deepspeed/moe/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/monitor/config.py` & `deepspeed-0.9.1/deepspeed/monitor/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/monitor/csv_monitor.py` & `deepspeed-0.9.1/deepspeed/monitor/csv_monitor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/monitor/monitor.py` & `deepspeed-0.9.1/deepspeed/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/monitor/tensorboard.py` & `deepspeed-0.9.1/deepspeed/monitor/tensorboard.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/monitor/utils.py` & `deepspeed-0.9.1/deepspeed/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/monitor/wandb.py` & `deepspeed-0.9.1/deepspeed/monitor/wandb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/nebula/config.py` & `deepspeed-0.9.1/deepspeed/nebula/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/nebula/constants.py` & `deepspeed-0.9.1/deepspeed/nebula/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/adagrad/cpu_adagrad.py` & `deepspeed-0.9.1/deepspeed/ops/adagrad/cpu_adagrad.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/adam/cpu_adam.py` & `deepspeed-0.9.1/deepspeed/ops/adam/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/adam/fused_adam.py` & `deepspeed-0.9.1/deepspeed/ops/adam/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/adam/cpu_adam.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/adam/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/adam/multi_tensor_adam.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/adam/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh` & `deepspeed-0.9.1/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/common/custom_cuda_kernel.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/common/custom_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/StopWatch.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/StopWatch.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/Timer.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/Timer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/context.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/context.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/conversion_utils.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/conversion_utils.h`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,20 @@
 }
 #endif
 
 /*********************  To Half Conversions *********************/
 template <>
 DS_D_INLINE __half to(double val)
 {
+#ifdef __HIP_PLATFORM_HCC__
+    float val_f = __double2float_rn(val);
+    return __float2half(val_f);
+#else
     return __double2half(val);
+#endif
 }
 template <>
 DS_D_INLINE __half to(float val)
 {
     return __float2half(val);
 }
 template <>
```

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/cpu_adagrad.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/cpu_adagrad.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/cpu_adam.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/cublas_wrappers.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/custom_cuda_layers.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/custom_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/dequantization_utils.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/dequantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/dropout.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/dropout.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/ds_kernel_utils.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/ds_kernel_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/ds_transformer_cuda.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/ds_transformer_cuda.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/feed_forward.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/feed_forward.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/gelu.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/gelu.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/gemm_test.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/gemm_test.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/general_kernels.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/general_kernels.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/memory_access_utils.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/memory_access_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/normalize_layer.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/quantization.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/quantization.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/quantization_utils.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/quantization_utils.h`

 * *Files 2% similar despite different names*

```diff
@@ -98,34 +98,34 @@
     float offset;
 
     DS_D_INLINE Params(float max, float min)
     {
         if (max == min) {
             scale = 1.0;
         } else {
-            scale = (1 << numBits) / (max - min);
+            scale = ((1 << numBits)) / (max - min);
         }
-        offset = -(1 << (numBits - 1)) - (min * scale);
+        offset = (max + min) / 2;
     }
 
     DS_D_INLINE int8_t quantize(__half val)
     {
         constexpr int32_t q_min = -(1 << (numBits - 1));
         constexpr int32_t q_max = (1 << (numBits - 1)) - 1;
 
-        float val_f = conversion::to<float>(val) * scale + offset;
+        float val_f = (conversion::to<float>(val) - offset) * scale;
         int32_t data_i32 = conversion::to<int32_t>(val_f);
         data_i32 = min(max(data_i32, q_min), q_max);
         return (int8_t)data_i32;
     }
 
     template <typename T>
     DS_D_INLINE T dequantize(int8_t val)
     {
-        const float val_deq_f = conversion::to<float>(val) * scale + offset;
+        const float val_deq_f = ((conversion::to<float>(val)) * scale) + offset;
         return conversion::to<__half>(val_deq_f);
     }
 
     DS_D_INLINE void store(float* params, int group_index)
     {
         // Codegen should turn this into stg.64
         const float store_scale = 1 / scale;
```

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/reduction_utils.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/reduction_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/simd.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/simd.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/softmax.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/softmax.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/strided_batch_gemm.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/includes/type_shim.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/includes/type_shim.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/quantization/dequantize.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/quantization/dequantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/quantization/fake_quantizer.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/quantization/fake_quantizer.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/quantization/pt_binding.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/quantization/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/quantization/quantize.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/quantization/quantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/random_ltd/gather_scatter.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/gather_scatter.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/random_ltd/pt_binding.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/random_ltd/token_sort.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/random_ltd/token_sort.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/sparse_attention/utils.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/sparse_attention/utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/cublas_wrappers.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/dropout_kernels.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/gelu_kernels.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/gelu_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/general_kernels.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -458,17 +458,17 @@
                        .dtype(query_key_value.options().dtype())
                        .layout(at::kStrided)
                        .device(at::kCUDA)
                        .requires_grad(false);
 
     T* workspace = (T*)InferenceContext::Instance().GetWorkSpace();
     size_t buf_size = bsz * seq_len * hidden_dim;
-    auto output = torch::from_blob(workspace + 3 * buf_size, {bsz, seq_len, hidden_dim}, options);
+    auto output = torch::from_blob(workspace + 4 * buf_size, {bsz, seq_len, hidden_dim}, options);
 
-    auto query_cont = workspace + 4 * buf_size;
+    auto query_cont = workspace + 5 * buf_size;
     size_t offset =
         10 * (hidden_dim * bsz * InferenceContext::Instance().GetMaxTokenLenght()) +
         layer_id * 2 * bsz * InferenceContext::Instance().GetMaxTokenLenght() * hidden_dim;
     unsigned all_tokens = soft_len;
     auto kv_cache = workspace + offset + (hidden_dim / heads) * (is_prompt ? 0 : soft_len - 1);
     size_t value_offset = bsz * InferenceContext::Instance().GetMaxTokenLenght() * hidden_dim;
```

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/normalize_kernels.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/softmax_kernels.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/transformer/transform_kernels.cu` & `deepspeed-0.9.1/deepspeed/ops/csrc/transformer/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/csrc/utils/flatten_unflatten.cpp` & `deepspeed-0.9.1/deepspeed/ops/csrc/utils/flatten_unflatten.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/lamb/fused_lamb.py` & `deepspeed-0.9.1/deepspeed/ops/lamb/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/op_builder/__init__.py` & `deepspeed-0.9.1/deepspeed/ops/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/op_builder/all_ops.py` & `deepspeed-0.9.1/deepspeed/ops/op_builder/all_ops.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/op_builder/async_io.py` & `deepspeed-0.9.1/deepspeed/ops/op_builder/async_io.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/op_builder/builder.py` & `deepspeed-0.9.1/deepspeed/ops/op_builder/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,14 @@
     print(f"{WARNING} unable to import torch, please install it if you want to pre-compile any deepspeed ops.")
 else:
     TORCH_MAJOR = int(torch.__version__.split('.')[0])
     TORCH_MINOR = int(torch.__version__.split('.')[1])
 
 
 def installed_cuda_version(name=""):
-    import torch.cuda
-    if not torch.cuda.is_available():
-        return 0, 0
     import torch.utils.cpp_extension
     cuda_home = torch.utils.cpp_extension.CUDA_HOME
     assert cuda_home is not None, "CUDA_HOME does not exist, unable to compile CUDA op(s)"
     # Ensure there is not a cuda version mismatch between torch and nvcc compiler
     output = subprocess.check_output([cuda_home + "/bin/nvcc", "-V"], universal_newlines=True)
     output_split = output.split()
     release_idx = output_split.index("release")
@@ -74,16 +71,14 @@
     ],
     11: ["11.0", "11.1", "11.2", "11.3", "11.4", "11.5", "11.6", "11.7", "11.8"],
 }
 
 
 def assert_no_cuda_mismatch(name=""):
     cuda_major, cuda_minor = installed_cuda_version(name)
-    if cuda_minor == 0 and cuda_major == 0:
-        return False
     sys_cuda_version = f'{cuda_major}.{cuda_minor}'
     torch_cuda_version = ".".join(torch.version.cuda.split('.')[:2])
     # This is a show-stopping error, should probably not proceed past this
     if sys_cuda_version != torch_cuda_version:
         if (cuda_major in cuda_minor_mismatch_ok and sys_cuda_version in cuda_minor_mismatch_ok[cuda_major]
                 and torch_cuda_version in cuda_minor_mismatch_ok[cuda_major]):
             print(f"Installed CUDA version {sys_cuda_version} does not match the "
@@ -340,18 +335,19 @@
         if cpu_info['arch'].startswith('PPC_'):
             # gcc does not provide -march on PowerPC, use -mcpu instead
             return '-mcpu=native'
         return '-march=native'
 
     def is_cuda_enable(self):
         try:
-            if torch.cuda.is_available():
-                return '-D__ENABLE_CUDA__'
-        except:
-            print(f"{WARNING} {self.name} torch.cuda is missing, only cpu ops can be compiled!")
+            assert_no_cuda_mismatch(self.name)
+            return '-D__ENABLE_CUDA__'
+        except BaseException:
+            print(f"{WARNING} {self.name} cuda is missing or is incompatible with installed torch, "
+                  "only cpu ops can be compiled!")
             return '-D__DISABLE_CUDA__'
         return '-D__DISABLE_CUDA__'
 
     def _backup_cpuinfo(self):
         # Construct cpu_info dict from lscpu that is similar to what py-cpuinfo provides
         if not self.command_exists('lscpu'):
             self.warning(f"{self.name} attempted to query 'lscpu' after failing to use py-cpuinfo "
@@ -455,15 +451,19 @@
             )
         try:
             import ninja  # noqa: F401
         except ImportError:
             raise RuntimeError(f"Unable to JIT load the {self.name} op due to ninja not being installed.")
 
         if isinstance(self, CUDAOpBuilder) and not self.is_rocm_pytorch():
-            self.build_for_cpu = not assert_no_cuda_mismatch(self.name)
+            try:
+                assert_no_cuda_mismatch(self.name)
+                self.build_for_cpu = False
+            except BaseException:
+                self.build_for_cpu = True
 
         self.jit_mode = True
         from torch.utils.cpp_extension import load
 
         start_build = time.time()
         sources = [self.deepspeed_src_path(path) for path in self.sources()]
         extra_include_paths = [self.deepspeed_src_path(path) for path in self.include_paths()]
@@ -575,15 +575,20 @@
             version_ge_1_5 = ['-DVERSION_GE_1_5']
         return version_ge_1_1 + version_ge_1_3 + version_ge_1_5
 
     def is_compatible(self, verbose=True):
         return super().is_compatible(verbose)
 
     def builder(self):
-        self.build_for_cpu = not assert_no_cuda_mismatch(self.name)
+        try:
+            assert_no_cuda_mismatch(self.name)
+            self.build_for_cpu = False
+        except BaseException:
+            self.build_for_cpu = True
+
         if self.build_for_cpu:
             from torch.utils.cpp_extension import CppExtension as ExtensionBuilder
         else:
             from torch.utils.cpp_extension import CUDAExtension as ExtensionBuilder
 
         compile_args = {'cxx': self.strip_empty_entries(self.cxx_args())} if self.build_for_cpu else \
                        {'cxx': self.strip_empty_entries(self.cxx_args()), \
```

### Comparing `deepspeed-0.9.0/deepspeed/ops/op_builder/cpu_adagrad.py` & `deepspeed-0.9.1/deepspeed/ops/op_builder/cpu_adagrad.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/op_builder/cpu_adam.py` & `deepspeed-0.9.1/deepspeed/ops/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/op_builder/fused_adam.py` & `deepspeed-0.9.1/deepspeed/ops/op_builder/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/op_builder/fused_lamb.py` & `deepspeed-0.9.1/deepspeed/ops/op_builder/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/op_builder/quantizer.py` & `deepspeed-0.9.1/deepspeed/ops/op_builder/quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/op_builder/random_ltd.py` & `deepspeed-0.9.1/deepspeed/ops/op_builder/random_ltd.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/op_builder/sparse_attn.py` & `deepspeed-0.9.1/deepspeed/ops/op_builder/sparse_attn.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,17 +51,18 @@
             major, minor = torch.version.cuda.split('.')[:2]
             cuda_compatible = (int(major) == 10 and int(minor) >= 1) or (int(major) >= 11)
             if not cuda_compatible:
                 self.warning(f"{self.NAME} requires CUDA version 10.1+")
 
         TORCH_MAJOR = int(torch.__version__.split('.')[0])
         TORCH_MINOR = int(torch.__version__.split('.')[1])
-        torch_compatible = TORCH_MAJOR == 1 and TORCH_MINOR >= 5
+        torch_compatible = (TORCH_MAJOR == 1 and TORCH_MINOR >= 5)
         if not torch_compatible:
-            self.warning(f'{self.NAME} requires a torch version >= 1.5 but detected {TORCH_MAJOR}.{TORCH_MINOR}')
+            self.warning(
+                f'{self.NAME} requires a torch version >= 1.5 and < 2.0 but detected {TORCH_MAJOR}.{TORCH_MINOR}')
 
         try:
             import triton
         except ImportError:
             # auto-install of triton is broken on some systems, reverting to manual install for now
             # see this issue: https://github.com/microsoft/DeepSpeed/issues/1710
             self.warning(f"please install triton==1.0.0 if you want to use sparse attention")
```

### Comparing `deepspeed-0.9.0/deepspeed/ops/op_builder/spatial_inference.py` & `deepspeed-0.9.1/deepspeed/ops/op_builder/spatial_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/op_builder/stochastic_transformer.py` & `deepspeed-0.9.1/deepspeed/ops/op_builder/stochastic_transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/op_builder/transformer.py` & `deepspeed-0.9.1/deepspeed/ops/op_builder/transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/op_builder/transformer_inference.py` & `deepspeed-0.9.1/deepspeed/ops/op_builder/transformer_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/quantizer/quantizer.py` & `deepspeed-0.9.1/deepspeed/ops/quantizer/quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/random_ltd/dropping_utils.py` & `deepspeed-0.9.1/deepspeed/ops/random_ltd/dropping_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py` & `deepspeed-0.9.1/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/sparse_attention/matmul.py` & `deepspeed-0.9.1/deepspeed/ops/sparse_attention/matmul.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/sparse_attention/softmax.py` & `deepspeed-0.9.1/deepspeed/ops/sparse_attention/softmax.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/sparse_attention/sparse_attention_utils.py` & `deepspeed-0.9.1/deepspeed/ops/sparse_attention/sparse_attention_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/sparse_attention/sparse_self_attention.py` & `deepspeed-0.9.1/deepspeed/ops/sparse_attention/sparse_self_attention.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/sparse_attention/sparsity_config.py` & `deepspeed-0.9.1/deepspeed/ops/sparse_attention/sparsity_config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/sparse_attention/trsrc/__init__.py` & `deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/sparse_attention/trsrc/matmul.tr` & `deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/matmul.tr`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr` & `deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr` & `deepspeed-0.9.1/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/bias_add.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/bias_add.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/config.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/diffusers_attention.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/diffusers_attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             if config.fp16 and input.dtype == torch.float32:
                 input = input.half()
             head_size = input.shape[-1] // config.heads
             do_flash_attn = (head_size <= 128)
             scale = (1 / norm_factor) * (1 / norm_factor)
             if do_flash_attn and context == None:
                 qkv_out = linear_func(input, attn_qkvw, attn_qkvb if attn_qkvb is not None else attn_qkvw, attn_qkvb
-                                      is not None, do_flash_attn, config.heads)
+                                      is not None, do_flash_attn, config.heads, False)
 
                 context_layer = triton_flash_attn_kernel(qkv_out[0], qkv_out[1], qkv_out[2], scale,
                                                          input.shape[-2] % 128 == 0)
                 context_layer = _transpose_for_context(context_layer[:, :, :, :head_size])
 
             else:
                 do_flash_attn = False
@@ -78,15 +78,15 @@
                     key = key.contiguous()
                     value = value.contiguous()
                 query, key, value = inference_cuda_module.pad_transform_fp16(query, key, value, config.heads,
                                                                              do_flash_attn)
                 attention_scores = (torch.matmul(query, key.transpose(-1, -2)) * scale).softmax(dim=-1)
                 context_layer = _transpose_for_context(torch.matmul(attention_scores, value))
 
-            output = linear_func(context_layer, attn_ow, attn_ob, do_out_bias, False, config.heads)
+            output = linear_func(context_layer, attn_ow, attn_ob, do_out_bias, False, config.heads, False)
             return output
 
         output = selfAttention_fp(input, context, input_mask)
 
         return output
 
     @staticmethod
@@ -180,15 +180,15 @@
                                     inference_cuda_module.allocate_workspace_fp16
 
     def forward(self, input, context=None, input_mask=None):
         if self.config.layer_id == 0:
             self.allocate_workspace(self.config.hidden_size, self.config.heads,
                                     input.size()[1],
                                     input.size()[0], DeepSpeedDiffusersAttention.layer_id, self.config.mp_size, False,
-                                    0, self.config.max_out_tokens)
+                                    0, self.config.max_out_tokens, self.config.min_out_tokens)
         output = DeepSpeedDiffusersAttentionFunction.apply(input, context, input_mask, self.config, self.attn_qkvw,
                                                            self.attn_qw, self.attn_kw, self.attn_vw, self.attn_qkvb,
                                                            self.num_attention_heads_per_partition, self.norm_factor,
                                                            self.hidden_size_per_partition, self.attn_ow, self.attn_ob,
                                                            self.do_out_bias, self.score_context_func, self.linear_func,
                                                            self.triton_flash_attn_kernel)
```

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/diffusers_transformer_block.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/diffusers_transformer_block.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/ds_attention.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/ds_attention.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/ds_mlp.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/ds_mlp.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/moe_inference.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/moe_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/base.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/base.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,11 +19,13 @@
 
     def forward(self,
                 input: torch.Tensor,
                 weight: torch.Tensor,
                 bias: torch.Tensor,
                 weight_out: torch.Tensor,
                 async_op: bool = False):
-        output = self.fused_gemm_gelu(input, weight, weight.scale, bias, weight_out, weight_out.scale,
+        output = self.fused_gemm_gelu(input, weight, weight.scale if hasattr(weight, "scale") else torch.empty(1),
+                                      bias, weight_out,
+                                      weight_out.scale if hasattr(weight_out, "scale") else torch.empty(1),
                                       self.config.epsilon, self.config.pre_layer_norm, self.config.q_int8, async_op,
                                       self.config.transposed_mode)
         return output
```

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/linear.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/linear.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/residual_add.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/residual_add.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/softmax.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/softmax.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/softmax_context.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/softmax_context.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/inference/triton_ops.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/inference/triton_ops.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/ops/transformer/transformer.py` & `deepspeed-0.9.1/deepspeed/ops/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/profiling/config.py` & `deepspeed-0.9.1/deepspeed/profiling/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/profiling/constants.py` & `deepspeed-0.9.1/deepspeed/profiling/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/profiling/flops_profiler/profiler.py` & `deepspeed-0.9.1/deepspeed/profiling/flops_profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/activation_checkpointing/checkpointing.py` & `deepspeed-0.9.1/deepspeed/runtime/activation_checkpointing/checkpointing.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/activation_checkpointing/config.py` & `deepspeed-0.9.1/deepspeed/runtime/activation_checkpointing/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/bf16_optimizer.py` & `deepspeed-0.9.1/deepspeed/runtime/bf16_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,16 @@
 
         for i, param_group in enumerate(self.optimizer.param_groups):
             see_memory_usage(f'before initializing group {i}', force=True)
 
             partition_id = dist.get_rank(group=self.real_dp_process_group[i])
 
             # grab the original list
-            self.bf16_groups.append(param_group['params'])
+            trainable_parameters = [param for param in param_group['params'] if param.requires_grad]
+            self.bf16_groups.append(trainable_parameters)
 
             # create flat bf16 params
             self.bf16_groups_flat.append(
                 self._flatten_dense_tensors_aligned(self.bf16_groups[i],
                                                     self.nccl_start_alignment_factor * dp_world_size))
 
             # Make bf16 params point to flat tensor storage
```

### Comparing `deepspeed-0.9.0/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py` & `deepspeed-0.9.1/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py` & `deepspeed-0.9.1/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py` & `deepspeed-0.9.1/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/comm/coalesced_collectives.py` & `deepspeed-0.9.1/deepspeed/runtime/comm/coalesced_collectives.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/comm/mpi.py` & `deepspeed-0.9.1/deepspeed/runtime/comm/mpi.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/comm/nccl.py` & `deepspeed-0.9.1/deepspeed/runtime/comm/nccl.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/compression/cupy.py` & `deepspeed-0.9.1/deepspeed/runtime/compression/cupy.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/config.py` & `deepspeed-0.9.1/deepspeed/runtime/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/config_utils.py` & `deepspeed-0.9.1/deepspeed/runtime/config_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/constants.py` & `deepspeed-0.9.1/deepspeed/runtime/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/data_pipeline/config.py` & `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/data_pipeline/constants.py` & `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/data_pipeline/curriculum_scheduler.py` & `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/curriculum_scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py` & `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_routing/helper.py` & `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/helper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_routing/scheduler.py` & `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_routing/utils.py` & `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_routing/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py` & `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py` & `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py` & `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/data_pipeline/data_sampling/utils.py` & `deepspeed-0.9.1/deepspeed/runtime/data_pipeline/data_sampling/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/dataloader.py` & `deepspeed-0.9.1/deepspeed/runtime/dataloader.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/eigenvalue.py` & `deepspeed-0.9.1/deepspeed/runtime/eigenvalue.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/engine.py` & `deepspeed-0.9.1/deepspeed/runtime/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler
 
 from typing import Callable, Dict, Union, Iterable
 
 import deepspeed
 
+from deepspeed import comm as dist
 from deepspeed.runtime.utils import see_memory_usage, DummyOptim
 from .zero.offload_config import OffloadDeviceEnum
 from deepspeed.runtime.zero.stage_1_and_2 import DeepSpeedZeroOptimizer
 from deepspeed.runtime.zero.partition_parameters import ZeroParamStatus
 from deepspeed.runtime.zero.utils import is_zero_supported_optimizer, ZeRORuntimeException
 from deepspeed.runtime.zero.parameter_offload import DeepSpeedZeRoOffload
 from deepspeed.runtime.zero.config import ZERO_OPTIMIZATION
@@ -51,15 +52,15 @@
     WEIGHT_QUANTIZE_GROUPS, \
     WEIGHT_QUANTIZE_FP16_MIXED_QUANTIZE, \
     WEIGHT_QUANTIZE_CHANGE_RATIO, \
     WEIGHT_QUANTIZE_TYPE, \
     WEIGHT_QUANTIZE_ROUNDING, \
     WEIGHT_QUANTIZE_VERBOSE, \
     WEIGHT_QUANTIZE_KERNEL
-from deepspeed.checkpoint.constants import OPTIMIZER_STATE_DICT
+from deepspeed.checkpoint.constants import OPTIMIZER_STATE_DICT, FROZEN_PARAM_FRAGMENTS
 from deepspeed.runtime.sparse_tensor import SparseTensor
 
 from deepspeed.runtime import lr_schedules
 from deepspeed.utils import groups
 from deepspeed.utils import logger, log_dist, instrument_w_nvtx
 from deepspeed.utils.timer import ThroughputTimer, SynchronizedWallClockTimer
 from deepspeed.utils.debug import debug_extract_module_and_param_names
@@ -92,17 +93,14 @@
 from deepspeed.utils.logging import print_json_dist, print_configuration
 
 from deepspeed.accelerator import get_accelerator
 from deepspeed.ops.op_builder import UtilsBuilder
 
 from deepspeed.runtime.config import DtypeEnum
 
-# Set to torch's distributed package or deepspeed.comm based inside DeepSpeedEngine init
-dist = None
-
 MEMORY_OPT_ALLREDUCE_SIZE = 500000000
 
 DeepSpeedOptimizerCallable = \
     Callable[[Union[Iterable[Parameter], Dict[str, Iterable]]], Optimizer]
 DeepSpeedSchedulerCallable = Callable[[Optimizer], _LRScheduler]
 
 try:
@@ -228,41 +226,23 @@
         self.moe_layers = []
         self._step_applied = False
         self._global_grad_norm = None
         self.use_ds_comm = False  # False --> Use torch.dist, True --> Use ds.comm backend.
 
         self.checkpoint_engine = None
 
-        global dist
-        from deepspeed import comm as dist
         self._is_gradient_accumulation_boundary = None
         self.scale_wrt_gas = None
 
         # for debug purposes - can then debug print: debug_get_module_name(module)
         debug_extract_module_and_param_names(model)
 
         # needed for zero_to_fp32 weights reconstruction to remap nameless data to state_dict
         self.param_names = {param: name for name, param in model.named_parameters()}
 
-        from deepspeed.comm import supported_torch_version
-        # This supported_torch_version check is for torch1.2 compatibility only
-        if supported_torch_version:
-            dist.init_distributed(dist_backend=self.dist_backend, dist_init_required=dist_init_required)
-        else:
-            if dist_init_required is None:
-                dist_init_required = not dist.is_initialized()
-
-            if dist_init_required is False:
-                assert (
-                    dist.is_initialized() is True
-                ), "Torch distributed not initialized. Please set dist_init_required to True or initialize before calling deepspeed.initialize()"
-            else:
-                if not dist.is_initialized():
-                    dist.init_process_group(backend=self.dist_backend)
-
         self._do_args_sanity_check(args)
         self._configure_with_arguments(args, mpu)
         self._do_sanity_check()
         see_memory_usage(f"DeepSpeed Engine: After args sanity test", force=self.memory_breakdown())
         if mpu is not None:
             if self.elasticity_enabled():
                 if not self.is_elastic_model_parallel_supported():
@@ -2410,22 +2390,36 @@
                         for key in list(expert_state_dict.keys()):
                             local_key = key.replace(f'{moe_str_prefix}{global_expert_id}',
                                                     f'{moe_str_prefix}{local_expert_id}')
                             expert_state_dict[local_key] = expert_state_dict.pop(key)
                         state_dict.update(expert_state_dict)
                     moe_layer_id += 1
 
-    def load_module_state_dict(self, state_dict, strict=True, custom_load_fn=None):
+    def load_module_state_dict(self, checkpoint, strict=True, custom_load_fn=None):
+        module_state_dict = checkpoint['module']
         if custom_load_fn:
-            custom_load_fn(src=state_dict, dst=self.module)
+            custom_load_fn(src=module_state_dict, dst=self.module)
         else:
             self.module.load_state_dict(
-                state_dict,  # TODO
+                module_state_dict,  # TODO
                 strict=strict)
 
+        if checkpoint.get(FROZEN_PARAM_FRAGMENTS, None) is not None:
+            saved_frozen_params = checkpoint[FROZEN_PARAM_FRAGMENTS]
+            for param in self.module.parameters():
+                if param.requires_grad:
+                    continue
+                if param not in self.param_names:
+                    raise ValueError(f"failed to find frozen {param} in named params")
+                name = self.param_names[param]
+                if hasattr(param, 'ds_id'):
+                    param.ds_tensor.data.copy_(saved_frozen_params[name].data)
+                else:
+                    param.data.copy_(saved_frozen_params[name].data)
+
     def _get_zero_ckpt_prefix(self, dp_rank, bf16_mode):
         return f'{"bf16_" if bf16_mode else ""}zero_pp_rank_{dp_rank}'
 
     def _get_rank_zero_ckpt_name(self, checkpoints_path, tag, mp_rank, dp_rank, bf16_mode):
         file_prefix = self._get_zero_ckpt_prefix(dp_rank, bf16_mode=bf16_mode)
         zero_ckpt_name = os.path.join(
             checkpoints_path,
@@ -2597,15 +2591,15 @@
                                                 state_dict=checkpoint['module'],
                                                 old_moe_load=old_moe_load,
                                                 model=self.module,
                                                 mpu=self.mpu,
                                                 num_experts=self.num_experts,
                                                 checkpoint_engine=self.checkpoint_engine)
         if not self.load_universal_checkpoint():
-            self.load_module_state_dict(state_dict=checkpoint['module'],
+            self.load_module_state_dict(checkpoint=checkpoint,
                                         strict=load_module_strict,
                                         custom_load_fn=custom_load_fn)
 
         self.loaded_checkpoint_dp_world_size = checkpoint['dp_world_size']
 
         if load_module_only:
             deepspeed_states = ['module']
@@ -3007,26 +3001,32 @@
 
     def _save_checkpoint(self, save_dir, tag, client_state={}):
 
         save_path = self._get_ckpt_name(save_dir, tag)
 
         zero_optimizer_state = self.zero_optimization() or self.bfloat16_enabled()
 
+        save_frozen_param = self.zero_optimization_partition_gradients()
+
         # A hack to save the checkpointing directory. Pipeline parallelism overrides
         # module_state_dict() and uses this path to save the model. module_state_dict()
         # then instead just returns None.  The module_state_dict() implementation in
         # PipelineEngine expects the save path to be set in self._curr_ckpt_path.
         self._curr_ckpt_path = os.path.join(save_dir, tag)
         module = self.module_state_dict()
         self._curr_ckpt_path = None
 
         state = dict(module=module,
                      buffer_names=self._get_buffer_names(),
                      optimizer=self.optimizer.state_dict() if self.optimizer and not zero_optimizer_state else None,
                      param_shapes=self._get_zero_param_shapes() if self.optimizer and zero_optimizer_state else None,
+                     frozen_param_shapes=self._get_zero_frozen_param_attributes(self._get_param_shape_func)
+                     if save_frozen_param else None,
+                     frozen_param_fragments=self._get_zero_frozen_param_attributes(self._get_param_fragment_func)
+                     if save_frozen_param else None,
                      lr_scheduler=self.lr_scheduler.state_dict() if self.lr_scheduler is not None else None,
                      data_sampler=self.training_dataloader.data_sampler.state_dict() if
                      (self.training_dataloader is not None and self.curriculum_learning_enabled()) else None,
                      random_ltd=self.random_ltd_scheduler.state_dict() if self.random_ltd_enabled() else None,
                      sparse_tensor_module_names=self.sparse_tensor_module_names,
                      skipped_steps=self.skipped_steps,
                      global_steps=self.global_steps,
@@ -3058,14 +3058,33 @@
                 if child is not None:
                     get_layer_named_buffers(child, prefix + name + ".")
 
         get_layer_named_buffers(self.module, prefix="")
 
         return buffer_names
 
+    def _get_param_shape_func(self, param):
+        return param.ds_shape if hasattr(param, 'ds_id') else param.shape
+
+    def _get_param_fragment_func(self, param):
+        return param.ds_tensor.detach().cpu() if hasattr(param, 'ds_id') else param.detach().cpu()
+
+    def _get_zero_frozen_param_attributes(self, attr_func):
+        frozen_param_fragments = OrderedDict()
+
+        for param in self.module.parameters():
+            if param.requires_grad:
+                continue
+            if param not in self.param_names:
+                raise ValueError(f"failed to find frozen {param} in named params")
+            name = self.param_names[param]
+            frozen_param_fragments[name] = attr_func(param)
+
+        return frozen_param_fragments
+
     def _get_zero_param_shapes(self):
         """Returns a dict of name to shape mapping, only for the flattened fp32 weights saved by the
         optimizer. the names are exactly as in state_dict. The order is absolutely important, since
         the saved data is just flattened data with no identifiers and requires reconstruction in the
         same order it was saved.
         We can't rely on self.module.named_parameters() to get the saved tensors, as some params
         will be missing and others unsaved and then it'd be impossible to reconstruct state_dict
```

### Comparing `deepspeed-0.9.0/deepspeed/runtime/fp16/fused_optimizer.py` & `deepspeed-0.9.1/deepspeed/runtime/fp16/fused_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/fp16/loss_scaler.py` & `deepspeed-0.9.1/deepspeed/runtime/fp16/loss_scaler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/fp16/onebit/adam.py` & `deepspeed-0.9.1/deepspeed/runtime/fp16/onebit/adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/fp16/onebit/lamb.py` & `deepspeed-0.9.1/deepspeed/runtime/fp16/onebit/lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/fp16/onebit/zoadam.py` & `deepspeed-0.9.1/deepspeed/runtime/fp16/onebit/zoadam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/fp16/unfused_optimizer.py` & `deepspeed-0.9.1/deepspeed/runtime/fp16/unfused_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/hybrid_engine.py` & `deepspeed-0.9.1/deepspeed/runtime/hybrid_engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/lr_schedules.py` & `deepspeed-0.9.1/deepspeed/runtime/lr_schedules.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/pipe/engine.py` & `deepspeed-0.9.1/deepspeed/runtime/pipe/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1244,26 +1244,27 @@
         assert isinstance(self.module, PipelineModule)
         assert self._curr_ckpt_path is not None, \
             "PipelineEngine expects module_state_dict() to be called from save_checkpoint()"
 
         self.module.save_state_dict(self._curr_ckpt_path, checkpoint_engine=self.checkpoint_engine)
         return None
 
-    def load_module_state_dict(self, state_dict, strict=True, custom_load_fn=None):
+    def load_module_state_dict(self, checkpoint, strict=True, custom_load_fn=None):
         """Override hack to instead use a directory path.
 
         This is important because pipeline models checkpoint by layer instead of rank.
 
         If ``state_dict`` is not ``None`` or a ``str``, we revert to ``super()`` expecting a ``dict``.
 
         Args:
             state_dict (str, None): unused
             strict (bool, optional): Strict state loading. Defaults to True.
         """
         assert custom_load_fn is None, "custom_load_fn not supported w. pipeline parallelism"
+        state_dict = checkpoint['module']
         if (state_dict is not None) and (not isinstance(state_dict, str)):
             super().load_module_state_dict(state_dict, strict)
             return
 
         self.module.load_state_dir(load_dir=self._curr_ckpt_path,
                                    strict=strict,
                                    checkpoint_engine=self.checkpoint_engine)
```

### Comparing `deepspeed-0.9.0/deepspeed/runtime/pipe/module.py` & `deepspeed-0.9.1/deepspeed/runtime/pipe/module.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/pipe/p2p.py` & `deepspeed-0.9.1/deepspeed/runtime/pipe/p2p.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/pipe/schedule.py` & `deepspeed-0.9.1/deepspeed/runtime/pipe/schedule.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/pipe/topology.py` & `deepspeed-0.9.1/deepspeed/runtime/pipe/topology.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/progressive_layer_drop.py` & `deepspeed-0.9.1/deepspeed/runtime/progressive_layer_drop.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/quantize.py` & `deepspeed-0.9.1/deepspeed/runtime/quantize.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/sparse_tensor.py` & `deepspeed-0.9.1/deepspeed/runtime/sparse_tensor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/state_dict_factory.py` & `deepspeed-0.9.1/deepspeed/runtime/state_dict_factory.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/swap_tensor/aio_config.py` & `deepspeed-0.9.1/deepspeed/runtime/swap_tensor/aio_config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/swap_tensor/async_swapper.py` & `deepspeed-0.9.1/deepspeed/runtime/swap_tensor/async_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/swap_tensor/constants.py` & `deepspeed-0.9.1/deepspeed/runtime/swap_tensor/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/swap_tensor/optimizer_utils.py` & `deepspeed-0.9.1/deepspeed/runtime/swap_tensor/optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py` & `deepspeed-0.9.1/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py` & `deepspeed-0.9.1/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py` & `deepspeed-0.9.1/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/swap_tensor/utils.py` & `deepspeed-0.9.1/deepspeed/runtime/swap_tensor/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/utils.py` & `deepspeed-0.9.1/deepspeed/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/weight_quantizer.py` & `deepspeed-0.9.1/deepspeed/runtime/weight_quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/zero/config.py` & `deepspeed-0.9.1/deepspeed/runtime/zero/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/zero/contiguous_memory_allocator.py` & `deepspeed-0.9.1/deepspeed/runtime/zero/contiguous_memory_allocator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/zero/linear.py` & `deepspeed-0.9.1/deepspeed/runtime/zero/linear.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/zero/offload_config.py` & `deepspeed-0.9.1/deepspeed/runtime/zero/offload_config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/zero/parameter_offload.py` & `deepspeed-0.9.1/deepspeed/runtime/zero/parameter_offload.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/zero/partition_parameters.py` & `deepspeed-0.9.1/deepspeed/runtime/zero/partition_parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 from deepspeed.utils.debug import (debug_param2name_id_shape, debug_param2name_id_shape_device, debug_module2name,
                                    debug_param2name_id, debug_param2name_id_shape_status)
 from deepspeed.accelerator import get_accelerator
 from ..swap_tensor.partitioned_param_swapper import AsyncPartitionedParameterSwapper, PartitionedParamStatus
 
 param_count = 0
 partitioned_param_data_shape = [0]
-zero_init_enabled = False
+zero_init_context = []
+all_wrapped_classes = set()
 
 
 class NoGatherHandle:
 
     def __init__(self, param: Parameter) -> None:
         if param.ds_status != ZeroParamStatus.INFLIGHT:
             raise RuntimeError(f"expected param {param.ds_summary()} to be available")
@@ -286,20 +287,19 @@
     def __init__(self, enabled=True, mem_efficient_linear=True, ds_config=None, dtype=None):
         self.mem_efficient_linear = mem_efficient_linear
         self.enabled = enabled
         self._set_dtype(ds_config, dtype)
         assert self.dtype in [
             torch.half, torch.bfloat16, torch.float
         ], f"Invalid data type {self.dtype}, allowed values are [torch.half, torch.bfloat16, torch.float]"
+        self.wrapped_cls = set()
 
     def __enter__(self):
-        global zero_init_enabled
         if not self.enabled:
             return
-        zero_init_enabled = True
 
         def apply_with_gather(orig_module_apply_fn: Callable) -> Callable:
             """many models make use of child modules like Linear or Embedding which
             perform their own weight initialization in their __init__ methods,
             but will then have more weight initialization in a parent module's __init__
             method that modifies weights of child modules, which is typically done
             using the Module.apply method.
@@ -396,48 +396,66 @@
             cls._old_init = cls.__init__
             cls.__init__ = partition_after(cls.__init__)
 
         def _init_subclass(cls, **kwargs):
             cls.__init__ = partition_after(cls.__init__)
 
         # Replace .__init__() for all existing subclasses of torch.nn.Module recursively
+        global zero_init_context
+        self.nest_level = len(zero_init_context)
+
+        global all_wrapped_classes
         for subclass in get_all_subclasses(torch.nn.modules.module.Module):
-            # print(f"subclass={subclass.__module__}.{subclass.__qualname__}")
-            _enable_class(subclass)
+            # Only wrap classes that haven't been wrapped yet
+            if subclass not in all_wrapped_classes:
+                _enable_class(subclass)
+                self.wrapped_cls.add(subclass)
+
+        all_wrapped_classes = all_wrapped_classes.union(self.wrapped_cls)
+
+        # Wrap some functions only at top level call of Init
+        if self.nest_level == 0:
+            # holding onto some methods so we can put them back the way they were in __exit__
+            torch.nn.modules.module.Module._old_init_subclass = torch.nn.modules.module.Module.__init_subclass__
+            torch.nn.modules.module.Module._old_apply = torch.nn.modules.module.Module.apply
+            torch.Tensor.__old_new__ = torch.Tensor.__new__
+
+            # Replace .__init__() for future subclasses of torch.nn.Module
+            torch.nn.modules.module.Module.__init_subclass__ = classmethod(_init_subclass)
+            torch.nn.modules.module.Module.apply = apply_with_gather(torch.nn.modules.module.Module._old_apply)
+
+            torch.Tensor.__new__ = get_new_tensor_fn_for_dtype(self.dtype)
+            torch.empty = zero_wrapper_for_fp_tensor_constructor(_orig_torch_empty, self.dtype)
+            torch.zeros = zero_wrapper_for_fp_tensor_constructor(_orig_torch_zeros, self.dtype)
+            torch.ones = zero_wrapper_for_fp_tensor_constructor(_orig_torch_ones, self.dtype)
+            torch.full = zero_wrapper_for_fp_tensor_constructor(_orig_torch_full, self.dtype)
+
+            if self.mem_efficient_linear:
+                print_rank_0(
+                    "nn.functional.linear has been overridden with a more memory efficient version. This will persist unless manually reset.",
+                    force=False)
+                self.linear_bk = torch.nn.functional.linear
+                torch.nn.functional.linear = zero3_linear_wrap
+
+            self.torch_func_wrapped = True
 
-        # holding onto some methods so we can put them back the way they were in __exit__
-        torch.nn.modules.module.Module._old_init_subclass = torch.nn.modules.module.Module.__init_subclass__
-        torch.nn.modules.module.Module._old_apply = torch.nn.modules.module.Module.apply
-        torch.Tensor.__old_new__ = torch.Tensor.__new__
-
-        # Replace .__init__() for future subclasses of torch.nn.Module
-        torch.nn.modules.module.Module.__init_subclass__ = classmethod(_init_subclass)
-        torch.nn.modules.module.Module.apply = apply_with_gather(torch.nn.modules.module.Module._old_apply)
-
-        torch.Tensor.__new__ = get_new_tensor_fn_for_dtype(self.dtype)
-        torch.empty = zero_wrapper_for_fp_tensor_constructor(_orig_torch_empty, self.dtype)
-        torch.zeros = zero_wrapper_for_fp_tensor_constructor(_orig_torch_zeros, self.dtype)
-        torch.ones = zero_wrapper_for_fp_tensor_constructor(_orig_torch_ones, self.dtype)
-        torch.full = zero_wrapper_for_fp_tensor_constructor(_orig_torch_full, self.dtype)
-
-        if self.mem_efficient_linear:
-            print_rank_0(
-                "nn.functional.linear has been overridden with a more memory efficient version. This will persist unless manually reset.",
-                force=False)
-            self.linear_bk = torch.nn.functional.linear
-            torch.nn.functional.linear = zero3_linear_wrap
+        zero_init_context.append(self)
 
     def __exit__(self, exc_type, exc_value, traceback):
         if not self.enabled:
             return
 
-        shutdown_init_context()
+        self.remove_wrappers()
 
-        if dist.get_rank() == 0:
-            logger.info("finished initializing model with %.2fB parameters", param_count / 1e9)
+        # Exiting the top level context
+        global zero_init_context
+        zero_init_context.pop()
+        if self.nest_level == 0:
+            if dist.get_rank() == 0:
+                logger.info("finished initializing model with %.2fB parameters", param_count / 1e9)
 
         # Now that we cleaned up the metaclass injection, raise the exception.
         if exc_type is not None:
             return False
 
     # To be implemented by inheriting classes
     def _post_init_method(self, module):
@@ -453,45 +471,59 @@
             elif ds_config.fp16_enabled:
                 self.dtype = torch.half
             else:
                 self.dtype = torch.float
         else:
             self.dtype = dtype or torch.half
 
+    def remove_wrappers(self):
 
-def shutdown_init_context():
-    global zero_init_enabled
-
-    if not zero_init_enabled:
-        return
+        def _disable_class(cls):
+            cls.__init__ = cls._old_init
 
-    def _disable_class(cls):
-        cls.__init__ = cls._old_init
+        for subclass in self.wrapped_cls:
+            _disable_class(subclass)
+        self.wrapped_cls.clear()
+
+        # This context is the top level of nested Init
+        if self.nest_level == 0 and self.torch_func_wrapped:
+            # putting methods back the way we found them
+            torch.nn.modules.module.Module.__init_subclass__ = torch.nn.modules.module.Module._old_init_subclass
+            torch.nn.modules.module.Module.apply = torch.nn.modules.module.Module._old_apply
+
+            torch.Tensor.__new__ = torch.Tensor.__old_new__
+            torch.empty = _orig_torch_empty
+            torch.zeros = _orig_torch_zeros
+            torch.ones = _orig_torch_ones
+            torch.full = _orig_torch_full
+
+            # un doing it here will undo it during training
+            # if self.mem_efficient_linear:
+            #    torch.nn.functional.linear = self.linear_bk
+            #        if self.mem_efficient_linear:
+            #            torch.nn.functional.linear = self.linear_bk
+
+            self.torch_func_wrapped = False
+
+            global all_wrapped_classes
+            for subclass in get_all_subclasses(torch.nn.modules.module.Module):
+                if subclass not in all_wrapped_classes:
+                    msg = f"`{subclass}' was not properly set up for sharding by zero.Init(). A subclass of torch.nn.Module must be defined before zero.Init() where an instance of the class is created."
+                    raise RuntimeError(msg)
+            all_wrapped_classes.clear()
 
-    # Replace .__init__() for all existing subclasses of torch.nn.Module
-    for subclass in get_all_subclasses(torch.nn.modules.module.Module):
-        _disable_class(subclass)
-
-    # putting methods back the way we found them
-    torch.nn.modules.module.Module.__init_subclass__ = torch.nn.modules.module.Module._old_init_subclass
-    torch.nn.modules.module.Module.apply = torch.nn.modules.module.Module._old_apply
-
-    torch.Tensor.__new__ = torch.Tensor.__old_new__
-    torch.empty = _orig_torch_empty
-    torch.zeros = _orig_torch_zeros
-    torch.ones = _orig_torch_ones
-    torch.full = _orig_torch_full
-
-    # un doing it here will undo it during training
-    # if self.mem_efficient_linear:
-    #    torch.nn.functional.linear = self.linear_bk
-    #        if self.mem_efficient_linear:
-    #            torch.nn.functional.linear = self.linear_bk
 
-    zero_init_enabled = False
+def shutdown_init_context():
+    """
+    This function is used to initialize deepspeed engine inside the context of Init.
+    We need to remove the wrappers but keep the list of contexts.
+    """
+    global zero_init_context
+    for ctx in zero_init_context:
+        ctx.remove_wrappers()
 
 
 class AllGatherHandle:
 
     def __init__(self, handle, param: Parameter) -> None:
         if param.ds_status != ZeroParamStatus.INFLIGHT:
             raise RuntimeError(f"expected param {param.ds_summary()} to be available")
```

### Comparing `deepspeed-0.9.0/deepspeed/runtime/zero/partitioned_param_coordinator.py` & `deepspeed-0.9.1/deepspeed/runtime/zero/partitioned_param_coordinator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/zero/stage3.py` & `deepspeed-0.9.1/deepspeed/runtime/zero/stage3.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/zero/stage_1_and_2.py` & `deepspeed-0.9.1/deepspeed/runtime/zero/stage_1_and_2.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/zero/test.py` & `deepspeed-0.9.1/deepspeed/runtime/zero/test.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/zero/tiling.py` & `deepspeed-0.9.1/deepspeed/runtime/zero/tiling.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/runtime/zero/utils.py` & `deepspeed-0.9.1/deepspeed/runtime/zero/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/utils/__init__.py` & `deepspeed-0.9.1/deepspeed/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/utils/comms_logging.py` & `deepspeed-0.9.1/deepspeed/utils/comms_logging.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/utils/debug.py` & `deepspeed-0.9.1/deepspeed/utils/debug.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/utils/groups.py` & `deepspeed-0.9.1/deepspeed/utils/groups.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/utils/init_on_device.py` & `deepspeed-0.9.1/deepspeed/utils/init_on_device.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/utils/logging.py` & `deepspeed-0.9.1/deepspeed/utils/logging.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/utils/mixed_precision_linkage.py` & `deepspeed-0.9.1/deepspeed/utils/mixed_precision_linkage.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/utils/tensor_fragment.py` & `deepspeed-0.9.1/deepspeed/utils/tensor_fragment.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/utils/timer.py` & `deepspeed-0.9.1/deepspeed/utils/timer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed/utils/zero_to_fp32.py` & `deepspeed-0.9.1/deepspeed/utils/zero_to_fp32.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,20 +15,33 @@
 import argparse
 import torch
 import glob
 import math
 import os
 import re
 from collections import OrderedDict
+from dataclasses import dataclass
 
 # while this script doesn't use deepspeed to recover data, since the checkpoints are pickled with
 # DeepSpeed data structures it has to be available in the current python environment.
 from deepspeed.utils import logger
 from deepspeed.checkpoint.constants import (DS_VERSION, OPTIMIZER_STATE_DICT, SINGLE_PARTITION_OF_FP32_GROUPS,
-                                            FP32_FLAT_GROUPS, ZERO_STAGE, PARTITION_COUNT, PARAM_SHAPES, BUFFER_NAMES)
+                                            FP32_FLAT_GROUPS, ZERO_STAGE, PARTITION_COUNT, PARAM_SHAPES, BUFFER_NAMES,
+                                            FROZEN_PARAM_SHAPES, FROZEN_PARAM_FRAGMENTS)
+
+
+@dataclass
+class zero_model_state:
+    buffers: dict()
+    param_shapes: dict()
+    shared_params: list
+    ds_version: int
+    frozen_param_shapes: dict()
+    frozen_param_fragments: dict()
+
 
 debug = 0
 
 # load to cpu
 device = torch.device('cpu')
 
 
@@ -57,57 +70,84 @@
 
     if not os.path.exists(file):
         raise FileNotFoundError(f"can't find model states file at '{file}'")
 
     return file
 
 
-def get_optim_files(checkpoint_dir):
+def get_checkpoint_files(checkpoint_dir, glob_pattern):
     # XXX: need to test that this simple glob rule works for multi-node setup too
-    optim_files = sorted(glob.glob(os.path.join(checkpoint_dir, "*_optim_states.pt")), key=natural_keys)
+    ckpt_files = sorted(glob.glob(os.path.join(checkpoint_dir, glob_pattern)), key=natural_keys)
 
-    if len(optim_files) == 0:
-        raise FileNotFoundError(f"can't find '*_optim_states.pt' files in directory '{checkpoint_dir}'")
+    if len(ckpt_files) == 0:
+        raise FileNotFoundError(f"can't find {glob_pattern} files in directory '{checkpoint_dir}'")
 
-    return optim_files
+    return ckpt_files
 
 
-def parse_model_state(file):
-    state_dict = torch.load(file, map_location=device)
+def get_optim_files(checkpoint_dir):
+    return get_checkpoint_files(checkpoint_dir, "*_optim_states.pt")
 
-    if BUFFER_NAMES not in state_dict:
-        raise ValueError(f"{file} is not a model state checkpoint")
-    buffer_names = state_dict[BUFFER_NAMES]
-    if debug:
-        print("Found buffers:", buffer_names)
 
-    # recover just the buffers while restoring them to fp32 if they were saved in fp16
-    buffers = {k: v.float() for k, v in state_dict["module"].items() if k in buffer_names}
-    param_shapes = state_dict[PARAM_SHAPES]
-
-    # collect parameters that are included in param_shapes
-    param_names = []
-    for s in param_shapes:
-        for name in s.keys():
-            param_names.append(name)
-
-    # record shared parameters so that they can be recovered based on partners
-    # this is because such parameters holding reference only are not saved by optimizer
-    shared_params = []
-    for param in state_dict["module"]:
-        if param not in [*param_names, *buffer_names]:
-            for share_param in state_dict["module"]:
-                if (state_dict["module"][share_param].data_ptr() == state_dict["module"][param].data_ptr()
-                        and share_param != param):
-                    shared_params.append([param, share_param])
-                    break
+def get_model_state_files(checkpoint_dir):
+    return get_checkpoint_files(checkpoint_dir, "*_model_states.pt")
+
+
+def parse_model_states(files):
+    zero_model_states = []
+    for file in files:
+        state_dict = torch.load(file, map_location=device)
+
+        if BUFFER_NAMES not in state_dict:
+            raise ValueError(f"{file} is not a model state checkpoint")
+        buffer_names = state_dict[BUFFER_NAMES]
+        if debug:
+            print("Found buffers:", buffer_names)
+
+        # recover just the buffers while restoring them to fp32 if they were saved in fp16
+        buffers = {k: v.float() for k, v in state_dict["module"].items() if k in buffer_names}
+        param_shapes = state_dict[PARAM_SHAPES]
+
+        # collect parameters that are included in param_shapes
+        param_names = []
+        for s in param_shapes:
+            for name in s.keys():
+                param_names.append(name)
+
+        # update with frozen parameters
+        frozen_param_shapes = state_dict.get(FROZEN_PARAM_SHAPES, None)
+        if frozen_param_shapes is not None:
+            if debug:
+                print(f"Found frozen_param_shapes: {frozen_param_shapes}")
+            param_names += list(frozen_param_shapes.keys())
 
-    ds_version = state_dict.get(DS_VERSION, None)
+        # record shared parameters so that they can be recovered based on partners
+        # this is because such parameters holding reference only are not saved by optimizer
+        shared_params = []
+        for param in state_dict["module"]:
+            if param not in [*param_names, *buffer_names]:
+                for share_param in state_dict["module"]:
+                    if (state_dict["module"][share_param].data_ptr() == state_dict["module"][param].data_ptr()
+                            and share_param != param):
+                        shared_params.append([param, share_param])
+                        break
+
+        ds_version = state_dict.get(DS_VERSION, None)
+
+        frozen_param_fragments = state_dict.get(FROZEN_PARAM_FRAGMENTS, None)
+
+        z_model_state = zero_model_state(buffers=buffers,
+                                         param_shapes=param_shapes,
+                                         shared_params=shared_params,
+                                         ds_version=ds_version,
+                                         frozen_param_shapes=frozen_param_shapes,
+                                         frozen_param_fragments=frozen_param_fragments)
+        zero_model_states.append(z_model_state)
 
-    return buffers, param_shapes, shared_params, ds_version
+    return zero_model_states
 
 
 def parse_optim_states(files, ds_checkpoint_dir):
 
     total_files = len(files)
     state_dicts = []
     for f in files:
@@ -165,27 +205,59 @@
     """
     print(f"Processing zero checkpoint '{ds_checkpoint_dir}'")
 
     optim_files = get_optim_files(ds_checkpoint_dir)
     zero_stage, world_size, fp32_flat_groups = parse_optim_states(optim_files, ds_checkpoint_dir)
     print(f"Detected checkpoint of type zero stage {zero_stage}, world_size: {world_size}")
 
-    model_file = get_model_state_file(ds_checkpoint_dir, zero_stage)
-    buffers, param_shapes, shared_params, ds_version = parse_model_state(model_file)
-    print(f'Parsing checkpoint created by deepspeed=={ds_version}')
+    model_files = get_model_state_files(ds_checkpoint_dir)
+
+    zero_model_states = parse_model_states(model_files)
+    print(f'Parsing checkpoint created by deepspeed=={zero_model_states[0].ds_version}')
 
     if zero_stage == 2:
-        return _get_fp32_state_dict_from_zero2_checkpoint(world_size, param_shapes, fp32_flat_groups, buffers,
-                                                          shared_params)
+        return _get_fp32_state_dict_from_zero2_checkpoint(world_size, fp32_flat_groups, zero_model_states)
     elif zero_stage == 3:
-        return _get_fp32_state_dict_from_zero3_checkpoint(world_size, param_shapes, fp32_flat_groups, buffers,
-                                                          shared_params)
+        return _get_fp32_state_dict_from_zero3_checkpoint(world_size, fp32_flat_groups, zero_model_states)
+
+
+def _zero2_merge_frozen_params(state_dict, zero_model_states):
+    if zero_model_states[0].frozen_param_shapes is None or len(zero_model_states[0].frozen_param_shapes) == 0:
+        return
+
+    frozen_param_shapes = zero_model_states[0].frozen_param_shapes
+    frozen_param_fragments = zero_model_states[0].frozen_param_fragments
+
+    if debug:
+        num_elem = sum(s.numel() for s in frozen_param_shapes.values())
+        print(f'rank 0: {FROZEN_PARAM_SHAPES}.numel = {num_elem}')
 
+        wanted_params = len(frozen_param_shapes)
+        wanted_numel = sum(s.numel() for s in frozen_param_shapes.values())
+        avail_numel = sum([p.numel() for p in frozen_param_fragments.values()])
+        print(f'Frozen params: Have {avail_numel} numels to process.')
+        print(f'Frozen params: Need {wanted_numel} numels in {wanted_params} params')
+
+    total_params = 0
+    total_numel = 0
+    for name, shape in frozen_param_shapes.items():
+        total_params += 1
+        unpartitioned_numel = shape.numel()
+        total_numel += unpartitioned_numel
 
-def _get_fp32_state_dict_from_zero2_checkpoint(world_size, param_shapes, fp32_flat_groups, buffers, shared_params):
+        state_dict[name] = frozen_param_fragments[name]
+
+        if debug:
+            print(f"{name} full shape: {shape} unpartitioned numel {unpartitioned_numel} ")
+
+    print(f"Reconstructed Frozen fp32 state dict with {total_params} params {total_numel} elements")
+
+
+def _zero2_merge_trainable_params(state_dict, world_size, fp32_flat_groups, zero_model_states):
+    param_shapes = zero_model_states[0].param_shapes
 
     # Reconstruction protocol:
     #
     # XXX: document this
 
     if debug:
         for i in range(world_size):
@@ -205,21 +277,14 @@
     if debug:
         wanted_params = sum([len(shapes) for shapes in param_shapes])
         wanted_numel = sum([sum(shape.numel() for shape in shapes.values()) for shapes in param_shapes])
         # not asserting if there is a mismatch due to possible padding
         print(f"Have {avail_numel} numels to process.")
         print(f"Need {wanted_numel} numels in {wanted_params} params.")
 
-    state_dict = OrderedDict()
-
-    # buffers
-    state_dict.update(buffers)
-    if debug:
-        print(f"added {len(buffers)} buffers")
-
     # params
     # XXX: for huge models that can't fit into the host's RAM we will have to recode this to support
     # out-of-core computing solution
     total_numel = 0
     total_params = 0
     for shapes, full_single_fp32_vector in zip(param_shapes, merged_single_partition_of_fp32_groups):
         offset = 0
@@ -253,55 +318,99 @@
         if debug:
             print(f"aligned  offset={offset}, avail_numel={avail_numel}")
 
         # Sanity check
         if offset != avail_numel:
             raise ValueError(f"consumed {offset} numels out of {avail_numel} - something is wrong")
 
+    print(f"Reconstructed fp32 state dict with {total_params} params {total_numel} elements")
+
+
+def _get_fp32_state_dict_from_zero2_checkpoint(world_size, fp32_flat_groups, zero_model_states):
+    state_dict = OrderedDict()
+
+    # buffers
+    buffers = zero_model_states[0].buffers
+    state_dict.update(buffers)
+    if debug:
+        print(f"added {len(buffers)} buffers")
+
+    _zero2_merge_frozen_params(state_dict, zero_model_states)
+
+    _zero2_merge_trainable_params(state_dict, world_size, fp32_flat_groups, zero_model_states)
+
     # recover shared parameters
-    for pair in shared_params:
+    for pair in zero_model_states[0].shared_params:
         state_dict[pair[0]] = state_dict[pair[1]]
 
-    print(f"Reconstructed fp32 state dict with {total_params} params {total_numel} elements")
-
     return state_dict
 
 
 def zero3_partitioned_param_info(unpartitioned_numel, world_size):
     remainder = unpartitioned_numel % world_size
     padding_numel = (world_size - remainder) if remainder else 0
     partitioned_numel = math.ceil(unpartitioned_numel / world_size)
     return partitioned_numel, padding_numel
 
 
-def _get_fp32_state_dict_from_zero3_checkpoint(world_size, param_shapes, fp32_flat_groups, buffers, shared_params):
+def _zero3_merge_frozen_params(state_dict, world_size, zero_model_states):
+    if zero_model_states[0].frozen_param_shapes is None or len(zero_model_states[0].frozen_param_shapes) == 0:
+        return
+
+    if debug:
+        for i in range(world_size):
+            num_elem = sum(s.numel() for s in zero_model_states[i].frozen_param_fragments.values())
+            print(f'rank {i}: {FROZEN_PARAM_SHAPES}.numel = {num_elem}')
+
+        frozen_param_shapes = zero_model_states[0].frozen_param_shapes
+        wanted_params = len(frozen_param_shapes)
+        wanted_numel = sum(s.numel() for s in frozen_param_shapes.values())
+        avail_numel = sum([p.numel() for p in zero_model_states[0].frozen_param_fragments.values()]) * world_size
+        print(f'Frozen params: Have {avail_numel} numels to process.')
+        print(f'Frozen params: Need {wanted_numel} numels in {wanted_params} params')
 
+    total_params = 0
+    total_numel = 0
+    for name, shape in zero_model_states[0].frozen_param_shapes.items():
+        total_params += 1
+        unpartitioned_numel = shape.numel()
+        total_numel += unpartitioned_numel
+
+        param_frags = tuple(model_state.frozen_param_fragments[name] for model_state in zero_model_states)
+        state_dict[name] = torch.cat(param_frags, 0).narrow(0, 0, unpartitioned_numel).view(shape)
+
+        partitioned_numel, partitioned_padding_numel = zero3_partitioned_param_info(unpartitioned_numel, world_size)
+
+        if debug:
+            print(
+                f"Frozen params: {total_params} {name} full shape: {shape} partition0 numel={partitioned_numel} partitioned_padding_numel={partitioned_padding_numel}"
+            )
+
+    print(f"Reconstructed Frozen fp32 state dict with {total_params} params {total_numel} elements")
+
+
+def _zero3_merge_trainable_params(state_dict, world_size, fp32_flat_groups, zero_model_states):
+    param_shapes = zero_model_states[0].param_shapes
+    avail_numel = fp32_flat_groups[0].numel() * world_size
     # Reconstruction protocol: For zero3 we need to zip the partitions together at boundary of each
     # param, re-consolidating each param, while dealing with padding if any
 
-    avail_numel = fp32_flat_groups[0].numel() * world_size
     # merge list of dicts, preserving order
     param_shapes = {k: v for d in param_shapes for k, v in d.items()}
 
     if debug:
         for i in range(world_size):
             print(f"{FP32_FLAT_GROUPS}[{i}].shape={fp32_flat_groups[i].shape}")
 
         wanted_params = len(param_shapes)
         wanted_numel = sum(shape.numel() for shape in param_shapes.values())
         # not asserting if there is a mismatch due to possible padding
-        print(f"Have {avail_numel} numels to process.")
-        print(f"Need {wanted_numel} numels in {wanted_params} params.")
-
-    state_dict = OrderedDict()
-
-    # buffers
-    state_dict.update(buffers)
-    if debug:
-        print(f"added {len(buffers)} buffers")
+        avail_numel = fp32_flat_groups[0].numel() * world_size
+        print(f"Trainable params: Have {avail_numel} numels to process.")
+        print(f"Trainable params: Need {wanted_numel} numels in {wanted_params} params.")
 
     # params
     # XXX: for huge models that can't fit into the host's RAM we will have to recode this to support
     # out-of-core computing solution
     offset = 0
     total_numel = 0
     total_params = 0
@@ -311,35 +420,49 @@
         total_numel += unpartitioned_numel
         total_params += 1
 
         partitioned_numel, partitioned_padding_numel = zero3_partitioned_param_info(unpartitioned_numel, world_size)
 
         if debug:
             print(
-                f"{total_params} {name} full shape: {shape} partition0 numel={partitioned_numel} partitioned_padding_numel={partitioned_padding_numel}"
+                f"Trainable params: {total_params} {name} full shape: {shape} partition0 numel={partitioned_numel} partitioned_padding_numel={partitioned_padding_numel}"
             )
 
         # XXX: memory usage doubles here
         state_dict[name] = torch.cat(
             tuple(fp32_flat_groups[i].narrow(0, offset, partitioned_numel) for i in range(world_size)),
             0).narrow(0, 0, unpartitioned_numel).view(shape)
         offset += partitioned_numel
 
     offset *= world_size
 
     # Sanity check
     if offset != avail_numel:
         raise ValueError(f"consumed {offset} numels out of {avail_numel} - something is wrong")
 
+    print(f"Reconstructed Trainable fp32 state dict with {total_params} params {total_numel} elements")
+
+
+def _get_fp32_state_dict_from_zero3_checkpoint(world_size, fp32_flat_groups, zero_model_states):
+    state_dict = OrderedDict()
+
+    # buffers
+    buffers = zero_model_states[0].buffers
+    state_dict.update(buffers)
+    if debug:
+        print(f"added {len(buffers)} buffers")
+
+    _zero3_merge_frozen_params(state_dict, world_size, zero_model_states)
+
+    _zero3_merge_trainable_params(state_dict, world_size, fp32_flat_groups, zero_model_states)
+
     # recover shared parameters
-    for pair in shared_params:
+    for pair in zero_model_states[0].shared_params:
         state_dict[pair[0]] = state_dict[pair[1]]
 
-    print(f"Reconstructed fp32 state dict with {total_params} params {total_numel} elements")
-
     return state_dict
 
 
 def get_fp32_state_dict_from_zero_checkpoint(checkpoint_dir, tag=None):
     """
     Convert ZeRO 2 or 3 checkpoint into a single fp32 consolidated state_dict that can be loaded with
     ``load_state_dict()`` and used for training without DeepSpeed or shared with others, for example
```

### Comparing `deepspeed-0.9.0/deepspeed.egg-info/PKG-INFO` & `deepspeed-0.9.1/deepspeed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepspeed
-Version: 0.9.0
+Version: 0.9.1
 Summary: DeepSpeed library
 Home-page: http://deepspeed.ai
 Author: DeepSpeed Team
 Author-email: deepspeed-info@microsoft.com
 License: MIT
 Project-URL: Documentation, https://deepspeed.readthedocs.io
 Project-URL: Source, https://github.com/microsoft/DeepSpeed
@@ -121,15 +121,15 @@
 
 DeepSpeed has been integrated with several different popular open-source DL frameworks such as:
 
 |                                                                                                | Documentation                                |
 | ---------------------------------------------------------------------------------------------- | -------------------------------------------- |
 <img src="docs/assets/images/transformers-light.png#gh-light-mode-only" width="250px"><img src="docs/assets/images/transformers-dark.png#gh-dark-mode-only" width="250px"> | [Transformers with DeepSpeed](https://huggingface.co/docs/transformers/main/main_classes/deepspeed) |
 | <img src="docs/assets/images/accelerate-light.png#gh-light-mode-only" width="250px"><img src="docs/assets/images/accelerate-dark.png#gh-dark-mode-only" width="250px"> | [Accelerate with DeepSpeed](https://huggingface.co/docs/accelerate/usage_guides/deepspeed) |
-| <img src="docs/assets/images/lightning-light.svg#gh-light-mode-only" width="200px"><img src="docs/assets/images/lightning-dark.svg#gh-dark-mode-only" width="200px"> | [Lightning with DeepSpeed](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.strategies.DeepSpeedStrategy.html) |
+| <img src="docs/assets/images/lightning-light.svg#gh-light-mode-only" width="200px"><img src="docs/assets/images/lightning-dark.svg#gh-dark-mode-only" width="200px"> | [Lightning with DeepSpeed](https://lightning.ai/docs/pytorch/stable/advanced/model_parallel.html#deepspeed) |
 | <img src="docs/assets/images/mosaicml.svg" width="200px"> | [MosaicML with DeepSpeed](https://docs.mosaicml.com/en/latest/trainer/using_the_trainer.html?highlight=deepspeed#deepspeed-integration) |
 | <img src="docs/assets/images/determined.svg" width="225px"> | [Determined with DeepSpeed](https://docs.determined.ai/latest/training/apis-howto/deepspeed/overview.html) |
 
 ---
 
 # Build Pipeline Status
 
@@ -202,15 +202,20 @@
 | [Tutorials](https://www.deepspeed.ai/tutorials/)                                               |  Tutorials                                   |
 | [Blogs](https://www.deepspeed.ai/posts/)                                                       |  Blogs                                   |
 
 
 # Contributing
 DeepSpeed welcomes your contributions! Please see our
 [contributing](CONTRIBUTING.md) guide for more details on formatting, testing,
-etc.
+etc.<br/>
+Thanks so much to all of our amazing contributors!
+
+<a href="https://github.com/microsoft/DeepSpeed/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=microsoft/DeepSpeed&r="  width="800px"/>
+</a>
 
 ## Contributor License Agreement
 This project welcomes contributions and suggestions. Most contributions require you to
 agree to a Contributor License Agreement (CLA) declaring that you have the right to, and
 actually do, grant us the rights to use your contribution. For details, visit
 https://cla.opensource.microsoft.com.
```

### Comparing `deepspeed-0.9.0/deepspeed.egg-info/SOURCES.txt` & `deepspeed-0.9.1/deepspeed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/deepspeed.egg-info/requires.txt` & `deepspeed-0.9.1/deepspeed.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 hjson
 ninja
 numpy
 packaging>=20.0
 psutil
 py-cpuinfo
-pydantic
+pydantic<2.0.0
 torch
 tqdm
 
 [1bit]
 
 [1bit_mpi]
 mpi4py
 
 [all]
-mpi4py
-tqdm
-sphinx-rtd-theme
-pytest-forked
-google
+pytest-xdist
+pytest
 torchvision
-diffusers
-torch
 packaging
-importlib-metadata>=4
-transformers[sentencepiece]
 hjson
-clang-format>=14.0.6
-pre-commit>=2.20.0
-triton==1.0.0
-recommonmark
-docutils<0.18
-psutil
-xgboost
-pytest-randomly
-tensorboard
-pytest
-pytest-xdist
-pydantic
-megatron-lm==1.1.5
+torch
 protobuf
-lm-eval==0.3.0
+tensorboard
+mpi4py
+google
+xgboost
 py-cpuinfo
+diffusers
+pytest-forked
+triton==1.0.0
+pytest-randomly
 future
+sphinx-rtd-theme
+importlib-metadata>=4
+tqdm
+docutils<0.18
 wandb
-autodoc_pydantic
-sphinx
-tabulate
+recommonmark
 triton==2.0.0.dev20221202
+megatron-lm==1.1.5
+pydantic<2.0.0
+pre-commit>=2.20.0
+sphinx
 transformers
+transformers[sentencepiece]
+psutil
+clang-format>=14.0.6
+lm-eval==0.3.0
+autodoc_pydantic<2.0.0
+tabulate
 
 [autotuning]
 tabulate
 
 [autotuning_ml]
 hjson
 tabulate
@@ -81,21 +81,21 @@
 google
 lm-eval==0.3.0
 protobuf
 transformers
 transformers[sentencepiece]
 
 [readthedocs]
-autodoc_pydantic
+autodoc_pydantic<2.0.0
 docutils<0.18
 hjson
 packaging
 psutil
 py-cpuinfo
-pydantic
+pydantic<2.0.0
 torch
 tqdm
 
 [sd]
 diffusers
 triton==2.0.0.dev20221202
```

### Comparing `deepspeed-0.9.0/op_builder/__init__.py` & `deepspeed-0.9.1/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/op_builder/all_ops.py` & `deepspeed-0.9.1/op_builder/all_ops.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/op_builder/async_io.py` & `deepspeed-0.9.1/op_builder/async_io.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/op_builder/builder.py` & `deepspeed-0.9.1/op_builder/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,14 @@
     print(f"{WARNING} unable to import torch, please install it if you want to pre-compile any deepspeed ops.")
 else:
     TORCH_MAJOR = int(torch.__version__.split('.')[0])
     TORCH_MINOR = int(torch.__version__.split('.')[1])
 
 
 def installed_cuda_version(name=""):
-    import torch.cuda
-    if not torch.cuda.is_available():
-        return 0, 0
     import torch.utils.cpp_extension
     cuda_home = torch.utils.cpp_extension.CUDA_HOME
     assert cuda_home is not None, "CUDA_HOME does not exist, unable to compile CUDA op(s)"
     # Ensure there is not a cuda version mismatch between torch and nvcc compiler
     output = subprocess.check_output([cuda_home + "/bin/nvcc", "-V"], universal_newlines=True)
     output_split = output.split()
     release_idx = output_split.index("release")
@@ -74,16 +71,14 @@
     ],
     11: ["11.0", "11.1", "11.2", "11.3", "11.4", "11.5", "11.6", "11.7", "11.8"],
 }
 
 
 def assert_no_cuda_mismatch(name=""):
     cuda_major, cuda_minor = installed_cuda_version(name)
-    if cuda_minor == 0 and cuda_major == 0:
-        return False
     sys_cuda_version = f'{cuda_major}.{cuda_minor}'
     torch_cuda_version = ".".join(torch.version.cuda.split('.')[:2])
     # This is a show-stopping error, should probably not proceed past this
     if sys_cuda_version != torch_cuda_version:
         if (cuda_major in cuda_minor_mismatch_ok and sys_cuda_version in cuda_minor_mismatch_ok[cuda_major]
                 and torch_cuda_version in cuda_minor_mismatch_ok[cuda_major]):
             print(f"Installed CUDA version {sys_cuda_version} does not match the "
@@ -340,18 +335,19 @@
         if cpu_info['arch'].startswith('PPC_'):
             # gcc does not provide -march on PowerPC, use -mcpu instead
             return '-mcpu=native'
         return '-march=native'
 
     def is_cuda_enable(self):
         try:
-            if torch.cuda.is_available():
-                return '-D__ENABLE_CUDA__'
-        except:
-            print(f"{WARNING} {self.name} torch.cuda is missing, only cpu ops can be compiled!")
+            assert_no_cuda_mismatch(self.name)
+            return '-D__ENABLE_CUDA__'
+        except BaseException:
+            print(f"{WARNING} {self.name} cuda is missing or is incompatible with installed torch, "
+                  "only cpu ops can be compiled!")
             return '-D__DISABLE_CUDA__'
         return '-D__DISABLE_CUDA__'
 
     def _backup_cpuinfo(self):
         # Construct cpu_info dict from lscpu that is similar to what py-cpuinfo provides
         if not self.command_exists('lscpu'):
             self.warning(f"{self.name} attempted to query 'lscpu' after failing to use py-cpuinfo "
@@ -455,15 +451,19 @@
             )
         try:
             import ninja  # noqa: F401
         except ImportError:
             raise RuntimeError(f"Unable to JIT load the {self.name} op due to ninja not being installed.")
 
         if isinstance(self, CUDAOpBuilder) and not self.is_rocm_pytorch():
-            self.build_for_cpu = not assert_no_cuda_mismatch(self.name)
+            try:
+                assert_no_cuda_mismatch(self.name)
+                self.build_for_cpu = False
+            except BaseException:
+                self.build_for_cpu = True
 
         self.jit_mode = True
         from torch.utils.cpp_extension import load
 
         start_build = time.time()
         sources = [self.deepspeed_src_path(path) for path in self.sources()]
         extra_include_paths = [self.deepspeed_src_path(path) for path in self.include_paths()]
@@ -575,15 +575,20 @@
             version_ge_1_5 = ['-DVERSION_GE_1_5']
         return version_ge_1_1 + version_ge_1_3 + version_ge_1_5
 
     def is_compatible(self, verbose=True):
         return super().is_compatible(verbose)
 
     def builder(self):
-        self.build_for_cpu = not assert_no_cuda_mismatch(self.name)
+        try:
+            assert_no_cuda_mismatch(self.name)
+            self.build_for_cpu = False
+        except BaseException:
+            self.build_for_cpu = True
+
         if self.build_for_cpu:
             from torch.utils.cpp_extension import CppExtension as ExtensionBuilder
         else:
             from torch.utils.cpp_extension import CUDAExtension as ExtensionBuilder
 
         compile_args = {'cxx': self.strip_empty_entries(self.cxx_args())} if self.build_for_cpu else \
                        {'cxx': self.strip_empty_entries(self.cxx_args()), \
```

### Comparing `deepspeed-0.9.0/op_builder/cpu_adagrad.py` & `deepspeed-0.9.1/op_builder/cpu_adagrad.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/op_builder/cpu_adam.py` & `deepspeed-0.9.1/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/op_builder/fused_adam.py` & `deepspeed-0.9.1/op_builder/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/op_builder/fused_lamb.py` & `deepspeed-0.9.1/op_builder/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/op_builder/quantizer.py` & `deepspeed-0.9.1/op_builder/quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/op_builder/random_ltd.py` & `deepspeed-0.9.1/op_builder/random_ltd.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/op_builder/sparse_attn.py` & `deepspeed-0.9.1/op_builder/sparse_attn.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,17 +51,18 @@
             major, minor = torch.version.cuda.split('.')[:2]
             cuda_compatible = (int(major) == 10 and int(minor) >= 1) or (int(major) >= 11)
             if not cuda_compatible:
                 self.warning(f"{self.NAME} requires CUDA version 10.1+")
 
         TORCH_MAJOR = int(torch.__version__.split('.')[0])
         TORCH_MINOR = int(torch.__version__.split('.')[1])
-        torch_compatible = TORCH_MAJOR == 1 and TORCH_MINOR >= 5
+        torch_compatible = (TORCH_MAJOR == 1 and TORCH_MINOR >= 5)
         if not torch_compatible:
-            self.warning(f'{self.NAME} requires a torch version >= 1.5 but detected {TORCH_MAJOR}.{TORCH_MINOR}')
+            self.warning(
+                f'{self.NAME} requires a torch version >= 1.5 and < 2.0 but detected {TORCH_MAJOR}.{TORCH_MINOR}')
 
         try:
             import triton
         except ImportError:
             # auto-install of triton is broken on some systems, reverting to manual install for now
             # see this issue: https://github.com/microsoft/DeepSpeed/issues/1710
             self.warning(f"please install triton==1.0.0 if you want to use sparse attention")
```

### Comparing `deepspeed-0.9.0/op_builder/spatial_inference.py` & `deepspeed-0.9.1/op_builder/spatial_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/op_builder/stochastic_transformer.py` & `deepspeed-0.9.1/op_builder/stochastic_transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/op_builder/transformer.py` & `deepspeed-0.9.1/op_builder/transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/op_builder/transformer_inference.py` & `deepspeed-0.9.1/op_builder/transformer_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.0/setup.py` & `deepspeed-0.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,20 @@
     cupy = None
     if is_rocm_pytorch:
         rocm_major, rocm_minor = rocm_version
         # XXX cupy support for rocm 5 is not available yet.
         if rocm_major <= 4:
             cupy = f"cupy-rocm-{rocm_major}-{rocm_minor}"
     else:
-        cupy = f"cupy-cuda{''.join(map(str,installed_cuda_version()))}"
+        cuda_major_ver, cuda_minor_ver = installed_cuda_version()
+        if (cuda_major_ver < 11) or ((cuda_major_ver == 11) and (cuda_minor_ver < 3)):
+            cupy = f"cupy-cuda{cuda_major_ver}{cuda_minor_ver}"
+        else:
+            cupy = f"cupy-cuda{cuda_major_ver}x"
+
     if cupy:
         extras_require['1bit'].append(cupy)
         extras_require['1bit_mpi'].append(cupy)
 
 # Make an [all] extra that installs all needed dependencies.
 all_extras = set()
 for extra in extras_require.items():
```

