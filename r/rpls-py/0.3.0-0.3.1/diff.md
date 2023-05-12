# Comparing `tmp/rpls_py-0.3.0.tar.gz` & `tmp/rpls_py-0.3.1.tar.gz`

## Comparing `rpls_py-0.3.0.tar` & `rpls_py-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 rpls_py-0.3.0/Cargo.toml
--rw-rw-r--   0     1000     1000     2905 2023-04-17 22:53:47.000000 rpls_py-0.3.0/.github/workflows/CI.yml
--rw-rw-r--   0     1000     1000      327 2023-04-17 19:52:01.000000 rpls_py-0.3.0/.gitignore
--rw-rw-r--   0     1000     1000        9 2023-04-17 18:22:01.000000 rpls_py-0.3.0/README.md
--rw-rw-r--   0     1000     1000      369 2023-04-17 18:23:20.000000 rpls_py-0.3.0/pyproject.toml
--rw-rw-r--   0     1000     1000      125 2023-04-17 19:51:20.000000 rpls_py-0.3.0/requirements.txt
--rw-rw-r--   0     1000     1000     1453 2023-04-19 19:55:06.000000 rpls_py-0.3.0/src/lib.rs
--rw-rw-r--   0     1000     1000    38462 2023-05-12 21:12:23.000000 rpls_py-0.3.0/Cargo.lock
--rw-r--r--   0        0        0      335 1970-01-01 00:00:00.000000 rpls_py-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 rpls_py-0.3.1/Cargo.toml
+-rw-rw-r--   0     1000     1000     2905 2023-04-17 22:53:47.000000 rpls_py-0.3.1/.github/workflows/CI.yml
+-rw-rw-r--   0     1000     1000      327 2023-04-17 19:52:01.000000 rpls_py-0.3.1/.gitignore
+-rw-rw-r--   0     1000     1000        9 2023-04-17 18:22:01.000000 rpls_py-0.3.1/README.md
+-rw-rw-r--   0     1000     1000      562 2023-05-12 21:28:21.000000 rpls_py-0.3.1/pyproject.toml
+-rw-rw-r--   0     1000     1000      125 2023-04-17 19:51:20.000000 rpls_py-0.3.1/requirements.txt
+-rw-rw-r--   0     1000     1000     1453 2023-04-19 19:55:06.000000 rpls_py-0.3.1/src/lib.rs
+-rw-rw-r--   0     1000     1000    38462 2023-05-12 21:27:48.000000 rpls_py-0.3.1/Cargo.lock
+-rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 rpls_py-0.3.1/PKG-INFO
```

### Comparing `rpls_py-0.3.0/.github/workflows/CI.yml` & `rpls_py-0.3.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rpls_py-0.3.0/src/lib.rs` & `rpls_py-0.3.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rpls_py-0.3.0/Cargo.lock` & `rpls_py-0.3.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -959,15 +959,15 @@
  "geo",
  "geo-types",
  "plotters",
 ]
 
 [[package]]
 name = "rpls-py"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
  "pyo3",
  "rpls",
 ]
 
 [[package]]
 name = "rstar"
```

