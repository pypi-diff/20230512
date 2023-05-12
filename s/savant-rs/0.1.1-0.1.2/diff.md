# Comparing `tmp/savant_rs-0.1.1.tar.gz` & `tmp/savant_rs-0.1.2.tar.gz`

## Comparing `savant_rs-0.1.1.tar` & `savant_rs-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,42 @@
--rw-r--r--   0        0        0     1063 1970-01-01 00:00:00.000000 savant_rs-0.1.1/Cargo.toml
--rw-r--r--   0     1001      123     1614 2023-05-12 07:21:06.000000 savant_rs-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      466 2023-05-12 07:21:06.000000 savant_rs-0.1.1/.gitignore
--rw-r--r--   0     1001      123    11357 2023-05-12 07:21:06.000000 savant_rs-0.1.1/LICENSE
--rw-r--r--   0     1001      123      270 2023-05-12 07:21:06.000000 savant_rs-0.1.1/README.md
--rw-r--r--   0     1001      123     1378 2023-05-12 07:21:06.000000 savant_rs-0.1.1/benches/message_save_load.rs
--rw-r--r--   0     1001      123       71 2023-05-12 07:21:06.000000 savant_rs-0.1.1/build.rs
--rw-r--r--   0     1001      123      459 2023-05-12 07:21:06.000000 savant_rs-0.1.1/pyproject.toml
--rw-r--r--   0     1001      123      200 2023-05-12 07:21:06.000000 savant_rs-0.1.1/python/test_pyo3_access/get_copy.py
--rw-r--r--   0     1001      123      184 2023-05-12 07:21:06.000000 savant_rs-0.1.1/python/test_pyo3_access/get_proxy.py
--rw-r--r--   0     1001      123      407 2023-05-12 07:21:06.000000 savant_rs-0.1.1/python/test_pyo3_access/get_pure.py
--rw-r--r--   0     1001      123      196 2023-05-12 07:21:06.000000 savant_rs-0.1.1/python/test_pyo3_access/get_py.py
--rw-r--r--   0     1001      123      213 2023-05-12 07:21:06.000000 savant_rs-0.1.1/python/test_pyo3_access/get_take.py
--rw-r--r--   0     1001      123     1018 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/lib.rs
--rw-r--r--   0     1001      123    12026 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/primitives/attribute.rs
--rw-r--r--   0     1001      123      872 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/primitives/bbox.rs
--rw-r--r--   0     1001      123      590 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/primitives/message/eos.rs
--rw-r--r--   0     1001      123     2807 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/primitives/message/loader.rs
--rw-r--r--   0     1001      123     2141 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/primitives/message/saver.rs
--rw-r--r--   0     1001      123     1493 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/primitives/message/video/batch.rs
--rw-r--r--   0     1001      123    25076 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/primitives/message/video/frame.rs
--rw-r--r--   0     1001      123    12536 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/primitives/message/video/object.rs
--rw-r--r--   0     1001      123       46 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/primitives/message/video.rs
--rw-r--r--   0     1001      123     6598 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/primitives/message.rs
--rw-r--r--   0     1001      123      597 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/primitives/point.rs
--rw-r--r--   0     1001      123    13432 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/primitives/polygonal_area.rs
--rw-r--r--   0     1001      123     1876 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/primitives/segment.rs
--rw-r--r--   0     1001      123     1491 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/primitives.rs
--rw-r--r--   0     1001      123     5759 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/test.rs
--rw-r--r--   0     1001      123     1071 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/test_rkyv_tuple.rs
--rw-r--r--   0     1001      123     2521 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/tests_pyo3_access.rs
--rw-r--r--   0     1001      123     5968 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/utils/fps_meter.rs
--rw-r--r--   0     1001      123      512 2023-05-12 07:21:06.000000 savant_rs-0.1.1/src/utils.rs
--rw-r--r--   0     1001      123    30329 2023-05-12 07:22:17.000000 savant_rs-0.1.1/Cargo.lock
--rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 savant_rs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 1970-01-01 00:00:00.000000 savant_rs-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      123     1614 2023-05-12 15:17:32.000000 savant_rs-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      466 2023-05-12 15:17:32.000000 savant_rs-0.1.2/.gitignore
+-rw-r--r--   0     1001      123    11357 2023-05-12 15:17:32.000000 savant_rs-0.1.2/LICENSE
+-rw-r--r--   0     1001      123      270 2023-05-12 15:17:32.000000 savant_rs-0.1.2/README.md
+-rw-r--r--   0     1001      123      769 2023-05-12 15:17:32.000000 savant_rs-0.1.2/benches/batch_snapshot.rs
+-rw-r--r--   0     1001      123     1197 2023-05-12 15:17:32.000000 savant_rs-0.1.2/benches/message_save_load.rs
+-rw-r--r--   0     1001      123       71 2023-05-12 15:17:32.000000 savant_rs-0.1.2/build.rs
+-rw-r--r--   0     1001      123      459 2023-05-12 15:17:32.000000 savant_rs-0.1.2/pyproject.toml
+-rw-r--r--   0     1001      123      269 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/fps_meter/rust_fps_meter.py
+-rw-r--r--   0     1001      123     3515 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/fps_meter/savant_fps_meter.py
+-rw-r--r--   0     1001      123      783 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/primitives/buf_copy.py
+-rw-r--r--   0     1001      123     3741 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/primitives/frame_ops.py
+-rw-r--r--   0     1001      123     1108 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/primitives/polygon_match.py
+-rw-r--r--   0     1001      123      200 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/test_pyo3_access/get_copy.py
+-rw-r--r--   0     1001      123      184 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/test_pyo3_access/get_proxy.py
+-rw-r--r--   0     1001      123      407 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/test_pyo3_access/get_pure.py
+-rw-r--r--   0     1001      123      196 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/test_pyo3_access/get_py.py
+-rw-r--r--   0     1001      123      213 2023-05-12 15:17:32.000000 savant_rs-0.1.2/python/test_pyo3_access/get_take.py
+-rw-r--r--   0     1001      123     1018 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      123    14168 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/attribute.rs
+-rw-r--r--   0     1001      123     1221 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/bbox.rs
+-rw-r--r--   0     1001      123      590 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/message/eos.rs
+-rw-r--r--   0     1001      123     2807 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/message/loader.rs
+-rw-r--r--   0     1001      123     2141 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/message/saver.rs
+-rw-r--r--   0     1001      123     1932 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/message/video/batch.rs
+-rw-r--r--   0     1001      123    28694 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/message/video/frame.rs
+-rw-r--r--   0     1001      123    14354 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/message/video/object.rs
+-rw-r--r--   0     1001      123       46 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/message/video.rs
+-rw-r--r--   0     1001      123     6710 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/message.rs
+-rw-r--r--   0     1001      123      853 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/point.rs
+-rw-r--r--   0     1001      123    13870 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/polygonal_area.rs
+-rw-r--r--   0     1001      123     2558 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/segment.rs
+-rw-r--r--   0     1001      123       87 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives/to_json_value.rs
+-rw-r--r--   0     1001      123     1628 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/primitives.rs
+-rw-r--r--   0     1001      123     5771 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/test.rs
+-rw-r--r--   0     1001      123     1071 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/test_rkyv_tuple.rs
+-rw-r--r--   0     1001      123     2521 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/tests_pyo3_access.rs
+-rw-r--r--   0     1001      123     5968 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/utils/fps_meter.rs
+-rw-r--r--   0     1001      123      512 2023-05-12 15:17:32.000000 savant_rs-0.1.2/src/utils.rs
+-rw-r--r--   0     1001      123    30961 2023-05-12 15:18:57.000000 savant_rs-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 savant_rs-0.1.2/PKG-INFO
```

### Comparing `savant_rs-0.1.1/Cargo.toml` & `savant_rs-0.1.2/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "savant_rs"
-version = "0.1.1"
+version = "0.1.2"
 edition = "2021"
 authors = ["Ivan Kudriavtsev <ivan.a.kudryavtsev@gmail.com>"]
 description = "Savant rust optimization library"
 homepage = "https://github.com/insight-platform/savant-rs"
 repository = "https://github.com/insight-platform/savant-rs"
 readme = "README.md"
 keywords = ["computer-vision", "video-processing"]
@@ -12,14 +12,15 @@
 license="Apache-2.0"
 rust-version = "1.66"
 
 [lib]
 crate-type = ["cdylib", "lib"]
 
 [dependencies]
+serde_json = "1.0"
 itertools = "0.10"
 anyhow = "1.0"
 thiserror = "1.0"
 geo = "0.24"
 rayon = "1.7"
 env_logger = "0.10"
 rkyv = { version = "0.7", features = ["validation", "archive_le"] }
```

### Comparing `savant_rs-0.1.1/.github/workflows/CI.yml` & `savant_rs-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.1/LICENSE` & `savant_rs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.1/src/lib.rs` & `savant_rs-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.1/src/primitives/attribute.rs` & `savant_rs-0.1.2/src/primitives/attribute.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+use crate::primitives::to_json_value::ToSerdeJsonValue;
 use crate::primitives::{BBox, Intersection, Point, PolygonalArea};
-use pyo3::{pyclass, pymethods, Py, PyAny, Python};
+use pyo3::{pyclass, pymethods, Py, PyAny};
 use rkyv::{Archive, Deserialize, Serialize};
 use std::collections::HashMap;
 use std::sync::{Arc, Mutex};
 
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone, Default)]
 #[archive(check_bytes)]
 pub enum ValueVariant {
@@ -23,23 +24,91 @@
     Polygon(PolygonalArea),
     PolygonVector(Vec<PolygonalArea>),
     Intersection(Intersection),
     #[default]
     None,
 }
 
+impl ToSerdeJsonValue for ValueVariant {
+    fn to_serde_json_value(&self) -> serde_json::Value {
+        match self {
+            ValueVariant::Bytes(dims, blob) => serde_json::json!({
+                "dims": dims,
+                "blob": blob,
+            }),
+            ValueVariant::String(s) => serde_json::json!({
+                "string": s,
+            }),
+            ValueVariant::StringVector(v) => serde_json::json!({
+                "string_vector": v,
+            }),
+            ValueVariant::Integer(i) => serde_json::json!({
+                "integer": i,
+            }),
+            ValueVariant::IntegerVector(v) => serde_json::json!({
+                "integer_vector": v,
+            }),
+            ValueVariant::Float(f) => serde_json::json!({
+                "float": f,
+            }),
+            ValueVariant::FloatVector(v) => serde_json::json!({
+                "float_vector": v,
+            }),
+            ValueVariant::Boolean(b) => serde_json::json!({
+                "boolean": b,
+            }),
+            ValueVariant::BooleanVector(v) => serde_json::json!({
+                "boolean_vector": v,
+            }),
+            ValueVariant::BBox(b) => serde_json::json!({
+                "bbox": b.to_serde_json_value(),
+            }),
+            ValueVariant::BBoxVector(v) => serde_json::json!({
+                "bbox_vector": v.into_iter().map(|b| b.to_serde_json_value()).collect::<Vec<_>>(),
+            }),
+            ValueVariant::Point(p) => serde_json::json!({
+                "point": p.to_serde_json_value(),
+            }),
+            ValueVariant::PointVector(v) => serde_json::json!({
+                "point_vector": v.into_iter().map(|p| p.to_serde_json_value()).collect::<Vec<_>>(),
+            }),
+            ValueVariant::Polygon(p) => serde_json::json!({
+                "polygon": p.to_serde_json_value(),
+            }),
+            ValueVariant::PolygonVector(v) => serde_json::json!({
+                "polygon_vector": v.into_iter().map(|p| p.to_serde_json_value()).collect::<Vec<_>>(),
+            }),
+            ValueVariant::Intersection(i) => serde_json::json!({
+                "intersection": i.to_serde_json_value(),
+            }),
+            ValueVariant::None => serde_json::json!({
+                "none": null,
+            }),
+        }
+    }
+}
+
 #[pyclass]
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone, Default)]
 #[archive(check_bytes)]
 pub struct Value {
     #[pyo3(get, set)]
     pub confidence: Option<f64>,
     v: ValueVariant,
 }
 
+impl ToSerdeJsonValue for Value {
+    fn to_serde_json_value(&self) -> serde_json::Value {
+        serde_json::json!({
+            "confidence": self.confidence,
+            "value": self.v.to_serde_json_value(),
+        })
+    }
+}
+
 #[pymethods]
 impl Value {
     #[classattr]
     const __hash__: Option<Py<PyAny>> = None;
 
     fn __repr__(&self) -> String {
         format!("{self:?}")
@@ -314,14 +383,25 @@
     pub name: String,
     #[pyo3(get)]
     pub values: Vec<Value>,
     #[pyo3(get)]
     pub hint: Option<String>,
 }
 
+impl ToSerdeJsonValue for Attribute {
+    fn to_serde_json_value(&self) -> serde_json::Value {
+        serde_json::json!({
+            "creator": self.creator,
+            "name": self.name,
+            "values": self.values.iter().map(|v| v.to_serde_json_value()).collect::<Vec<_>>(),
+            "hint": self.hint,
+        })
+    }
+}
+
 #[pymethods]
 impl Attribute {
     #[classattr]
     const __hash__: Option<Py<PyAny>> = None;
 
     fn __repr__(&self) -> String {
         format!("{self:?}")
@@ -346,121 +426,104 @@
     fn get_attributes_ref(&self) -> &HashMap<(String, String), Attribute>;
     fn get_attributes_ref_mut(&mut self) -> &mut HashMap<(String, String), Attribute>;
 }
 
 pub trait Attributive<T: InnerAttributes + Send> {
     fn get_inner(&self) -> Arc<Mutex<T>>;
 
-    fn inner_attributes(&self) -> Vec<(String, String)> {
-        let inner = self.get_inner();
-        Python::with_gil(move |py| {
-            py.allow_threads(move || {
-                inner
-                    .lock()
-                    .unwrap()
-                    .get_attributes_ref()
-                    .iter()
-                    .map(|((creator, name), _)| (creator.clone(), name.clone()))
-                    .collect()
-            })
-        })
+    fn get_attributes(&self) -> Vec<(String, String)> {
+        self.get_inner()
+            .lock()
+            .unwrap()
+            .get_attributes_ref()
+            .iter()
+            .map(|((creator, name), _)| (creator.clone(), name.clone()))
+            .collect()
     }
 
-    fn inner_get_attribute(&self, creator: String, name: String) -> Option<Attribute> {
-        let inner = self.get_inner();
-        let res = inner
+    fn get_attribute(&self, creator: String, name: String) -> Option<Attribute> {
+        self.get_inner()
             .lock()
             .unwrap()
             .get_attributes_ref()
             .get(&(creator, name))
-            .cloned();
-        res
+            .cloned()
     }
 
-    fn inner_delete_attribute(&mut self, creator: String, name: String) -> Option<Attribute> {
-        let inner = self.get_inner();
-        let res = inner
+    fn delete_attribute(&mut self, creator: String, name: String) -> Option<Attribute> {
+        self.get_inner()
             .lock()
             .unwrap()
             .get_attributes_ref_mut()
-            .remove(&(creator, name));
-        res
+            .remove(&(creator, name))
     }
 
-    fn inner_set_attribute(&mut self, attribute: Attribute) -> Option<Attribute> {
-        let inner = self.get_inner();
-        let res = inner.lock().unwrap().get_attributes_ref_mut().insert(
-            (attribute.creator.clone(), attribute.name.clone()),
-            attribute,
-        );
-        res
+    fn set_attribute(&mut self, attribute: Attribute) -> Option<Attribute> {
+        self.get_inner()
+            .lock()
+            .unwrap()
+            .get_attributes_ref_mut()
+            .insert(
+                (attribute.creator.clone(), attribute.name.clone()),
+                attribute,
+            )
     }
 
     #[allow(clippy::let_unit_value)]
-    fn inner_clear_attributes(&mut self) {
-        let inner = self.get_inner();
-        let res = inner.lock().unwrap().get_attributes_ref_mut().clear();
-        res
+    fn clear_attributes(&mut self) {
+        self.get_inner()
+            .lock()
+            .unwrap()
+            .get_attributes_ref_mut()
+            .clear()
     }
 
-    fn inner_delete_attributes(
-        &mut self,
-        negated: bool,
-        creator: Option<String>,
-        names: Vec<String>,
-    ) {
-        let inner = self.get_inner();
-        Python::with_gil(move |py| {
-            py.allow_threads(move || {
-                inner.lock().unwrap().get_attributes_ref_mut().retain(
-                    |(c, label), _| match creator {
-                        Some(ref creator) => {
-                            ((names.is_empty() || names.contains(label)) && creator == c) ^ !negated
-                        }
-                        None => names.contains(label) ^ !negated,
-                    },
-                );
-            })
-        });
+    fn delete_attributes(&mut self, negated: bool, creator: Option<String>, names: Vec<String>) {
+        // let inner = self.get_inner();
+        self.get_inner()
+            .lock()
+            .unwrap()
+            .get_attributes_ref_mut()
+            .retain(|(c, label), _| match creator {
+                Some(ref creator) => {
+                    ((names.is_empty() || names.contains(label)) && creator == c) ^ !negated
+                }
+                None => names.contains(label) ^ !negated,
+            });
     }
 
-    fn inner_find_attributes(
+    fn find_attributes(
         &self,
         creator: Option<String>,
         name: Option<String>,
         hint: Option<String>,
     ) -> Vec<(String, String)> {
-        let inner = self.get_inner();
-        Python::with_gil(move |py| {
-            py.allow_threads(move || {
-                inner
-                    .lock()
-                    .unwrap()
-                    .get_attributes_ref()
-                    .iter()
-                    .filter(|((_, _), a)| {
-                        if let Some(creator) = &creator {
-                            if a.creator != *creator {
-                                return false;
-                            }
-                        }
-
-                        if let Some(name) = &name {
-                            if a.name != *name {
-                                return false;
-                            }
-                        }
-
-                        if let Some(hint) = &hint {
-                            if a.hint.as_ref() != Some(hint) {
-                                return false;
-                            }
-                        }
-
-                        true
-                    })
-                    .map(|((c, n), _)| (c.clone(), n.clone()))
-                    .collect()
+        self.get_inner()
+            .lock()
+            .unwrap()
+            .get_attributes_ref()
+            .iter()
+            .filter(|((_, _), a)| {
+                if let Some(creator) = &creator {
+                    if a.creator != *creator {
+                        return false;
+                    }
+                }
+
+                if let Some(name) = &name {
+                    if a.name != *name {
+                        return false;
+                    }
+                }
+
+                if let Some(hint) = &hint {
+                    if a.hint.as_ref() != Some(hint) {
+                        return false;
+                    }
+                }
+
+                true
             })
-        })
+            .map(|((c, n), _)| (c.clone(), n.clone()))
+            .collect()
     }
 }
```

### Comparing `savant_rs-0.1.1/src/primitives/bbox.rs` & `savant_rs-0.1.2/src/primitives/point.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,42 @@
+use crate::primitives::to_json_value::ToSerdeJsonValue;
 use pyo3::{pyclass, pymethods, Py, PyAny};
 use rkyv::{Archive, Deserialize, Serialize};
+use serde_json::Value;
 
 #[pyclass]
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone)]
 #[archive(check_bytes)]
-pub struct BBox {
+pub struct Point {
     #[pyo3(get, set)]
-    pub xc: f64,
+    pub x: f64,
     #[pyo3(get, set)]
-    pub yc: f64,
-    #[pyo3(get, set)]
-    pub width: f64,
-    #[pyo3(get, set)]
-    pub height: f64,
-    #[pyo3(get, set)]
-    pub angle: Option<f64>,
+    pub y: f64,
+}
+
+impl ToSerdeJsonValue for Point {
+    fn to_serde_json_value(&self) -> Value {
+        serde_json::json!({
+            "x": self.x,
+            "y": self.y,
+        })
+    }
 }
 
 #[pymethods]
-impl BBox {
+impl Point {
     #[classattr]
     const __hash__: Option<Py<PyAny>> = None;
 
     fn __repr__(&self) -> String {
         format!("{self:?}")
     }
 
     fn __str__(&self) -> String {
         self.__repr__()
     }
 
     #[new]
-    pub fn new(xc: f64, yc: f64, width: f64, height: f64, angle: Option<f64>) -> Self {
-        Self {
-            xc,
-            yc,
-            width,
-            height,
-            angle,
-        }
+    pub fn new(x: f64, y: f64) -> Self {
+        Self { x, y }
     }
 }
```

### Comparing `savant_rs-0.1.1/src/primitives/message/eos.rs` & `savant_rs-0.1.2/src/primitives/message/eos.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.1/src/primitives/message/loader.rs` & `savant_rs-0.1.2/src/primitives/message/loader.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.1/src/primitives/message/saver.rs` & `savant_rs-0.1.2/src/primitives/message/saver.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.1/src/primitives/message/video/batch.rs` & `savant_rs-0.1.2/src/primitives/message/video/batch.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use crate::primitives::message::video::frame::InnerVideoFrame;
 use crate::primitives::VideoFrame;
-use pyo3::{pyclass, pymethods};
+use pyo3::{pyclass, pymethods, Python};
 use rkyv::{with::Skip, Archive, Deserialize, Serialize};
 use std::collections::HashMap;
 
 #[pyclass]
 #[derive(Archive, Deserialize, Serialize, Debug, Clone, Default)]
 #[archive(check_bytes)]
 pub struct VideoFrameBatch {
@@ -25,14 +25,22 @@
     pub(crate) fn prepare_before_save(&mut self) {
         for (id, frame) in self.frames.iter_mut() {
             let mut frame = frame.inner.lock().unwrap();
             frame.prepare_before_save();
             self.offline_frames.insert(*id, frame.as_ref().clone());
         }
     }
+
+    pub fn snapshot(&mut self) {
+        self.prepare_before_save();
+    }
+
+    pub fn restore(&mut self) {
+        self.prepare_after_load();
+    }
 }
 
 #[pymethods]
 impl VideoFrameBatch {
     #[new]
     pub fn new() -> Self {
         Self::default()
@@ -45,8 +53,18 @@
     pub fn get(&self, id: i64) -> Option<VideoFrame> {
         self.frames.get(&id).cloned()
     }
 
     pub fn del(&mut self, id: i64) -> Option<VideoFrame> {
         self.frames.remove(&id)
     }
+
+    #[pyo3(name = "snapshot")]
+    pub fn snapshot_py(&mut self) {
+        Python::with_gil(|py| py.allow_threads(|| self.snapshot()))
+    }
+
+    #[pyo3(name = "restore")]
+    pub fn restore_py(&mut self) {
+        Python::with_gil(|py| py.allow_threads(|| self.restore()))
+    }
 }
```

### Comparing `savant_rs-0.1.1/src/primitives/message/video/frame.rs` & `savant_rs-0.1.2/src/primitives/message/video/frame.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 use crate::primitives::attribute::{Attributive, InnerAttributes};
 use crate::primitives::message::video::object::InnerObject;
+use crate::primitives::to_json_value::ToSerdeJsonValue;
 use crate::primitives::{Attribute, Object};
 use pyo3::{pyclass, pymethods, Py, PyAny, PyResult, Python};
 use rkyv::{with::Skip, Archive, Deserialize, Serialize};
+use serde_json::Value;
 use std::collections::HashMap;
 use std::sync::{Arc, Mutex};
 
 #[pyclass]
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone)]
 #[archive(check_bytes)]
 pub struct ExternalFrame {
     #[pyo3(get, set)]
     pub method: String,
     #[pyo3(get, set)]
     pub location: Option<String>,
 }
 
+impl ToSerdeJsonValue for ExternalFrame {
+    fn to_serde_json_value(&self) -> Value {
+        serde_json::json!({
+            "method": self.method,
+            "location": self.location,
+        })
+    }
+}
+
 #[pymethods]
 impl ExternalFrame {
     #[classattr]
     const __hash__: Option<Py<PyAny>> = None;
 
     fn __repr__(&self) -> String {
         format!("{self:?}")
@@ -39,14 +50,28 @@
 #[archive(check_bytes)]
 pub enum VideoFrameContent {
     External(ExternalFrame),
     Internal(Vec<u8>),
     None,
 }
 
+impl ToSerdeJsonValue for VideoFrameContent {
+    fn to_serde_json_value(&self) -> Value {
+        match self {
+            VideoFrameContent::External(data) => {
+                serde_json::json!({"external": data.to_serde_json_value()})
+            }
+            VideoFrameContent::Internal(_) => {
+                serde_json::json!({ "internal": Value::Null })
+            }
+            VideoFrameContent::None => Value::Null,
+        }
+    }
+}
+
 #[pyclass]
 #[derive(Debug, Clone)]
 pub struct PyVideoFrameContent {
     pub(crate) inner: VideoFrameContent,
 }
 
 impl PyVideoFrameContent {
@@ -137,28 +162,56 @@
 pub enum FrameTransformation {
     InitialSize(u64, u64),
     Scale(u64, u64),
     Padding(u64, u64, u64, u64),
     None,
 }
 
+impl ToSerdeJsonValue for FrameTransformation {
+    fn to_serde_json_value(&self) -> Value {
+        match self {
+            FrameTransformation::InitialSize(width, height) => {
+                serde_json::json!({"initial_size": [width, height]})
+            }
+            FrameTransformation::Scale(width, height) => {
+                serde_json::json!({"scale": [width, height]})
+            }
+            FrameTransformation::Padding(left, top, right, bottom) => {
+                serde_json::json!({"padding": [left, top, right, bottom]})
+            }
+            FrameTransformation::None => serde_json::json!(null),
+        }
+    }
+}
+
 #[pyclass]
 #[derive(Debug, Clone)]
 pub struct PyFrameTransformation {
     pub(crate) inner: FrameTransformation,
 }
 
 impl PyFrameTransformation {
     pub fn new(inner: FrameTransformation) -> Self {
         Self { inner }
     }
 }
 
 #[pymethods]
 impl PyFrameTransformation {
+    #[classattr]
+    const __hash__: Option<Py<PyAny>> = None;
+
+    fn __repr__(&self) -> String {
+        format!("{:?}", self.inner)
+    }
+
+    fn __str__(&self) -> String {
+        self.__repr__()
+    }
+
     #[staticmethod]
     pub fn initial_size(width: i64, height: i64) -> Self {
         assert!(width > 0 && height > 0);
         Self {
             inner: FrameTransformation::InitialSize(
                 u64::try_from(width).unwrap(),
                 u64::try_from(height).unwrap(),
@@ -175,15 +228,15 @@
                 u64::try_from(height).unwrap(),
             ),
         }
     }
 
     #[staticmethod]
     pub fn padding(left: i64, top: i64, right: i64, bottom: i64) -> Self {
-        assert!(left > 0 && top > 0 && right > 0 && bottom > 0);
+        assert!(left >= 0 && top >= 0 && right >= 0 && bottom >= 0);
         Self {
             inner: FrameTransformation::Padding(
                 u64::try_from(left).unwrap(),
                 u64::try_from(top).unwrap(),
                 u64::try_from(right).unwrap(),
                 u64::try_from(bottom).unwrap(),
             ),
@@ -213,29 +266,32 @@
     }
 
     #[getter]
     pub fn is_none(&self) -> bool {
         matches!(self.inner, FrameTransformation::None)
     }
 
-    pub fn get_initial_size(&self) -> Option<(u64, u64)> {
+    #[getter]
+    pub fn as_initial_size(&self) -> Option<(u64, u64)> {
         match &self.inner {
             FrameTransformation::InitialSize(w, h) => Some((*w, *h)),
             _ => None,
         }
     }
 
-    pub fn get_scale(&self) -> Option<(u64, u64)> {
+    #[getter]
+    pub fn as_scale(&self) -> Option<(u64, u64)> {
         match &self.inner {
             FrameTransformation::Scale(w, h) => Some((*w, *h)),
             _ => None,
         }
     }
 
-    pub fn get_padding(&self) -> Option<(u64, u64, u64, u64)> {
+    #[getter]
+    pub fn as_padding(&self) -> Option<(u64, u64, u64, u64)> {
         match &self.inner {
             FrameTransformation::Padding(l, t, r, b) => Some((*l, *t, *r, *b)),
             _ => None,
         }
     }
 }
 
@@ -255,14 +311,36 @@
     pub transformations: Vec<FrameTransformation>,
     pub attributes: HashMap<(String, String), Attribute>,
     pub offline_objects: Vec<InnerObject>,
     #[with(Skip)]
     pub(crate) resident_objects: Vec<Arc<Mutex<InnerObject>>>,
 }
 
+impl ToSerdeJsonValue for InnerVideoFrame {
+    fn to_serde_json_value(&self) -> Value {
+        serde_json::json!(
+            {
+                "source_id": self.source_id,
+                "framerate": self.framerate,
+                "width": self.width,
+                "height": self.height,
+                "codec": self.codec,
+                "keyframe": self.keyframe,
+                "pts": self.pts,
+                "dts": self.dts,
+                "duration": self.duration,
+                "content": self.content.to_serde_json_value(),
+                "transformations": self.transformations.iter().map(|t| t.to_serde_json_value()).collect::<Vec<_>>(),
+                "attributes": self.attributes.iter().map(|(_, v)| v.to_serde_json_value()).collect::<Vec<_>>(),
+                "objects": self.resident_objects.iter().map(|o| o.lock().unwrap().to_serde_json_value()).collect::<Vec<_>>(),
+            }
+        )
+    }
+}
+
 impl InnerAttributes for Box<InnerVideoFrame> {
     fn get_attributes_ref(&self) -> &HashMap<(String, String), Attribute> {
         &self.attributes
     }
 
     fn get_attributes_ref_mut(&mut self) -> &mut HashMap<(String, String), Attribute> {
         &mut self.attributes
@@ -303,14 +381,20 @@
     pub(crate) fn from_inner(object: InnerVideoFrame) -> Self {
         VideoFrame {
             inner: Arc::new(Mutex::new(Box::new(object))),
         }
     }
 }
 
+impl ToSerdeJsonValue for VideoFrame {
+    fn to_serde_json_value(&self) -> Value {
+        self.inner.lock().unwrap().to_serde_json_value()
+    }
+}
+
 #[pymethods]
 impl VideoFrame {
     #[classattr]
     const __hash__: Option<Py<PyAny>> = None;
 
     fn __repr__(&self) -> String {
         format!("{:#?}", self.inner.lock().unwrap())
@@ -356,14 +440,19 @@
     }
 
     #[getter]
     pub fn get_source_id(&self) -> String {
         self.inner.lock().unwrap().source_id.clone()
     }
 
+    #[getter]
+    pub fn get_json(&self) -> String {
+        serde_json::to_string(&self.to_serde_json_value()).unwrap()
+    }
+
     #[setter]
     pub fn set_source_id(&mut self, source_id: String) {
         let mut frame = self.inner.lock().unwrap();
         frame.source_id = source_id;
     }
 
     #[getter]
@@ -463,14 +552,15 @@
     }
 
     pub fn add_transformation(&mut self, transformation: PyFrameTransformation) {
         let mut frame = self.inner.lock().unwrap();
         frame.transformations.push(transformation.inner);
     }
 
+    #[getter]
     pub fn get_transformations(&self) -> Vec<PyFrameTransformation> {
         let frame = self.inner.lock().unwrap();
         frame
             .transformations
             .iter()
             .map(|t| PyFrameTransformation::new(t.clone()))
             .collect()
@@ -498,40 +588,60 @@
     pub fn set_content(&mut self, content: PyVideoFrameContent) {
         let mut frame = self.inner.lock().unwrap();
         frame.content = content.inner;
     }
 
     #[getter]
     pub fn attributes(&self) -> Vec<(String, String)> {
-        self.inner_attributes()
+        Python::with_gil(move |py| py.allow_threads(move || self.get_attributes()))
     }
 
-    pub fn find_attributes(
+    #[pyo3(name = "find_attributes")]
+    pub fn find_attributes_py(
         &self,
         creator: Option<String>,
         name: Option<String>,
         hint: Option<String>,
     ) -> Vec<(String, String)> {
-        self.inner_find_attributes(creator, name, hint)
+        Python::with_gil(move |py| {
+            py.allow_threads(move || self.find_attributes(creator, name, hint))
+        })
+    }
+
+    #[pyo3(name = "get_attribute")]
+    pub fn get_attribute_py(&self, creator: String, name: String) -> Option<Attribute> {
+        self.get_attribute(creator, name)
     }
 
-    pub fn get_attribute(&self, creator: String, name: String) -> Option<Attribute> {
-        self.inner_get_attribute(creator, name)
+    #[pyo3(signature = (negated=false, creator=None, names=vec![]))]
+    #[pyo3(name = "delete_attributes")]
+    pub fn delete_attributes_py(
+        &mut self,
+        negated: bool,
+        creator: Option<String>,
+        names: Vec<String>,
+    ) {
+        Python::with_gil(move |py| {
+            py.allow_threads(move || self.delete_attributes(negated, creator, names))
+        })
     }
 
-    pub fn delete_attribute(&mut self, creator: String, name: String) -> Option<Attribute> {
-        self.inner_delete_attribute(creator, name)
+    #[pyo3(name = "delete_attribute")]
+    pub fn delete_attribute_py(&mut self, creator: String, name: String) -> Option<Attribute> {
+        self.delete_attribute(creator, name)
     }
 
-    pub fn set_attribute(&mut self, attribute: Attribute) -> Option<Attribute> {
-        self.inner_set_attribute(attribute)
+    #[pyo3(name = "set_attribute")]
+    pub fn set_attribute_py(&mut self, attribute: Attribute) -> Option<Attribute> {
+        self.set_attribute(attribute)
     }
 
-    pub fn clear_attributes(&mut self) {
-        self.inner_clear_attributes()
+    #[pyo3(name = "clear_attributes")]
+    pub fn clear_attributes_py(&mut self) {
+        self.clear_attributes()
     }
 
     pub fn get_object(&self, id: i64) -> Option<Object> {
         Python::with_gil(|py| {
             py.allow_threads(|| {
                 let frame = self.inner.lock().unwrap();
                 frame
@@ -665,14 +775,15 @@
             })
         })
     }
 }
 
 #[cfg(test)]
 mod tests {
+    use crate::primitives::attribute::Attributive;
     use crate::primitives::Modification;
     use crate::test::utils::gen_frame;
 
     #[test]
     fn test_access_objects_by_id() {
         pyo3::prepare_freethreaded_python();
         let t = gen_frame();
@@ -747,34 +858,34 @@
         );
     }
 
     #[test]
     fn test_find_attributes() {
         pyo3::prepare_freethreaded_python();
         let t = gen_frame();
-        let mut attributes = t.find_attributes(Some("system".to_string()), None, None);
+        let mut attributes = t.find_attributes_py(Some("system".to_string()), None, None);
         attributes.sort();
         assert_eq!(attributes.len(), 2);
         assert_eq!(attributes[0], ("system".to_string(), "test".to_string()));
         assert_eq!(attributes[1], ("system".to_string(), "test2".to_string()));
 
         let attributes =
-            t.find_attributes(Some("system".to_string()), Some("test".to_string()), None);
+            t.find_attributes_py(Some("system".to_string()), Some("test".to_string()), None);
         assert_eq!(attributes.len(), 1);
         assert_eq!(attributes[0], ("system".to_string(), "test".to_string()));
 
-        let attributes = t.find_attributes(
+        let attributes = t.find_attributes_py(
             Some("system".to_string()),
             Some("test".to_string()),
             Some("test".to_string()),
         );
         assert_eq!(attributes.len(), 1);
         assert_eq!(attributes[0], ("system".to_string(), "test".to_string()));
 
-        let mut attributes = t.find_attributes(None, None, Some("test".to_string()));
+        let mut attributes = t.find_attributes_py(None, None, Some("test".to_string()));
         attributes.sort();
         assert_eq!(attributes.len(), 2);
         assert_eq!(attributes[0], ("system".to_string(), "test".to_string()));
         assert_eq!(attributes[1], ("system".to_string(), "test2".to_string()));
     }
 
     #[test]
```

### Comparing `savant_rs-0.1.1/src/primitives/message/video/object.rs` & `savant_rs-0.1.2/src/primitives/message/video/object.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use crate::primitives::attribute::{Attributive, InnerAttributes};
+use crate::primitives::to_json_value::ToSerdeJsonValue;
 use crate::primitives::{Attribute, BBox};
-use pyo3::{pyclass, pymethods, Py, PyAny};
+use pyo3::{pyclass, pymethods, Py, PyAny, Python};
 use rkyv::{with::Skip, Archive, Deserialize, Serialize};
 use std::collections::HashMap;
 use std::sync::{Arc, Mutex};
 
 #[pyclass]
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone)]
 #[archive(check_bytes)]
@@ -13,14 +14,24 @@
     pub id: i64,
     #[pyo3(get, set)]
     pub creator: String,
     #[pyo3(get, set)]
     pub label: String,
 }
 
+impl ToSerdeJsonValue for ParentObject {
+    fn to_serde_json_value(&self) -> serde_json::Value {
+        serde_json::json!({
+            "id": self.id,
+            "creator": self.creator,
+            "label": self.label,
+        })
+    }
+}
+
 #[pymethods]
 impl ParentObject {
     #[classattr]
     const __hash__: Option<Py<PyAny>> = None;
 
     fn __repr__(&self) -> String {
         format!("{self:?}")
@@ -45,14 +56,20 @@
     BoundingBox,
     Attributes,
     Confidence,
     Parent,
     TrackId,
 }
 
+impl ToSerdeJsonValue for Modification {
+    fn to_serde_json_value(&self) -> serde_json::Value {
+        serde_json::json!(format!("{:?}", self))
+    }
+}
+
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone, derive_builder::Builder)]
 #[archive(check_bytes)]
 pub struct InnerObject {
     pub id: i64,
     pub creator: String,
     pub label: String,
     pub bbox: BBox,
@@ -60,14 +77,30 @@
     pub confidence: Option<f64>,
     pub parent: Option<ParentObject>,
     pub track_id: Option<i64>,
     #[with(Skip)]
     pub modifications: Vec<Modification>,
 }
 
+impl ToSerdeJsonValue for InnerObject {
+    fn to_serde_json_value(&self) -> serde_json::Value {
+        serde_json::json!({
+            "id": self.id,
+            "creator": self.creator,
+            "label": self.label,
+            "bbox": self.bbox.to_serde_json_value(),
+            "attributes": self.attributes.iter().map(|(_, v)| v.to_serde_json_value()).collect::<Vec<_>>(),
+            "confidence": self.confidence,
+            "parent": self.parent.as_ref().map(|p| p.to_serde_json_value()),
+            "track_id": self.track_id,
+            "modifications": self.modifications.iter().map(|m| m.to_serde_json_value()).collect::<Vec<serde_json::Value>>(),
+        })
+    }
+}
+
 impl InnerAttributes for InnerObject {
     fn get_attributes_ref(&self) -> &HashMap<(String, String), Attribute> {
         &self.attributes
     }
 
     fn get_attributes_ref_mut(&mut self) -> &mut HashMap<(String, String), Attribute> {
         &mut self.attributes
@@ -76,14 +109,20 @@
 
 #[pyclass]
 #[derive(Debug, Clone)]
 pub struct Object {
     pub(crate) inner: Arc<Mutex<InnerObject>>,
 }
 
+impl ToSerdeJsonValue for Object {
+    fn to_serde_json_value(&self) -> serde_json::Value {
+        self.inner.lock().unwrap().to_serde_json_value()
+    }
+}
+
 impl Attributive<InnerObject> for Object {
     fn get_inner(&self) -> Arc<Mutex<InnerObject>> {
         self.inner.clone()
     }
 }
 
 impl Object {
@@ -225,79 +264,90 @@
         let mut object = self.inner.lock().unwrap();
         object.parent = parent;
         object.modifications.push(Modification::Parent);
     }
 
     #[getter]
     pub fn attributes(&self) -> Vec<(String, String)> {
-        self.inner_attributes()
+        Python::with_gil(move |py| py.allow_threads(move || self.get_attributes()))
     }
 
-    pub fn get_attribute(&self, creator: String, name: String) -> Option<Attribute> {
-        self.inner_get_attribute(creator, name)
+    #[pyo3(name = "get_attribute")]
+    pub fn get_attribute_py(&self, creator: String, name: String) -> Option<Attribute> {
+        self.get_attribute(creator, name)
     }
 
-    pub fn delete_attribute(&mut self, creator: String, name: String) -> Option<Attribute> {
-        match self.inner_get_attribute(creator, name) {
+    #[pyo3(name = "delete_attribute")]
+    pub fn delete_attribute_py(&mut self, creator: String, name: String) -> Option<Attribute> {
+        match self.delete_attribute(creator, name) {
             Some(attribute) => {
                 let mut object = self.inner.lock().unwrap();
                 object.modifications.push(Modification::Attributes);
                 Some(attribute)
             }
             None => None,
         }
     }
 
-    pub fn set_attribute(&mut self, attribute: Attribute) -> Option<Attribute> {
+    #[pyo3(name = "set_attribute")]
+    pub fn set_attribute_py(&mut self, attribute: Attribute) -> Option<Attribute> {
         {
             let mut object = self.inner.lock().unwrap();
             object.modifications.push(Modification::Attributes);
         }
-        self.inner_set_attribute(attribute)
+        self.set_attribute(attribute)
     }
 
-    pub fn clear_attributes(&mut self) {
+    #[pyo3(name = "clear_attributes")]
+    pub fn clear_attributes_py(&mut self) {
         {
             let mut object = self.inner.lock().unwrap();
             object.modifications.push(Modification::Attributes);
         }
-        self.inner_clear_attributes()
+        self.clear_attributes()
     }
 
     #[pyo3(signature = (negated=false, creator=None, names=vec![]))]
-    pub fn delete_attributes(
+    #[pyo3(name = "delete_attributes")]
+    pub fn delete_attributes_py(
         &mut self,
         negated: bool,
         creator: Option<String>,
         names: Vec<String>,
     ) {
-        {
-            let mut object = self.inner.lock().unwrap();
-            object.modifications.push(Modification::Attributes);
-        }
-        self.inner_delete_attributes(negated, creator, names)
+        Python::with_gil(move |py| {
+            py.allow_threads(move || {
+                {
+                    let mut object = self.inner.lock().unwrap();
+                    object.modifications.push(Modification::Attributes);
+                }
+                self.delete_attributes(negated, creator, names)
+            })
+        })
     }
 
-    pub fn find_attributes(
+    #[pyo3(name = "find_attributes")]
+    pub fn find_attributes_py(
         &self,
         creator: Option<String>,
         name: Option<String>,
         hint: Option<String>,
     ) -> Vec<(String, String)> {
-        self.inner_find_attributes(creator, name, hint)
+        Python::with_gil(move |py| py.allow_threads(|| self.find_attributes(creator, name, hint)))
     }
 
     pub fn take_modifications(&self) -> Vec<Modification> {
         let mut object = self.inner.lock().unwrap();
         std::mem::take(&mut object.modifications)
     }
 }
 
 #[cfg(test)]
 mod tests {
+    use crate::primitives::attribute::Attributive;
     use crate::primitives::message::video::object::InnerObjectBuilder;
     use crate::primitives::{AttributeBuilder, BBox, Modification, Object, Value};
 
     fn get_object() -> Object {
         Object::from_inner_object(
             InnerObjectBuilder::default()
                 .id(1)
@@ -409,15 +459,15 @@
     fn test_modifications() {
         let mut t = get_object();
         t.set_label("label2".to_string());
         assert_eq!(t.take_modifications(), vec![Modification::Label]);
         assert_eq!(t.take_modifications(), vec![]);
 
         t.set_bbox(BBox::new(0.0, 0.0, 1.0, 1.0, None));
-        t.clear_attributes();
+        t.clear_attributes_py();
         assert_eq!(
             t.take_modifications(),
             vec![Modification::BoundingBox, Modification::Attributes]
         );
         assert_eq!(t.take_modifications(), vec![]);
     }
 }
```

### Comparing `savant_rs-0.1.1/src/primitives/message.rs` & `savant_rs-0.1.2/src/primitives/message.rs`

 * *Files 2% similar despite different names*

```diff
@@ -92,51 +92,59 @@
     #[staticmethod]
     pub fn end_of_stream(eos: EndOfStream) -> Self {
         Self {
             frame: NativeMessage::EndOfStream(eos),
         }
     }
 
+    #[getter]
     pub fn is_unknown(&self) -> bool {
         matches!(self.frame, NativeMessage::Unknown(_))
     }
 
+    #[getter]
     pub fn is_end_of_stream(&self) -> bool {
         matches!(self.frame, NativeMessage::EndOfStream(_))
     }
 
+    #[getter]
     pub fn is_video_frame(&self) -> bool {
         matches!(self.frame, NativeMessage::VideoFrame(_))
     }
 
+    #[getter]
     pub fn is_video_frame_batch(&self) -> bool {
         matches!(self.frame, NativeMessage::VideoFrameBatch(_))
     }
 
+    #[getter]
     pub fn as_unknown(&self) -> Option<String> {
         match &self.frame {
             NativeMessage::Unknown(s) => Some(s.clone()),
             _ => None,
         }
     }
 
+    #[getter]
     pub fn as_end_of_stream(&self) -> Option<EndOfStream> {
         match &self.frame {
             NativeMessage::EndOfStream(eos) => Some(eos.clone()),
             _ => None,
         }
     }
 
+    #[getter]
     pub fn as_video_frame(&self) -> Option<VideoFrame> {
         match &self.frame {
             NativeMessage::VideoFrame(frame) => Some(frame.clone()),
             _ => None,
         }
     }
 
+    #[getter]
     pub fn as_video_frame_batch(&self) -> Option<VideoFrameBatch> {
         match &self.frame {
             NativeMessage::VideoFrameBatch(batch) => Some(batch.clone()),
             _ => None,
         }
     }
 }
```

### Comparing `savant_rs-0.1.1/src/primitives/polygonal_area.rs` & `savant_rs-0.1.2/src/primitives/polygonal_area.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,41 @@
 use crate::primitives::point::Point;
+use crate::primitives::to_json_value::ToSerdeJsonValue;
 use crate::primitives::{Intersection, IntersectionKind, Segment};
 use geo::{Contains, Intersects, Line, LineString};
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 use rayon::prelude::*;
 use rkyv::{with::Skip, Archive, Deserialize, Serialize};
+use serde_json::Value;
 use std::sync::Arc;
 
 #[pyclass]
 #[derive(Archive, Deserialize, Serialize, Debug, Default, Clone, PartialEq)]
 #[archive(check_bytes)]
 pub struct PolygonalArea {
     pub vertices: Arc<Vec<Point>>,
     pub tags: Arc<Option<Vec<Option<String>>>>,
     #[with(Skip)]
     polygon: Option<geo::Polygon>,
 }
 
+impl ToSerdeJsonValue for PolygonalArea {
+    fn to_serde_json_value(&self) -> Value {
+        let mut vertices = Vec::new();
+        for v in self.vertices.iter() {
+            vertices.push(v.to_serde_json_value());
+        }
+        serde_json::json!({
+            "vertices": vertices,
+            "tags": self.tags.as_ref().as_ref().unwrap_or(&Vec::new()),
+        })
+    }
+}
+
 #[pymethods]
 impl PolygonalArea {
     #[classattr]
     const __hash__: Option<Py<PyAny>> = None;
 
     fn __repr__(&self) -> String {
         format!("{self:?}")
@@ -381,18 +396,16 @@
                 Some(format!("{LOWER}_2")),
                 Some(format!("{LEFT}_2")),
             ]),
         );
 
         let seg1 = Segment::new(Point::new(-2.0, 0.5), Point::new(3.0, 0.5));
         let seg2 = Segment::new(Point::new(-0.5, 2.0), Point::new(-0.5, -2.0));
-        let intersections = PolygonalArea::segments_intersections(
-            vec![area1, area2],
-            vec![seg1, seg2],
-        );
+        let intersections =
+            PolygonalArea::segments_intersections(vec![area1, area2], vec![seg1, seg2]);
         assert_eq!(
             intersections,
             vec![
                 vec![
                     Intersection::new(
                         IntersectionKind::Cross,
                         vec![
```

### Comparing `savant_rs-0.1.1/src/primitives/segment.rs` & `savant_rs-0.1.2/src/primitives/segment.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 use crate::primitives::point::Point;
+use crate::primitives::to_json_value::ToSerdeJsonValue;
 use pyo3::{pyclass, pymethods, Py, PyAny};
 use rkyv::{Archive, Deserialize, Serialize};
+use serde_json::Value;
 
 #[pyclass]
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone)]
 #[archive(check_bytes)]
 pub struct Segment {
     #[pyo3(get, set)]
     pub begin: Point,
     #[pyo3(get, set)]
     pub end: Point,
 }
 
+impl ToSerdeJsonValue for Segment {
+    fn to_serde_json_value(&self) -> Value {
+        serde_json::json!({
+            "begin": self.begin.to_serde_json_value(),
+            "end": self.end.to_serde_json_value(),
+        })
+    }
+}
+
 #[pymethods]
 impl Segment {
     #[classattr]
     const __hash__: Option<Py<PyAny>> = None;
 
     fn __repr__(&self) -> String {
         format!("{self:?}")
@@ -38,14 +49,20 @@
     Enter,
     Inside,
     Leave,
     Cross,
     Outside,
 }
 
+impl ToSerdeJsonValue for IntersectionKind {
+    fn to_serde_json_value(&self) -> Value {
+        serde_json::json!(format!("{:?}", self))
+    }
+}
+
 #[pymethods]
 impl IntersectionKind {
     #[classattr]
     const __hash__: Option<Py<PyAny>> = None;
 
     fn __repr__(&self) -> String {
         format!("{self:?}")
@@ -60,14 +77,23 @@
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone)]
 #[archive(check_bytes)]
 pub struct Intersection {
     pub kind: IntersectionKind,
     pub edges: Vec<(usize, Option<String>)>,
 }
 
+impl ToSerdeJsonValue for Intersection {
+    fn to_serde_json_value(&self) -> Value {
+        serde_json::json!({
+            "kind": self.kind.to_serde_json_value(),
+            "edges": self.edges,
+        })
+    }
+}
+
 #[pymethods]
 impl Intersection {
     #[classattr]
     const __hash__: Option<Py<PyAny>> = None;
 
     fn __repr__(&self) -> String {
         format!("{self:?}")
```

### Comparing `savant_rs-0.1.1/src/primitives.rs` & `savant_rs-0.1.2/src/primitives.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 pub mod attribute;
 pub mod bbox;
 pub mod message;
 pub mod point;
 pub mod polygonal_area;
 pub mod segment;
+pub mod to_json_value;
 
+use crate::primitives::message::video::frame::PyFrameTransformation;
 pub use attribute::Attribute;
 pub use attribute::AttributeBuilder;
 pub use attribute::Value;
 pub use bbox::BBox;
 pub use message::eos::EndOfStream;
 pub use message::loader::load_message;
 pub use message::saver::save_message;
@@ -40,10 +42,11 @@
     m.add_class::<Object>()?;
     m.add_class::<ParentObject>()?;
     m.add_class::<VideoFrame>()?;
     m.add_class::<VideoFrameBatch>()?;
     m.add_class::<EndOfStream>()?;
     m.add_class::<Message>()?;
     m.add_class::<PyVideoFrameContent>()?;
+    m.add_class::<PyFrameTransformation>()?;
     m.add_class::<Modification>()?;
     Ok(())
 }
```

### Comparing `savant_rs-0.1.1/src/test.rs` & `savant_rs-0.1.2/src/test.rs`

 * *Files 4% similar despite different names*

```diff
@@ -70,46 +70,46 @@
                             .unwrap(),
                     )),
                 ])
                 .build()
                 .unwrap(),
         );
 
-        f.set_attribute(
+        f.set_attribute_py(
             AttributeBuilder::default()
                 .creator("system".into())
                 .name("test".into())
                 .hint(None)
                 .hint(Some("test".into()))
                 .values(vec![Value::string("1".into(), None)])
                 .build()
                 .unwrap(),
         );
 
-        f.set_attribute(
+        f.set_attribute_py(
             AttributeBuilder::default()
                 .creator("system2".into())
                 .name("test2".into())
                 .hint(None)
                 .values(vec![Value::string("2".into(), None)])
                 .build()
                 .unwrap(),
         );
 
-        f.set_attribute(
+        f.set_attribute_py(
             AttributeBuilder::default()
                 .creator("system".into())
                 .name("test2".into())
                 .hint(Some("test".into()))
                 .values(vec![Value::string("3".into(), None)])
                 .build()
                 .unwrap(),
         );
 
-        f.set_attribute(
+        f.set_attribute_py(
             AttributeBuilder::default()
                 .creator("test".to_string())
                 .name("test".to_string())
                 .hint(Some("hint".to_string()))
                 .values(vec![
                     Value::bytes(vec![8, 3, 8, 8], [0; 192].into(), None),
                     Value::integers([0, 1, 2, 3, 4, 5].into(), None),
```

### Comparing `savant_rs-0.1.1/src/test_rkyv_tuple.rs` & `savant_rs-0.1.2/src/test_rkyv_tuple.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.1/src/tests_pyo3_access.rs` & `savant_rs-0.1.2/src/tests_pyo3_access.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.1/src/utils/fps_meter.rs` & `savant_rs-0.1.2/src/utils/fps_meter.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.1/src/utils.rs` & `savant_rs-0.1.2/src/utils.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.1/Cargo.lock` & `savant_rs-0.1.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -411,14 +411,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itoa"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+
+[[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
@@ -818,29 +824,36 @@
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "ryu"
+version = "1.0.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+
+[[package]]
 name = "savant_rs"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "anyhow",
  "derive_builder",
  "env_logger",
  "geo",
  "itertools",
  "num_cpus",
  "numpy",
  "pyo3",
  "pyo3-build-config",
  "pyo3-log",
  "rayon",
  "rkyv",
+ "serde_json",
  "thiserror",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -875,14 +888,25 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.15",
 ]
 
 [[package]]
+name = "serde_json"
+version = "1.0.96"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+dependencies = [
+ "itoa",
+ "ryu",
+ "serde",
+]
+
+[[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
 name = "smallvec"
```

### Comparing `savant_rs-0.1.1/PKG-INFO` & `savant_rs-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: savant_rs
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Savant rust optimization library
 Keywords: computer-vision,video-processing
 Home-Page: https://github.com/insight-platform/savant-rs
```

