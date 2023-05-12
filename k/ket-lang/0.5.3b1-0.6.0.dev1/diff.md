# Comparing `tmp/ket-lang-0.5.3b1.tar.gz` & `tmp/ket-lang-0.6.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ket-lang-0.5.3b1.tar", last modified: Thu Apr 13 18:04:47 2023, max compression
+gzip compressed data, was "ket-lang-0.6.0.dev1.tar", last modified: Fri May 12 19:47:45 2023, max compression
```

## Comparing `ket-lang-0.5.3b1.tar` & `ket-lang-0.6.0.dev1.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.265780 ket-lang-0.5.3b1/
--rw-rw-rw-   0 root         (0) root         (0)    11455 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7166 2023-04-13 18:04:47.265780 ket-lang-0.5.3b1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6412 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1131 2023-04-13 18:04:47.266780 ket-lang-0.5.3b1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.236778 ket-lang-0.5.3b1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.242778 ket-lang-0.5.3b1/src/ket/
--rw-rw-rw-   0 root         (0) root         (0)     1311 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1642 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    28956 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.244778 ket-lang-0.5.3b1/src/ket/clib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/clib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3937 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/clib/kbw.py
--rw-rw-rw-   0 root         (0) root         (0)     8828 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/clib/libket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.244778 ket-lang-0.5.3b1/src/ket/clib/libs/
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/clib/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.247779 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-13 18:04:35.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/.git
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      527 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      716 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/Cargo.toml
--rw-rw-rw-   0 root         (0) root         (0)    11460 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/README.md
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/kbw.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.250779 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/
--rw-rw-rw-   0 root         (0) root         (0)     1255 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/bitwise.rs
--rw-rw-rw-   0 root         (0) root         (0)     4404 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/c_wrapper.rs
--rw-rw-rw-   0 root         (0) root         (0)     1942 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/convert.rs
--rw-rw-rw-   0 root         (0) root         (0)    20501 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/dense.rs
--rw-rw-rw-   0 root         (0) root         (0)     2247 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/error.rs
--rw-rw-rw-   0 root         (0) root         (0)      311 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/lib.rs
--rw-rw-rw-   0 root         (0) root         (0)     9825 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/quantum_execution.rs
--rw-rw-rw-   0 root         (0) root         (0)    20230 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/sparse.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.250779 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/tests/shor.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.253779 ket-lang-0.5.3b1/src/ket/clib/libs/libket/
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/.git
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      351 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/Cargo.toml
--rw-rw-rw-   0 root         (0) root         (0)    11460 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      746 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/README.md
--rw-rw-rw-   0 root         (0) root         (0)     8385 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/libket.h
--rw-rw-rw-   0 root         (0) root         (0)    10365 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/libket.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.257779 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.258780 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/error.rs
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/mod.rs
--rw-rw-rw-   0 root         (0) root         (0)     6838 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/objects.rs
--rw-rw-rw-   0 root         (0) root         (0)    10966 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/process.rs
--rw-rw-rw-   0 root         (0) root         (0)     5725 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/code_block.rs
--rw-rw-rw-   0 root         (0) root         (0)     4523 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/error.rs
--rw-rw-rw-   0 root         (0) root         (0)     6275 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/gates.rs
--rw-rw-rw-   0 root         (0) root         (0)     4540 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/instruction.rs
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/ir.rs
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/lib.rs
--rw-rw-rw-   0 root         (0) root         (0)     4147 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/object.rs
--rw-rw-rw-   0 root         (0) root         (0)    20114 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/process.rs
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/serialize.rs
--rw-rw-rw-   0 root         (0) root         (0)     3101 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/clib/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.259780 ket-lang-0.5.3b1/src/ket/gates/
--rw-rw-rw-   0 root         (0) root         (0)     8530 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/gates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/gates/base_gates.py
--rw-rw-rw-   0 root         (0) root         (0)     4245 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/gates/quantum_gate.py
--rw-rw-rw-   0 root         (0) root         (0)     3913 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/import_ket.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/kbw.py
--rw-rw-rw-   0 root         (0) root         (0)     5795 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/plugins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.261780 ket-lang-0.5.3b1/src/ket/preprocessor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/preprocessor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2222 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/preprocessor/statements.py
--rw-rw-rw-   0 root         (0) root         (0)     8995 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/preprocessor/transformer.py
--rw-rw-rw-   0 root         (0) root         (0)     3751 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.262780 ket-lang-0.5.3b1/src/ket/standard/
--rw-rw-rw-   0 root         (0) root         (0)     1817 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4593 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/standard/adj.py
--rw-rw-rw-   0 root         (0) root         (0)     7792 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/standard/ctrl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.264780 ket-lang-0.5.3b1/src/ket_lang.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7166 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2215 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.265780 ket-lang-0.5.3b1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3056 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/tests/test_gates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.416518 ket-lang-0.6.0.dev1/
+-rw-rw-rw-   0 root         (0) root         (0)    11455 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7173 2023-05-12 19:47:45.417518 ket-lang-0.6.0.dev1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6412 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-05-12 19:47:45.417518 ket-lang-0.6.0.dev1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.388515 ket-lang-0.6.0.dev1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.394515 ket-lang-0.6.0.dev1/src/ket/
+-rw-rw-rw-   0 root         (0) root         (0)     1313 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1642 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29132 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.395516 ket-lang-0.6.0.dev1/src/ket/clib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/clib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3937 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/clib/kbw.py
+-rw-rw-rw-   0 root         (0) root         (0)     9012 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/clib/libket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.396516 ket-lang-0.6.0.dev1/src/ket/clib/libs/
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.398516 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/.git
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      761 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/Cargo.toml
+-rw-rw-rw-   0 root         (0) root         (0)    11460 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/kbw.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.401516 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/bitwise.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4404 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/c_wrapper.rs
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/convert.rs
+-rw-rw-rw-   0 root         (0) root         (0)    20501 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/dense.rs
+-rw-rw-rw-   0 root         (0) root         (0)     2247 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)      311 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/lib.rs
+-rw-rw-rw-   0 root         (0) root         (0)     9825 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/quantum_execution.rs
+-rw-rw-rw-   0 root         (0) root         (0)    20230 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/sparse.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.402516 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/tests/shor.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.405516 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/.git
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/Cargo.toml
+-rw-rw-rw-   0 root         (0) root         (0)    11460 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      746 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     8457 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/libket.h
+-rw-rw-rw-   0 root         (0) root         (0)    10442 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/libket.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.409517 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.410517 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/c_wrapper/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/c_wrapper/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/c_wrapper/mod.rs
+-rw-rw-rw-   0 root         (0) root         (0)     6838 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/c_wrapper/objects.rs
+-rw-rw-rw-   0 root         (0) root         (0)    11058 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/c_wrapper/process.rs
+-rw-rw-rw-   0 root         (0) root         (0)     6119 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/code_block.rs
+-rw-rw-rw-   0 root         (0) root         (0)     8846 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/decompose.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4605 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)     6275 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/gates.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4853 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/instruction.rs
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/ir.rs
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/lib.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/object.rs
+-rw-rw-rw-   0 root         (0) root         (0)    21092 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/process.rs
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/serialize.rs
+-rw-rw-rw-   0 root         (0) root         (0)     3101 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/clib/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.411517 ket-lang-0.6.0.dev1/src/ket/gates/
+-rw-rw-rw-   0 root         (0) root         (0)     8530 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/gates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/gates/base_gates.py
+-rw-rw-rw-   0 root         (0) root         (0)     4245 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/gates/quantum_gate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3913 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/import_ket.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/kbw.py
+-rw-rw-rw-   0 root         (0) root         (0)     5795 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/plugins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.413517 ket-lang-0.6.0.dev1/src/ket/preprocessor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/preprocessor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/preprocessor/statements.py
+-rw-rw-rw-   0 root         (0) root         (0)     8995 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/preprocessor/transformer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3751 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.414517 ket-lang-0.6.0.dev1/src/ket/standard/
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4593 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/standard/adj.py
+-rw-rw-rw-   0 root         (0) root         (0)     7792 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/standard/ctrl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.416518 ket-lang-0.6.0.dev1/src/ket_lang.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7173 2023-05-12 19:47:45.000000 ket-lang-0.6.0.dev1/src/ket_lang.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2257 2023-05-12 19:47:45.000000 ket-lang-0.6.0.dev1/src/ket_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 19:47:45.000000 ket-lang-0.6.0.dev1/src/ket_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-12 19:47:45.000000 ket-lang-0.6.0.dev1/src/ket_lang.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 19:47:45.000000 ket-lang-0.6.0.dev1/src/ket_lang.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-12 19:47:45.000000 ket-lang-0.6.0.dev1/src/ket_lang.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.416518 ket-lang-0.6.0.dev1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4698 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/tests/test_gates.py
```

### Comparing `ket-lang-0.5.3b1/LICENSE` & `ket-lang-0.6.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/PKG-INFO` & `ket-lang-0.6.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: ket-lang
-Version: 0.5.3b1
+Version: 0.6.0.dev1
 Summary: Ket quantum programming language interpreter and library
 Home-page: https://quantumket.org
 Author: Evandro Chagas Ribeiro da Rosa
-Author-email: ev.crr97@gmail.com
+Author-email: evandro@quantuloop.com
 License: Apache-2.0
 Project-URL: Source, https://gitlab.com/quantum-ket/ket
 Keywords: quantum computer,quantum programming,quantum simulator
 Platform: linux
 Platform: win32
 Platform: osx
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Rust
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 [![PyPI](https://img.shields.io/pypi/v/ket-lang.svg)](https://pypi.org/project/ket-lang/)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
 
 # Ket Quantum Programming
```

### Comparing `ket-lang-0.5.3b1/README.md` & `ket-lang-0.6.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/setup.cfg` & `ket-lang-0.6.0.dev1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = ket-lang
 version = attr: ket.__version__
 url = https://quantumket.org
 project_urls = 
 	Source = https://gitlab.com/quantum-ket/ket
 author = Evandro Chagas Ribeiro da Rosa
-author_email = ev.crr97@gmail.com
+author_email = evandro@quantuloop.com
 classifiers = 
 	Intended Audience :: Science/Research
 	Operating System :: POSIX :: Linux
 	Operating System :: Microsoft :: Windows
 	Operating System :: MacOS
 	Programming Language :: Python :: 3
 	Programming Language :: Rust
@@ -21,15 +21,15 @@
 keywords = quantum computer, quantum programming, quantum simulator
 platforms = linux, win32, osx
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 package_dir = 
 	= src
 setup_requires = 
 	wheel
 
 [options.packages.find]
 where = src
```

### Comparing `ket-lang-0.5.3b1/src/ket/__init__.py` & `ket-lang-0.6.0.dev1/src/ket/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .process import *
 from .gates import __all__ as all_gate
 from .import_ket import __all__ as all_import
 from .base import __all__ as all_base
 from .standard import __all__ as all_standard
 from .process import __all__ as all_process
 
-__version__ = '0.5.3b1'
+__version__ = '0.6.0dev1'
 __all__ = all_gate + all_import + all_base + all_standard + all_process
 
 from .import_ket import code_ket
 
 from .base import QUANTUM_EXECUTION_TARGET
 if QUANTUM_EXECUTION_TARGET is None:
     from .kbw import use_sparse
```

### Comparing `ket-lang-0.5.3b1/src/ket/__main__.py` & `ket-lang-0.6.0.dev1/src/ket/__main__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/base.py` & `ket-lang-0.6.0.dev1/src/ket/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -746,27 +746,31 @@
 def set_process_features(*, allow_dirty_qubits: bool = True,
                          allow_free_qubits: bool = True,
                          valid_after_measure: bool = True,
                          classical_control_flow: bool = True,
                          allow_dump: bool = True,
                          allow_measure: bool = True,
                          continue_after_dump: bool = True,
+                         decompose: bool = False,
+                         use_rz_as_phase: bool = False,
                          plugins: list[str] | None = None):
     """Disable and enable process features"""
 
     global FEATURES
 
     FEATURES = Features(
         allow_dirty_qubits=allow_dirty_qubits,
         allow_free_qubits=allow_free_qubits,
         valid_after_measure=valid_after_measure,
         classical_control_flow=classical_control_flow,
         allow_dump=allow_dump,
         allow_measure=allow_measure,
         continue_after_dump=continue_after_dump,
+        decompose=decompose,
+        use_rz_as_phase=use_rz_as_phase,
     )
 
     if plugins is not None:
         for name in plugins:
             FEATURES.register_plugin(name.encode())
 
     process_top().set_features(FEATURES)
```

### Comparing `ket-lang-0.5.3b1/src/ket/clib/kbw.py` & `ket-lang-0.6.0.dev1/src/ket/clib/kbw.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libket.py` & `ket-lang-0.6.0.dev1/src/ket/clib/libket.py`

 * *Files 11% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     'ket_process_exec_time': ([c_void_p], [c_double]),
     'ket_process_set_timeout': ([c_void_p, c_uint64], []),
     'ket_process_serialize_metrics': ([c_void_p, c_int32], []),
     'ket_process_serialize_quantum_code': ([c_void_p, c_int32], []),
     'ket_process_get_serialized_metrics': ([c_void_p], [POINTER(c_uint8), c_size_t, c_int32]),
     'ket_process_get_serialized_quantum_code': ([c_void_p], [POINTER(c_uint8), c_size_t, c_int32]),
     'ket_process_set_serialized_result': ([c_void_p, POINTER(c_uint8), c_size_t, c_int32], []),
-    'ket_features_new': ([c_bool, c_bool, c_bool, c_bool, c_bool, c_bool, c_bool], [c_void_p]),
+    'ket_features_new': ([c_bool, c_bool, c_bool, c_bool, c_bool, c_bool, c_bool, c_bool, c_bool], [c_void_p]),  # pylint: disable=C0301
     'ket_features_delete': ([c_void_p], []),
     'ket_features_all': ([], [c_void_p]),
     'ket_features_none': ([], [c_void_p]),
     'ket_features_register_plugin': ([c_void_p, POINTER(c_char)], []),
     'ket_qubit_delete': ([c_void_p], []),
     'ket_qubit_index': ([c_void_p], [c_size_t]),
     'ket_qubit_pid': ([c_void_p], [c_size_t]),
@@ -177,23 +177,27 @@
     def __init__(self, *,
                  allow_dirty_qubits: bool = True,
                  allow_free_qubits: bool = True,
                  valid_after_measure: bool = True,
                  classical_control_flow: bool = True,
                  allow_dump: bool = True,
                  allow_measure: bool = True,
-                 continue_after_dump: bool = True):
+                 continue_after_dump: bool = True,
+                 decompose: bool = False,
+                 use_rz_as_phase: bool = False):
         self._as_parameter_ = API['ket_features_new'](
             allow_dirty_qubits,
             allow_free_qubits,
             valid_after_measure,
             classical_control_flow,
             allow_dump,
             allow_measure,
-            continue_after_dump
+            continue_after_dump,
+            decompose,
+            use_rz_as_phase,
         )
         self._finalizer = weakref.finalize(
             self, API['ket_features_delete'], self._as_parameter_)
 
     def __getattr__(self, name: str):
         return lambda *args: API['ket_features_' + name](self, *args)
```

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/__init__.py` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/CHANGELOG.md` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 0.1.6
+
+- Libket updated to 0.3.0.
+
 ## 0.1.5
 
 - Fixed plugin `pown` for the Dense simulator.
 - Libket updated to 0.2.3.
 
 ## 0.1.4
```

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/Cargo.toml` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
 name = "kbw"
-version = "0.1.5"
+version = "0.1.6"
 authors = ["Evandro Chagas Ribeiro da Rosa <evandro@quantuloop.com>"]
 description = "Ket Bitwise Simulator"
 repository = "https://gitlab.com/quantum-ket/kbw"
 documentation = "https://quantumket.org"
 license = "Apache-2.0"
 readme = "README.md"
 edition = "2021"
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-libket = "0.2.3"
+libket = { git = "https://gitlab.com/quantum-ket/libket.git"}
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "1.0"
 bincode = "1.3"
 num = "0.4"
 rand = "0.8.5"
 rayon = "1.5.3"
 twox-hash = "1.6.3"
```

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/LICENSE` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/README.md` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/README.md`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/kbw.h` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/kbw.h`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/bitwise.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/bitwise.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/c_wrapper.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/c_wrapper.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/convert.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/convert.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/dense.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/dense.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/error.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/error.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/quantum_execution.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/quantum_execution.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/sparse.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/sparse.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/tests/shor.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/tests/shor.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/libket/Cargo.toml` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "libket"
-version = "0.2.3"
+version = "0.3.0"
 authors = ["Evandro Chagas Ribeiro da Rosa <evandro@quantuloop.com>"]
 description = "Runtime library for the Ket programming language"
 repository = "https://gitlab.com/quantum-ket/libket"
 documentation = "https://quantumket.org"
 license = "Apache-2.0"
 readme = "README.md"
 edition = "2021"
```

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/libket/LICENSE` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/libket/README.md` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/README.md`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/libket/libket.h` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/libket.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #pragma once
 #ifdef __cplusplus
 extern "C" {
 #endif
 
+#include <stdbool.h>
 #include <stddef.h>
 #include <stdint.h>
-#include <stdbool.h>
 
 typedef void *ket_process_t;
 typedef void *ket_qubit_t;
 typedef void *ket_future_t;
 typedef void *ket_dump_t;
 typedef void *ket_label_t;
 typedef void *ket_features_t;
@@ -72,15 +72,15 @@
 #define KET_JSON 0
 #define KET_BIN 1
 
 #define KET_DUMP_VECTOR 0
 #define KET_DUMP_PROBABILITY 1
 #define KET_DUMP_SHOTS 2
 
-const uint8_t* ket_error_message(ket_error_code_t error_code, size_t *size);
+const uint8_t *ket_error_message(ket_error_code_t error_code, size_t *size);
 
 ket_error_code_t ket_process_new(size_t pid, ket_process_t *process);
 
 ket_error_code_t ket_process_delete(ket_process_t process);
 
 ket_error_code_t ket_process_set_features(ket_process_t process,
                                           ket_features_t features);
@@ -164,14 +164,15 @@
                                                    int32_t data_type);
 
 ket_error_code_t ket_features_new(bool allow_dirty_qubits,
                                   bool allow_free_qubits,
                                   bool valid_after_measure,
                                   bool classical_control_flow, bool allow_dump,
                                   bool allow_measure, bool continue_after_dump,
+                                  bool decompose, bool use_rz_as_phase,
                                   ket_features_t *features);
 
 ket_error_code_t ket_features_delete(ket_features_t features);
 
 ket_error_code_t ket_features_all(ket_features_t *features);
 
 ket_error_code_t ket_features_none(ket_features_t *features);
```

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/libket/libket.hpp` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/libket.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -35,20 +35,21 @@
 
 class Features {
   friend class Process;
 
  public:
   Features(bool allow_dirty_qubits, bool allow_free_qubits,
            bool valid_after_measure, bool classical_control_flow,
-           bool allow_dump, bool allow_measure, bool continue_after_dump) {
+           bool allow_dump, bool allow_measure, bool continue_after_dump,
+           bool decompose, bool use_rz_as_phase) {
     ket_features_t features;
     ket_throw(ket_features_new(allow_dirty_qubits, allow_free_qubits,
                                valid_after_measure, classical_control_flow,
                                allow_dump, allow_measure, continue_after_dump,
-                               &features));
+                               decompose, use_rz_as_phase, &features));
     self = std::shared_ptr<void>(
         features, [](void* features) { ket_features_delete(features); });
   }
 
   static Features none() { return Features{ket_features_none}; };
 
   static Features all() { return Features{ket_features_all}; }
```

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/objects.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/c_wrapper/objects.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/process.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/c_wrapper/process.rs`

 * *Files 1% similar despite different names*

```diff
@@ -354,24 +354,28 @@
     allow_dirty_qubits: bool,
     allow_free_qubits: bool,
     valid_after_measure: bool,
     classical_control_flow: bool,
     allow_dump: bool,
     allow_measure: bool,
     continue_after_dump: bool,
+    decompose: bool,
+    use_rz_as_phase: bool,
     features: &mut *mut Features,
 ) -> i32 {
     *features = Box::into_raw(Box::new(Features::new(
         allow_dirty_qubits,
         allow_free_qubits,
         valid_after_measure,
         classical_control_flow,
         allow_dump,
         allow_measure,
         continue_after_dump,
+        decompose,
+        use_rz_as_phase,
     )));
     KetError::Success.error_code()
 }
 
 #[no_mangle]
 pub unsafe extern "C" fn ket_features_delete(features: *mut Features) -> i32 {
     unsafe { Box::from_raw(features) };
```

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/code_block.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/code_block.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,38 +11,49 @@
     pub gate_count: HashMap<usize, usize>,
     pub depth: usize,
 }
 
 #[derive(Default, Debug)]
 pub struct CodeBlockHandler {
     block: CodeBlock,
+    pub use_rz_as_phase: bool,
     adj_instructions: Vec<Vec<Instruction>>,
     gate_per_qubit: HashMap<usize, usize>,
     ended: bool,
 }
 
 impl CodeBlockHandler {
     pub fn add_instruction(&mut self, instruction: Instruction) -> Result<()> {
         if self.ended {
             return Err(KetError::TerminatedBlock);
         }
 
         if let Some(instruction) = match &instruction {
             Instruction::Gate {
-                gate: _,
+                gate,
                 target,
                 control,
             } => {
                 *self.block.gate_count.entry(control.len() + 1).or_default() += 1;
                 *self.gate_per_qubit.entry(*target).or_default() += 1;
 
                 control.iter().for_each(|control| {
                     *self.gate_per_qubit.entry(*control).or_default() += 1;
                 });
 
+                let instruction = if self.use_rz_as_phase && gate.is_phase() {
+                    Instruction::Gate {
+                        gate: gate.from_phase_to_rz()?,
+                        target: *target,
+                        control: control.to_vec(),
+                    }
+                } else {
+                    instruction
+                };
+
                 if self.adj_instructions.is_empty() {
                     Some(instruction)
                 } else {
                     self.adj_instructions.last_mut().unwrap().push(instruction);
                     None
                 }
             }
```

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/error.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/error.rs`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     UnmatchedPid,
     DirtyNotAllowed,
     DumpNotAllowed,
     MeasureNotAllowed,
     FreeNotAllowed,
     PluginNotRegistered,
     ControlFlowNotAllowed,
+    NotPhaseGate,
     UndefinedError,
 }
 
 pub type Result<T> = result::Result<T, KetError>;
 
 impl KetError {
     pub fn to_str(&self) -> &'static str {
@@ -66,14 +67,15 @@
             KetError::FreeNotAllowed => "cannot free qubit (feature disabled)",
             KetError::PluginNotRegistered => "plugin not registered",
             KetError::ControlFlowNotAllowed => {
                 "classical control flow not allowed (feature disabled)"
             }
             KetError::DumpNotAllowed => "cannot dump qubits (feature disabled)",
             KetError::MeasureNotAllowed => "cannot measure qubit (feature disabled)",
+            KetError::NotPhaseGate => "expecting a phase gate",
         }
     }
 
     pub fn error_code(&self) -> i32 {
         self.to_i32().unwrap()
     }
```

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/gates.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/gates.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/instruction.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/instruction.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use num::complex::Complex64;
 use num_derive::{FromPrimitive, ToPrimitive};
 use serde::{Deserialize, Serialize};
 
 use crate::error::{KetError, Result};
 
-#[derive(Debug, Serialize, Deserialize)]
+#[derive(Debug, Clone, Serialize, Deserialize)]
 pub enum QuantumGate {
     PauliX,
     PauliY,
     PauliZ,
     Hadamard,
     Phase(f64),
     RX(f64),
@@ -56,14 +56,25 @@
             QuantumGate::RZ(theta) => QuantumGate::RZ(-theta),
             QuantumGate::Unitary(u) => QuantumGate::Unitary([
                 [(u[0][0].0, -u[0][0].1), (u[1][0].0, -u[1][0].1)],
                 [(u[0][1].0, -u[0][1].1), (u[1][1].0, -u[1][1].1)],
             ]),
         }
     }
+
+    pub fn is_phase(&self) -> bool {
+        matches!(self, QuantumGate::Phase(_))
+    }
+
+    pub fn from_phase_to_rz(&self) -> Result<QuantumGate> {
+        match self {
+            QuantumGate::Phase(lambda) => Ok(QuantumGate::RZ(*lambda)),
+            _ => Err(KetError::NotPhaseGate),
+        }
+    }
 }
 
 #[derive(Debug, Serialize, Deserialize, FromPrimitive, ToPrimitive)]
 pub enum ClassicalOp {
     Eq,
     Neq,
     Gt,
```

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/ir.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/ir.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/object.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/object.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/process.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/process.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use std::{cell::RefCell, collections::BTreeSet, ops::Deref, rc::Rc};
 
 use rand::Rng;
 
 use crate::{
     code_block::{CodeBlock, CodeBlockHandler},
+    decompose::decompose,
     error::{KetError, Result},
     instruction::{ClassicalOp, EndInstruction, Instruction, QuantumGate},
     ir::{Metrics, ResultData},
     object::{Dump, DumpData, Future, Label, Pid, Qubit},
     serialize::{DataType, SerializedData},
 };
 
@@ -17,61 +18,72 @@
     allow_free_qubits: bool,
     valid_after_measure: bool,
     plugins: BTreeSet<String>,
     classical_control_flow: bool,
     allow_dump: bool,
     allow_measure: bool,
     continue_after_dump: bool,
+    decompose: bool,
+    use_rz_as_phase: bool,
 }
 
 impl Features {
+    #[allow(clippy::too_many_arguments)]
     pub fn new(
         allow_dirty_qubits: bool,
         allow_free_qubits: bool,
         valid_after_measure: bool,
         classical_control_flow: bool,
         allow_dump: bool,
         allow_measure: bool,
         continue_after_dump: bool,
+        decompose: bool,
+        use_rz_as_phase: bool,
     ) -> Features {
         Features {
             allow_dirty_qubits,
             allow_free_qubits,
             valid_after_measure,
             plugins: BTreeSet::new(),
             classical_control_flow,
             allow_dump,
             allow_measure,
             continue_after_dump,
+            decompose,
+            use_rz_as_phase,
         }
     }
 
     pub fn all() -> Features {
         Features {
             allow_dirty_qubits: true,
             allow_free_qubits: true,
             valid_after_measure: true,
             plugins: BTreeSet::new(),
             classical_control_flow: true,
             allow_dump: true,
             allow_measure: true,
             continue_after_dump: true,
+            decompose: false,
+            use_rz_as_phase: false,
         }
     }
 
     pub fn none() -> Features {
         Features {
             allow_dirty_qubits: false,
             allow_free_qubits: false,
             valid_after_measure: false,
             plugins: BTreeSet::new(),
             classical_control_flow: false,
             allow_dump: false,
             allow_measure: true,
             continue_after_dump: false,
+            decompose: false,
+            use_rz_as_phase: false,
         }
     }
 
     pub fn register_plugin(&mut self, plugin: &str) {
         self.plugins.insert(plugin.to_string());
     }
 }
@@ -147,14 +159,18 @@
             Err(KetError::TargetOnControl)
         } else {
             Ok(())
         }
     }
 
     pub fn set_features(&mut self, features: Features) {
+        self.blocks
+            .get_mut(self.current_block)
+            .unwrap()
+            .use_rz_as_phase = features.use_rz_as_phase;
         self.features = features;
     }
 
     pub fn allocate_qubit(&mut self, dirty: bool) -> Result<Qubit> {
         if !self.features.allow_dirty_qubits && dirty {
             return Err(KetError::DirtyNotAllowed);
         }
@@ -210,20 +226,29 @@
         let control = self.get_control_qubits();
         self.assert_target_not_in_control(target)?;
 
         let block = self.blocks.get_mut(self.current_block).unwrap();
 
         let gate = if block.in_adj() { gate.inverse() } else { gate };
 
-        block.add_instruction(Instruction::Gate {
-            gate,
-            target: target.index(),
-            control,
-        })?;
-
+        if self.features.decompose {
+            let mut decomposed_gate = decompose(gate, control, target.index());
+            if block.in_adj() {
+                decomposed_gate.reverse();
+            }
+            for instruction in decomposed_gate {
+                block.add_instruction(instruction)?;
+            }
+        } else {
+            block.add_instruction(Instruction::Gate {
+                gate,
+                target: target.index(),
+                control,
+            })?;
+        }
         Ok(())
     }
 
     pub fn apply_plugin(&mut self, name: &str, target: &[&Qubit], args: &str) -> Result<()> {
         if !self.features.plugins.contains(name) {
             return Err(KetError::PluginNotRegistered);
         }
@@ -412,15 +437,17 @@
     pub fn get_label(&mut self) -> Result<Label> {
         if !self.features.classical_control_flow {
             return Err(KetError::ControlFlowNotAllowed);
         }
 
         let index = self.metrics.block_count;
         self.metrics.block_count += 1;
-        self.blocks.push(Default::default());
+        let mut new_block = CodeBlockHandler::default();
+        new_block.use_rz_as_phase = self.features.use_rz_as_phase;
+        self.blocks.push(new_block);
         Ok(Label::new(index, self.pid))
     }
 
     pub fn open_block(&mut self, label: &Label) -> Result<()> {
         self.match_pid(label)?;
         self.current_block = label.index();
         Ok(())
```

### Comparing `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/serialize.rs` & `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/serialize.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/clib/wrapper.py` & `ket-lang-0.6.0.dev1/src/ket/clib/wrapper.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/gates/__init__.py` & `ket-lang-0.6.0.dev1/src/ket/gates/__init__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/gates/base_gates.py` & `ket-lang-0.6.0.dev1/src/ket/gates/base_gates.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/gates/quantum_gate.py` & `ket-lang-0.6.0.dev1/src/ket/gates/quantum_gate.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/import_ket.py` & `ket-lang-0.6.0.dev1/src/ket/import_ket.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/kbw.py` & `ket-lang-0.6.0.dev1/src/ket/kbw.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/lib.py` & `ket-lang-0.6.0.dev1/src/ket/lib.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/plugins.py` & `ket-lang-0.6.0.dev1/src/ket/plugins.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/preprocessor/statements.py` & `ket-lang-0.6.0.dev1/src/ket/preprocessor/statements.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/preprocessor/transformer.py` & `ket-lang-0.6.0.dev1/src/ket/preprocessor/transformer.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/process.py` & `ket-lang-0.6.0.dev1/src/ket/process.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/standard/__init__.py` & `ket-lang-0.6.0.dev1/src/ket/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/standard/adj.py` & `ket-lang-0.6.0.dev1/src/ket/standard/adj.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket/standard/ctrl.py` & `ket-lang-0.6.0.dev1/src/ket/standard/ctrl.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.3b1/src/ket_lang.egg-info/PKG-INFO` & `ket-lang-0.6.0.dev1/src/ket_lang.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: ket-lang
-Version: 0.5.3b1
+Version: 0.6.0.dev1
 Summary: Ket quantum programming language interpreter and library
 Home-page: https://quantumket.org
 Author: Evandro Chagas Ribeiro da Rosa
-Author-email: ev.crr97@gmail.com
+Author-email: evandro@quantuloop.com
 License: Apache-2.0
 Project-URL: Source, https://gitlab.com/quantum-ket/ket
 Keywords: quantum computer,quantum programming,quantum simulator
 Platform: linux
 Platform: win32
 Platform: osx
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Rust
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 [![PyPI](https://img.shields.io/pypi/v/ket-lang.svg)](https://pypi.org/project/ket-lang/)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
 
 # Ket Quantum Programming
```

### Comparing `ket-lang-0.5.3b1/src/ket_lang.egg-info/SOURCES.txt` & `ket-lang-0.6.0.dev1/src/ket_lang.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 src/ket/clib/libs/libket/CHANGELOG.md
 src/ket/clib/libs/libket/Cargo.toml
 src/ket/clib/libs/libket/LICENSE
 src/ket/clib/libs/libket/README.md
 src/ket/clib/libs/libket/libket.h
 src/ket/clib/libs/libket/libket.hpp
 src/ket/clib/libs/libket/src/code_block.rs
+src/ket/clib/libs/libket/src/decompose.rs
 src/ket/clib/libs/libket/src/error.rs
 src/ket/clib/libs/libket/src/gates.rs
 src/ket/clib/libs/libket/src/instruction.rs
 src/ket/clib/libs/libket/src/ir.rs
 src/ket/clib/libs/libket/src/lib.rs
 src/ket/clib/libs/libket/src/object.rs
 src/ket/clib/libs/libket/src/process.rs
```

