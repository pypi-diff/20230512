# Comparing `tmp/granian-0.4.0.tar.gz` & `tmp/granian-0.4.1.tar.gz`

## Comparing `granian-0.4.0.tar` & `granian-0.4.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 granian-0.4.0/Cargo.toml
--rw-r--r--   0     1001      123     1486 2023-05-09 12:42:50.000000 granian-0.4.0/LICENSE
--rw-r--r--   0     1001      123     4024 2023-05-09 12:42:50.000000 granian-0.4.0/README.md
--rw-r--r--   0     1001      123       54 2023-05-09 12:42:50.000000 granian-0.4.0/build.rs
--rw-r--r--   0     1001      123       28 2023-05-09 12:42:50.000000 granian-0.4.0/granian/__init__.py
--rw-r--r--   0     1001      123       22 2023-05-09 12:42:50.000000 granian-0.4.0/granian/__version__.py
--rw-r--r--   0     1001      123     1868 2023-05-09 12:42:50.000000 granian-0.4.0/granian/_granian.pyi
--rw-r--r--   0     1001      123     1677 2023-05-09 12:42:50.000000 granian-0.4.0/granian/_internal.py
--rw-r--r--   0     1001      123     2862 2023-05-09 12:42:50.000000 granian-0.4.0/granian/_loops.py
--rw-r--r--   0     1001      123       93 2023-05-09 12:42:50.000000 granian-0.4.0/granian/_types.py
--rw-r--r--   0     1001      123     4682 2023-05-09 12:42:50.000000 granian-0.4.0/granian/asgi.py
--rw-r--r--   0     1001      123     3590 2023-05-09 12:42:50.000000 granian-0.4.0/granian/cli.py
--rw-r--r--   0     1001      123      357 2023-05-09 12:42:50.000000 granian-0.4.0/granian/constants.py
--rw-r--r--   0     1001      123     1328 2023-05-09 12:42:50.000000 granian-0.4.0/granian/log.py
--rw-r--r--   0     1001      123      153 2023-05-09 12:42:50.000000 granian-0.4.0/granian/net.py
--rw-r--r--   0     1001      123        0 2023-05-09 12:42:50.000000 granian-0.4.0/granian/py.typed
--rw-r--r--   0     1001      123      462 2023-05-09 12:42:50.000000 granian-0.4.0/granian/rsgi.py
--rw-r--r--   0     1001      123    10646 2023-05-09 12:42:50.000000 granian-0.4.0/granian/server.py
--rw-r--r--   0     1001      123     2068 2023-05-09 12:42:50.000000 granian-0.4.0/granian/wsgi.py
--rw-r--r--   0     1001      123     1624 2023-05-09 12:42:50.000000 granian-0.4.0/pyproject.toml
--rw-r--r--   0     1001      123     5700 2023-05-09 12:42:50.000000 granian-0.4.0/src/asgi/callbacks.rs
--rw-r--r--   0     1001      123     1611 2023-05-09 12:42:50.000000 granian-0.4.0/src/asgi/errors.rs
--rw-r--r--   0     1001      123     4765 2023-05-09 12:42:50.000000 granian-0.4.0/src/asgi/http.rs
--rw-r--r--   0     1001      123    15092 2023-05-09 12:42:50.000000 granian-0.4.0/src/asgi/io.rs
--rw-r--r--   0     1001      123      329 2023-05-09 12:42:50.000000 granian-0.4.0/src/asgi/mod.rs
--rw-r--r--   0     1001      123     2995 2023-05-09 12:42:50.000000 granian-0.4.0/src/asgi/serve.rs
--rw-r--r--   0     1001      123     2708 2023-05-09 12:42:50.000000 granian-0.4.0/src/asgi/types.rs
--rw-r--r--   0     1001      123     8605 2023-05-09 12:42:50.000000 granian-0.4.0/src/callbacks.rs
--rw-r--r--   0     1001      123      415 2023-05-09 12:42:50.000000 granian-0.4.0/src/http.rs
--rw-r--r--   0     1001      123      550 2023-05-09 12:42:50.000000 granian-0.4.0/src/lib.rs
--rw-r--r--   0     1001      123     4934 2023-05-09 12:42:50.000000 granian-0.4.0/src/rsgi/callbacks.rs
--rw-r--r--   0     1001      123      565 2023-05-09 12:42:50.000000 granian-0.4.0/src/rsgi/errors.rs
--rw-r--r--   0     1001      123     5186 2023-05-09 12:42:50.000000 granian-0.4.0/src/rsgi/http.rs
--rw-r--r--   0     1001      123    10350 2023-05-09 12:42:50.000000 granian-0.4.0/src/rsgi/io.rs
--rw-r--r--   0     1001      123      609 2023-05-09 12:42:50.000000 granian-0.4.0/src/rsgi/mod.rs
--rw-r--r--   0     1001      123     2995 2023-05-09 12:42:50.000000 granian-0.4.0/src/rsgi/serve.rs
--rw-r--r--   0     1001      123     5619 2023-05-09 12:42:50.000000 granian-0.4.0/src/rsgi/types.rs
--rw-r--r--   0     1001      123     8066 2023-05-09 12:42:50.000000 granian-0.4.0/src/runtime.rs
--rw-r--r--   0     1001      123     4301 2023-05-09 12:42:50.000000 granian-0.4.0/src/tcp.rs
--rw-r--r--   0     1001      123     2431 2023-05-09 12:42:50.000000 granian-0.4.0/src/tls.rs
--rw-r--r--   0     1001      123      837 2023-05-09 12:42:50.000000 granian-0.4.0/src/utils.rs
--rw-r--r--   0     1001      123    16456 2023-05-09 12:42:50.000000 granian-0.4.0/src/workers.rs
--rw-r--r--   0     1001      123     3435 2023-05-09 12:42:50.000000 granian-0.4.0/src/ws.rs
--rw-r--r--   0     1001      123     1027 2023-05-09 12:42:50.000000 granian-0.4.0/src/wsgi/callbacks.rs
--rw-r--r--   0     1001      123      308 2023-05-09 12:42:50.000000 granian-0.4.0/src/wsgi/errors.rs
--rw-r--r--   0     1001      123     1638 2023-05-09 12:42:50.000000 granian-0.4.0/src/wsgi/http.rs
--rw-r--r--   0     1001      123      312 2023-05-09 12:42:50.000000 granian-0.4.0/src/wsgi/mod.rs
--rw-r--r--   0     1001      123     2206 2023-05-09 12:42:50.000000 granian-0.4.0/src/wsgi/serve.rs
--rw-r--r--   0     1001      123     4151 2023-05-09 12:42:50.000000 granian-0.4.0/src/wsgi/types.rs
--rw-r--r--   0     1001      123     3078 2023-05-09 12:42:50.000000 granian-0.4.0/tests/apps/asgi.py
--rw-r--r--   0     1001      123     2490 2023-05-09 12:42:50.000000 granian-0.4.0/tests/apps/rsgi.py
--rw-r--r--   0     1001      123      861 2023-05-09 12:42:50.000000 granian-0.4.0/tests/apps/wsgi.py
--rw-r--r--   0     1001      123     1759 2023-05-09 12:42:50.000000 granian-0.4.0/tests/conftest.py
--rw-r--r--   0     1001      123     1139 2023-05-09 12:42:50.000000 granian-0.4.0/tests/fixtures/tls/cert.pem
--rw-r--r--   0     1001      123     1704 2023-05-09 12:42:50.000000 granian-0.4.0/tests/fixtures/tls/key.pem
--rw-r--r--   0     1001      123     1830 2023-05-09 12:42:50.000000 granian-0.4.0/tests/test_asgi.py
--rw-r--r--   0     1001      123     1851 2023-05-09 12:42:50.000000 granian-0.4.0/tests/test_https.py
--rw-r--r--   0     1001      123     1450 2023-05-09 12:42:50.000000 granian-0.4.0/tests/test_rsgi.py
--rw-r--r--   0     1001      123     2487 2023-05-09 12:42:50.000000 granian-0.4.0/tests/test_ws.py
--rw-r--r--   0     1001      123     1438 2023-05-09 12:42:50.000000 granian-0.4.0/tests/test_wsgi.py
--rw-r--r--   0     1001      123    33385 2023-05-09 12:42:50.000000 granian-0.4.0/Cargo.lock
--rw-r--r--   0        0        0     5801 1970-01-01 00:00:00.000000 granian-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 granian-0.4.1/Cargo.toml
+-rw-r--r--   0     1001      123     1486 2023-05-12 10:32:03.000000 granian-0.4.1/LICENSE
+-rw-r--r--   0     1001      123     4024 2023-05-12 10:32:03.000000 granian-0.4.1/README.md
+-rw-r--r--   0     1001      123       54 2023-05-12 10:32:03.000000 granian-0.4.1/build.rs
+-rw-r--r--   0     1001      123       28 2023-05-12 10:32:03.000000 granian-0.4.1/granian/__init__.py
+-rw-r--r--   0     1001      123       22 2023-05-12 10:32:03.000000 granian-0.4.1/granian/__version__.py
+-rw-r--r--   0     1001      123     1868 2023-05-12 10:32:03.000000 granian-0.4.1/granian/_granian.pyi
+-rw-r--r--   0     1001      123     1677 2023-05-12 10:32:03.000000 granian-0.4.1/granian/_internal.py
+-rw-r--r--   0     1001      123     2862 2023-05-12 10:32:03.000000 granian-0.4.1/granian/_loops.py
+-rw-r--r--   0     1001      123       93 2023-05-12 10:32:03.000000 granian-0.4.1/granian/_types.py
+-rw-r--r--   0     1001      123     4682 2023-05-12 10:32:03.000000 granian-0.4.1/granian/asgi.py
+-rw-r--r--   0     1001      123     3590 2023-05-12 10:32:03.000000 granian-0.4.1/granian/cli.py
+-rw-r--r--   0     1001      123      357 2023-05-12 10:32:03.000000 granian-0.4.1/granian/constants.py
+-rw-r--r--   0     1001      123     1328 2023-05-12 10:32:03.000000 granian-0.4.1/granian/log.py
+-rw-r--r--   0     1001      123      153 2023-05-12 10:32:03.000000 granian-0.4.1/granian/net.py
+-rw-r--r--   0     1001      123        0 2023-05-12 10:32:03.000000 granian-0.4.1/granian/py.typed
+-rw-r--r--   0     1001      123      462 2023-05-12 10:32:03.000000 granian-0.4.1/granian/rsgi.py
+-rw-r--r--   0     1001      123    10646 2023-05-12 10:32:03.000000 granian-0.4.1/granian/server.py
+-rw-r--r--   0     1001      123     2068 2023-05-12 10:32:03.000000 granian-0.4.1/granian/wsgi.py
+-rw-r--r--   0     1001      123     1624 2023-05-12 10:32:03.000000 granian-0.4.1/pyproject.toml
+-rw-r--r--   0     1001      123     6824 2023-05-12 10:32:03.000000 granian-0.4.1/src/asgi/callbacks.rs
+-rw-r--r--   0     1001      123     1611 2023-05-12 10:32:03.000000 granian-0.4.1/src/asgi/errors.rs
+-rw-r--r--   0     1001      123     4765 2023-05-12 10:32:03.000000 granian-0.4.1/src/asgi/http.rs
+-rw-r--r--   0     1001      123    15092 2023-05-12 10:32:03.000000 granian-0.4.1/src/asgi/io.rs
+-rw-r--r--   0     1001      123      329 2023-05-12 10:32:03.000000 granian-0.4.1/src/asgi/mod.rs
+-rw-r--r--   0     1001      123     2995 2023-05-12 10:32:03.000000 granian-0.4.1/src/asgi/serve.rs
+-rw-r--r--   0     1001      123     2708 2023-05-12 10:32:03.000000 granian-0.4.1/src/asgi/types.rs
+-rw-r--r--   0     1001      123     8784 2023-05-12 10:32:03.000000 granian-0.4.1/src/callbacks.rs
+-rw-r--r--   0     1001      123      415 2023-05-12 10:32:03.000000 granian-0.4.1/src/http.rs
+-rw-r--r--   0     1001      123      550 2023-05-12 10:32:03.000000 granian-0.4.1/src/lib.rs
+-rw-r--r--   0     1001      123     6058 2023-05-12 10:32:03.000000 granian-0.4.1/src/rsgi/callbacks.rs
+-rw-r--r--   0     1001      123      565 2023-05-12 10:32:03.000000 granian-0.4.1/src/rsgi/errors.rs
+-rw-r--r--   0     1001      123     5186 2023-05-12 10:32:03.000000 granian-0.4.1/src/rsgi/http.rs
+-rw-r--r--   0     1001      123    10350 2023-05-12 10:32:03.000000 granian-0.4.1/src/rsgi/io.rs
+-rw-r--r--   0     1001      123      609 2023-05-12 10:32:03.000000 granian-0.4.1/src/rsgi/mod.rs
+-rw-r--r--   0     1001      123     2995 2023-05-12 10:32:03.000000 granian-0.4.1/src/rsgi/serve.rs
+-rw-r--r--   0     1001      123     5619 2023-05-12 10:32:03.000000 granian-0.4.1/src/rsgi/types.rs
+-rw-r--r--   0     1001      123     8066 2023-05-12 10:32:03.000000 granian-0.4.1/src/runtime.rs
+-rw-r--r--   0     1001      123     4301 2023-05-12 10:32:03.000000 granian-0.4.1/src/tcp.rs
+-rw-r--r--   0     1001      123     2431 2023-05-12 10:32:03.000000 granian-0.4.1/src/tls.rs
+-rw-r--r--   0     1001      123      837 2023-05-12 10:32:03.000000 granian-0.4.1/src/utils.rs
+-rw-r--r--   0     1001      123    16456 2023-05-12 10:32:03.000000 granian-0.4.1/src/workers.rs
+-rw-r--r--   0     1001      123     3435 2023-05-12 10:32:03.000000 granian-0.4.1/src/ws.rs
+-rw-r--r--   0     1001      123     1027 2023-05-12 10:32:03.000000 granian-0.4.1/src/wsgi/callbacks.rs
+-rw-r--r--   0     1001      123      308 2023-05-12 10:32:03.000000 granian-0.4.1/src/wsgi/errors.rs
+-rw-r--r--   0     1001      123     1638 2023-05-12 10:32:03.000000 granian-0.4.1/src/wsgi/http.rs
+-rw-r--r--   0     1001      123      312 2023-05-12 10:32:03.000000 granian-0.4.1/src/wsgi/mod.rs
+-rw-r--r--   0     1001      123     2206 2023-05-12 10:32:03.000000 granian-0.4.1/src/wsgi/serve.rs
+-rw-r--r--   0     1001      123     4151 2023-05-12 10:32:03.000000 granian-0.4.1/src/wsgi/types.rs
+-rw-r--r--   0     1001      123     3078 2023-05-12 10:32:03.000000 granian-0.4.1/tests/apps/asgi.py
+-rw-r--r--   0     1001      123     2490 2023-05-12 10:32:03.000000 granian-0.4.1/tests/apps/rsgi.py
+-rw-r--r--   0     1001      123      861 2023-05-12 10:32:03.000000 granian-0.4.1/tests/apps/wsgi.py
+-rw-r--r--   0     1001      123     1759 2023-05-12 10:32:03.000000 granian-0.4.1/tests/conftest.py
+-rw-r--r--   0     1001      123     1139 2023-05-12 10:32:03.000000 granian-0.4.1/tests/fixtures/tls/cert.pem
+-rw-r--r--   0     1001      123     1704 2023-05-12 10:32:03.000000 granian-0.4.1/tests/fixtures/tls/key.pem
+-rw-r--r--   0     1001      123     1830 2023-05-12 10:32:03.000000 granian-0.4.1/tests/test_asgi.py
+-rw-r--r--   0     1001      123     1851 2023-05-12 10:32:03.000000 granian-0.4.1/tests/test_https.py
+-rw-r--r--   0     1001      123     1450 2023-05-12 10:32:03.000000 granian-0.4.1/tests/test_rsgi.py
+-rw-r--r--   0     1001      123     2487 2023-05-12 10:32:03.000000 granian-0.4.1/tests/test_ws.py
+-rw-r--r--   0     1001      123     1438 2023-05-12 10:32:03.000000 granian-0.4.1/tests/test_wsgi.py
+-rw-r--r--   0     1001      123    33385 2023-05-12 10:32:03.000000 granian-0.4.1/Cargo.lock
+-rw-r--r--   0        0        0     5801 1970-01-01 00:00:00.000000 granian-0.4.1/PKG-INFO
```

### Comparing `granian-0.4.0/Cargo.toml` & `granian-0.4.1/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "granian"
-version = "0.4.0"
+version = "0.4.1"
 description = "A Rust HTTP server for Python applications"
 authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 edition = "2021"
 
 keywords = ["web", "asyncio"]
```

### Comparing `granian-0.4.0/LICENSE` & `granian-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/README.md` & `granian-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/granian/_granian.pyi` & `granian-0.4.1/granian/_granian.pyi`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/granian/_internal.py` & `granian-0.4.1/granian/_internal.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/granian/_loops.py` & `granian-0.4.1/granian/_loops.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/granian/asgi.py` & `granian-0.4.1/granian/asgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/granian/cli.py` & `granian-0.4.1/granian/cli.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/granian/log.py` & `granian-0.4.1/granian/log.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/granian/server.py` & `granian-0.4.1/granian/server.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/granian/wsgi.py` & `granian-0.4.1/granian/wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/pyproject.toml` & `granian-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/asgi/callbacks.rs` & `granian-0.4.1/src/rsgi/callbacks.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,181 +1,209 @@
-use hyper::{Body, Request, Response};
 use pyo3::prelude::*;
+use pyo3_asyncio::TaskLocals;
 use tokio::sync::oneshot;
 
 use crate::{
     callbacks::{
         CallbackWrapper,
         callback_impl_run,
+        callback_impl_loop_run,
         callback_impl_loop_step,
         callback_impl_loop_wake,
         callback_impl_loop_err
     },
     runtime::RuntimeRef,
     ws::{HyperWebsocket, UpgradeData}
 };
 use super::{
-    io::{ASGIHTTPProtocol as HTTPProtocol, ASGIWebsocketProtocol as WebsocketProtocol},
-    types::ASGIScope as Scope
+    io::{RSGIHTTPProtocol as HTTPProtocol, RSGIWebsocketProtocol as WebsocketProtocol},
+    types::{RSGIScope as Scope, PyResponse, PyResponseBytes}
 };
 
 
 #[pyclass]
 pub(crate) struct CallbackRunnerHTTP {
     proto: Py<HTTPProtocol>,
-    event_loop: PyObject,
-    context: PyObject,
+    context: TaskLocals,
     cb: PyObject
 }
 
 impl CallbackRunnerHTTP {
     pub fn new(
         py: Python,
         cb: CallbackWrapper,
         proto: HTTPProtocol,
         scope: Scope
     ) -> Self {
         let pyproto = Py::new(py, proto).unwrap();
         Self {
             proto: pyproto.clone(),
-            event_loop: cb.context.event_loop(py).into(),
-            context: cb.context.context(py).into(),
+            context: cb.context,
             cb: cb.callback.call1(py, (scope, pyproto)).unwrap()
         }
     }
 
+    callback_impl_run!();
+}
+
+#[pymethods]
+impl CallbackRunnerHTTP {
+    fn _loop_task<'p>(&self, py: Python<'p>) -> PyResult<&'p PyAny> {
+        CallbackTaskHTTP::new(py, self.cb.clone(), self.proto.clone(), self.context.clone())?.run(py)
+    }
+}
+
+#[pyclass]
+pub(crate) struct CallbackTaskHTTP {
+    proto: Py<HTTPProtocol>,
+    context: TaskLocals,
+    cb: PyObject
+}
+
+impl CallbackTaskHTTP {
+    pub fn new(
+        py: Python,
+        cb: PyObject,
+        proto: Py<HTTPProtocol>,
+        context: TaskLocals
+    ) -> PyResult<Self> {
+        Ok(Self { proto, context: context.copy_context(py)?, cb })
+    }
+
     fn done(&self, py: Python) {
         if let Ok(mut proto) = self.proto.as_ref(py).try_borrow_mut() {
             if let Some(tx) = proto.tx() {
-                let mut res = Response::new("Internal server error".into());
-                *res.status_mut() = hyper::StatusCode::INTERNAL_SERVER_ERROR;
-                let _ = tx.send(res);
+                let _ = tx.send(
+                    PyResponse::Bytes(PyResponseBytes::empty(500, Vec::new()))
+                );
             }
         }
     }
 
     fn err(&self, py: Python) {
         log::warn!("Application callable raised an exception");
         self.done(py)
     }
 
-    callback_impl_run!();
+    callback_impl_loop_run!();
     callback_impl_loop_err!();
 }
 
 #[pymethods]
-impl CallbackRunnerHTTP {
+impl CallbackTaskHTTP {
     fn _loop_step(pyself: PyRef<'_, Self>, py: Python) -> PyResult<PyObject> {
         callback_impl_loop_step!(pyself, py)
     }
 
     fn _loop_wake(pyself: PyRef<'_, Self>, py: Python, fut: PyObject) -> PyResult<PyObject> {
         callback_impl_loop_wake!(pyself, py, fut)
     }
 }
 
 #[pyclass]
 pub(crate) struct CallbackRunnerWebsocket {
     proto: Py<WebsocketProtocol>,
-    event_loop: PyObject,
-    context: PyObject,
+    context: TaskLocals,
     cb: PyObject
 }
 
 impl CallbackRunnerWebsocket {
     pub fn new(
         py: Python,
         cb: CallbackWrapper,
         proto: WebsocketProtocol,
         scope: Scope
     ) -> Self {
         let pyproto = Py::new(py, proto).unwrap();
         Self {
             proto: pyproto.clone(),
-            event_loop: cb.context.event_loop(py).into(),
-            context: cb.context.context(py).into(),
+            context: cb.context,
             cb: cb.callback.call1(py, (scope, pyproto)).unwrap()
         }
     }
 
+    callback_impl_run!();
+}
+
+#[pymethods]
+impl CallbackRunnerWebsocket {
+    fn _loop_task<'p>(&self, py: Python<'p>) -> PyResult<&'p PyAny> {
+        CallbackTaskWebsocket::new(py, self.cb.clone(), self.proto.clone(), self.context.clone())?.run(py)
+    }
+}
+
+#[pyclass]
+pub(crate) struct CallbackTaskWebsocket {
+    proto: Py<WebsocketProtocol>,
+    context: TaskLocals,
+    cb: PyObject
+}
+
+impl CallbackTaskWebsocket {
+    pub fn new(
+        py: Python,
+        cb: PyObject,
+        proto: Py<WebsocketProtocol>,
+        context: TaskLocals
+    ) -> PyResult<Self> {
+        Ok(Self { proto, context: context.copy_context(py)?, cb })
+    }
+
     fn done(&self, py: Python) {
         if let Ok(mut proto) = self.proto.as_ref(py).try_borrow_mut() {
             if let (Some(tx), res) = proto.tx() {
                 let _ = tx.send(res);
             }
         }
     }
 
     fn err(&self, py: Python) {
         log::warn!("Application callable raised an exception");
         self.done(py)
     }
 
-    callback_impl_run!();
+    callback_impl_loop_run!();
     callback_impl_loop_err!();
 }
 
 #[pymethods]
-impl CallbackRunnerWebsocket {
+impl CallbackTaskWebsocket {
     fn _loop_step(pyself: PyRef<'_, Self>, py: Python) -> PyResult<PyObject> {
         callback_impl_loop_step!(pyself, py)
     }
 
     fn _loop_wake(pyself: PyRef<'_, Self>, py: Python, fut: PyObject) -> PyResult<PyObject> {
         callback_impl_loop_wake!(pyself, py, fut)
     }
 }
 
-// NOTE: we cannot use single `impl` function as structs with pyclass won't handle
-//       dyn fields easily.
-// pub(crate) async fn call(
-//     cb: CallbackWrapper,
-//     protocol: impl ASGIProtocol + IntoPy<PyObject>,
-//     scope: Scope
-// ) -> Result<(), ASGIFlowError> {
-//     let (tx, rx) = oneshot::channel();
-//     let callback = cb.callback.clone();
-//     Python::with_gil(|py| {
-//         callback.call1(py, (CallbackWatcher::new(py, cb, tx), scope, protocol))
-//     })?;
-
-//     match rx.await {
-//         Ok(true) => Ok(()),
-//         Ok(false) => {
-//             log::warn!("Application callable raised an exception");
-//             error_flow!()
-//         },
-//         _ => error_flow!()
-//     }
-// }
-
 pub(crate) fn call_rtb_http(
     cb: CallbackWrapper,
     rt: RuntimeRef,
-    req: Request<Body>,
+    req: hyper::Request<hyper::Body>,
     scope: Scope
-) -> oneshot::Receiver<Response<Body>> {
+) -> oneshot::Receiver<PyResponse> {
     let (tx, rx) = oneshot::channel();
-    let protocol = HTTPProtocol::new(rt, req, tx);
+    let protocol = HTTPProtocol::new(rt, tx, req);
 
     Python::with_gil(|py| {
         let _ = CallbackRunnerHTTP::new(py, cb, protocol, scope).run(py);
     });
 
     rx
 }
 
 pub(crate) fn call_rtt_http(
     cb: CallbackWrapper,
     rt: RuntimeRef,
-    req: Request<Body>,
+    req: hyper::Request<hyper::Body>,
     scope: Scope
-) -> oneshot::Receiver<Response<Body>> {
+) -> oneshot::Receiver<PyResponse> {
     let (tx, rx) = oneshot::channel();
-    let protocol = HTTPProtocol::new(rt, req, tx);
+    let protocol = HTTPProtocol::new(rt, tx, req);
 
     tokio::task::spawn_blocking(move || {
         Python::with_gil(|py| {
             let _ = CallbackRunnerHTTP::new(py, cb, protocol, scope).run(py);
         });
     });
 
@@ -184,15 +212,15 @@
 
 pub(crate) fn call_rtb_ws(
     cb: CallbackWrapper,
     rt: RuntimeRef,
     ws: HyperWebsocket,
     upgrade: UpgradeData,
     scope: Scope
-) -> oneshot::Receiver<bool> {
+) -> oneshot::Receiver<(i32, bool)> {
     let (tx, rx) = oneshot::channel();
     let protocol = WebsocketProtocol::new(rt, tx, ws, upgrade);
 
     Python::with_gil(|py| {
         let _ = CallbackRunnerWebsocket::new(py, cb, protocol, scope).run(py);
     });
 
@@ -201,15 +229,15 @@
 
 pub(crate) fn call_rtt_ws(
     cb: CallbackWrapper,
     rt: RuntimeRef,
     ws: HyperWebsocket,
     upgrade: UpgradeData,
     scope: Scope
-) -> oneshot::Receiver<bool> {
+) -> oneshot::Receiver<(i32, bool)> {
     let (tx, rx) = oneshot::channel();
     let protocol = WebsocketProtocol::new(rt, tx, ws, upgrade);
 
     tokio::task::spawn_blocking(move || {
         Python::with_gil(|py| {
             let _ = CallbackRunnerWebsocket::new(py, cb, protocol, scope).run(py);
         });
```

### Comparing `granian-0.4.0/src/asgi/errors.rs` & `granian-0.4.1/src/asgi/errors.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/asgi/http.rs` & `granian-0.4.1/src/asgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/asgi/io.rs` & `granian-0.4.1/src/asgi/io.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/asgi/serve.rs` & `granian-0.4.1/src/asgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/asgi/types.rs` & `granian-0.4.1/src/asgi/types.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/callbacks.rs` & `granian-0.4.1/src/callbacks.rs`

 * *Files 6% similar despite different names*

```diff
@@ -187,25 +187,29 @@
     fn __await__(&mut self, py: Python) -> PyObject {
         self.inner.to_object(py)
     }
 }
 
 macro_rules! callback_impl_run {
     () => {
-        pub fn run(self, py: Python) -> PyResult<PyObject> {
-            let event_loop = self.event_loop.clone();
-            let context = self.context.clone();
-            let target = self.into_py(py).getattr(py, pyo3::intern!(py, "_loop_step"))?;
-            let kwctx = pyo3::types::PyDict::new(py);
-            kwctx.set_item("context", context)?;
-            event_loop.call_method(
-                py,
-                pyo3::intern!(py, "call_soon_threadsafe"),
-                (target,),
-                Some(kwctx)
+        pub fn run<'p>(self, py: Python<'p>) -> PyResult<&'p PyAny> {
+            let event_loop = self.context.event_loop(py);
+            let target = self.into_py(py).getattr(py, pyo3::intern!(py, "_loop_task"))?;
+            event_loop.call_method1(pyo3::intern!(py, "call_soon_threadsafe"), (target,))
+        }
+    };
+}
+
+macro_rules! callback_impl_loop_run {
+    () => {
+        pub fn run<'p>(self, py: Python<'p>) -> PyResult<&'p PyAny> {
+            let context = self.context.context(py);
+            context.call_method1(
+                pyo3::intern!(py, "run"),
+                (self.into_py(py).getattr(py, pyo3::intern!(py, "_loop_step"))?,)
             )
         }
     };
 }
 
 macro_rules! callback_impl_loop_step {
     ($pyself:expr, $py:expr) => {
@@ -215,16 +219,17 @@
                     $py,
                     pyo3::intern!($py, "_asyncio_future_blocking")
                 ) {
                     Ok(v) => v.extract($py)?,
                     _ => false
                 };
 
+                let ctx = $pyself.context.context($py);
                 let kwctx = pyo3::types::PyDict::new($py);
-                kwctx.set_item("context", $pyself.context.clone())?;
+                kwctx.set_item("context", ctx)?;
 
                 match blocking {
                     true => {
                         res.setattr(
                             $py,
                             pyo3::intern!($py, "_asyncio_future_blocking"),
                             false
@@ -238,17 +243,16 @@
                                 .getattr($py, pyo3::intern!($py, "_loop_wake"))?,
                             ),
                             Some(kwctx)
                         )?;
                         Ok($py.None())
                     },
                     false => {
-                        let event_loop = $pyself.event_loop.clone();
+                        let event_loop = $pyself.context.event_loop($py);
                         event_loop.call_method(
-                            $py,
                             pyo3::intern!($py, "call_soon"),
                             (
                                 $pyself
                                 .into_py($py)
                                 .getattr($py, pyo3::intern!($py, "_loop_step"))?,
                             ),
                             Some(kwctx)
@@ -289,10 +293,11 @@
             self.err(py);
             cberr
         }
     };
 }
 
 pub(crate) use callback_impl_run;
+pub(crate) use callback_impl_loop_run;
 pub(crate) use callback_impl_loop_step;
 pub(crate) use callback_impl_loop_wake;
 pub(crate) use callback_impl_loop_err;
```

### Comparing `granian-0.4.0/src/lib.rs` & `granian-0.4.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/rsgi/callbacks.rs` & `granian-0.4.1/src/asgi/callbacks.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,157 +1,233 @@
+use hyper::{Body, Request, Response};
 use pyo3::prelude::*;
+use pyo3_asyncio::TaskLocals;
 use tokio::sync::oneshot;
 
 use crate::{
     callbacks::{
         CallbackWrapper,
         callback_impl_run,
+        callback_impl_loop_run,
         callback_impl_loop_step,
         callback_impl_loop_wake,
         callback_impl_loop_err
     },
     runtime::RuntimeRef,
     ws::{HyperWebsocket, UpgradeData}
 };
 use super::{
-    io::{RSGIHTTPProtocol as HTTPProtocol, RSGIWebsocketProtocol as WebsocketProtocol},
-    types::{RSGIScope as Scope, PyResponse, PyResponseBytes}
+    io::{ASGIHTTPProtocol as HTTPProtocol, ASGIWebsocketProtocol as WebsocketProtocol},
+    types::ASGIScope as Scope
 };
 
 
 #[pyclass]
 pub(crate) struct CallbackRunnerHTTP {
     proto: Py<HTTPProtocol>,
-    event_loop: PyObject,
-    context: PyObject,
+    context: TaskLocals,
     cb: PyObject
 }
 
 impl CallbackRunnerHTTP {
     pub fn new(
         py: Python,
         cb: CallbackWrapper,
         proto: HTTPProtocol,
         scope: Scope
     ) -> Self {
         let pyproto = Py::new(py, proto).unwrap();
         Self {
             proto: pyproto.clone(),
-            event_loop: cb.context.event_loop(py).into(),
-            context: cb.context.context(py).into(),
+            context: cb.context,
             cb: cb.callback.call1(py, (scope, pyproto)).unwrap()
         }
     }
 
+    callback_impl_run!();
+}
+
+#[pymethods]
+impl CallbackRunnerHTTP {
+    fn _loop_task<'p>(&self, py: Python<'p>) -> PyResult<&'p PyAny> {
+        CallbackTaskHTTP::new(py, self.cb.clone(), self.proto.clone(), self.context.clone())?.run(py)
+    }
+}
+
+#[pyclass]
+pub(crate) struct CallbackTaskHTTP {
+    proto: Py<HTTPProtocol>,
+    context: TaskLocals,
+    cb: PyObject
+}
+
+impl CallbackTaskHTTP {
+    pub fn new(
+        py: Python,
+        cb: PyObject,
+        proto: Py<HTTPProtocol>,
+        context: TaskLocals
+    ) -> PyResult<Self> {
+        Ok(Self { proto, context: context.copy_context(py)?, cb })
+    }
+
     fn done(&self, py: Python) {
         if let Ok(mut proto) = self.proto.as_ref(py).try_borrow_mut() {
             if let Some(tx) = proto.tx() {
-                let _ = tx.send(
-                    PyResponse::Bytes(PyResponseBytes::empty(500, Vec::new()))
-                );
+                let mut res = Response::new("Internal server error".into());
+                *res.status_mut() = hyper::StatusCode::INTERNAL_SERVER_ERROR;
+                let _ = tx.send(res);
             }
         }
     }
 
     fn err(&self, py: Python) {
         log::warn!("Application callable raised an exception");
         self.done(py)
     }
 
-    callback_impl_run!();
+    callback_impl_loop_run!();
     callback_impl_loop_err!();
 }
 
 #[pymethods]
-impl CallbackRunnerHTTP {
+impl CallbackTaskHTTP {
     fn _loop_step(pyself: PyRef<'_, Self>, py: Python) -> PyResult<PyObject> {
         callback_impl_loop_step!(pyself, py)
     }
 
     fn _loop_wake(pyself: PyRef<'_, Self>, py: Python, fut: PyObject) -> PyResult<PyObject> {
         callback_impl_loop_wake!(pyself, py, fut)
     }
 }
 
 #[pyclass]
 pub(crate) struct CallbackRunnerWebsocket {
     proto: Py<WebsocketProtocol>,
-    event_loop: PyObject,
-    context: PyObject,
+    context: TaskLocals,
     cb: PyObject
 }
 
 impl CallbackRunnerWebsocket {
     pub fn new(
         py: Python,
         cb: CallbackWrapper,
         proto: WebsocketProtocol,
         scope: Scope
     ) -> Self {
         let pyproto = Py::new(py, proto).unwrap();
         Self {
             proto: pyproto.clone(),
-            event_loop: cb.context.event_loop(py).into(),
-            context: cb.context.context(py).into(),
+            context: cb.context,
             cb: cb.callback.call1(py, (scope, pyproto)).unwrap()
         }
     }
 
+    callback_impl_run!();
+}
+
+#[pymethods]
+impl CallbackRunnerWebsocket {
+    fn _loop_task<'p>(&self, py: Python<'p>) -> PyResult<&'p PyAny> {
+        CallbackTaskWebsocket::new(py, self.cb.clone(), self.proto.clone(), self.context.clone())?.run(py)
+    }
+}
+
+#[pyclass]
+pub(crate) struct CallbackTaskWebsocket {
+    proto: Py<WebsocketProtocol>,
+    context: TaskLocals,
+    cb: PyObject
+}
+
+impl CallbackTaskWebsocket {
+    pub fn new(
+        py: Python,
+        cb: PyObject,
+        proto: Py<WebsocketProtocol>,
+        context: TaskLocals
+    ) -> PyResult<Self> {
+        Ok(Self { proto, context: context.copy_context(py)?, cb })
+    }
+
     fn done(&self, py: Python) {
         if let Ok(mut proto) = self.proto.as_ref(py).try_borrow_mut() {
             if let (Some(tx), res) = proto.tx() {
                 let _ = tx.send(res);
             }
         }
     }
 
     fn err(&self, py: Python) {
         log::warn!("Application callable raised an exception");
         self.done(py)
     }
 
-    callback_impl_run!();
+    callback_impl_loop_run!();
     callback_impl_loop_err!();
 }
 
 #[pymethods]
-impl CallbackRunnerWebsocket {
+impl CallbackTaskWebsocket {
     fn _loop_step(pyself: PyRef<'_, Self>, py: Python) -> PyResult<PyObject> {
         callback_impl_loop_step!(pyself, py)
     }
 
     fn _loop_wake(pyself: PyRef<'_, Self>, py: Python, fut: PyObject) -> PyResult<PyObject> {
         callback_impl_loop_wake!(pyself, py, fut)
     }
 }
 
+// NOTE: we cannot use single `impl` function as structs with pyclass won't handle
+//       dyn fields easily.
+// pub(crate) async fn call(
+//     cb: CallbackWrapper,
+//     protocol: impl ASGIProtocol + IntoPy<PyObject>,
+//     scope: Scope
+// ) -> Result<(), ASGIFlowError> {
+//     let (tx, rx) = oneshot::channel();
+//     let callback = cb.callback.clone();
+//     Python::with_gil(|py| {
+//         callback.call1(py, (CallbackWatcher::new(py, cb, tx), scope, protocol))
+//     })?;
+
+//     match rx.await {
+//         Ok(true) => Ok(()),
+//         Ok(false) => {
+//             log::warn!("Application callable raised an exception");
+//             error_flow!()
+//         },
+//         _ => error_flow!()
+//     }
+// }
+
 pub(crate) fn call_rtb_http(
     cb: CallbackWrapper,
     rt: RuntimeRef,
-    req: hyper::Request<hyper::Body>,
+    req: Request<Body>,
     scope: Scope
-) -> oneshot::Receiver<PyResponse> {
+) -> oneshot::Receiver<Response<Body>> {
     let (tx, rx) = oneshot::channel();
-    let protocol = HTTPProtocol::new(rt, tx, req);
+    let protocol = HTTPProtocol::new(rt, req, tx);
 
     Python::with_gil(|py| {
         let _ = CallbackRunnerHTTP::new(py, cb, protocol, scope).run(py);
     });
 
     rx
 }
 
 pub(crate) fn call_rtt_http(
     cb: CallbackWrapper,
     rt: RuntimeRef,
-    req: hyper::Request<hyper::Body>,
+    req: Request<Body>,
     scope: Scope
-) -> oneshot::Receiver<PyResponse> {
+) -> oneshot::Receiver<Response<Body>> {
     let (tx, rx) = oneshot::channel();
-    let protocol = HTTPProtocol::new(rt, tx, req);
+    let protocol = HTTPProtocol::new(rt, req, tx);
 
     tokio::task::spawn_blocking(move || {
         Python::with_gil(|py| {
             let _ = CallbackRunnerHTTP::new(py, cb, protocol, scope).run(py);
         });
     });
 
@@ -160,15 +236,15 @@
 
 pub(crate) fn call_rtb_ws(
     cb: CallbackWrapper,
     rt: RuntimeRef,
     ws: HyperWebsocket,
     upgrade: UpgradeData,
     scope: Scope
-) -> oneshot::Receiver<(i32, bool)> {
+) -> oneshot::Receiver<bool> {
     let (tx, rx) = oneshot::channel();
     let protocol = WebsocketProtocol::new(rt, tx, ws, upgrade);
 
     Python::with_gil(|py| {
         let _ = CallbackRunnerWebsocket::new(py, cb, protocol, scope).run(py);
     });
 
@@ -177,15 +253,15 @@
 
 pub(crate) fn call_rtt_ws(
     cb: CallbackWrapper,
     rt: RuntimeRef,
     ws: HyperWebsocket,
     upgrade: UpgradeData,
     scope: Scope
-) -> oneshot::Receiver<(i32, bool)> {
+) -> oneshot::Receiver<bool> {
     let (tx, rx) = oneshot::channel();
     let protocol = WebsocketProtocol::new(rt, tx, ws, upgrade);
 
     tokio::task::spawn_blocking(move || {
         Python::with_gil(|py| {
             let _ = CallbackRunnerWebsocket::new(py, cb, protocol, scope).run(py);
         });
```

### Comparing `granian-0.4.0/src/rsgi/errors.rs` & `granian-0.4.1/src/rsgi/errors.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/rsgi/http.rs` & `granian-0.4.1/src/rsgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/rsgi/io.rs` & `granian-0.4.1/src/rsgi/io.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/rsgi/mod.rs` & `granian-0.4.1/src/rsgi/mod.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/rsgi/serve.rs` & `granian-0.4.1/src/rsgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/rsgi/types.rs` & `granian-0.4.1/src/rsgi/types.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/runtime.rs` & `granian-0.4.1/src/runtime.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/tcp.rs` & `granian-0.4.1/src/tcp.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/tls.rs` & `granian-0.4.1/src/tls.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/utils.rs` & `granian-0.4.1/src/utils.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/workers.rs` & `granian-0.4.1/src/workers.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/ws.rs` & `granian-0.4.1/src/ws.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/wsgi/callbacks.rs` & `granian-0.4.1/src/wsgi/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/wsgi/http.rs` & `granian-0.4.1/src/wsgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/wsgi/serve.rs` & `granian-0.4.1/src/wsgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/src/wsgi/types.rs` & `granian-0.4.1/src/wsgi/types.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/tests/apps/asgi.py` & `granian-0.4.1/tests/apps/asgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/tests/apps/rsgi.py` & `granian-0.4.1/tests/apps/rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/tests/apps/wsgi.py` & `granian-0.4.1/tests/apps/wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/tests/conftest.py` & `granian-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/tests/fixtures/tls/cert.pem` & `granian-0.4.1/tests/fixtures/tls/cert.pem`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/tests/fixtures/tls/key.pem` & `granian-0.4.1/tests/fixtures/tls/key.pem`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/tests/test_asgi.py` & `granian-0.4.1/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/tests/test_https.py` & `granian-0.4.1/tests/test_https.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/tests/test_rsgi.py` & `granian-0.4.1/tests/test_rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/tests/test_ws.py` & `granian-0.4.1/tests/test_ws.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/tests/test_wsgi.py` & `granian-0.4.1/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.0/Cargo.lock` & `granian-0.4.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "granian"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "bytes",
  "futures",
  "hyper",
  "log",
  "mimalloc",
  "once_cell",
```

### Comparing `granian-0.4.0/PKG-INFO` & `granian-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granian
-Version: 0.4.0
+Version: 0.4.1
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -30,17 +30,17 @@
 Keywords: web,asyncio
 Home-Page: https://github.com/emmett-framework/granian
 Author: Giovanni Barillari <g@baro.dev>
 Author-email: Giovanni Barillari <g@baro.dev>
 License: BSD-3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Source, https://github.com/emmett-framework/granian
 Project-URL: Homepage, https://github.com/emmett-framework/granian
 Project-URL: Funding, https://github.com/sponsors/gi0baro
+Project-URL: Source, https://github.com/emmett-framework/granian
 
 # Granian
 
 A Rust HTTP server for Python applications.
 
 ## Rationale
```

