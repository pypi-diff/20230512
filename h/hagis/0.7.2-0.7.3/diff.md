# Comparing `tmp/hagis-0.7.2.tar.gz` & `tmp/hagis-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.7.2.tar", last modified: Tue May  9 12:42:11 2023, max compression
+gzip compressed data, was "hagis-0.7.3.tar", last modified: Fri May 12 11:55:46 2023, max compression
```

## Comparing `hagis-0.7.2.tar` & `hagis-0.7.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 12:42:11.471745 hagis-0.7.2/
--rw-rw-rw-   0        0        0      923 2023-05-09 12:42:11.463751 hagis-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.7.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 12:42:11.455492 hagis-0.7.2/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-05-09 12:42:11.000000 hagis-0.7.2/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-05-09 12:42:11.000000 hagis-0.7.2/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 12:42:11.000000 hagis-0.7.2/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-09 12:42:11.000000 hagis-0.7.2/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    23599 2023-05-09 12:26:32.000000 hagis-0.7.2/hagis.py
--rw-rw-rw-   0        0        0      589 2023-05-09 12:40:09.000000 hagis-0.7.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 12:42:11.471745 hagis-0.7.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 11:55:46.081746 hagis-0.7.3/
+-rw-rw-rw-   0        0        0      923 2023-05-12 11:55:46.072140 hagis-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.7.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 11:55:46.072140 hagis-0.7.3/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-05-12 11:55:45.000000 hagis-0.7.3/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-05-12 11:55:45.000000 hagis-0.7.3/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 11:55:45.000000 hagis-0.7.3/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-12 11:55:45.000000 hagis-0.7.3/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    23894 2023-05-12 00:42:32.000000 hagis-0.7.3/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-05-11 20:03:14.000000 hagis-0.7.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 11:55:46.084694 hagis-0.7.3/setup.cfg
```

### Comparing `hagis-0.7.2/PKG-INFO` & `hagis-0.7.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.7.2
+Version: 0.7.3
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.7.2/hagis.egg-info/PKG-INFO` & `hagis-0.7.3/hagis.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.7.2
+Version: 0.7.3
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.7.2/hagis.py` & `hagis-0.7.3/hagis.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from uuid import UUID
 from requests import Session
 from requests.adapters import HTTPAdapter, Retry
 
 T = TypeVar("T")
 
 
-class Layer(Generic[T]):  # pylint: disable=too-many-instance-attributes
+class Layer(Generic[T], Iterator[T]):  # pylint: disable=too-many-instance-attributes
     """ Layer class.
 
     Args:
         Generic (T): Type argument.
     """
     def __init__(self, layer_url: str, model: Type[T] = SimpleNamespace,
                  oid_field: str = "objectid", shape_property_name: str = "shape", **mapping: str) -> None:
@@ -32,14 +32,15 @@
             layer_url (str): Layer url (e.g. .../FeatureServer/0).
             model (Type[T], optional): Model to map to.  Defaults to SimpleNamespace.
             oid_field (str, optional): Name of the Object ID field.  Defaults to "objectid".
             shape_property_name (str, optional): Name of the shape property.  Defaults to "shape".
         """
         self._layer_url = layer_url
         self._model = model
+        self._iterator = None
         self._oid_field = oid_field
         self._shape_property_name = shape_property_name
         self._shape_property_type = None
         self._unknown_shape_types = [Any, object, SimpleNamespace]
         self._property_name_to_lower_field: Dict[str, str] = {}
         self._lower_field_to_property_name_type: Dict[str, Tuple[str, type]] = {}
         self._generate_token: Callable[[], str] = lambda: ""
@@ -280,14 +281,23 @@
             id_set = set(map(str, ids))
         else:
             field_name = id_field if id_field else "globalid"
             id_set = set((f"'{_id}'" for _id in ids))
 
         return f"({field_name} IN ({','.join(id_set)}))"
 
+    def __iter__(self) -> Iterator[T]:
+        self._iterator = self.query()
+        return self
+
+    def __next__(self) -> T:
+        if not self._iterator:
+            self._iterator = self.query()
+        return self._iterator.__next__()
+
     def _to_dict(self, item: T) -> Dict[str, Any]:
         dictionary: Dict[str, Any] = {}
         attributes: Dict[str, Any] = {}
 
         dictionary["attributes"] = attributes
 
         for key, value in item.__dict__.items():
```

### Comparing `hagis-0.7.2/pyproject.toml` & `hagis-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.7.2"
+version = "0.7.3"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

