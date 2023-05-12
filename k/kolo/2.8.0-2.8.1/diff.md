# Comparing `tmp/kolo-2.8.0.tar.gz` & `tmp/kolo-2.8.1.tar.gz`

## Comparing `kolo-2.8.0.tar` & `kolo-2.8.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 kolo-2.8.0/rust/Cargo.toml
--rw-rw-r--   0     1000     1001       54 2023-05-03 16:01:08.000000 kolo-2.8.0/rust/build.rs
--rw-rw-r--   0     1000     1001    35236 2023-05-03 16:01:08.000000 kolo-2.8.0/rust/src/lib.rs
--rw-rw-r--   0     1000     1001     2129 2023-05-03 16:01:08.000000 kolo-2.8.0/pyproject.toml
--rw-rw-r--   0     1000     1001    11199 2023-05-03 16:02:03.000000 kolo-2.8.0/rust/Cargo.lock
--rw-rw-r--   0     1000     1001     2149 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/django_schema.py
--rw-rw-r--   0     1000     1001     3798 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/serialize.py
--rw-rw-r--   0     1000     1001     3400 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/filters/requests.py
--rw-rw-r--   0     1000     1001      348 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/filters/kolo.py
--rw-rw-r--   0     1000     1001     1322 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/filters/unittest.py
--rw-rw-r--   0     1000     1001     4448 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/filters/exception.py
--rw-rw-r--   0     1000     1001     1457 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/filters/pytest.py
--rw-rw-r--   0     1000     1001     4345 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/filters/sql.py
--rw-rw-r--   0     1000     1001     2262 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/filters/celery.py
--rw-rw-r--   0     1000     1001     3157 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/filters/urllib.py
--rw-rw-r--   0     1000     1001     4141 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/filters/django.py
--rw-rw-r--   0     1000     1001     1778 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/filters/logging.py
--rw-rw-r--   0     1000     1001     5180 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/filters/core.py
--rw-rw-r--   0     1000     1001      809 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/filters/attrs.py
--rw-rw-r--   0     1000     1001     3707 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/filters/urllib3.py
--rw-rw-r--   0     1000     1001      141 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/filters/pypy.py
--rw-rw-r--   0     1000     1001        0 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/filters/__init__.py
--rw-rw-r--   0     1000     1001     2921 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/filters/huey.py
--rw-rw-r--   0     1000     1001     2640 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/middleware.py
--rw-rw-r--   0     1000     1001     1831 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/templates/django_request_test.py.j2
--rw-rw-r--   0     1000     1001    13710 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/profiler.py
--rw-rw-r--   0     1000     1001      169 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/version.py
--rw-rw-r--   0     1000     1001    12633 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/generate_tests.py
--rw-rw-r--   0     1000     1001      360 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/utils.py
--rw-rw-r--   0     1000     1001    10215 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/__main__.py
--rw-rw-r--   0     1000     1001     4846 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/db.py
--rw-rw-r--   0     1000     1001      473 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/git.py
--rw-rw-r--   0     1000     1001      228 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/pytest_plugin.py
--rw-rw-r--   0     1000     1001      108 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/__init__.py
--rw-rw-r--   0     1000     1001     2881 2023-05-03 16:01:08.000000 kolo-2.8.0/src/kolo/config.py
--rw-rw-r--   0     1000     1001      228 2023-05-03 16:01:08.000000 kolo-2.8.0/README.md
--rw-r--r--   0        0        0     2280 1970-01-01 00:00:00.000000 kolo-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 kolo-2.8.1/rust/Cargo.toml
+-rw-rw-r--   0     1000     1001       54 2023-05-11 21:53:18.000000 kolo-2.8.1/rust/build.rs
+-rw-rw-r--   0     1000     1001    35207 2023-05-11 21:53:18.000000 kolo-2.8.1/rust/src/lib.rs
+-rw-rw-r--   0     1000     1001     2156 2023-05-11 21:53:18.000000 kolo-2.8.1/pyproject.toml
+-rw-rw-r--   0     1000     1001    11199 2023-05-11 21:54:05.000000 kolo-2.8.1/rust/Cargo.lock
+-rw-rw-r--   0     1000     1001     2149 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/django_schema.py
+-rw-rw-r--   0     1000     1001     3798 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/serialize.py
+-rw-rw-r--   0     1000     1001     3400 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/filters/requests.py
+-rw-rw-r--   0     1000     1001      348 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/filters/kolo.py
+-rw-rw-r--   0     1000     1001     1322 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/filters/unittest.py
+-rw-rw-r--   0     1000     1001     4448 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/filters/exception.py
+-rw-rw-r--   0     1000     1001     1457 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/filters/pytest.py
+-rw-rw-r--   0     1000     1001     4345 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/filters/sql.py
+-rw-rw-r--   0     1000     1001     2262 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/filters/celery.py
+-rw-rw-r--   0     1000     1001     3157 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/filters/urllib.py
+-rw-rw-r--   0     1000     1001     4141 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/filters/django.py
+-rw-rw-r--   0     1000     1001     1778 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/filters/logging.py
+-rw-rw-r--   0     1000     1001     5180 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/filters/core.py
+-rw-rw-r--   0     1000     1001      809 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/filters/attrs.py
+-rw-rw-r--   0     1000     1001     3707 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/filters/urllib3.py
+-rw-rw-r--   0     1000     1001      141 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/filters/pypy.py
+-rw-rw-r--   0     1000     1001        0 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/filters/__init__.py
+-rw-rw-r--   0     1000     1001     2921 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/filters/huey.py
+-rw-rw-r--   0     1000     1001     2640 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/middleware.py
+-rw-rw-r--   0     1000     1001     1831 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/templates/django_request_test.py.j2
+-rw-rw-r--   0     1000     1001    13710 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/profiler.py
+-rw-rw-r--   0     1000     1001      169 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/version.py
+-rw-rw-r--   0     1000     1001    12684 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/generate_tests.py
+-rw-rw-r--   0     1000     1001      360 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/utils.py
+-rw-rw-r--   0     1000     1001    10215 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/__main__.py
+-rw-rw-r--   0     1000     1001     4846 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/db.py
+-rw-rw-r--   0     1000     1001      473 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/git.py
+-rw-rw-r--   0     1000     1001      228 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/pytest_plugin.py
+-rw-rw-r--   0     1000     1001      108 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/__init__.py
+-rw-rw-r--   0     1000     1001     2881 2023-05-11 21:53:18.000000 kolo-2.8.1/src/kolo/config.py
+-rw-rw-r--   0     1000     1001      228 2023-05-11 21:53:18.000000 kolo-2.8.1/README.md
+-rw-r--r--   0        0        0     2280 1970-01-01 00:00:00.000000 kolo-2.8.1/PKG-INFO
```

### Comparing `kolo-2.8.0/rust/src/lib.rs` & `kolo-2.8.1/rust/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -106,19 +106,18 @@
             .as_secs_f64()
     }
 
     fn frame_path(frame: &PyFrame, py: Python) -> Result<String, PyErr> {
         let f_code = frame.getattr(intern!(py, "f_code"))?;
         let co_filename = f_code.getattr(intern!(py, "co_filename"))?;
         let filename = co_filename.extract::<String>()?;
-        let path = Path::new(&filename).canonicalize().unwrap();
+        let path = Path::new(&filename).canonicalize()?;
         let dir = current_dir()
             .expect("Current directory is invalid")
-            .canonicalize()
-            .unwrap();
+            .canonicalize()?;
         let relative_path = match path.strip_prefix(&dir) {
             Ok(relative_path) => relative_path,
             Err(_) => &path,
         };
         let lineno = frame.getattr(intern!(py, "f_lineno"))?;
         Ok(format!("{}:{}", relative_path.display(), lineno))
     }
```

### Comparing `kolo-2.8.0/pyproject.toml` & `kolo-2.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "kolo"
-version = "2.8.0"
+version = "2.8.1"
 description = "See everything happening in your running Django app"
 readme = "README.md"
 authors = [
     {name = "Wilhelm Klopp", email = "team@kolo.app"},
     {name = "Lily Foote", email = "lily@kolo.app"},
 ]
 urls.Homepage = "https://kolo.app"
@@ -65,7 +65,8 @@
 [project.entry-points."pytest11"]
 kolo = "kolo.pytest_plugin"
 
 [tool.maturin]
 
 features = ["pyo3/extension-module"]
 profile = "release"
+module-name = "kolo._kolo"
```

### Comparing `kolo-2.8.0/rust/Cargo.lock` & `kolo-2.8.1/rust/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "_kolo"
-version = "2.6.0"
+version = "2.8.1"
 dependencies = [
  "bstr",
  "once_cell",
  "pyo3",
  "pyo3-build-config",
  "serde_json",
  "ulid",
@@ -81,17 +81,17 @@
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "libc"
-version = "0.2.142"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -216,17 +216,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -282,17 +282,17 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.160"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
+checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
```

### Comparing `kolo-2.8.0/src/kolo/django_schema.py` & `kolo-2.8.1/src/kolo/django_schema.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/serialize.py` & `kolo-2.8.1/src/kolo/serialize.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/filters/requests.py` & `kolo-2.8.1/src/kolo/filters/requests.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/filters/unittest.py` & `kolo-2.8.1/src/kolo/filters/unittest.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/filters/exception.py` & `kolo-2.8.1/src/kolo/filters/exception.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/filters/pytest.py` & `kolo-2.8.1/src/kolo/filters/pytest.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/filters/sql.py` & `kolo-2.8.1/src/kolo/filters/sql.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/filters/celery.py` & `kolo-2.8.1/src/kolo/filters/celery.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/filters/urllib.py` & `kolo-2.8.1/src/kolo/filters/urllib.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/filters/django.py` & `kolo-2.8.1/src/kolo/filters/django.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/filters/logging.py` & `kolo-2.8.1/src/kolo/filters/logging.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/filters/core.py` & `kolo-2.8.1/src/kolo/filters/core.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/filters/attrs.py` & `kolo-2.8.1/src/kolo/filters/attrs.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/filters/urllib3.py` & `kolo-2.8.1/src/kolo/filters/urllib3.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/filters/huey.py` & `kolo-2.8.1/src/kolo/filters/huey.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/middleware.py` & `kolo-2.8.1/src/kolo/middleware.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/templates/django_request_test.py.j2` & `kolo-2.8.1/src/kolo/templates/django_request_test.py.j2`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/profiler.py` & `kolo-2.8.1/src/kolo/profiler.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/generate_tests.py` & `kolo-2.8.1/src/kolo/generate_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,30 @@
         # https://github.com/pallets/jinja/issues/1675
         if platform.system() == "Windows":
             unc_prefix = "\\\\?\\"
             if self._template_root.startswith(unc_prefix):  # pragma: no cover
                 self._template_root = self._template_root[len(unc_prefix) :]
 
 
+def maybe_black(rendered):
+    try:
+        from black import format_file_contents
+        from black.mode import Mode
+        from black.parsing import InvalidInput
+    except ImportError:  # pragma: no cover
+        return rendered
+
+    try:
+        return format_file_contents(
+            rendered, fast=True, mode=Mode(magic_trailing_comma=False)
+        )
+    except InvalidInput:  # pragma: no cover
+        return rendered
+
+
 env = Environment(loader=KoloPackageLoader("kolo"))
 
 
 def _format_header(header: str) -> str:
     header = header.upper().replace("-", "_")
     if header in ("CONTENT_LENGTH", "CONTENT_TYPE"):
         return header
@@ -39,15 +55,15 @@
 UUID_REPR_REGEX = re.compile(
     r"UUID\(\'([0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12})\'\)"
 )
 
 
 def parse_value(column, value, schema_data):
     column_schema = schema_data[column.table]["fields"][column.name]
-    if column_schema["django_field"] == "UUIDField":
+    if column_schema["django_field"] == "django.db.models.fields.UUIDField":
         uuid_match = UUID_REPR_REGEX.match(str(value))
         if uuid_match:
             value = uuid_match[1]
     return value
 
 
 @total_ordering
@@ -335,21 +351,8 @@
         prettified_request_body=prettified_request_body,
         query_params=query_params,
         template_names=served_request_frames[0]["templates"],
         outbound_request_frames=outbound_request_frames,
         sql_fixtures=sql_fixtures,
         imports=sorted(imports),
     )
-    try:
-        from black import format_file_contents
-        from black.mode import Mode
-        from black.parsing import InvalidInput
-    except ImportError:  # pragma: no cover
-        pass
-    else:
-        try:
-            rendered = format_file_contents(
-                rendered, fast=True, mode=Mode(magic_trailing_comma=False)
-            )
-        except InvalidInput:  # pragma: no cover
-            pass
-    return rendered
+    return maybe_black(rendered)
```

### Comparing `kolo-2.8.0/src/kolo/__main__.py` & `kolo-2.8.1/src/kolo/__main__.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/db.py` & `kolo-2.8.1/src/kolo/db.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/src/kolo/config.py` & `kolo-2.8.1/src/kolo/config.py`

 * *Files identical despite different names*

### Comparing `kolo-2.8.0/PKG-INFO` & `kolo-2.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolo
-Version: 2.8.0
+Version: 2.8.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -36,17 +36,17 @@
 Requires-Dist: sqlglot>=11.3.1; extra == 'test_generation'
 Provides-Extra: test_generation
 Summary: See everything happening in your running Django app
 Author-email: Wilhelm Klopp <team@kolo.app>, Lily Foote <lily@kolo.app>
 License: © Kolo
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Homepage, https://kolo.app
-Project-URL: Repository, https://github.com/kolofordjango/kolo
 Project-URL: Changelog, https://docs.kolo.app/en/latest/python-changelog.html
+Project-URL: Repository, https://github.com/kolofordjango/kolo
+Project-URL: Homepage, https://kolo.app
 
 # Kolo
 
 See everything happening in your running Django app
 
 More information: https://kolo.app
```

