# Comparing `tmp/matfree-0.0.6.tar.gz` & `tmp/matfree-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matfree-0.0.6.tar", last modified: Thu May 11 05:39:24 2023, max compression
+gzip compressed data, was "matfree-0.0.7.tar", last modified: Fri May 12 07:51:56 2023, max compression
```

## Comparing `matfree-0.0.6.tar` & `matfree-0.0.7.tar`

### file list

```diff
@@ -1,86 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.995245 matfree-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.979245 matfree-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.983245 matfree-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-11 05:39:06.000000 matfree-0.0.6/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-11 05:39:06.000000 matfree-0.0.6/.github/workflows/doc-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-11 05:39:06.000000 matfree-0.0.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-11 05:39:06.000000 matfree-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-11 05:39:06.000000 matfree-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-11 05:39:06.000000 matfree-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-11 05:39:06.000000 matfree-0.0.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-11 05:39:24.995245 matfree-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-11 05:39:06.000000 matfree-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.983245 matfree-0.0.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.983245 matfree-0.0.6/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/api/decomp.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/api/hutchinson.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/api/montecarlo.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/api/slq.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.987245 matfree-0.0.6/docs/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/benchmarks/control_variates.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/benchmarks/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/benchmarks/jacobian_squared.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/control_variates.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.987245 matfree-0.0.6/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/dev/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/higher_moments.md
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.987245 matfree-0.0.6/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/log_determinants.md
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/vector_calculus.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.987245 matfree-0.0.6/matfree/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-11 05:39:24.000000 matfree-0.0.6/matfree/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.991245 matfree-0.0.6/matfree/backend/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/control_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/func.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/np.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/plt.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/prng.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/benchmark_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/decomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/hutchinson.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/slq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.987245 matfree-0.0.6/matfree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-11 05:39:24.000000 matfree-0.0.6/matfree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-11 05:39:24.000000 matfree-0.0.6/matfree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 05:39:24.000000 matfree-0.0.6/matfree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-11 05:39:24.000000 matfree-0.0.6/matfree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 05:39:24.000000 matfree-0.0.6/matfree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-11 05:39:06.000000 matfree-0.0.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-11 05:39:06.000000 matfree-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-11 05:39:24.995245 matfree-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-11 05:39:06.000000 matfree-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.991245 matfree-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.991245 matfree-0.0.6/tests/test_decomp/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_decomp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_decomp/test_gkl_full_reortho.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_decomp/test_lanczos_full_reortho.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_decomp/test_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.991245 matfree-0.0.6/tests/test_hutchinson/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_hutchinson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_hutchinson/test_diagonal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_hutchinson/test_frobeniusnorm_squared.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_hutchinson/test_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_hutchinson/test_trace_and_diagonal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_hutchinson/test_trace_moments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.995245 matfree-0.0.6/tests/test_montecarlo/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_montecarlo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_montecarlo/test_estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_montecarlo/test_multiestimate.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_montecarlo/test_van_der_corput.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.995245 matfree-0.0.6/tests/test_slq/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_slq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_slq/test_logdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_slq/test_logdet_autodiff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:51:56.914090 matfree-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:51:56.902089 matfree-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:51:56.906090 matfree-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-12 07:51:36.000000 matfree-0.0.7/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-12 07:51:36.000000 matfree-0.0.7/.github/workflows/doc-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-12 07:51:36.000000 matfree-0.0.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-12 07:51:36.000000 matfree-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-12 07:51:36.000000 matfree-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-12 07:51:36.000000 matfree-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-12 07:51:36.000000 matfree-0.0.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-12 07:51:56.914090 matfree-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-12 07:51:36.000000 matfree-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:51:56.906090 matfree-0.0.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:51:56.906090 matfree-0.0.7/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-12 07:51:36.000000 matfree-0.0.7/docs/api/decomp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 07:51:36.000000 matfree-0.0.7/docs/api/hutchinson.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 07:51:36.000000 matfree-0.0.7/docs/api/montecarlo.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 07:51:36.000000 matfree-0.0.7/docs/api/slq.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:51:56.906090 matfree-0.0.7/docs/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-12 07:51:36.000000 matfree-0.0.7/docs/benchmarks/control_variates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-12 07:51:36.000000 matfree-0.0.7/docs/benchmarks/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-12 07:51:36.000000 matfree-0.0.7/docs/benchmarks/jacobian_squared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-12 07:51:36.000000 matfree-0.0.7/docs/control_variates.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:51:56.906090 matfree-0.0.7/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-12 07:51:36.000000 matfree-0.0.7/docs/dev/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-12 07:51:36.000000 matfree-0.0.7/docs/higher_moments.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-12 07:51:36.000000 matfree-0.0.7/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:51:56.906090 matfree-0.0.7/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-12 07:51:36.000000 matfree-0.0.7/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-12 07:51:36.000000 matfree-0.0.7/docs/log_determinants.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-12 07:51:36.000000 matfree-0.0.7/docs/vector_calculus.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:51:56.910090 matfree-0.0.7/matfree/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-12 07:51:56.000000 matfree-0.0.7/matfree/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:51:56.910090 matfree-0.0.7/matfree/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/backend/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/backend/control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/backend/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/backend/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/backend/np.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/backend/plt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/backend/prng.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/backend/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/backend/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/backend/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/backend/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/benchmark_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/decomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/hutchinson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/montecarlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/slq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-12 07:51:36.000000 matfree-0.0.7/matfree/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:51:56.910090 matfree-0.0.7/matfree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-12 07:51:56.000000 matfree-0.0.7/matfree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-12 07:51:56.000000 matfree-0.0.7/matfree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 07:51:56.000000 matfree-0.0.7/matfree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-12 07:51:56.000000 matfree-0.0.7/matfree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 07:51:56.000000 matfree-0.0.7/matfree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-12 07:51:36.000000 matfree-0.0.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-12 07:51:36.000000 matfree-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-12 07:51:56.914090 matfree-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-12 07:51:36.000000 matfree-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:51:56.910090 matfree-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:51:56.910090 matfree-0.0.7/tests/test_decomp/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_decomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_decomp/test_gkl_full_reortho.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_decomp/test_lanczos_full_reortho.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_decomp/test_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:51:56.914090 matfree-0.0.7/tests/test_hutchinson/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_hutchinson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_hutchinson/test_diagonal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_hutchinson/test_frobeniusnorm_squared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_hutchinson/test_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_hutchinson/test_trace_and_diagonal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_hutchinson/test_trace_moments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:51:56.914090 matfree-0.0.7/tests/test_montecarlo/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_montecarlo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_montecarlo/test_estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_montecarlo/test_multiestimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_montecarlo/test_van_der_corput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:51:56.914090 matfree-0.0.7/tests/test_slq/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_slq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_slq/test_logdet_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_slq/test_logdet_spd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_slq/test_logdet_spd_autodiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-12 07:51:36.000000 matfree-0.0.7/tests/test_slq/test_schatten_norm.py
```

### Comparing `matfree-0.0.6/.github/workflows/ci.yaml` & `matfree-0.0.7/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/.github/workflows/doc-publish.yml` & `matfree-0.0.7/.github/workflows/doc-publish.yml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/.github/workflows/release.yml` & `matfree-0.0.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/.gitignore` & `matfree-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/.pre-commit-config.yaml` & `matfree-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/LICENSE` & `matfree-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/PKG-INFO` & `matfree-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matfree
-Version: 0.0.6
+Version: 0.0.7
 Summary: Matrix-free numerical linear algebra including trace-estimation.
 Author: Nicholas Krämer
 Author-email: pekra@dtu.dk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cpu
@@ -49,32 +49,32 @@
 >>> a = jnp.reshape(jnp.arange(12.0), (6, 2))
 >>> key = jax.random.PRNGKey(1)
 
 ```
 
 Estimate traces as such:
 ```python
->>> sample_fun = montecarlo.normal(shape=(2,))
+>>> normal = montecarlo.normal(shape=(2,))
 >>> matvec = lambda x: a.T @ (a @ x)
->>> trace = hutchinson.trace(matvec, key=key, sample_fun=sample_fun)
+>>> trace = hutchinson.trace(matvec, key=key, sample_fun=normal)
 >>> print(jnp.round(trace))
 514.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 ```
 The number of keys determines the number of sequential batches.
 Many small batches reduces memory.
 Few large batches increases memory and runtime.
 
 Determine the number of samples per batch as follows.
 
 ```python
->>> trace = hutchinson.trace(matvec, key=key, sample_fun=sample_fun, num_batches=10)
+>>> trace = hutchinson.trace(matvec, key=key, sample_fun=normal, num_batches=10)
 >>> print(jnp.round(trace))
 508.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 ```
```

### Comparing `matfree-0.0.6/README.md` & `matfree-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -32,32 +32,32 @@
 >>> a = jnp.reshape(jnp.arange(12.0), (6, 2))
 >>> key = jax.random.PRNGKey(1)
 
 ```
 
 Estimate traces as such:
 ```python
->>> sample_fun = montecarlo.normal(shape=(2,))
+>>> normal = montecarlo.normal(shape=(2,))
 >>> matvec = lambda x: a.T @ (a @ x)
->>> trace = hutchinson.trace(matvec, key=key, sample_fun=sample_fun)
+>>> trace = hutchinson.trace(matvec, key=key, sample_fun=normal)
 >>> print(jnp.round(trace))
 514.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 ```
 The number of keys determines the number of sequential batches.
 Many small batches reduces memory.
 Few large batches increases memory and runtime.
 
 Determine the number of samples per batch as follows.
 
 ```python
->>> trace = hutchinson.trace(matvec, key=key, sample_fun=sample_fun, num_batches=10)
+>>> trace = hutchinson.trace(matvec, key=key, sample_fun=normal, num_batches=10)
 >>> print(jnp.round(trace))
 508.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 ```
```

### Comparing `matfree-0.0.6/docs/benchmarks/control_variates.py` & `matfree-0.0.7/docs/benchmarks/control_variates.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/docs/benchmarks/jacobian_squared.py` & `matfree-0.0.7/docs/benchmarks/jacobian_squared.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     dim = 10
     num_samples = 2 ** np.arange(4, 12)
     num_restarts = 10
 
     (matfun, jvp, Av, trace, JJ), (k, sample_fun) = problem(dim)
 
     x = hutchinson.trace(Av, key=k, sample_fun=sample_fun)
-    y = slq.trace_of_matfun_symmetric(matfun, jvp, 5, key=k, sample_fun=sample_fun)
+    y = slq.trace_of_matfun_spd(matfun, jvp, 5, key=k, sample_fun=sample_fun)
     assert np.allclose(x, trace, atol=1e-1, rtol=1e-1), (x, trace)
     assert np.allclose(y, trace, atol=1e-1, rtol=1e-1), (y, trace)
 
     error_fun = func.partial(benchmark_util.rmse_relative, expected=trace)
 
     @func.partial(benchmark_util.error_and_time, error_fun=error_fun)
     @func.partial(func.jit, static_argnums=0)
@@ -70,28 +70,28 @@
             Av, key=key, sample_fun=sample_fun, num_samples_per_batch=num
         )
 
     @func.partial(benchmark_util.error_and_time, error_fun=error_fun)
     @func.partial(func.jit, static_argnums=0)
     def slq_low(num, key):
         """SLQ(1)"""  # noqa: D400,D415
-        return slq.trace_of_matfun_symmetric(
+        return slq.trace_of_matfun_spd(
             matfun,
             jvp,
             1,
             key=key,
             sample_fun=sample_fun,
             num_samples_per_batch=num,
         )
 
     @func.partial(benchmark_util.error_and_time, error_fun=error_fun)
     @func.partial(func.jit, static_argnums=0)
     def slq_high(num, key):
         """SLQ(5)"""  # noqa: D400,D415
-        return slq.trace_of_matfun_symmetric(
+        return slq.trace_of_matfun_spd(
             matfun,
             jvp,
             5,
             key=key,
             sample_fun=sample_fun,
             num_samples_per_batch=num,
         )
```

### Comparing `matfree-0.0.6/docs/control_variates.md` & `matfree-0.0.7/docs/control_variates.md`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/docs/dev/index.md` & `matfree-0.0.7/docs/dev/index.md`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/docs/higher_moments.md` & `matfree-0.0.7/docs/higher_moments.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 >>> import jax
 >>> import jax.numpy as jnp
 >>> from matfree import hutchinson, montecarlo, slq
 
 >>> a = jnp.reshape(jnp.arange(12.0), (6, 2))
 >>> key = jax.random.PRNGKey(1)
 
->>> matvec = lambda x: a.T @ (a @ x)
+>>> mvp = lambda x: a.T @ (a @ x)
 >>> sample_fun = montecarlo.normal(shape=(2,))
 
 ```
 
 ## Higher moments
 
 Trace estimation involves estimating expected values of random variables.
 Sometimes, second and higher moments of a random variable are interesting.
 Compute them as such
 
 ```python
 >>> a = jnp.reshape(jnp.arange(36.0), (6, 6)) / 36
->>> sample_fun = montecarlo.normal(shape=(6,))
->>> matvec = lambda x: a.T @ (a @ x) + x
->>> first, second = hutchinson.trace_moments(matvec, key=key, sample_fun=sample_fun)
+>>> normal = montecarlo.normal(shape=(6,))
+>>> mvp = lambda x: a.T @ (a @ x) + x
+>>> first, second = hutchinson.trace_moments(mvp, key=key, sample_fun=normal)
 >>> print(jnp.round(first, 1))
 17.5
 >>> print(jnp.round(second, 1))
 631.7
 
 ```
 
@@ -51,17 +51,17 @@
 divided by the number of samples.
 Implement this as follows:
 
 ```python
 >>> a = jnp.reshape(jnp.arange(36.0), (6, 6)) / 36
 >>> sample_fun = montecarlo.normal(shape=(6,))
 >>> num_samples = 10_000
->>> matvec = lambda x: a.T @ (a @ x) + x
+>>> mvp = lambda x: a.T @ (a @ x) + x
 >>> first, second = hutchinson.trace_moments(
-...     matvec,
+...     mvp,
 ...     key=key,
 ...     sample_fun=sample_fun,
 ...     moments=(1, 2),
 ...     num_batches=1,
 ...     num_samples_per_batch=num_samples,
 ... )
 >>> variance = (second - first**2) / num_samples
```

### Comparing `matfree-0.0.6/docs/index.md` & `matfree-0.0.7/docs/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -32,32 +32,32 @@
 >>> a = jnp.reshape(jnp.arange(12.0), (6, 2))
 >>> key = jax.random.PRNGKey(1)
 
 ```
 
 Estimate traces as such:
 ```python
->>> sample_fun = montecarlo.normal(shape=(2,))
+>>> normal = montecarlo.normal(shape=(2,))
 >>> matvec = lambda x: a.T @ (a @ x)
->>> trace = hutchinson.trace(matvec, key=key, sample_fun=sample_fun)
+>>> trace = hutchinson.trace(matvec, key=key, sample_fun=normal)
 >>> print(jnp.round(trace))
 514.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 ```
 The number of keys determines the number of sequential batches.
 Many small batches reduces memory.
 Few large batches increases memory and runtime.
 
 Determine the number of samples per batch as follows.
 
 ```python
->>> trace = hutchinson.trace(matvec, key=key, sample_fun=sample_fun, num_batches=10)
+>>> trace = hutchinson.trace(matvec, key=key, sample_fun=normal, num_batches=10)
 >>> print(jnp.round(trace))
 508.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 ```
```

### Comparing `matfree-0.0.6/docs/log_determinants.md` & `matfree-0.0.7/docs/log_determinants.md`

 * *Files 21% similar despite different names*

```diff
@@ -19,15 +19,35 @@
 
 Estimate log-determinants as such:
 ```python
 >>> a = jnp.reshape(jnp.arange(36.0), (6, 6)) / 36
 >>> sample_fun = montecarlo.normal(shape=(6,))
 >>> matvec = lambda x: a.T @ (a @ x) + x
 >>> order = 3
->>> logdet = slq.logdet(matvec, order, key=key, sample_fun=sample_fun)
+>>> logdet = slq.logdet_spd(order, matvec, key=key, sample_fun=sample_fun)
 >>> print(jnp.round(logdet))
 3.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.linalg.slogdet(a.T @ a + jnp.eye(6))[1]))
 3.0
 
 ```
+
+We can compute the log determinant of a matrix of the form $M = B^\top B$, purely based
+on arithmetic with $B$; no need to assemble $M$:
+
+```python
+>>> a = jnp.reshape(jnp.arange(36.0), (6, 6)) / 36 + jnp.eye(6)
+>>> sample_fun = montecarlo.normal(shape=(6,))
+>>> matvec = lambda x: (a @ x)
+>>> vecmat = lambda x: (a.T @ x)
+>>> order = 3
+>>> logdet = slq.logdet_product(
+...     order, matvec, vecmat, matrix_shape=(6, 6), key=key, sample_fun=sample_fun
+... )
+>>> print(jnp.round(logdet))
+2.0
+>>> # for comparison:
+>>> print(jnp.round(jnp.linalg.slogdet(a.T @ a)[1]))
+2.0
+
+```
```

### Comparing `matfree-0.0.6/docs/vector_calculus.md` & `matfree-0.0.7/docs/vector_calculus.md`

 * *Files 6% similar despite different names*

```diff
@@ -61,37 +61,37 @@
 If we have access to Jacobian-vector products (which we usually do), we can use matrix-free trace estimation
 to approximate divergences and Laplacians without forming full Jacobians:
 
 
 ```python
 
 >>> def divergence_matfree(vf, *, key, sample_fun):
-...     """Compute the divergence of a vector field only using matrix-vector products."""
+...     """Estimate the divergence of a vector field."""
 ...
 ...     def div_fn(x):
 ...         def jvp(v):
-...             _vf_value, jvp_value = jax.jvp(fun=vf, primals=(x,), tangents=(v,))
-...             return jvp_value
+...             _vf_val, jvp_val = jax.jvp(fun=vf, primals=(x,), tangents=(v,))
+...             return jvp_val
 ...
 ...         return hutchinson.trace(jvp, key=key, sample_fun=sample_fun)
 ...
 ...     return div_fn
 ...
 
 ```
 The difference to the above implementation is that `divergence_matfree` does not form dense Jacobians.
 It requires $O(d)$ memory and  $O(d N)$ operations (for $N$ Monte-Carlo samples).
 For large-scale problems, it may be the only way of computing Laplacians reliably.
 
 ```python
->>> sample_fun = montecarlo.normal(shape=(3,))
 >>> laplacian_dense = divergence_dense(gradient)
->>> laplacian_matfree = divergence_matfree(
-...     gradient, key=jax.random.PRNGKey(1), sample_fun=sample_fun
-... )
+>>>
+>>> normal = montecarlo.normal(shape=(3,))
+>>> key = jax.random.PRNGKey(1)
+>>> laplacian_matfree = divergence_matfree(gradient, key=key, sample_fun=normal)
 >>>
 >>> print(jnp.round(laplacian_dense(x0), 1))
 280.0
 
 >>> print(jnp.round(laplacian_matfree(x0), 1))
 278.4
```

### Comparing `matfree-0.0.6/matfree/backend/control_flow.py` & `matfree-0.0.7/matfree/backend/control_flow.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/matfree/backend/func.py` & `matfree-0.0.7/matfree/backend/func.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/matfree/backend/linalg.py` & `matfree-0.0.7/matfree/backend/linalg.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/matfree/backend/np.py` & `matfree-0.0.7/matfree/backend/np.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/matfree/backend/prng.py` & `matfree-0.0.7/matfree/backend/prng.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/matfree/benchmark_util.py` & `matfree-0.0.7/matfree/benchmark_util.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/matfree/decomp.py` & `matfree-0.0.7/matfree/decomp.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,14 +170,21 @@
 
 def gkl_full_reortho(depth, /, matrix_shape) -> AlgorithmType:
     """**Golub-Kahan-Lanczos** algorithm with pre-allocation & full reorthogonalisation.
 
     Decompose a matrix into a product of orthogonal-**bidiagonal**-orthogonal matrices.
     Use this algorithm for approximate **singular value** decompositions.
     """
+    nrows, ncols = matrix_shape
+    max_depth = min(nrows, ncols) - 1
+    if depth > max_depth or depth < 0:
+        msg1 = f"Depth {depth} exceeds the matrix' dimensions. "
+        msg2 = f"Expected: 0 <= depth <= min(nrows, ncols) - 1 = {max_depth} "
+        msg3 = f"for a matrix with shape {matrix_shape}."
+        raise ValueError(msg1 + msg2 + msg3)
     return _DecompAlg(
         init=func.partial(_gkl_full_reortho_init, depth, matrix_shape),
         step=_gkl_full_reortho_apply,
         extract=_gkl_full_reortho_extract,
         lower_upper=(0, depth + 1),
     )
```

### Comparing `matfree-0.0.6/matfree/hutchinson.py` & `matfree-0.0.7/matfree/hutchinson.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/matfree/montecarlo.py` & `matfree-0.0.7/matfree/montecarlo.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/matfree/slq.py` & `matfree-0.0.7/matfree/slq.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """Stochastic Lanczos quadrature."""
 
 from matfree import decomp, montecarlo
 from matfree.backend import func, linalg, np
 
 
-def logdet(*args, **kwargs):
+def logdet_spd(*args, **kwargs):
     """Estimate the log-determinant of a symmetric, positive definite matrix."""
-    return trace_of_matfun_symmetric(np.log, *args, **kwargs)
+    return trace_of_matfun_spd(np.log, *args, **kwargs)
 
 
-# todo: nuclear norm, schatten-p norms.
-#  But for this we should use bi-diagonalisation
-
-
-def trace_of_matfun_symmetric(matfun, Av, order, /, **kwargs):
+def trace_of_matfun_spd(matfun, order, Av, /, **kwargs):
     """Compute the trace of the function of a symmetric matrix."""
-    quadratic_form = quadratic_form_slq_symmetric(matfun, Av, order)
+    quadratic_form = _quadratic_form_slq_spd(matfun, order, Av)
     return montecarlo.estimate(quadratic_form, **kwargs)
 
 
-def quadratic_form_slq_symmetric(matfun, Av, order, /):
-    """Approximate quadratic form for stochastic Lanczos quadrature."""
+def _quadratic_form_slq_spd(matfun, order, Av, /):
+    """Quadratic form for stochastic Lanczos quadrature.
+
+    Assumes a symmetric, positive definite matrix.
+    """
 
     def quadform(v0, /):
         algorithm = decomp.lanczos_full_reortho(order)
         _, tridiag = decomp.decompose_fori_loop(v0, Av, algorithm=algorithm)
         (diag, off_diag) = tridiag
 
         # todo: once jax supports eigh_tridiagonal(eigvals_only=False),
@@ -40,7 +39,71 @@
         # and therefore (Q v)^T f(D) (Qv) = Q[0] * f(diag) * Q[0]
         (dim,) = v0.shape
 
         fx_eigvals = func.vmap(matfun)(eigvals)
         return dim * linalg.vecdot(eigvecs[0, :], fx_eigvals * eigvecs[0, :])
 
     return quadform
+
+
+def logdet_product(*args, **kwargs):
+    r"""Compute the log-determinant of a product of matrices.
+
+    Here, "product" refers to $X = A^\top A$.
+    """
+    return trace_of_matfun_product(np.log, *args, **kwargs)
+
+
+def schatten_norm(*args, power, **kwargs):
+    r"""Compute the Schatten-p norm of a matrix via stochastic Lanczos quadrature."""
+
+    def matfun(x):
+        """Matrix-function for Schatten-p norms."""
+        return x ** (power / 2)
+
+    trace = trace_of_matfun_product(matfun, *args, **kwargs)
+    return trace ** (1 / power)
+
+
+def trace_of_matfun_product(matfun, order, *matvec_funs, matrix_shape, **kwargs):
+    r"""Compute the trace of a function of a product of matrices.
+
+    Here, "product" refers to $X = A^\top A$.
+    """
+    quadratic_form = _quadratic_form_slq_product(
+        matfun, order, *matvec_funs, matrix_shape=matrix_shape
+    )
+    return montecarlo.estimate(quadratic_form, **kwargs)
+
+
+def _quadratic_form_slq_product(matfun, depth, *matvec_funs, matrix_shape):
+    r"""Quadratic form for stochastic Lanczos quadrature.
+
+    Instead of the trace of a function of a matrix,
+    compute the trace of a function of the product of matrices.
+    Here, "product" refers to $X = A^\top A$.
+    """
+
+    def quadform(v0, /):
+        # Decompose into orthogonal-bidiag-orthogonal
+        algorithm = decomp.gkl_full_reortho(depth, matrix_shape=matrix_shape)
+        output = decomp.decompose_fori_loop(v0, *matvec_funs, algorithm=algorithm)
+        u, (d, e), vt, _ = output
+
+        # Compute SVD of factorisation
+        B = _bidiagonal_dense(d, e)
+        _, S, Vt = linalg.svd(B, full_matrices=False)
+
+        # Since Q orthogonal (orthonormal) to v0, Q v = Q[0],
+        # and therefore (Q v)^T f(D) (Qv) = Q[0] * f(diag) * Q[0]
+        _, ncols = matrix_shape
+        eigvals, eigvecs = S**2, Vt.T
+        fx_eigvals = func.vmap(matfun)(eigvals)
+        return ncols * linalg.vecdot(eigvecs[0, :], fx_eigvals * eigvecs[0, :])
+
+    return quadform
+
+
+def _bidiagonal_dense(d, e):
+    diag = linalg.diagonal_matrix(d)
+    offdiag = linalg.diagonal_matrix(e, 1)
+    return diag + offdiag
```

### Comparing `matfree-0.0.6/matfree/test_util.py` & `matfree-0.0.7/matfree/test_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Test utilities."""
 
 from matfree.backend import linalg, np
 
 
 def symmetric_matrix_from_eigenvalues(eigvals, /):
     """Generate a symmetric matrix with prescribed eigenvalues."""
+    assert np.array_min(eigvals) > 0
     (n,) = eigvals.shape
 
     # Need _some_ matrix to start with
     A = np.reshape(np.arange(1.0, n**2 + 1.0), (n, n))
     A = A / linalg.matrix_norm(A, which="fro")
     X = A.T @ A + np.eye(n)
 
@@ -20,11 +21,12 @@
     # return Q D Q.T.
     # This matrix will be dense, symmetric, and have a given spectrum.
     return Q @ (eigvals[:, None] * Q.T)
 
 
 def asymmetric_matrix_from_singular_values(vals, /, nrows, ncols):
     """Generate an asymmetric matrix with specific singular values."""
+    assert np.array_min(vals) > 0
     A = np.reshape(np.arange(1.0, nrows * ncols + 1.0), (nrows, ncols))
     A /= nrows * ncols
     U, S, Vt = linalg.svd(A, full_matrices=False)
     return U @ linalg.diagonal(vals) @ Vt
```

### Comparing `matfree-0.0.6/matfree.egg-info/PKG-INFO` & `matfree-0.0.7/matfree.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matfree
-Version: 0.0.6
+Version: 0.0.7
 Summary: Matrix-free numerical linear algebra including trace-estimation.
 Author: Nicholas Krämer
 Author-email: pekra@dtu.dk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cpu
@@ -49,32 +49,32 @@
 >>> a = jnp.reshape(jnp.arange(12.0), (6, 2))
 >>> key = jax.random.PRNGKey(1)
 
 ```
 
 Estimate traces as such:
 ```python
->>> sample_fun = montecarlo.normal(shape=(2,))
+>>> normal = montecarlo.normal(shape=(2,))
 >>> matvec = lambda x: a.T @ (a @ x)
->>> trace = hutchinson.trace(matvec, key=key, sample_fun=sample_fun)
+>>> trace = hutchinson.trace(matvec, key=key, sample_fun=normal)
 >>> print(jnp.round(trace))
 514.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 ```
 The number of keys determines the number of sequential batches.
 Many small batches reduces memory.
 Few large batches increases memory and runtime.
 
 Determine the number of samples per batch as follows.
 
 ```python
->>> trace = hutchinson.trace(matvec, key=key, sample_fun=sample_fun, num_batches=10)
+>>> trace = hutchinson.trace(matvec, key=key, sample_fun=normal, num_batches=10)
 >>> print(jnp.round(trace))
 508.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 ```
```

### Comparing `matfree-0.0.6/matfree.egg-info/SOURCES.txt` & `matfree-0.0.7/matfree.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -61,9 +61,11 @@
 tests/test_hutchinson/test_trace_and_diagonal.py
 tests/test_hutchinson/test_trace_moments.py
 tests/test_montecarlo/__init__.py
 tests/test_montecarlo/test_estimate.py
 tests/test_montecarlo/test_multiestimate.py
 tests/test_montecarlo/test_van_der_corput.py
 tests/test_slq/__init__.py
-tests/test_slq/test_logdet.py
-tests/test_slq/test_logdet_autodiff.py
+tests/test_slq/test_logdet_product.py
+tests/test_slq/test_logdet_spd.py
+tests/test_slq/test_logdet_spd_autodiff.py
+tests/test_slq/test_schatten_norm.py
```

### Comparing `matfree-0.0.6/mkdocs.yml` & `matfree-0.0.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/pyproject.toml` & `matfree-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/setup.cfg` & `matfree-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/tests/test_decomp/test_lanczos_full_reortho.py` & `matfree-0.0.7/tests/test_decomp/test_lanczos_full_reortho.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/tests/test_decomp/test_svd.py` & `matfree-0.0.7/tests/test_decomp/test_svd.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/tests/test_hutchinson/test_diagonal.py` & `matfree-0.0.7/tests/test_hutchinson/test_diagonal.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/tests/test_hutchinson/test_frobeniusnorm_squared.py` & `matfree-0.0.7/tests/test_hutchinson/test_frobeniusnorm_squared.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/tests/test_hutchinson/test_trace.py` & `matfree-0.0.7/tests/test_hutchinson/test_trace.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/tests/test_hutchinson/test_trace_and_diagonal.py` & `matfree-0.0.7/tests/test_hutchinson/test_trace_and_diagonal.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/tests/test_hutchinson/test_trace_moments.py` & `matfree-0.0.7/tests/test_hutchinson/test_trace_moments.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/tests/test_montecarlo/test_estimate.py` & `matfree-0.0.7/tests/test_montecarlo/test_estimate.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/tests/test_montecarlo/test_multiestimate.py` & `matfree-0.0.7/tests/test_montecarlo/test_multiestimate.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/tests/test_montecarlo/test_van_der_corput.py` & `matfree-0.0.7/tests/test_montecarlo/test_van_der_corput.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.6/tests/test_slq/test_logdet.py` & `matfree-0.0.7/tests/test_slq/test_logdet_spd.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 
 
 @testing.parametrize("n", [200])
 @testing.parametrize("num_significant_eigvals", [30])
 @testing.parametrize("order", [10])
 # usually: ~1.5 * num_significant_eigvals.
 # But logdet seems to converge sooo much faster.
-def test_logdet(A, order):
+def test_logdet_spd(A, order):
     """Assert that the log-determinant estimation matches the true log-determinant."""
     n, _ = np.shape(A)
     key = prng.prng_key(1)
     fun = montecarlo.normal(shape=(n,))
-    received = slq.logdet(
-        lambda v: A @ v,
+    received = slq.logdet_spd(
         order,
+        lambda v: A @ v,
         key=key,
         num_samples_per_batch=10,
         num_batches=1,
         sample_fun=fun,
     )
     expected = linalg.slogdet(A)[1]
     print_if_assert_fails = ("error", np.abs(received - expected), "target:", expected)
```

### Comparing `matfree-0.0.6/tests/test_slq/test_logdet_autodiff.py` & `matfree-0.0.7/tests/test_slq/test_logdet_spd_autodiff.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     testing.check_grads(fun, (A,), order=1, atol=1e-1, rtol=1e-1)
 
 
 def _logdet(A, order, key):
     n, _ = np.shape(A)
     fun = montecarlo.normal(shape=(n,))
-    return slq.logdet(
-        lambda v: A @ v,
+    return slq.logdet_spd(
         order,
+        lambda v: A @ v,
         key=key,
         num_samples_per_batch=10,
         num_batches=1,
         sample_fun=fun,
     )
```

