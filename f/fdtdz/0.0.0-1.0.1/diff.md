# Comparing `tmp/fdtdz-0.0.0.tar.gz` & `tmp/fdtdz-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdtdz-0.0.0.tar", last modified: Fri May 12 16:10:37 2023, max compression
+gzip compressed data, was "fdtdz-1.0.1.tar", last modified: Fri May 12 17:17:41 2023, max compression
```

## Comparing `fdtdz-0.0.0.tar` & `fdtdz-1.0.1.tar`

### file list

```diff
@@ -1,206 +1,206 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 16:10:37.063276 fdtdz-0.0.0/
--rw-rw-r--   0 dev       (1000) dev       (1000)      932 2023-05-02 23:06:13.000000 fdtdz-0.0.0/CMakeLists.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)     1072 2023-04-29 07:29:27.000000 fdtdz-0.0.0/LICENSE
--rw-rw-r--   0 dev       (1000) dev       (1000)       94 2023-05-02 23:06:13.000000 fdtdz-0.0.0/MANIFEST.in
--rw-rw-r--   0 dev       (1000) dev       (1000)     6958 2023-05-12 16:10:37.063276 fdtdz-0.0.0/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)     6629 2023-05-12 15:25:08.000000 fdtdz-0.0.0/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 16:10:36.863274 fdtdz-0.0.0/cuda/
--rw-rw-r--   0 dev       (1000) dev       (1000)     4337 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/CMakeLists.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)     6751 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/buffer.h
--rw-rw-r--   0 dev       (1000) dev       (1000)     4260 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/buffer_indexing.h
--rw-rw-r--   0 dev       (1000) dev       (1000)     6315 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/buffer_ops.h
--rw-rw-r--   0 dev       (1000) dev       (1000)    12667 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/buffer_test.cu
--rw-rw-r--   0 dev       (1000) dev       (1000)     9028 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/cbuf.h
--rw-rw-r--   0 dev       (1000) dev       (1000)    11278 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/cbuf_test.cu
--rw-rw-r--   0 dev       (1000) dev       (1000)     2470 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/defs.h
--rw-rw-r--   0 dev       (1000) dev       (1000)      662 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/defs_test.cu
--rw-rw-r--   0 dev       (1000) dev       (1000)    10537 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/diamond.h
--rw-rw-r--   0 dev       (1000) dev       (1000)     5889 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/diamond_test.cu
--rw-rw-r--   0 dev       (1000) dev       (1000)     3389 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/field.h
--rw-rw-r--   0 dev       (1000) dev       (1000)     1807 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/field_test.cu
--rw-rw-r--   0 dev       (1000) dev       (1000)     1514 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/jax_ops.cc
--rw-rw-r--   0 dev       (1000) dev       (1000)     8067 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/kernel.h
--rw-rw-r--   0 dev       (1000) dev       (1000)     1380 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/kernel_helpers.h
--rw-rw-r--   0 dev       (1000) dev       (1000)     2398 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/kernel_jax.cc.cu
--rw-rw-r--   0 dev       (1000) dev       (1000)     2100 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/kernel_jax.h
--rw-rw-r--   0 dev       (1000) dev       (1000)      528 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/kernel_jax_test.cu
--rw-rw-r--   0 dev       (1000) dev       (1000)     5102 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/kernel_precompiled.h
--rw-rw-r--   0 dev       (1000) dev       (1000)     1045 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/kernel_precompiled_test.cu
--rw-rw-r--   0 dev       (1000) dev       (1000)      656 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/kernel_ptx.cu
--rw-rw-r--   0 dev       (1000) dev       (1000)     4247 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/kernel_test.cu
--rw-rw-r--   0 dev       (1000) dev       (1000)      586 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/macros.h
--rw-rw-r--   0 dev       (1000) dev       (1000)      825 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/pybind11_kernel_helpers.h
--rw-rw-r--   0 dev       (1000) dev       (1000)     5622 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/reference.h
--rw-rw-r--   0 dev       (1000) dev       (1000)     6544 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/reference_test.cu
--rw-rw-r--   0 dev       (1000) dev       (1000)     4549 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/scanner.h
--rw-rw-r--   0 dev       (1000) dev       (1000)     2286 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/scanner_impl.h
--rw-rw-r--   0 dev       (1000) dev       (1000)    15743 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/scanner_test.cu
--rw-rw-r--   0 dev       (1000) dev       (1000)     4152 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/shapedefs.h
--rw-rw-r--   0 dev       (1000) dev       (1000)     8991 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/slice.h
--rw-rw-r--   0 dev       (1000) dev       (1000)    10769 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/slice_test.cu
--rw-rw-r--   0 dev       (1000) dev       (1000)    14618 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/testutils.h
--rw-rw-r--   0 dev       (1000) dev       (1000)    11624 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/update.h
--rw-rw-r--   0 dev       (1000) dev       (1000)    28934 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/update_test.cu
--rw-rw-r--   0 dev       (1000) dev       (1000)     4314 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/verification.h
--rw-rw-r--   0 dev       (1000) dev       (1000)    12241 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/verification_test.cu
--rw-rw-r--   0 dev       (1000) dev       (1000)     5439 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/zcoeff.h
--rw-rw-r--   0 dev       (1000) dev       (1000)     2396 2023-05-02 23:06:13.000000 fdtdz-0.0.0/cuda/zcoeff_test.cu
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 16:10:36.863274 fdtdz-0.0.0/paper/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 16:10:36.867274 fdtdz-0.0.0/paper/fig/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1238 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/1d-helpers.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      788 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/2d-grids.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)     1689 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/2d-helpers.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      618 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/2d-te-diamond.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      499 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/2d-tm-diamond.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      433 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/2x2-cell.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      580 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/2x2-halo.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      692 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/3d-composite.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)     1544 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/3d-connect.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)     1932 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/3d-decomposition.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)     1432 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/3d-e-layer.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)     1878 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/3d-grids.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)     1354 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/3d-h-layer.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)     1203 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/3d-systolic.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)     1408 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/bandwidth-global.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      476 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/block-diamond.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      640 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/diagonal-drag.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)     1716 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/diamond-array.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      491 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/diamond-structure.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      842 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/empty-3d-grid.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      467 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/flat-drag.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      988 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/gpu-problem.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)     1162 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/gpu-systolic.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      642 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/left-drag.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)     1191 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/meta-diamond.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      283 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/single-yee-cell.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      228 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/zig-helpers.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)     1507 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/fig/zigzag.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)   188509 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/paper.pdf
--rw-rw-r--   0 dev       (1000) dev       (1000)    28237 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/paper.tex
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 16:10:36.867274 fdtdz-0.0.0/paper/tab/
--rw-rw-r--   0 dev       (1000) dev       (1000)      137 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/tab/bandwidth-shared.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      383 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/tab/data-channels.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      545 2023-05-02 23:06:13.000000 fdtdz-0.0.0/paper/tab/performance.tex
--rw-rw-r--   0 dev       (1000) dev       (1000)      220 2023-05-12 15:25:04.000000 fdtdz-0.0.0/pyproject.toml
--rw-rw-r--   0 dev       (1000) dev       (1000)       63 2023-05-12 16:10:37.063276 fdtdz-0.0.0/setup.cfg
--rw-rw-r--   0 dev       (1000) dev       (1000)     3387 2023-05-12 15:25:04.000000 fdtdz-0.0.0/setup.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 16:10:36.851274 fdtdz-0.0.0/src/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 16:10:36.871275 fdtdz-0.0.0/src/fdtdz.egg-info/
--rw-rw-r--   0 dev       (1000) dev       (1000)     6958 2023-05-12 16:10:36.000000 fdtdz-0.0.0/src/fdtdz.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)     6305 2023-05-12 16:10:36.000000 fdtdz-0.0.0/src/fdtdz.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-05-12 16:10:36.000000 fdtdz-0.0.0/src/fdtdz.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       26 2023-05-12 16:10:36.000000 fdtdz-0.0.0/src/fdtdz.egg-info/requires.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       10 2023-05-12 16:10:36.000000 fdtdz-0.0.0/src/fdtdz.egg-info/top_level.txt
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 16:10:36.871275 fdtdz-0.0.0/src/fdtdz_jax/
--rw-rw-r--   0 dev       (1000) dev       (1000)      187 2023-05-12 15:25:04.000000 fdtdz-0.0.0/src/fdtdz_jax/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)    23670 2023-05-12 15:25:04.000000 fdtdz-0.0.0/src/fdtdz_jax/fdtdz_jax.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      211 2023-05-12 15:25:04.000000 fdtdz-0.0.0/src/fdtdz_jax/fdtdz_jax_version.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 16:10:37.063276 fdtdz-0.0.0/src/fdtdz_jax/ptx/
--rw-rw-r--   0 dev       (1000) dev       (1000)   250216 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_0_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   250307 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_10_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   250368 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_1_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   250368 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_2_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   250368 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_3_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   250368 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_4_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   250298 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_5_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   250298 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_6_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   250298 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_7_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   250296 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_8_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   250368 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_9_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249607 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_0_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249698 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_10_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_1_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_2_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_3_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_4_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249689 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_5_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249689 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_6_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249689 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_7_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249687 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_8_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_9_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249607 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_0_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249698 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_10_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_1_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_2_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_3_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_4_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249689 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_5_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249689 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_6_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   224041 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_7_001.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   102463 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_7_010.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   237317 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_7_011.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   111684 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_7_100.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   243078 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_7_101.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   118610 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_7_110.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249689 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_7_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249687 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_8_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_9_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   237367 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_0_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   237458 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_10_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   237519 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_1_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   237519 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_2_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   237519 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_3_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   237519 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_4_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   237449 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_5_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   237449 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_6_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   237449 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_7_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   237447 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_8_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   237519 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_9_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135276 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_0_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135369 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_10_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135428 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_1_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135428 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_2_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135428 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_3_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135428 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_4_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135358 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_5_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135358 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_6_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135358 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_7_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135356 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_8_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135428 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_9_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135393 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_0_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135486 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_10_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135545 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_1_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135545 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_2_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135545 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_3_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135545 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_4_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135475 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_5_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135475 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_6_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135475 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_7_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135473 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_8_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   135545 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_9_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134687 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_0_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134780 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_10_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_1_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_2_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_3_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_4_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_5_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_6_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_7_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134767 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_8_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_9_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134687 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_0_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134780 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_10_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_1_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_2_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_3_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_4_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_5_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_6_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_7_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134767 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_8_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_9_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134687 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_0_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134780 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_10_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_1_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_2_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_3_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_4_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_5_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_6_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_7_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134767 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_8_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_9_111.ptx
--rw-rw-r--   0 dev       (1000) dev       (1000)     3412 2023-05-12 15:25:04.000000 fdtdz-0.0.0/src/fdtdz_jax/residual.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 16:10:37.063276 fdtdz-0.0.0/tests/
--rw-rw-r--   0 dev       (1000) dev       (1000)    13942 2023-05-12 15:25:04.000000 fdtdz-0.0.0/tests/test_fdtdz_jax.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 17:17:41.825710 fdtdz-1.0.1/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      932 2023-05-02 23:06:13.000000 fdtdz-1.0.1/CMakeLists.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1072 2023-04-29 07:29:27.000000 fdtdz-1.0.1/LICENSE
+-rw-rw-r--   0 dev       (1000) dev       (1000)       94 2023-05-02 23:06:13.000000 fdtdz-1.0.1/MANIFEST.in
+-rw-rw-r--   0 dev       (1000) dev       (1000)     8474 2023-05-12 17:17:41.825710 fdtdz-1.0.1/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)     8145 2023-05-12 16:41:15.000000 fdtdz-1.0.1/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 17:17:41.797710 fdtdz-1.0.1/cuda/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4337 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/CMakeLists.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)     6751 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/buffer.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4260 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/buffer_indexing.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)     6315 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/buffer_ops.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)    12667 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/buffer_test.cu
+-rw-rw-r--   0 dev       (1000) dev       (1000)     9028 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/cbuf.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)    11278 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/cbuf_test.cu
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2470 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/defs.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)      662 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/defs_test.cu
+-rw-rw-r--   0 dev       (1000) dev       (1000)    10537 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/diamond.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)     5889 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/diamond_test.cu
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3389 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/field.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1807 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/field_test.cu
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1514 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/jax_ops.cc
+-rw-rw-r--   0 dev       (1000) dev       (1000)     8067 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/kernel.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1380 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/kernel_helpers.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2398 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/kernel_jax.cc.cu
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2100 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/kernel_jax.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)      528 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/kernel_jax_test.cu
+-rw-rw-r--   0 dev       (1000) dev       (1000)     5102 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/kernel_precompiled.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1045 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/kernel_precompiled_test.cu
+-rw-rw-r--   0 dev       (1000) dev       (1000)      656 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/kernel_ptx.cu
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4247 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/kernel_test.cu
+-rw-rw-r--   0 dev       (1000) dev       (1000)      586 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/macros.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)      825 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/pybind11_kernel_helpers.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)     5622 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/reference.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)     6544 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/reference_test.cu
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4549 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/scanner.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2286 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/scanner_impl.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)    15743 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/scanner_test.cu
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4152 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/shapedefs.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)     8991 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/slice.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)    10769 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/slice_test.cu
+-rw-rw-r--   0 dev       (1000) dev       (1000)    14618 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/testutils.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)    11624 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/update.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)    28934 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/update_test.cu
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4314 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/verification.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)    12241 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/verification_test.cu
+-rw-rw-r--   0 dev       (1000) dev       (1000)     5439 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/zcoeff.h
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2396 2023-05-02 23:06:13.000000 fdtdz-1.0.1/cuda/zcoeff_test.cu
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 17:17:41.797710 fdtdz-1.0.1/paper/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 17:17:41.801710 fdtdz-1.0.1/paper/fig/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1238 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/1d-helpers.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      788 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/2d-grids.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1689 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/2d-helpers.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      618 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/2d-te-diamond.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      499 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/2d-tm-diamond.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      433 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/2x2-cell.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      580 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/2x2-halo.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      692 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/3d-composite.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1544 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/3d-connect.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1932 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/3d-decomposition.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1432 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/3d-e-layer.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1878 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/3d-grids.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1354 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/3d-h-layer.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1203 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/3d-systolic.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1408 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/bandwidth-global.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      476 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/block-diamond.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      640 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/diagonal-drag.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1716 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/diamond-array.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      491 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/diamond-structure.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      842 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/empty-3d-grid.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      467 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/flat-drag.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      988 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/gpu-problem.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1162 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/gpu-systolic.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      642 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/left-drag.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1191 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/meta-diamond.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      283 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/single-yee-cell.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      228 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/zig-helpers.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1507 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/fig/zigzag.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)   188509 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/paper.pdf
+-rw-rw-r--   0 dev       (1000) dev       (1000)    28237 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/paper.tex
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 17:17:41.801710 fdtdz-1.0.1/paper/tab/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      137 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/tab/bandwidth-shared.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      383 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/tab/data-channels.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      545 2023-05-02 23:06:13.000000 fdtdz-1.0.1/paper/tab/performance.tex
+-rw-rw-r--   0 dev       (1000) dev       (1000)      220 2023-05-12 17:04:15.000000 fdtdz-1.0.1/pyproject.toml
+-rw-rw-r--   0 dev       (1000) dev       (1000)       63 2023-05-12 17:17:41.825710 fdtdz-1.0.1/setup.cfg
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3452 2023-05-12 17:16:58.000000 fdtdz-1.0.1/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 17:17:41.793710 fdtdz-1.0.1/src/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 17:17:41.801710 fdtdz-1.0.1/src/fdtdz.egg-info/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     8474 2023-05-12 17:17:41.000000 fdtdz-1.0.1/src/fdtdz.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)     6305 2023-05-12 17:17:41.000000 fdtdz-1.0.1/src/fdtdz.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-05-12 17:17:41.000000 fdtdz-1.0.1/src/fdtdz.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       26 2023-05-12 17:17:41.000000 fdtdz-1.0.1/src/fdtdz.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       10 2023-05-12 17:17:41.000000 fdtdz-1.0.1/src/fdtdz.egg-info/top_level.txt
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 17:17:41.801710 fdtdz-1.0.1/src/fdtdz_jax/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      187 2023-05-12 16:41:15.000000 fdtdz-1.0.1/src/fdtdz_jax/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)    23670 2023-05-12 16:41:15.000000 fdtdz-1.0.1/src/fdtdz_jax/fdtdz_jax.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      160 2023-05-12 17:17:41.000000 fdtdz-1.0.1/src/fdtdz_jax/fdtdz_jax_version.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 17:17:41.825710 fdtdz-1.0.1/src/fdtdz_jax/ptx/
+-rw-rw-r--   0 dev       (1000) dev       (1000)   250216 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_0_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   250307 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_10_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   250368 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_1_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   250368 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_2_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   250368 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_3_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   250368 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_4_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   250298 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_5_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   250298 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_6_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   250298 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_7_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   250296 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_8_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   250368 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_9_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249607 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_0_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249698 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_10_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_1_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_2_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_3_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_4_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249689 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_5_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249689 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_6_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249689 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_7_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249687 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_8_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_9_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249607 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_0_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249698 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_10_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_1_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_2_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_3_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_4_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249689 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_5_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249689 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_6_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   224041 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_7_001.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   102463 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_7_010.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   237317 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_7_011.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   111684 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_7_100.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   243078 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_7_101.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   118610 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_7_110.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249689 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_7_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249687 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_8_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   249759 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_9_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   237367 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_0_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   237458 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_10_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   237519 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_1_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   237519 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_2_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   237519 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_3_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   237519 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_4_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   237449 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_5_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   237449 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_6_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   237449 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_7_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   237447 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_8_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   237519 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_9_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135276 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_0_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135369 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_10_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135428 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_1_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135428 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_2_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135428 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_3_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135428 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_4_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135358 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_5_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135358 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_6_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135358 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_7_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135356 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_8_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135428 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_9_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135393 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_0_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135486 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_10_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135545 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_1_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135545 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_2_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135545 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_3_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135545 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_4_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135475 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_5_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135475 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_6_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135475 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_7_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135473 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_8_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   135545 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_9_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134687 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_0_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134780 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_10_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_1_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_2_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_3_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_4_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_5_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_6_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_7_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134767 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_8_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_9_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134687 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_0_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134780 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_10_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_1_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_2_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_3_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_4_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_5_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_6_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_7_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134767 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_8_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_9_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134687 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_0_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134780 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_10_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_1_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_2_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_3_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_4_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_5_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_6_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134769 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_7_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134767 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_8_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134837 2023-05-02 23:06:13.000000 fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_9_111.ptx
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3412 2023-05-12 16:41:15.000000 fdtdz-1.0.1/src/fdtdz_jax/residual.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-12 17:17:41.825710 fdtdz-1.0.1/tests/
+-rw-rw-r--   0 dev       (1000) dev       (1000)    13942 2023-05-12 16:41:15.000000 fdtdz-1.0.1/tests/test_fdtdz_jax.py
```

### Comparing `fdtdz-0.0.0/CMakeLists.txt` & `fdtdz-1.0.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/LICENSE` & `fdtdz-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/PKG-INFO` & `fdtdz-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,35 @@
-Metadata-Version: 2.1
-Name: fdtdz
-Version: 0.0.0
-Summary: Fast, scalable, and free photonic simulation
-Home-page: https://github.com/spinsphotonics/fdtdz
-Author: Jesse Lu
-Author-email: jesselu@spinsphotonics.com
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # [*fdtd-z*](github.com/spinsphotonics/fdtdz) -- fast, scalable, and free photonic simulation
 ***fdtd-z*** is our first step in *revolutionizing photonic design* by enabling photonic engineers to **harness compute at scale**.
 
 * **fast**: 100x faster than CPU implementations such as Meep, Lumerical, RSoft, ..., 
 * **scalable**: easily runs simulations on hundreds of nodes and beyond,
 * **free**: open-source, no license-fees!
 
 Give it a test drive [![in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/jlu-spins/0f3c5459bd4386150ae30b17f7c6a5e3/welcome-to-fdtd-z.ipynb),
 join the chat [![on https://gitter.im/fdtdz/community](https://badges.gitter.im/fdtdz/community.svg)](https://app.gitter.im/#/room/#fdtdz:gitter.im), and read the [whitepaper](paper/paper.pdf).
 
+### API
+
+***fdtd-z*** exposes a low-level API `fdtdz()` to launch FDTD kernels on the GPU while giving the user fine-grained control over values for permittivity, current source, boundary conditions, and more.
+
+In order to optimize the simulation throughput for nanophotonic applications, a number of constraints are placed on the allowable inputs such as limited dimension of the z-axis, simple non-absorbing dielectric materials only, and adiabatic absorption boundaries along the x- and y-axes.
+See the `fdtdz()` docstring for all the details.
+
+While it does not include all the bells and whistles, it is *fast*: delivering ~100X speed-up compared to MEEP/Lumerical even on commodity GPUs such as the Nvidia T4; and we're looking forward to building out the required functionality with the open-source photonics community!
+
+That said, don't take our word for it, [try it out for yourself](https://colab.research.google.com/gist/jlu-spins/0f3c5459bd4386150ae30b17f7c6a5e3/welcome-to-fdtd-z.ipynb)!
+
+### Install
+
+You must have the GPU-version of [JAX](https://github.com/google/jax) installed first, see [instructions here](https://github.com/google/jax#pip-installation-gpu-cuda-installed-via-pip-easier).
+Once this is done, you can just do `pip install fdtdz`.
+
+Of course, you can always circumvent things and just `!pip install fdtdz` directly from a Colab notebook as is done in the [example notebook](https://colab.research.google.com/gist/jlu-spins/0f3c5459bd4386150ae30b17f7c6a5e3/welcome-to-fdtd-z.ipynb).
+
 ## Frequently Asked Questions
 
 ### Is the plan to build additional functionality inside the *fdtd-z* repo?
 
 *fdtd-z* is intended to be a super low-level utility in the UNIX philosophy of "just do one thing".
 As such, a number of seemingly critical functionality is intentionally missing such as waveguide mode solving, utilities for building dielectric structures, and more.
 
@@ -66,9 +71,7 @@
 ### `CUDA_ERROR_COOPERATIVE_LAUNCH_TOO_LARGE`
 
 *fdtd-z* uses CUDA [cooperative groups](https://docs.nvidia.com/cuda/cuda-c-programming-guide/#cooperative-groups) to implement the systolic scheme outlined in the [whitepaper](paper/paper.pdf) and get around the GPU bandwidth bottleneck.
 Because of this, the [launch parameters](https://docs.nvidia.com/cuda/cuda-c-programming-guide/#thread-hierarchy) of the kernel become tightly connected to the underlying architecture of the GPU. 
 In particular the `(gridu, gridv)` part of the launch parameters must not exceed the number of streaming multiprocessors (SMs) that are on the GPU.
 For example, the RTX4000 has 36 GPUs so it would make sense to use `(gridu, gridv) = (6, 6)` (note that there is the additional constraint that `blocku * gridu <= blockv * gridv`).
 If `gridu * gridv` is greater than the number of available GPUs, then an attempt to launch the kernel will result in the `CUDA_ERROR_COOPERATIVE_LAUNCH_TOO_LARGE` error.
-
-
```

### Comparing `fdtdz-0.0.0/README.md` & `fdtdz-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,48 @@
+Metadata-Version: 2.1
+Name: fdtdz
+Version: 1.0.1
+Summary: Fast, scalable, and free photonic simulation
+Home-page: https://github.com/spinsphotonics/fdtdz
+Author: Jesse Lu
+Author-email: jesselu@spinsphotonics.com
+License: MIT
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # [*fdtd-z*](github.com/spinsphotonics/fdtdz) -- fast, scalable, and free photonic simulation
 ***fdtd-z*** is our first step in *revolutionizing photonic design* by enabling photonic engineers to **harness compute at scale**.
 
 * **fast**: 100x faster than CPU implementations such as Meep, Lumerical, RSoft, ..., 
 * **scalable**: easily runs simulations on hundreds of nodes and beyond,
 * **free**: open-source, no license-fees!
 
 Give it a test drive [![in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/jlu-spins/0f3c5459bd4386150ae30b17f7c6a5e3/welcome-to-fdtd-z.ipynb),
 join the chat [![on https://gitter.im/fdtdz/community](https://badges.gitter.im/fdtdz/community.svg)](https://app.gitter.im/#/room/#fdtdz:gitter.im), and read the [whitepaper](paper/paper.pdf).
 
+### API
+
+***fdtd-z*** exposes a low-level API `fdtdz()` to launch FDTD kernels on the GPU while giving the user fine-grained control over values for permittivity, current source, boundary conditions, and more.
+
+In order to optimize the simulation throughput for nanophotonic applications, a number of constraints are placed on the allowable inputs such as limited dimension of the z-axis, simple non-absorbing dielectric materials only, and adiabatic absorption boundaries along the x- and y-axes.
+See the `fdtdz()` docstring for all the details.
+
+While it does not include all the bells and whistles, it is *fast*: delivering ~100X speed-up compared to MEEP/Lumerical even on commodity GPUs such as the Nvidia T4; and we're looking forward to building out the required functionality with the open-source photonics community!
+
+That said, don't take our word for it, [try it out for yourself](https://colab.research.google.com/gist/jlu-spins/0f3c5459bd4386150ae30b17f7c6a5e3/welcome-to-fdtd-z.ipynb)!
+
+### Install
+
+You must have the GPU-version of [JAX](https://github.com/google/jax) installed first, see [instructions here](https://github.com/google/jax#pip-installation-gpu-cuda-installed-via-pip-easier).
+Once this is done, you can just do `pip install fdtdz`.
+
+Of course, you can always circumvent things and just `!pip install fdtdz` directly from a Colab notebook as is done in the [example notebook](https://colab.research.google.com/gist/jlu-spins/0f3c5459bd4386150ae30b17f7c6a5e3/welcome-to-fdtd-z.ipynb).
+
 ## Frequently Asked Questions
 
 ### Is the plan to build additional functionality inside the *fdtd-z* repo?
 
 *fdtd-z* is intended to be a super low-level utility in the UNIX philosophy of "just do one thing".
 As such, a number of seemingly critical functionality is intentionally missing such as waveguide mode solving, utilities for building dielectric structures, and more.
 
@@ -53,7 +84,9 @@
 ### `CUDA_ERROR_COOPERATIVE_LAUNCH_TOO_LARGE`
 
 *fdtd-z* uses CUDA [cooperative groups](https://docs.nvidia.com/cuda/cuda-c-programming-guide/#cooperative-groups) to implement the systolic scheme outlined in the [whitepaper](paper/paper.pdf) and get around the GPU bandwidth bottleneck.
 Because of this, the [launch parameters](https://docs.nvidia.com/cuda/cuda-c-programming-guide/#thread-hierarchy) of the kernel become tightly connected to the underlying architecture of the GPU. 
 In particular the `(gridu, gridv)` part of the launch parameters must not exceed the number of streaming multiprocessors (SMs) that are on the GPU.
 For example, the RTX4000 has 36 GPUs so it would make sense to use `(gridu, gridv) = (6, 6)` (note that there is the additional constraint that `blocku * gridu <= blockv * gridv`).
 If `gridu * gridv` is greater than the number of available GPUs, then an attempt to launch the kernel will result in the `CUDA_ERROR_COOPERATIVE_LAUNCH_TOO_LARGE` error.
+
+
```

### Comparing `fdtdz-0.0.0/cuda/CMakeLists.txt` & `fdtdz-1.0.1/cuda/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/buffer.h` & `fdtdz-1.0.1/cuda/buffer.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/buffer_indexing.h` & `fdtdz-1.0.1/cuda/buffer_indexing.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/buffer_ops.h` & `fdtdz-1.0.1/cuda/buffer_ops.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/buffer_test.cu` & `fdtdz-1.0.1/cuda/buffer_test.cu`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/cbuf.h` & `fdtdz-1.0.1/cuda/cbuf.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/cbuf_test.cu` & `fdtdz-1.0.1/cuda/cbuf_test.cu`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/defs.h` & `fdtdz-1.0.1/cuda/defs.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/defs_test.cu` & `fdtdz-1.0.1/cuda/defs_test.cu`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/diamond.h` & `fdtdz-1.0.1/cuda/diamond.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/diamond_test.cu` & `fdtdz-1.0.1/cuda/diamond_test.cu`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/field.h` & `fdtdz-1.0.1/cuda/field.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/field_test.cu` & `fdtdz-1.0.1/cuda/field_test.cu`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/jax_ops.cc` & `fdtdz-1.0.1/cuda/jax_ops.cc`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/kernel.h` & `fdtdz-1.0.1/cuda/kernel.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/kernel_helpers.h` & `fdtdz-1.0.1/cuda/kernel_helpers.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/kernel_jax.cc.cu` & `fdtdz-1.0.1/cuda/kernel_jax.cc.cu`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/kernel_jax.h` & `fdtdz-1.0.1/cuda/kernel_jax.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/kernel_jax_test.cu` & `fdtdz-1.0.1/cuda/kernel_jax_test.cu`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/kernel_precompiled.h` & `fdtdz-1.0.1/cuda/kernel_precompiled.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/kernel_precompiled_test.cu` & `fdtdz-1.0.1/cuda/kernel_precompiled_test.cu`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/kernel_ptx.cu` & `fdtdz-1.0.1/cuda/kernel_ptx.cu`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/kernel_test.cu` & `fdtdz-1.0.1/cuda/kernel_test.cu`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/macros.h` & `fdtdz-1.0.1/cuda/macros.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/pybind11_kernel_helpers.h` & `fdtdz-1.0.1/cuda/pybind11_kernel_helpers.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/reference.h` & `fdtdz-1.0.1/cuda/reference.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/reference_test.cu` & `fdtdz-1.0.1/cuda/reference_test.cu`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/scanner.h` & `fdtdz-1.0.1/cuda/scanner.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/scanner_impl.h` & `fdtdz-1.0.1/cuda/scanner_impl.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/scanner_test.cu` & `fdtdz-1.0.1/cuda/scanner_test.cu`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/shapedefs.h` & `fdtdz-1.0.1/cuda/shapedefs.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/slice.h` & `fdtdz-1.0.1/cuda/slice.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/slice_test.cu` & `fdtdz-1.0.1/cuda/slice_test.cu`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/testutils.h` & `fdtdz-1.0.1/cuda/testutils.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/update.h` & `fdtdz-1.0.1/cuda/update.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/update_test.cu` & `fdtdz-1.0.1/cuda/update_test.cu`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/verification.h` & `fdtdz-1.0.1/cuda/verification.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/verification_test.cu` & `fdtdz-1.0.1/cuda/verification_test.cu`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/zcoeff.h` & `fdtdz-1.0.1/cuda/zcoeff.h`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/cuda/zcoeff_test.cu` & `fdtdz-1.0.1/cuda/zcoeff_test.cu`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/1d-helpers.tex` & `fdtdz-1.0.1/paper/fig/1d-helpers.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/2d-grids.tex` & `fdtdz-1.0.1/paper/fig/2d-grids.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/2d-helpers.tex` & `fdtdz-1.0.1/paper/fig/2d-helpers.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/2d-te-diamond.tex` & `fdtdz-1.0.1/paper/fig/2d-te-diamond.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/2x2-halo.tex` & `fdtdz-1.0.1/paper/fig/2x2-halo.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/3d-composite.tex` & `fdtdz-1.0.1/paper/fig/3d-composite.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/3d-connect.tex` & `fdtdz-1.0.1/paper/fig/3d-connect.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/3d-decomposition.tex` & `fdtdz-1.0.1/paper/fig/3d-decomposition.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/3d-e-layer.tex` & `fdtdz-1.0.1/paper/fig/3d-e-layer.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/3d-grids.tex` & `fdtdz-1.0.1/paper/fig/3d-grids.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/3d-h-layer.tex` & `fdtdz-1.0.1/paper/fig/3d-h-layer.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/3d-systolic.tex` & `fdtdz-1.0.1/paper/fig/3d-systolic.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/bandwidth-global.tex` & `fdtdz-1.0.1/paper/fig/bandwidth-global.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/diagonal-drag.tex` & `fdtdz-1.0.1/paper/fig/diagonal-drag.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/diamond-array.tex` & `fdtdz-1.0.1/paper/fig/diamond-array.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/empty-3d-grid.tex` & `fdtdz-1.0.1/paper/fig/empty-3d-grid.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/gpu-problem.tex` & `fdtdz-1.0.1/paper/fig/gpu-problem.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/gpu-systolic.tex` & `fdtdz-1.0.1/paper/fig/gpu-systolic.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/left-drag.tex` & `fdtdz-1.0.1/paper/fig/left-drag.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/meta-diamond.tex` & `fdtdz-1.0.1/paper/fig/meta-diamond.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/fig/zigzag.tex` & `fdtdz-1.0.1/paper/fig/zigzag.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/paper.pdf` & `fdtdz-1.0.1/paper/paper.pdf`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/paper.tex` & `fdtdz-1.0.1/paper/paper.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/paper/tab/performance.tex` & `fdtdz-1.0.1/paper/tab/performance.tex`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/setup.py` & `fdtdz-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,11 +99,13 @@
     description=("Fast, scalable, and free photonic simulation"),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     install_requires=["jax", "jaxlib"],
+    setup_requires=["setuptools_scm"],
+    use_scm_version=True,
     extras_require={"test": "pytest"},
     ext_modules=extensions,
     cmdclass={"build_ext": CMakeBuildExt},
 )
```

### Comparing `fdtdz-0.0.0/src/fdtdz.egg-info/PKG-INFO` & `fdtdz-1.0.1/src/fdtdz.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdtdz
-Version: 0.0.0
+Version: 1.0.1
 Summary: Fast, scalable, and free photonic simulation
 Home-page: https://github.com/spinsphotonics/fdtdz
 Author: Jesse Lu
 Author-email: jesselu@spinsphotonics.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -17,14 +17,32 @@
 * **fast**: 100x faster than CPU implementations such as Meep, Lumerical, RSoft, ..., 
 * **scalable**: easily runs simulations on hundreds of nodes and beyond,
 * **free**: open-source, no license-fees!
 
 Give it a test drive [![in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/jlu-spins/0f3c5459bd4386150ae30b17f7c6a5e3/welcome-to-fdtd-z.ipynb),
 join the chat [![on https://gitter.im/fdtdz/community](https://badges.gitter.im/fdtdz/community.svg)](https://app.gitter.im/#/room/#fdtdz:gitter.im), and read the [whitepaper](paper/paper.pdf).
 
+### API
+
+***fdtd-z*** exposes a low-level API `fdtdz()` to launch FDTD kernels on the GPU while giving the user fine-grained control over values for permittivity, current source, boundary conditions, and more.
+
+In order to optimize the simulation throughput for nanophotonic applications, a number of constraints are placed on the allowable inputs such as limited dimension of the z-axis, simple non-absorbing dielectric materials only, and adiabatic absorption boundaries along the x- and y-axes.
+See the `fdtdz()` docstring for all the details.
+
+While it does not include all the bells and whistles, it is *fast*: delivering ~100X speed-up compared to MEEP/Lumerical even on commodity GPUs such as the Nvidia T4; and we're looking forward to building out the required functionality with the open-source photonics community!
+
+That said, don't take our word for it, [try it out for yourself](https://colab.research.google.com/gist/jlu-spins/0f3c5459bd4386150ae30b17f7c6a5e3/welcome-to-fdtd-z.ipynb)!
+
+### Install
+
+You must have the GPU-version of [JAX](https://github.com/google/jax) installed first, see [instructions here](https://github.com/google/jax#pip-installation-gpu-cuda-installed-via-pip-easier).
+Once this is done, you can just do `pip install fdtdz`.
+
+Of course, you can always circumvent things and just `!pip install fdtdz` directly from a Colab notebook as is done in the [example notebook](https://colab.research.google.com/gist/jlu-spins/0f3c5459bd4386150ae30b17f7c6a5e3/welcome-to-fdtd-z.ipynb).
+
 ## Frequently Asked Questions
 
 ### Is the plan to build additional functionality inside the *fdtd-z* repo?
 
 *fdtd-z* is intended to be a super low-level utility in the UNIX philosophy of "just do one thing".
 As such, a number of seemingly critical functionality is intentionally missing such as waveguide mode solving, utilities for building dielectric structures, and more.
```

### Comparing `fdtdz-0.0.0/src/fdtdz.egg-info/SOURCES.txt` & `fdtdz-1.0.1/src/fdtdz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/fdtdz_jax.py` & `fdtdz-1.0.1/src/fdtdz_jax/fdtdz_jax.py`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_0_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_0_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_10_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_10_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_1_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_1_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_2_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_2_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_3_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_3_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_4_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_4_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_5_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_5_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_6_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_6_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_7_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_7_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_8_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_8_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_60_9_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_60_9_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_0_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_0_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_10_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_10_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_1_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_1_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_2_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_2_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_3_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_3_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_4_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_4_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_5_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_5_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_6_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_6_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_7_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_7_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_8_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_8_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_70_9_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_70_9_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_0_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_0_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_10_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_10_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_1_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_1_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_2_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_2_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_3_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_3_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_4_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_4_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_5_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_5_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_6_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_6_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_7_001.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_7_001.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_7_010.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_7_010.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_7_011.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_7_011.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_7_100.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_7_100.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_7_101.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_7_101.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_7_110.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_7_110.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_7_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_7_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_8_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_8_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_75_9_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_75_9_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_0_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_0_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_10_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_10_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_1_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_1_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_2_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_2_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_3_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_3_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_4_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_4_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_5_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_5_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_6_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_6_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_7_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_7_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_8_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_8_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_16_80_9_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_16_80_9_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_0_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_0_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_10_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_10_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_1_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_1_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_2_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_2_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_3_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_3_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_4_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_4_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_5_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_5_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_6_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_6_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_7_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_7_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_8_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_8_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_37_9_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_37_9_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_0_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_0_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_10_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_10_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_1_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_1_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_2_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_2_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_3_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_3_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_4_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_4_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_5_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_5_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_6_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_6_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_7_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_7_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_8_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_8_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_60_9_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_60_9_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_0_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_0_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_10_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_10_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_1_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_1_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_2_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_2_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_3_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_3_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_4_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_4_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_5_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_5_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_6_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_6_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_7_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_7_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_8_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_8_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_70_9_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_70_9_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_0_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_0_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_10_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_10_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_1_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_1_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_2_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_2_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_3_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_3_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_4_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_4_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_5_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_5_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_6_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_6_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_7_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_7_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_8_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_8_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_75_9_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_75_9_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_0_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_0_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_10_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_10_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_1_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_1_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_2_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_2_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_3_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_3_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_4_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_4_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_5_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_5_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_6_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_6_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_7_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_7_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_8_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_8_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/ptx/kernel_32_80_9_111.ptx` & `fdtdz-1.0.1/src/fdtdz_jax/ptx/kernel_32_80_9_111.ptx`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/src/fdtdz_jax/residual.py` & `fdtdz-1.0.1/src/fdtdz_jax/residual.py`

 * *Files identical despite different names*

### Comparing `fdtdz-0.0.0/tests/test_fdtdz_jax.py` & `fdtdz-1.0.1/tests/test_fdtdz_jax.py`

 * *Files identical despite different names*

