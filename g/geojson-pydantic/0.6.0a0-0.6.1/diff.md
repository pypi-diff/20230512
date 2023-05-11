# Comparing `tmp/geojson-pydantic-0.6.0a0.tar.gz` & `tmp/geojson-pydantic-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geojson-pydantic-0.6.0a0.tar", last modified: Tue Apr  4 12:52:00 2023, max compression
+gzip compressed data, was "geojson-pydantic-0.6.1.tar", last modified: Thu May 11 23:04:37 2023, max compression
```

## Comparing `geojson-pydantic-0.6.0a0.tar` & `geojson-pydantic-0.6.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0      222 2023-04-04 12:51:52.732794 geojson-pydantic-0.6.0a0/.bumpversion.cfg
--rw-r--r--   0        0        0      116 2023-04-04 12:51:52.732794 geojson-pydantic-0.6.0a0/.flake8
--rw-r--r--   0        0        0     1173 2023-04-04 12:51:52.732794 geojson-pydantic-0.6.0a0/.gitignore
--rw-r--r--   0        0        0     1119 2023-04-04 12:51:52.732794 geojson-pydantic-0.6.0a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-04-04 12:51:52.732794 geojson-pydantic-0.6.0a0/LICENSE
--rw-r--r--   0        0        0     6560 2023-04-04 12:51:52.732794 geojson-pydantic-0.6.0a0/README.md
--rw-r--r--   0        0        0      450 2023-04-04 12:51:52.732794 geojson-pydantic-0.6.0a0/geojson_pydantic/__init__.py
--rw-r--r--   0        0        0     2571 2023-04-04 12:51:52.732794 geojson-pydantic-0.6.0a0/geojson_pydantic/features.py
--rw-r--r--   0        0        0      705 2023-04-04 12:51:52.732794 geojson-pydantic-0.6.0a0/geojson_pydantic/geo_interface.py
--rw-r--r--   0        0        0    10818 2023-04-04 12:51:52.732794 geojson-pydantic-0.6.0a0/geojson_pydantic/geometries.py
--rw-r--r--   0        0        0        0 2023-04-04 12:51:52.732794 geojson-pydantic-0.6.0a0/geojson_pydantic/py.typed
--rw-r--r--   0        0        0      694 2023-04-04 12:51:52.732794 geojson-pydantic-0.6.0a0/geojson_pydantic/types.py
--rw-r--r--   0        0        0     1656 2023-04-04 12:51:52.736794 geojson-pydantic-0.6.0a0/pyproject.toml
--rw-r--r--   0        0        0     7566 1970-01-01 00:00:00.000000 geojson-pydantic-0.6.0a0/PKG-INFO
+-rw-r--r--   0        0        0      220 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/.bumpversion.cfg
+-rw-r--r--   0        0        0     1173 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/.gitignore
+-rw-r--r--   0        0        0      792 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/LICENSE
+-rw-r--r--   0        0        0     6592 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/README.md
+-rw-r--r--   0        0        0      448 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/geojson_pydantic/__init__.py
+-rw-r--r--   0        0        0     2624 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/geojson_pydantic/features.py
+-rw-r--r--   0        0        0      705 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/geojson_pydantic/geo_interface.py
+-rw-r--r--   0        0        0    10811 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/geojson_pydantic/geometries.py
+-rw-r--r--   0        0        0        0 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/geojson_pydantic/py.typed
+-rw-r--r--   0        0        0      694 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/geojson_pydantic/types.py
+-rw-r--r--   0        0        0     2293 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     7596 1970-01-01 00:00:00.000000 geojson-pydantic-0.6.1/PKG-INFO
```

### Comparing `geojson-pydantic-0.6.0a0/.gitignore` & `geojson-pydantic-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `geojson-pydantic-0.6.0a0/LICENSE` & `geojson-pydantic-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geojson-pydantic-0.6.0a0/README.md` & `geojson-pydantic-0.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,34 +16,34 @@
   <a href="https://pypistats.org/packages/geojson-pydantic" target="_blank">
       <img src="https://img.shields.io/pypi/dm/geojson-pydantic.svg" alt="Downloads">
   </a>
   <a href="https://github.com/developmentseed/geojson-pydantic/blob/main/LICENSE" target="_blank">
       <img src="https://img.shields.io/github/license/developmentseed/geojson-pydantic.svg" alt="License">
   </a>
   <a href="https://anaconda.org/conda-forge/geojson-pydantic" target="_blank">
-      <img src="https://anaconda.org/conda-forge/geojson-pydantic/badges/installer/conda.svg" alt="Conda">
+      <img src="https://anaconda.org/conda-forge/geojson-pydantic/badges/version.svg" alt="Conda">
   </a>
 </p>
 
 ## Description
 
 `geojson_pydantic` provides a suite of Pydantic models matching the GeoJSON specification [rfc7946](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.1). Those models can be used for creating or validating geojson data.
 
 ## Install
 
 ```bash
-$ pip install -U pip
-$ pip install geojson-pydantic
+$ python -m pip install -U pip
+$ python -m pip install geojson-pydantic
 ```
 
 Or install from source:
 
 ```bash
-$ pip install -U pip
-$ pip install git+https://github.com/developmentseed/geojson-pydantic.git
+$ python -m pip install -U pip
+$ python -m pip install git+https://github.com/developmentseed/geojson-pydantic.git
 ```
 
 Install with conda from [`conda-forge`](https://anaconda.org/conda-forge/geojson-pydantic):
 
 ```bash
 $ conda install -c conda-forge geojson-pydantic
 ```
```

### Comparing `geojson-pydantic-0.6.0a0/geojson_pydantic/features.py` & `geojson-pydantic-0.6.1/geojson_pydantic/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,26 +26,32 @@
         """Model configuration."""
 
         use_enum_values = True
 
     @validator("bbox", pre=True)
     def check_bbox(cls, bbox: BBox) -> BBox:
         """Check that bbox is valid."""
+        if bbox is None:
+            return bbox
+
         if len(bbox) == 6:
             if bbox[0] > bbox[3] or bbox[1] > bbox[4] or bbox[2] > bbox[5]:  # type: ignore
                 raise ValueError(
                     "BBox must be in the form [west, south, bottom, east, north, top]"
                 )
+
         elif len(bbox) == 4:
             if bbox[0] > bbox[2] or bbox[1] > bbox[3]:
                 raise ValueError("BBox must be in the form [west, south, east, north]")
+
         else:
             raise ValueError(
                 "BBox must be in the form [west, south, east, north] or [west, south, bottom, east, north, top]"
             )
+
         return bbox
 
     @validator("geometry", pre=True, always=True)
     def set_geometry(cls, geometry: Any) -> Any:
         """set geometry from geo interface or input"""
         if hasattr(geometry, "__geo_interface__"):
             return geometry.__geo_interface__
```

### Comparing `geojson-pydantic-0.6.0a0/geojson_pydantic/geo_interface.py` & `geojson-pydantic-0.6.1/geojson_pydantic/geo_interface.py`

 * *Files identical despite different names*

### Comparing `geojson-pydantic-0.6.0a0/geojson_pydantic/geometries.py` & `geojson-pydantic-0.6.1/geojson_pydantic/geometries.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     def __wkt_coordinates__(self, coordinates: Any, force_z: bool) -> str:
         """return WKT coordinates."""
         return _lines_wtk_coordinates(coordinates, force_z)
 
     @validator("coordinates")
     def check_closure(cls, coordinates: List) -> List:
         """Validate that Polygon is closed (first and last coordinate are the same)."""
-        if any([ring[-1] != ring[0] for ring in coordinates]):
+        if any(ring[-1] != ring[0] for ring in coordinates):
             raise ValueError("All linear rings have the same start and end coordinates")
 
         return coordinates
 
     @property
     def exterior(self) -> Union[LinearRing, None]:
         """Return the exterior Linear Ring of the polygon."""
@@ -234,15 +234,15 @@
     def has_z(self) -> bool:
         """Checks if any coordinates have a Z value."""
         return any(_lines_has_z(polygon) for polygon in self.coordinates)
 
     @validator("coordinates")
     def check_closure(cls, coordinates: List) -> List:
         """Validate that Polygon is closed (first and last coordinate are the same)."""
-        if any([ring[-1] != ring[0] for polygon in coordinates for ring in polygon]):
+        if any(ring[-1] != ring[0] for polygon in coordinates for ring in polygon):
             raise ValueError("All linear rings have the same start and end coordinates")
 
         return coordinates
 
 
 Geometry = Annotated[
     Union[Point, MultiPoint, LineString, MultiLineString, Polygon, MultiPolygon],
@@ -294,15 +294,15 @@
             warnings.warn(
                 "GeometryCollection should not be used for single geometries."
             )
         if any(geom.type == "GeometryCollection" for geom in geometries):
             warnings.warn(
                 "GeometryCollection should not be used for nested GeometryCollections."
             )
-        if len(set(geom.type for geom in geometries)) == 1:
+        if len({geom.type for geom in geometries}) == 1:
             warnings.warn(
                 "GeometryCollection should not be used for homogeneous collections."
             )
         return geometries
 
 
 def parse_geometry_obj(obj: Any) -> Geometry:
```

### Comparing `geojson-pydantic-0.6.0a0/geojson_pydantic/types.py` & `geojson-pydantic-0.6.1/geojson_pydantic/types.py`

 * *Files identical despite different names*

### Comparing `geojson-pydantic-0.6.0a0/pyproject.toml` & `geojson-pydantic-0.6.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -41,31 +41,54 @@
     "tests/",
     "docs/",
     ".github/",
     "CHANGELOG.md",
     "CONTRIBUTING.md",
 ]
 
+[tool.coverage.run]
+branch = true
+parallel = true
+
+[tool.coverage.report]
+exclude_lines = [
+  "no cov",
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:",
+]
+
 [tool.isort]
 profile = "black"
 known_first_party = ["geojson_pydantic"]
 known_third_party = ["pydantic"]
 default_section = "THIRDPARTY"
 
 [tool.mypy]
-plugins = [
-  "pydantic.mypy"
-]
+plugins = ["pydantic.mypy"]
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
+warn_untyped_fields = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
-[tool.pydantic-mypy]
-warn_untyped_fields = true
+[tool.ruff]
+select = [
+    "D1",  # pydocstyle errors
+    "E",  # pycodestyle errors
+    "W",  # pycodestyle warnings
+    "F",  # flake8
+    "C",  # flake8-comprehensions
+    "B",  # flake8-bugbear
+]
+ignore = [
+    "E501",  # line too long, handled by black
+    "B008",  # do not perform function calls in argument defaults
+    "B905",  # ignore zip() without an explicit strict= parameter, only support with python >3.10
+]
 
-[tool.pydocstyle]
-select = "D1"
-match = "(?!test).*.py"
+[tool.ruff.per-file-ignores]
+"tests/test_geometries.py" = ["D1"]
+"tests/test_features.py" = ["D1"]
+"tests/test_package.py" = ["D1"]
```

### Comparing `geojson-pydantic-0.6.0a0/PKG-INFO` & `geojson-pydantic-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geojson-pydantic
-Version: 0.6.0a0
+Version: 0.6.1
 Summary: Pydantic data models for the GeoJSON spec.
 Keywords: geojson,Pydantic
 Author-email: Drew Bollinger <drew@developmentseed.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -42,34 +42,34 @@
   <a href="https://pypistats.org/packages/geojson-pydantic" target="_blank">
       <img src="https://img.shields.io/pypi/dm/geojson-pydantic.svg" alt="Downloads">
   </a>
   <a href="https://github.com/developmentseed/geojson-pydantic/blob/main/LICENSE" target="_blank">
       <img src="https://img.shields.io/github/license/developmentseed/geojson-pydantic.svg" alt="License">
   </a>
   <a href="https://anaconda.org/conda-forge/geojson-pydantic" target="_blank">
-      <img src="https://anaconda.org/conda-forge/geojson-pydantic/badges/installer/conda.svg" alt="Conda">
+      <img src="https://anaconda.org/conda-forge/geojson-pydantic/badges/version.svg" alt="Conda">
   </a>
 </p>
 
 ## Description
 
 `geojson_pydantic` provides a suite of Pydantic models matching the GeoJSON specification [rfc7946](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.1). Those models can be used for creating or validating geojson data.
 
 ## Install
 
 ```bash
-$ pip install -U pip
-$ pip install geojson-pydantic
+$ python -m pip install -U pip
+$ python -m pip install geojson-pydantic
 ```
 
 Or install from source:
 
 ```bash
-$ pip install -U pip
-$ pip install git+https://github.com/developmentseed/geojson-pydantic.git
+$ python -m pip install -U pip
+$ python -m pip install git+https://github.com/developmentseed/geojson-pydantic.git
 ```
 
 Install with conda from [`conda-forge`](https://anaconda.org/conda-forge/geojson-pydantic):
 
 ```bash
 $ conda install -c conda-forge geojson-pydantic
 ```
```

