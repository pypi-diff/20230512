# Comparing `tmp/fudgeo-0.4.2-py3-none-any.whl.zip` & `tmp/fudgeo-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 26762 bytes, number of entries: 17
--rw-r--r--  2.0 unx      117 b- defN 23-May-11 12:46 fudgeo/__init__.py
--rw-r--r--  2.0 unx     2538 b- defN 23-May-11 01:39 fudgeo/constant.py
+Zip file size: 28058 bytes, number of entries: 17
+-rw-r--r--  2.0 unx      117 b- defN 23-May-12 16:27 fudgeo/__init__.py
+-rw-r--r--  2.0 unx     2538 b- defN 23-May-11 16:25 fudgeo/constant.py
 -rw-r--r--  2.0 unx     1157 b- defN 23-Jan-04 21:53 fudgeo/enumeration.py
--rw-r--r--  2.0 unx    20081 b- defN 23-May-06 22:48 fudgeo/geopkg.py
+-rw-r--r--  2.0 unx    20081 b- defN 23-May-12 12:57 fudgeo/geopkg.py
 -rw-r--r--  2.0 unx     2673 b- defN 23-May-06 22:48 fudgeo/geopkg.sql
 -rw-r--r--  2.0 unx     7768 b- defN 23-May-06 22:48 fudgeo/sql.py
 -rw-r--r--  2.0 unx      974 b- defN 23-May-06 22:48 fudgeo/geometry/__init__.py
--rw-r--r--  2.0 unx     2000 b- defN 23-May-11 12:45 fudgeo/geometry/base.py
--rw-r--r--  2.0 unx    18653 b- defN 23-May-11 12:45 fudgeo/geometry/linestring.py
--rw-r--r--  2.0 unx    19794 b- defN 23-May-11 12:45 fudgeo/geometry/point.py
--rw-r--r--  2.0 unx    26366 b- defN 23-May-11 12:45 fudgeo/geometry/polygon.py
--rw-r--r--  2.0 unx    15891 b- defN 23-May-11 12:45 fudgeo/geometry/util.py
--rw-r--r--  2.0 unx     1088 b- defN 23-May-11 12:46 fudgeo-0.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     9095 b- defN 23-May-11 12:46 fudgeo-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-11 12:46 fudgeo-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-11 12:46 fudgeo-0.4.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1322 b- defN 23-May-11 12:46 fudgeo-0.4.2.dist-info/RECORD
-17 files, 129616 bytes uncompressed, 24630 bytes compressed:  81.0%
+-rw-r--r--  2.0 unx     2012 b- defN 23-May-11 23:19 fudgeo/geometry/base.py
+-rw-r--r--  2.0 unx    18786 b- defN 23-May-12 01:46 fudgeo/geometry/linestring.py
+-rw-r--r--  2.0 unx    20019 b- defN 23-May-12 12:56 fudgeo/geometry/point.py
+-rw-r--r--  2.0 unx    26589 b- defN 23-May-12 01:46 fudgeo/geometry/polygon.py
+-rw-r--r--  2.0 unx    16275 b- defN 23-May-12 13:03 fudgeo/geometry/util.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-May-12 18:48 fudgeo-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12609 b- defN 23-May-12 18:48 fudgeo-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 18:48 fudgeo-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-12 18:48 fudgeo-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1323 b- defN 23-May-12 18:48 fudgeo-0.5.0.dist-info/RECORD
+17 files, 134108 bytes uncompressed, 25926 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: fudgeo/geometry/polygon.py
 Comment: 
 
 Filename: fudgeo/geometry/util.py
 Comment: 
 
-Filename: fudgeo-0.4.2.dist-info/LICENSE
+Filename: fudgeo-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: fudgeo-0.4.2.dist-info/METADATA
+Filename: fudgeo-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: fudgeo-0.4.2.dist-info/WHEEL
+Filename: fudgeo-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: fudgeo-0.4.2.dist-info/top_level.txt
+Filename: fudgeo-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fudgeo-0.4.2.dist-info/RECORD
+Filename: fudgeo-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fudgeo/__init__.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 """
 Package Initialization
 """
 
 
-__version__ = '0.4.2'
+__version__ = '0.5.0'
 
 
 if __name__ == '__main__':
     pass
```

## fudgeo/geometry/base.py

```diff
@@ -1,19 +1,16 @@
 # -*- coding: utf-8 -*-
 """
 Base Classes
 """
 
 
 from abc import abstractmethod
-from functools import reduce
-from operator import add
 from typing import List, Optional, Tuple
 
-from fudgeo.constant import EMPTY
 from fudgeo.geometry.util import EMPTY_ENVELOPE, Envelope, make_header
 
 
 class AbstractGeometry:
     """
     Abstract Geometry
     """
@@ -22,31 +19,35 @@
     def __init__(self, srs_id: int) -> None:
         """
         Initialize the AbstractGeometry class
         """
         super().__init__()
         self.srs_id: int = srs_id
         self._env: Envelope = EMPTY_ENVELOPE
-        self._args: Optional[Tuple[bytes, int]] = None
+        self._args: Optional[Tuple[memoryview, int]] = None
     # End init built-in
 
     @abstractmethod
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:  # pragma: nocover
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:  # pragma: nocover
         """
         To WKB
         """
         pass
     # End _to_wkb method
 
     @staticmethod
-    def _join_geometries(geoms: List['AbstractGeometry']) -> bytes:
+    def _join_geometries(prefix: bytes,
+                         geoms: List['AbstractGeometry']) -> bytearray:
         """
         Join Geometries
         """
-        return reduce(add, [geom._to_wkb() for geom in geoms], EMPTY)
+        ary = bytearray(prefix)
+        for geom in geoms:
+            ary.extend(geom._to_wkb())
+        return ary
     # End _join_geometries method
 
     @property
     @abstractmethod
     def is_empty(self) -> bool:
         """
         Is Empty
```

## fudgeo/geometry/linestring.py

```diff
@@ -1,59 +1,63 @@
 # -*- coding: utf-8 -*-
 """
 Line String
 """
 
 
 from struct import pack
-from typing import List
+from typing import List, TYPE_CHECKING
 
 from fudgeo.constant import (
     COUNT_CODE, DOUBLE, FOUR_D, QUADRUPLE, THREE_D, TRIPLE, TWO_D,
     WKB_LINESTRING_M_PRE, WKB_LINESTRING_PRE, WKB_LINESTRING_ZM_PRE,
     WKB_LINESTRING_Z_PRE, WKB_MULTI_LINESTRING_M_PRE, WKB_MULTI_LINESTRING_PRE,
     WKB_MULTI_LINESTRING_ZM_PRE, WKB_MULTI_LINESTRING_Z_PRE)
 from fudgeo.geometry.base import AbstractGeometry
 from fudgeo.geometry.point import Point, PointM, PointZ, PointZM
 from fudgeo.geometry.util import (
-    EMPTY_ENVELOPE, Envelope, envelope_from_coordinates,
+    EMPTY_ENVELOPE, Envelope, as_array, envelope_from_coordinates,
     envelope_from_coordinates_m, envelope_from_coordinates_z,
     envelope_from_coordinates_zm, envelope_from_geometries,
     envelope_from_geometries_m, envelope_from_geometries_z,
     envelope_from_geometries_zm, lazy_unpack, pack_coordinates, unpack_line,
     unpack_lines)
 
 
+if TYPE_CHECKING:
+    from numpy import ndarray
+
+
 class LineString(AbstractGeometry):
     """
     LineString
     """
     __slots__ = '_coordinates',
 
     def __init__(self, coordinates: List[DOUBLE], srs_id: int) -> None:
         """
         Initialize the LineString class
         """
         super().__init__(srs_id=srs_id)
-        self._coordinates: List[DOUBLE] = coordinates
+        self._coordinates: 'ndarray' = as_array(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'LineString') -> bool:
         """
         Equals
         """
         if not isinstance(other, LineString):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
-    def coordinates(self) -> List[DOUBLE]:
+    def coordinates(self) -> 'ndarray':
         """
         Coordinates
         """
         if self._args:
             self._coordinates = unpack_line(*self._args)
             self._args = None
         # noinspection PyTypeChecker
@@ -85,19 +89,19 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
-        return WKB_LINESTRING_PRE + pack_coordinates(self.coordinates)
+        return pack_coordinates(WKB_LINESTRING_PRE, self.coordinates)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LineString':
         """
         From Geopackage
         """
@@ -113,30 +117,30 @@
     __slots__ = '_coordinates',
 
     def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
         """
         Initialize the LineStringZ class
         """
         super().__init__(srs_id=srs_id)
-        self._coordinates: List[TRIPLE] = coordinates
+        self._coordinates: 'ndarray' = as_array(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'LineStringZ') -> bool:
         """
         Equals
         """
         if not isinstance(other, LineStringZ):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
-    def coordinates(self) -> List[TRIPLE]:
+    def coordinates(self) -> 'ndarray':
         """
         Coordinates
         """
         if self._args:
             self._coordinates = unpack_line(*self._args)
             self._args = None
         # noinspection PyTypeChecker
@@ -169,20 +173,20 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates_z(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
-        return WKB_LINESTRING_Z_PRE + pack_coordinates(
-            self.coordinates, has_z=True)
+        return pack_coordinates(
+            WKB_LINESTRING_Z_PRE, self.coordinates, has_z=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LineStringZ':
         """
         From Geopackage
         """
@@ -198,30 +202,30 @@
     __slots__ = '_coordinates',
 
     def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
         """
         Initialize the LineStringM class
         """
         super().__init__(srs_id=srs_id)
-        self._coordinates: List[TRIPLE] = coordinates
+        self._coordinates: 'ndarray' = as_array(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'LineStringM') -> bool:
         """
         Equals
         """
         if not isinstance(other, LineStringM):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
-    def coordinates(self) -> List[TRIPLE]:
+    def coordinates(self) -> 'ndarray':
         """
         Coordinates
         """
         if self._args:
             self._coordinates = unpack_line(*self._args)
             self._args = None
         # noinspection PyTypeChecker
@@ -254,20 +258,20 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates_m(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
-        return WKB_LINESTRING_M_PRE + pack_coordinates(
-            self.coordinates, has_m=True)
+        return pack_coordinates(
+            WKB_LINESTRING_M_PRE, self.coordinates, has_m=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LineStringM':
         """
         From Geopackage
         """
@@ -283,30 +287,30 @@
     __slots__ = '_coordinates',
 
     def __init__(self, coordinates: List[QUADRUPLE], srs_id: int) -> None:
         """
         Initialize the LineStringZM class
         """
         super().__init__(srs_id=srs_id)
-        self._coordinates: List[QUADRUPLE] = coordinates
+        self._coordinates: 'ndarray' = as_array(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'LineStringZM') -> bool:
         """
         Equals
         """
         if not isinstance(other, LineStringZM):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
-    def coordinates(self) -> List[QUADRUPLE]:
+    def coordinates(self) -> 'ndarray':
         """
         Coordinates
         """
         if self._args:
             self._coordinates = unpack_line(*self._args)
             self._args = None
         # noinspection PyTypeChecker
@@ -339,20 +343,20 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates_zm(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
-        return WKB_LINESTRING_ZM_PRE + pack_coordinates(
-            self.coordinates, has_z=True, has_m=True)
+        return pack_coordinates(
+            WKB_LINESTRING_ZM_PRE, self.coordinates, has_z=True, has_m=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LineStringZM':
         """
         From Geopackage
         """
@@ -410,21 +414,21 @@
     def is_empty(self) -> bool:
         """
         Is Empty
         """
         return not (bool(self._args) or bool(self.lines))
     # End is_empty property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
         geoms = self.lines
-        return (WKB_MULTI_LINESTRING_PRE + pack(COUNT_CODE, len(geoms)) +
-                self._join_geometries(geoms))
+        prefix = WKB_MULTI_LINESTRING_PRE + pack(COUNT_CODE, len(geoms))
+        return self._join_geometries(prefix, geoms)
     # End _to_wkb method
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
@@ -506,21 +510,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_z(self.lines)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
         geoms = self.lines
-        return (WKB_MULTI_LINESTRING_Z_PRE + pack(COUNT_CODE, len(geoms)) +
-                self._join_geometries(geoms))
+        prefix = WKB_MULTI_LINESTRING_Z_PRE + pack(COUNT_CODE, len(geoms))
+        return self._join_geometries(prefix, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiLineStringZ':
         """
         From Geopackage
         """
@@ -590,21 +594,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_m(self.lines)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
         geoms = self.lines
-        return (WKB_MULTI_LINESTRING_M_PRE + pack(COUNT_CODE, len(geoms)) +
-                self._join_geometries(geoms))
+        prefix = WKB_MULTI_LINESTRING_M_PRE + pack(COUNT_CODE, len(geoms))
+        return self._join_geometries(prefix, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiLineStringM':
         """
         From Geopackage
         """
@@ -675,21 +679,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_zm(self.lines)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
         geoms = self.lines
-        return (WKB_MULTI_LINESTRING_ZM_PRE + pack(COUNT_CODE, len(geoms)) +
-                self._join_geometries(geoms))
+        prefix = WKB_MULTI_LINESTRING_ZM_PRE + pack(COUNT_CODE, len(geoms))
+        return self._join_geometries(prefix, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiLineStringZM':
         """
         From Geopackage
         """
```

## fudgeo/geometry/point.py

```diff
@@ -2,30 +2,34 @@
 """
 Points
 """
 
 
 from math import isnan, nan
 from struct import pack, unpack
-from typing import List
+from typing import List, TYPE_CHECKING
 
 from fudgeo.constant import (
     DOUBLE, EMPTY, FOUR_D, FOUR_D_PACK_CODE, FOUR_D_UNPACK_CODE, HEADER_OFFSET,
     QUADRUPLE, THREE_D, THREE_D_PACK_CODE, THREE_D_UNPACK_CODE, TRIPLE, TWO_D,
     TWO_D_PACK_CODE, TWO_D_UNPACK_CODE, WKB_MULTI_POINT_M_PRE,
     WKB_MULTI_POINT_PRE, WKB_MULTI_POINT_ZM_PRE, WKB_MULTI_POINT_Z_PRE,
     WKB_POINT_M_PRE, WKB_POINT_PRE, WKB_POINT_ZM_PRE, WKB_POINT_Z_PRE)
 from fudgeo.geometry.base import AbstractGeometry
 from fudgeo.geometry.util import (
-    EMPTY_ENVELOPE, Envelope, envelope_from_coordinates,
+    EMPTY_ENVELOPE, Envelope, as_array, envelope_from_coordinates,
     envelope_from_coordinates_m, envelope_from_coordinates_z,
     envelope_from_coordinates_zm, lazy_unpack, make_header, pack_coordinates,
     unpack_header, unpack_points)
 
 
+if TYPE_CHECKING:
+    from numpy import ndarray
+
+
 class Point(AbstractGeometry):
     """
     Point
     """
     __slots__ = 'x', 'y'
 
     def __init__(self, *, x: float, y: float, srs_id: int) -> None:
@@ -53,19 +57,19 @@
         """
         Is Empty
         """
         return isnan(self.x) and isnan(self.y)
     # End is_empty property
 
     @staticmethod
-    def _unpack(value: bytes) -> DOUBLE:
+    def _unpack(view: memoryview) -> DOUBLE:
         """
         Unpack Values
         """
-        *_, x, y = unpack(TWO_D_UNPACK_CODE, value)
+        *_, x, y = unpack(TWO_D_UNPACK_CODE, view)
         return x, y
     # End _unpack method
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -81,27 +85,28 @@
         return EMPTY_ENVELOPE
     # End envelope property
 
     def to_gpkg(self) -> bytes:
         """
         To Geopackage
         """
-        return (make_header(srs_id=self.srs_id, is_empty=self.is_empty,
-                            envelope_code=0) + self._to_wkb())
+        return (make_header(srs_id=self.srs_id,
+                            is_empty=self.is_empty) + self._to_wkb())
     # End to_gpkg method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'Point':
         """
         From Geopackage
         """
-        srs_id, _, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
+        view = memoryview(value)
+        srs_id, _, offset, is_empty = unpack_header(view[:HEADER_OFFSET])
         if is_empty:
             return cls.empty(srs_id)
-        x, y = cls._unpack(value[offset:])
+        x, y = cls._unpack(view[offset:])
         return cls(x=x, y=y, srs_id=srs_id)
     # End from_gpkg method
 
     @classmethod
     def from_tuple(cls, xy: DOUBLE, srs_id: int) -> 'Point':
         """
         From Tuple
@@ -152,19 +157,19 @@
         """
         Is Empty
         """
         return isnan(self.x) and isnan(self.y) and isnan(self.z)
     # End is_empty property
 
     @staticmethod
-    def _unpack(value: bytes) -> TRIPLE:
+    def _unpack(view: memoryview) -> TRIPLE:
         """
         Unpack Values
         """
-        *_, x, y, z = unpack(THREE_D_UNPACK_CODE, value)
+        *_, x, y, z = unpack(THREE_D_UNPACK_CODE, view)
         return x, y, z
     # End _unpack method
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -180,27 +185,28 @@
         return EMPTY_ENVELOPE
     # End envelope property
 
     def to_gpkg(self) -> bytes:
         """
         To Geopackage
         """
-        return (make_header(srs_id=self.srs_id, is_empty=self.is_empty,
-                            envelope_code=0) + self._to_wkb())
+        return (make_header(srs_id=self.srs_id,
+                            is_empty=self.is_empty) + self._to_wkb())
     # End to_gpkg method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PointZ':
         """
         From Geopackage
         """
-        srs_id, _, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
+        view = memoryview(value)
+        srs_id, _, offset, is_empty = unpack_header(view[:HEADER_OFFSET])
         if is_empty:
             return cls.empty(srs_id)
-        x, y, z = cls._unpack(value[offset:])
+        x, y, z = cls._unpack(view[offset:])
         return cls(x=x, y=y, z=z, srs_id=srs_id)
     # End from_gpkg method
 
     @classmethod
     def from_tuple(cls, xyz: TRIPLE, srs_id: int) -> 'PointZ':
         """
         From Tuple
@@ -251,19 +257,19 @@
         """
         Is Empty
         """
         return isnan(self.x) and isnan(self.y) and isnan(self.m)
     # End is_empty property
 
     @staticmethod
-    def _unpack(value: bytes) -> TRIPLE:
+    def _unpack(view: memoryview) -> TRIPLE:
         """
         Unpack Values
         """
-        *_, x, y, m = unpack(THREE_D_UNPACK_CODE, value)
+        *_, x, y, m = unpack(THREE_D_UNPACK_CODE, view)
         return x, y, m
     # End _unpack method
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -279,27 +285,28 @@
         return EMPTY_ENVELOPE
     # End envelope property
 
     def to_gpkg(self) -> bytes:
         """
         To Geopackage
         """
-        return (make_header(srs_id=self.srs_id, is_empty=self.is_empty,
-                            envelope_code=0) + self._to_wkb())
+        return (make_header(srs_id=self.srs_id,
+                            is_empty=self.is_empty) + self._to_wkb())
     # End to_gpkg method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PointM':
         """
         From Geopackage
         """
-        srs_id, _, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
+        view = memoryview(value)
+        srs_id, _, offset, is_empty = unpack_header(view[:HEADER_OFFSET])
         if is_empty:
             return cls.empty(srs_id)
-        x, y, m = cls._unpack(value[offset:])
+        x, y, m = cls._unpack(view[offset:])
         return cls(x=x, y=y, m=m, srs_id=srs_id)
     # End from_gpkg method
 
     @classmethod
     def from_tuple(cls, xym: TRIPLE, srs_id: int) -> 'PointM':
         """
         From Tuple
@@ -354,19 +361,19 @@
         Is Empty
         """
         return (isnan(self.x) and isnan(self.y) and
                 isnan(self.z) and isnan(self.m))
     # End is_empty property
 
     @staticmethod
-    def _unpack(value: bytes) -> QUADRUPLE:
+    def _unpack(view: memoryview) -> QUADRUPLE:
         """
         Unpack Values
         """
-        *_, x, y, z, m = unpack(FOUR_D_UNPACK_CODE, value)
+        *_, x, y, z, m = unpack(FOUR_D_UNPACK_CODE, view)
         return x, y, z, m
     # End _unpack method
 
     def _to_wkb(self, use_prefix: bool = True) -> bytes:
         """
         To WKB
         """
@@ -382,27 +389,28 @@
         return EMPTY_ENVELOPE
     # End envelope property
 
     def to_gpkg(self) -> bytes:
         """
         To Geopackage
         """
-        return (make_header(srs_id=self.srs_id, is_empty=self.is_empty,
-                            envelope_code=0) + self._to_wkb())
+        return (make_header(srs_id=self.srs_id,
+                            is_empty=self.is_empty) + self._to_wkb())
     # End to_gpkg method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PointZM':
         """
         From Geopackage
         """
-        srs_id, _, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
+        view = memoryview(value)
+        srs_id, _, offset, is_empty = unpack_header(view[:HEADER_OFFSET])
         if is_empty:
             return cls.empty(srs_id)
-        x, y, z, m = cls._unpack(value[offset:])
+        x, y, z, m = cls._unpack(view[offset:])
         return cls(x=x, y=y, z=z, m=m, srs_id=srs_id)
     # End from_gpkg method
 
     @classmethod
     def from_tuple(cls, xyzm: QUADRUPLE, srs_id: int) -> 'PointZM':
         """
         From Tuple
@@ -428,30 +436,30 @@
     __slots__ = '_coordinates',
 
     def __init__(self, coordinates: List[DOUBLE], srs_id: int) -> None:
         """
         Initialize the MultiPoint class
         """
         super().__init__(srs_id=srs_id)
-        self._coordinates: List[DOUBLE] = coordinates
+        self._coordinates: 'ndarray' = as_array(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'MultiPoint') -> bool:
         """
         Equals
         """
         if not isinstance(other, MultiPoint):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
-    def coordinates(self) -> List[DOUBLE]:
+    def coordinates(self) -> 'ndarray':
         """
         Coordinates
         """
         if self._args:
             self._coordinates = unpack_points(*self._args)
             self._args = None
         # noinspection PyTypeChecker
@@ -483,20 +491,20 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
-        return WKB_MULTI_POINT_PRE + pack_coordinates(
-            self.coordinates, use_prefix=True)
+        return pack_coordinates(
+            WKB_MULTI_POINT_PRE, self.coordinates, use_point_prefix=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPoint':
         """
         From Geopackage
         """
@@ -512,30 +520,30 @@
     __slots__ = '_coordinates',
 
     def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
         """
         Initialize the MultiPointZ class
         """
         super().__init__(srs_id=srs_id)
-        self._coordinates: List[TRIPLE] = coordinates
+        self._coordinates: 'ndarray' = as_array(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'MultiPointZ') -> bool:
         """
         Equals
         """
         if not isinstance(other, MultiPointZ):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
-    def coordinates(self) -> List[TRIPLE]:
+    def coordinates(self) -> 'ndarray':
         """
         Coordinates
         """
         if self._args:
             self._coordinates = unpack_points(*self._args)
             self._args = None
         # noinspection PyTypeChecker
@@ -568,20 +576,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates_z(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
-        return WKB_MULTI_POINT_Z_PRE + pack_coordinates(
-            self.coordinates, has_z=True, use_prefix=True)
+        return pack_coordinates(
+            WKB_MULTI_POINT_Z_PRE, self.coordinates,
+            has_z=True, use_point_prefix=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPointZ':
         """
         From Geopackage
         """
@@ -597,30 +606,30 @@
     __slots__ = '_coordinates',
 
     def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
         """
         Initialize the MultiPointM class
         """
         super().__init__(srs_id=srs_id)
-        self._coordinates: List[TRIPLE] = coordinates
+        self._coordinates: 'ndarray' = as_array(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'MultiPointM') -> bool:
         """
         Equals
         """
         if not isinstance(other, MultiPointM):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
-    def coordinates(self) -> List[TRIPLE]:
+    def coordinates(self) -> 'ndarray':
         """
         Coordinates
         """
         if self._args:
             self._coordinates = unpack_points(*self._args)
             self._args = None
         # noinspection PyTypeChecker
@@ -653,20 +662,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates_m(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
-        return WKB_MULTI_POINT_M_PRE + pack_coordinates(
-            self.coordinates, has_m=True, use_prefix=True)
+        return pack_coordinates(
+            WKB_MULTI_POINT_M_PRE, self.coordinates,
+            has_m=True, use_point_prefix=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPointM':
         """
         From Geopackage
         """
@@ -682,30 +692,30 @@
     __slots__ = '_coordinates',
 
     def __init__(self, coordinates: List[QUADRUPLE], srs_id: int) -> None:
         """
         Initialize the MultiPointZM class
         """
         super().__init__(srs_id=srs_id)
-        self._coordinates: List[QUADRUPLE] = coordinates
+        self._coordinates: 'ndarray' = as_array(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'MultiPointZM') -> bool:
         """
         Equals
         """
         if not isinstance(other, MultiPointZM):  # pragma: nocover
             return NotImplemented
         if self.srs_id != other.srs_id:
             return False
         return self.points == other.points
     # End eq built-in
 
     @property
-    def coordinates(self) -> List[QUADRUPLE]:
+    def coordinates(self) -> 'ndarray':
         """
         Coordinates
         """
         if self._args:
             self._coordinates = unpack_points(*self._args)
             self._args = None
         # noinspection PyTypeChecker
@@ -738,20 +748,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates_zm(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
-        return WKB_MULTI_POINT_ZM_PRE + pack_coordinates(
-            self.coordinates, has_z=True, has_m=True, use_prefix=True)
+        return pack_coordinates(
+            WKB_MULTI_POINT_ZM_PRE, self.coordinates,
+            has_z=True, has_m=True, use_point_prefix=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPointZM':
         """
         From Geopackage
         """
```

## fudgeo/geometry/polygon.py

```diff
@@ -1,44 +1,48 @@
 # -*- coding: utf-8 -*-
 """
 Polygons
 """
 
 
 from struct import pack
-from typing import List
+from typing import List, TYPE_CHECKING
 
 from fudgeo.constant import (
-    COUNT_CODE, DOUBLE, FOUR_D, QUADRUPLE, THREE_D, TRIPLE, TWO_D,
+    COUNT_CODE, DOUBLE, EMPTY, FOUR_D, QUADRUPLE, THREE_D, TRIPLE, TWO_D,
     WKB_MULTI_POLYGON_M_PRE, WKB_MULTI_POLYGON_PRE, WKB_MULTI_POLYGON_ZM_PRE,
     WKB_MULTI_POLYGON_Z_PRE, WKB_POLYGON_M_PRE, WKB_POLYGON_PRE,
     WKB_POLYGON_ZM_PRE, WKB_POLYGON_Z_PRE)
 from fudgeo.geometry.base import AbstractGeometry
 from fudgeo.geometry.point import Point, PointM, PointZ, PointZM
 from fudgeo.geometry.util import (
-    EMPTY_ENVELOPE, Envelope, envelope_from_coordinates,
+    EMPTY_ENVELOPE, Envelope, as_array, envelope_from_coordinates,
     envelope_from_coordinates_m, envelope_from_coordinates_z,
     envelope_from_coordinates_zm, envelope_from_geometries,
     envelope_from_geometries_m, envelope_from_geometries_z,
     envelope_from_geometries_zm, lazy_unpack, pack_coordinates, unpack_lines,
     unpack_polygons)
 
 
+if TYPE_CHECKING:
+    from numpy import ndarray
+
+
 class LinearRing(AbstractGeometry):
     """
     Linear Ring
     """
     __slots__ = 'coordinates',
 
     def __init__(self, coordinates: List[DOUBLE], srs_id: int) -> None:
         """
         Initialize the LinearRing class
         """
         super().__init__(srs_id=srs_id)
-        self.coordinates: List[DOUBLE] = coordinates
+        self.coordinates: 'ndarray' = as_array(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'LinearRing') -> bool:
         """
         Equals
         """
         if not isinstance(other, LinearRing):  # pragma: nocover
@@ -73,19 +77,19 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
-        return pack_coordinates(self.coordinates)
+        return pack_coordinates(EMPTY, self.coordinates)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LinearRing':  # pragma: nocover
         """
         From Geopackage, no-op for Linear Ring
         """
@@ -101,15 +105,15 @@
     __slots__ = 'coordinates',
 
     def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
         """
         Initialize the LinearRingZ class
         """
         super().__init__(srs_id=srs_id)
-        self.coordinates: List[TRIPLE] = coordinates
+        self.coordinates: 'ndarray' = as_array(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'LinearRingZ') -> bool:
         """
         Equals
         """
         if not isinstance(other, LinearRingZ):  # pragma: nocover
@@ -133,19 +137,19 @@
         Points
         """
         srs_id = self.srs_id
         return [PointZ(x=x, y=y, z=z, srs_id=srs_id)
                 for x, y, z in self.coordinates]
     # End points property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
-        return pack_coordinates(self.coordinates, has_z=True)
+        return pack_coordinates(EMPTY, self.coordinates, has_z=True)
     # End _to_wkb method
 
     @property
     def envelope(self) -> Envelope:
         """
         Envelope
         """
@@ -173,15 +177,15 @@
     __slots__ = 'coordinates',
 
     def __init__(self, coordinates: List[TRIPLE], srs_id: int) -> None:
         """
         Initialize the LinearRingM class
         """
         super().__init__(srs_id=srs_id)
-        self.coordinates: List[TRIPLE] = coordinates
+        self.coordinates: 'ndarray' = as_array(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'LinearRingM') -> bool:
         """
         Equals
         """
         if not isinstance(other, LinearRingM):  # pragma: nocover
@@ -217,19 +221,19 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates_m(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
-        return pack_coordinates(self.coordinates, has_m=True)
+        return pack_coordinates(EMPTY, self.coordinates, has_m=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LinearRingM':  # pragma: nocover
         """
         From Geopackage, no-op for Linear Ring
         """
@@ -245,15 +249,15 @@
     __slots__ = 'coordinates',
 
     def __init__(self, coordinates: List[QUADRUPLE], srs_id: int) -> None:
         """
         Initialize the LinearRingZM class
         """
         super().__init__(srs_id=srs_id)
-        self.coordinates: List[QUADRUPLE] = coordinates
+        self.coordinates: 'ndarray' = as_array(coordinates)
     # End init built-in
 
     def __eq__(self, other: 'LinearRingZM') -> bool:
         """
         Equals
         """
         if not isinstance(other, LinearRingZM):  # pragma: nocover
@@ -287,19 +291,19 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_coordinates_zm(self.coordinates)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
-        return pack_coordinates(self.coordinates, has_z=True, has_m=True)
+        return pack_coordinates(EMPTY, self.coordinates, has_z=True, has_m=True)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'LinearRingZM':  # pragma: nocover
         """
         From Geopackage, no-op for Linear Ring
         """
@@ -370,21 +374,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries(self.rings)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
         geoms = self.rings
-        return (WKB_POLYGON_PRE + pack(COUNT_CODE, len(geoms)) +
-                self._join_geometries(geoms))
+        prefix = WKB_POLYGON_PRE + pack(COUNT_CODE, len(geoms))
+        return self._join_geometries(prefix, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'Polygon':
         """
         From Geopackage
         """
@@ -455,21 +459,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_z(self.rings)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
         geoms = self.rings
-        return (WKB_POLYGON_Z_PRE + pack(COUNT_CODE, len(geoms)) +
-                self._join_geometries(geoms))
+        prefix = WKB_POLYGON_Z_PRE + pack(COUNT_CODE, len(geoms))
+        return self._join_geometries(prefix, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PolygonZ':
         """
         From Geopackage
         """
@@ -540,21 +544,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_m(self.rings)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
         geoms = self.rings
-        return (WKB_POLYGON_M_PRE + pack(COUNT_CODE, len(geoms)) +
-                self._join_geometries(geoms))
+        prefix = WKB_POLYGON_M_PRE + pack(COUNT_CODE, len(geoms))
+        return self._join_geometries(prefix, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PolygonM':
         """
         From Geopackage
         """
@@ -626,21 +630,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_zm(self.rings)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
         geoms = self.rings
-        return (WKB_POLYGON_ZM_PRE + pack(COUNT_CODE, len(geoms)) +
-                self._join_geometries(geoms))
+        prefix = WKB_POLYGON_ZM_PRE + pack(COUNT_CODE, len(geoms))
+        return self._join_geometries(prefix, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'PolygonZM':
         """
         From Geopackage
         """
@@ -712,21 +716,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries(self.polygons)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
         geoms = self.polygons
-        return (WKB_MULTI_POLYGON_PRE + pack(COUNT_CODE, len(geoms)) +
-                self._join_geometries(geoms))
+        prefix = WKB_MULTI_POLYGON_PRE + pack(COUNT_CODE, len(geoms))
+        return self._join_geometries(prefix, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPolygon':
         """
         From Geopackage
         """
@@ -798,21 +802,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_z(self.polygons)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
         geoms = self.polygons
-        return (WKB_MULTI_POLYGON_Z_PRE + pack(COUNT_CODE, len(geoms)) +
-                self._join_geometries(geoms))
+        prefix = WKB_MULTI_POLYGON_Z_PRE + pack(COUNT_CODE, len(geoms))
+        return self._join_geometries(prefix, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPolygonZ':
         """
         From Geopackage
         """
@@ -884,21 +888,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_m(self.polygons)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
         geoms = self.polygons
-        return (WKB_MULTI_POLYGON_M_PRE + pack(COUNT_CODE, len(geoms)) +
-                self._join_geometries(geoms))
+        prefix = WKB_MULTI_POLYGON_M_PRE + pack(COUNT_CODE, len(geoms))
+        return self._join_geometries(prefix, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPolygonM':
         """
         From Geopackage
         """
@@ -970,21 +974,21 @@
         if self._env is not EMPTY_ENVELOPE:
             return self._env
         env = envelope_from_geometries_zm(self.polygons)
         self._env = env
         return env
     # End envelope property
 
-    def _to_wkb(self, use_prefix: bool = True) -> bytes:
+    def _to_wkb(self, use_prefix: bool = True) -> bytearray:
         """
         To WKB
         """
         geoms = self.polygons
-        return (WKB_MULTI_POLYGON_ZM_PRE + pack(COUNT_CODE, len(geoms)) +
-                self._join_geometries(geoms))
+        prefix = WKB_MULTI_POLYGON_ZM_PRE + pack(COUNT_CODE, len(geoms))
+        return self._join_geometries(prefix, geoms)
     # End _to_wkb method
 
     @classmethod
     def from_gpkg(cls, value: bytes) -> 'MultiPolygonZM':
         """
         From Geopackage
         """
```

## fudgeo/geometry/util.py

```diff
@@ -1,24 +1,25 @@
 # -*- coding: utf-8 -*-
 """
 Utility Functions
 """
 
 
-from functools import lru_cache, reduce
-from math import isfinite, nan
-from operator import add
+from functools import lru_cache
+from math import nan
 # noinspection PyPep8Naming
 from struct import error as StructError, pack, unpack
 from typing import Any, List, TYPE_CHECKING, Tuple, Union
 
+from numpy import array, frombuffer, ndarray
+from bottleneck import nanmax, nanmin
+
 from fudgeo.constant import (
-    COORDINATES, COUNT_CODE, DOUBLE, EMPTY, ENVELOPE_COUNT, ENVELOPE_OFFSET,
-    GP_MAGIC, HEADER_CODE, HEADER_OFFSET, POINT_PREFIX, QUADRUPLE, TRIPLE,
-    TWO_D)
+    COUNT_CODE, EMPTY, ENVELOPE_COUNT, ENVELOPE_OFFSET, GP_MAGIC, HEADER_CODE,
+    HEADER_OFFSET, POINT_PREFIX)
 
 
 if TYPE_CHECKING:  # pragma: no cover
     # noinspection PyUnresolvedReferences
     from fudgeo.geometry.linestring import (
         LineString, LineStringZ, LineStringM, LineStringZM)
     # noinspection PyUnresolvedReferences
@@ -27,15 +28,24 @@
         Polygon, PolygonZ, PolygonM, PolygonZM)
 
 
 GEOMS = Union[List['LineString'], List['LinearRing'], List['Polygon']]
 GEOMS_Z = Union[List['LineStringZ'], List['LinearRingZ'], List['PolygonZ']]
 GEOMS_M = Union[List['LineStringM'], List['LinearRingM'], List['PolygonM']]
 GEOMS_ZM = Union[List['LineStringZM'], List['LinearRingZM'], List['PolygonZM']]
-VALUES = List[float]
+
+
+def as_array(coordinates: Any) -> ndarray:
+    """
+    Convert input coordinates to an array
+    """
+    if not isinstance(coordinates, ndarray):
+        coordinates = array(coordinates, dtype=float)
+    return coordinates
+# End as_array function
 
 
 class Envelope:
     """
     Envelope
     """
     __slots__ = ['_code', '_min_x', '_max_x', '_min_y', '_max_y',
@@ -192,120 +202,122 @@
 EMPTY_ENVELOPE = Envelope(code=0, min_x=nan, max_x=nan, min_y=nan, max_y=nan)
 
 
 def lazy_unpack(cls: Any, value: bytes, dimension: int) -> Any:
     """
     Unpack just the header and envelope, adding data to class for later use.
     """
-    srs_id, env_code, offset, is_empty = unpack_header(value[:HEADER_OFFSET])
+    view = memoryview(value)
+    srs_id, env_code, offset, is_empty = unpack_header(view[:HEADER_OFFSET])
     obj = cls([], srs_id=srs_id)
     if is_empty:
         return obj
-    obj._env = unpack_envelope(code=env_code, value=value[:offset])
-    obj._args = value[offset:], dimension
+    obj._env = unpack_envelope(code=env_code, view=view[:offset])
+    obj._args = view[offset:], dimension
     return obj
 # End lazy_unpack function
 
 
-def unpack_line(value: bytes, dimension: int,
+def unpack_line(view: memoryview, dimension: int,
                 is_ring: bool = False) -> List[Tuple[float, ...]]:
     """
     Unpack Values for LineString
     """
-    count, data = get_count_and_data(value, is_ring=is_ring)
-    total = dimension * count
-    values: Tuple[float, ...] = unpack(f'<{total}d', data)
-    return [values[i:i + dimension] for i in range(0, total, dimension)]
+    count, data = get_count_and_data(view, is_ring=is_ring)
+    return frombuffer(
+        data, dtype=float, count=dimension * count).reshape(-1, dimension)
 # End unpack_line function
 
 
-def unpack_points(value: bytes, dimension: int) -> List[Tuple[float, ...]]:
+def unpack_points(view: memoryview, dimension: int) -> ndarray:
     """
     Unpack Values for Multi Point
     """
     offset = 5
     size = (8 * dimension) + offset
-    count, data = get_count_and_data(value)
+    count, data = get_count_and_data(view)
     if not count:
-        return []
-    total = dimension * count
-    data = [data[i + offset:i + size] for i in range(0, len(data), size)]
-    values: Tuple[float, ...] = unpack(f'<{total}d', reduce(add, data))
-    return [values[i:i + dimension] for i in range(0, total, dimension)]
+        return array([], dtype=float)
+    ary = bytearray()
+    for i in range(0, len(data), size):
+        ary.extend(data[i + offset:i + size])
+    return frombuffer(
+        ary, dtype=float, count=dimension * count).reshape(-1, dimension)
 # End unpack_points function
 
 
-def pack_coordinates(coordinates: COORDINATES, has_z: bool = False,
-                     has_m: bool = False, use_prefix: bool = False) -> bytes:
+def pack_coordinates(prefix: bytes, coordinates: ndarray,
+                     has_z: bool = False, has_m: bool = False,
+                     use_point_prefix: bool = False) -> bytearray:
     """
     Pack Coordinates
     """
-    flat = []
-    for coords in coordinates:
-        flat.extend(coords)
     count = len(coordinates)
-    total = count * sum((TWO_D, has_z, has_m))
-    data = pack(f'<{total}d', *flat)
-    if not use_prefix:
-        return pack(COUNT_CODE, count) + data
+    ary = bytearray(prefix + pack(COUNT_CODE, count))
+    data = coordinates.tobytes()
+    if not use_point_prefix:
+        ary.extend(data)
+        return ary
     length = len(data)
+    view = memoryview(data)
     step = length // count
     prefix = POINT_PREFIX.get((has_z, has_m))
-    parts = [prefix + data[i:i + step] for i in range(0, length, step)]
-    return pack(COUNT_CODE, count) + EMPTY.join(parts)
+    for i in range(0, length, step):
+        ary.extend(prefix)
+        ary.extend(view[i:i + step])
+    return ary
 # End pack_coordinates function
 
 
-def unpack_lines(value: bytes, dimension: int, is_ring: bool = False) \
+def unpack_lines(view: memoryview, dimension: int, is_ring: bool = False) \
         -> List[List[Tuple[float, ...]]]:
     """
     Unpack Values for Multi LineString and Polygons
     """
     size, last_end = 8 * dimension, 0
     offset, unit = (4, COUNT_CODE) if is_ring else (9, '<BII')
-    count, data = get_count_and_data(value)
+    count, data = get_count_and_data(view)
     lines = []
     for _ in range(count):
         *_, length = unpack(unit, data[last_end:last_end + offset])
         end = last_end + offset + (size * length)
         # noinspection PyTypeChecker
         points: List[Tuple[float, ...]] = unpack_line(
             data[last_end:end], dimension, is_ring=is_ring)
         last_end = end
         lines.append(points)
     return lines
 # End unpack_lines function
 
 
-def unpack_polygons(value: bytes, dimension: int) \
+def unpack_polygons(view: memoryview, dimension: int) \
         -> List[List[List[Tuple[float, ...]]]]:
     """
     Unpack Values for Multi Polygon Type Containing Polygons
     """
     size, last_end = 8 * dimension, 0
-    count, data = get_count_and_data(value)
+    count, data = get_count_and_data(view)
     polygons = []
     for _ in range(0, count):
         points = unpack_lines(data[last_end:], dimension, is_ring=True)
         point_count = sum(len(x) for x in points)
         last_end += (point_count * size) + (len(points) * 4) + 9
         polygons.append(points)
     return polygons
 # End unpack_polygons method
 
 
-def get_count_and_data(value: bytes, is_ring: bool = False) \
-        -> Tuple[int, bytes]:
+def get_count_and_data(view: memoryview, is_ring: bool = False) \
+        -> Tuple[int, memoryview]:
     """
     Get Count from header and return the value portion of the stream
     """
     first, second = (0, 4) if is_ring else (5, 9)
-    header, data = value[first: second], value[second:]
-    count, = unpack(COUNT_CODE, header)
-    return count, data
+    count, = unpack(COUNT_CODE, view[first: second])
+    return count, view[second:]
 # End get_count_and_data function
 
 
 @lru_cache(maxsize=None)
 def make_header(srs_id: int, is_empty: bool, envelope_code: int = 0) -> bytes:
     """
     Cached Creation of a GeoPackage Geometry Header
@@ -316,26 +328,26 @@
         envelope_code = 0
     flags |= (envelope_code << 1)
     return pack(HEADER_CODE, GP_MAGIC, 0, flags, srs_id)
 # End make_header function
 
 
 @lru_cache(maxsize=None)
-def unpack_header(value: bytes) -> Tuple[int, int, int, bool]:
+def unpack_header(view: memoryview) -> Tuple[int, int, int, bool]:
     """
     Cached Unpacking of a GeoPackage Geometry Header
     """
-    _, _, flags, srs_id = unpack(HEADER_CODE, value)
+    _, _, flags, srs_id = unpack(HEADER_CODE, view)
     envelope_code = (flags & (0x07 << 1)) >> 1
     is_empty = bool((flags & (0x01 << 4)) >> 4)
     return srs_id, envelope_code, ENVELOPE_OFFSET[envelope_code], is_empty
 # End unpack_header function
 
 
-def unpack_envelope(code: int, value: bytes) -> Envelope:
+def unpack_envelope(code: int, view: memoryview) -> Envelope:
     """
     Unpack Envelope
 
     From Geopackage spec (v1.3.1)
     0: no envelope (space saving slower indexing option), 0 bytes
     1: envelope is [minx, maxx, miny, maxy], 32 bytes
     2: envelope is [minx, maxx, miny, maxy, minz, maxz], 48 bytes
@@ -343,15 +355,15 @@
     4: envelope is [minx, maxx, miny, maxy, minz, maxz, minm, maxm], 64 bytes
     """
     if not code:
         return EMPTY_ENVELOPE
     if code not in ENVELOPE_COUNT:  # pragma: no cover
         return EMPTY_ENVELOPE
     try:
-        values = unpack(f'<{ENVELOPE_COUNT[code]}d', value[HEADER_OFFSET:])
+        values = unpack(f'<{ENVELOPE_COUNT[code]}d', view[HEADER_OFFSET:])
     except StructError:  # pragma: no cover
         return EMPTY_ENVELOPE
     min_x = max_x = min_y = max_y = min_z = max_z = min_m = max_m = nan
     if code == 1:
         min_x, max_x, min_y, max_y = values
     elif code == 2:
         min_x, max_x, min_y, max_y, min_z, max_z = values
@@ -361,40 +373,26 @@
         min_x, max_x, min_y, max_y, min_z, max_z, min_m, max_m = values
     return Envelope(
         code=code, min_x=min_x, max_x=max_x, min_y=min_y, max_y=max_y,
         min_z=min_z, max_z=max_z, min_m=min_m, max_m=max_m)
 # End unpack_envelope function
 
 
-def _min_max(values: Union[VALUES, Tuple[float, ...]]) \
-        -> Tuple[float, float]:
-    """
-    Min and Max values, returns nan's if empty list or no finite values.
-    """
-    if not len(values):
-        return nan, nan
-    values = [v for v in values if isfinite(v)]
-    if not values:
-        return nan, nan
-    return min(values), max(values)
-# End _min_max function
-
-
 def envelope_from_geometries(geoms: GEOMS) -> Envelope:
     """
     Envelope from Geometries
     """
     if not geoms:
         return EMPTY_ENVELOPE
     xs, ys = [], []
     for geom in geoms:
         env = geom.envelope
         xs.extend((env.min_x, env.max_x))
         ys.extend((env.min_y, env.max_y))
-    return _envelope_xy(xs=xs, ys=ys)
+    return _envelope_xy(xs=array(xs, dtype=float), ys=array(ys, dtype=float))
 # End envelope_from_geometries function
 
 
 def envelope_from_geometries_z(geoms: GEOMS_Z) -> Envelope:
     """
     Envelope from Geometries with Z
     """
@@ -402,15 +400,17 @@
         return EMPTY_ENVELOPE
     xs, ys, zs = [], [], []
     for geom in geoms:
         env = geom.envelope
         xs.extend((env.min_x, env.max_x))
         ys.extend((env.min_y, env.max_y))
         zs.extend((env.min_z, env.max_z))
-    return _envelope_xyz(xs=xs, ys=ys, zs=zs)
+    return _envelope_xyz(
+        xs=array(xs, dtype=float), ys=array(ys, dtype=float),
+        zs=array(zs, dtype=float))
 # End envelope_from_geometries_z function
 
 
 def envelope_from_geometries_m(geoms: GEOMS_M) -> Envelope:
     """
     Envelope from Geometries with M
     """
@@ -418,15 +418,17 @@
         return EMPTY_ENVELOPE
     xs, ys, ms = [], [], []
     for geom in geoms:
         env = geom.envelope
         xs.extend((env.min_x, env.max_x))
         ys.extend((env.min_y, env.max_y))
         ms.extend((env.min_m, env.max_m))
-    return _envelope_xym(xs=xs, ys=ys, ms=ms)
+    return _envelope_xym(
+        xs=array(xs, dtype=float), ys=array(ys, dtype=float),
+        ms=array(ms, dtype=float))
 # End envelope_from_geometries_m function
 
 
 def envelope_from_geometries_zm(geoms: GEOMS_ZM) -> Envelope:
     """
     Envelope from Geometries with ZM
     """
@@ -435,102 +437,109 @@
     xs, ys, zs, ms = [], [], [], []
     for geom in geoms:
         env = geom.envelope
         xs.extend((env.min_x, env.max_x))
         ys.extend((env.min_y, env.max_y))
         zs.extend((env.min_z, env.max_z))
         ms.extend((env.min_m, env.max_m))
-    return _envelope_xyzm(xs=xs, ys=ys, zs=zs, ms=ms)
+    return _envelope_xyzm(
+        xs=array(xs, dtype=float), ys=array(ys, dtype=float),
+        zs=array(zs, dtype=float), ms=array(ms, dtype=float))
 # End envelope_from_geometries_zm function
 
 
-def envelope_from_coordinates(coordinates: List[DOUBLE]) -> Envelope:
+def envelope_from_coordinates(coordinates: ndarray) -> Envelope:
     """
     Envelope from Coordinates
     """
     if not len(coordinates):
         return EMPTY_ENVELOPE
-    return _envelope_xy(*zip(*coordinates))
+    return _envelope_xy(xs=coordinates[:, 0], ys=coordinates[:, 1])
 # End envelope_from_coordinates function
 
 
-def envelope_from_coordinates_z(coordinates: List[TRIPLE]) -> Envelope:
+def envelope_from_coordinates_z(coordinates: ndarray) -> Envelope:
     """
     Envelope from Coordinates with Z
     """
     if not len(coordinates):
         return EMPTY_ENVELOPE
-    return _envelope_xyz(*zip(*coordinates))
+    return _envelope_xyz(
+        xs=coordinates[:, 0], ys=coordinates[:, 1], zs=coordinates[:, 2])
 # End envelope_from_coordinates_z function
 
 
-def envelope_from_coordinates_m(coordinates: List[TRIPLE]) -> Envelope:
+def envelope_from_coordinates_m(coordinates: ndarray) -> Envelope:
     """
     Envelope from Coordinates with M
     """
     if not len(coordinates):
         return EMPTY_ENVELOPE
-    return _envelope_xym(*zip(*coordinates))
+    return _envelope_xym(
+        xs=coordinates[:, 0], ys=coordinates[:, 1], ms=coordinates[:, 2])
 # End envelope_from_coordinates_m function
 
 
-def envelope_from_coordinates_zm(coordinates: List[QUADRUPLE]) -> Envelope:
+def envelope_from_coordinates_zm(coordinates: ndarray) -> Envelope:
     """
     Envelope from Coordinates with ZM
     """
     if not len(coordinates):
         return EMPTY_ENVELOPE
-    return _envelope_xyzm(*zip(*coordinates))
+    return _envelope_xyzm(
+        xs=coordinates[:, 0], ys=coordinates[:, 1],
+        zs=coordinates[:, 2], ms=coordinates[:, 3])
 # End envelope_from_coordinates_zm function
 
 
-def _envelope_xy(xs: VALUES, ys: VALUES) -> Envelope:
+def _envelope_xy(xs: ndarray, ys: ndarray) -> Envelope:
     """
     Envelope XY
     """
-    min_x, max_x = _min_max(xs)
-    min_y, max_y = _min_max(ys)
+    min_x, max_x = nanmin(xs), nanmax(xs)
+    min_y, max_y = nanmin(ys), nanmax(ys)
     return Envelope(code=1, min_x=min_x, max_x=max_x, min_y=min_y, max_y=max_y)
 # End _envelope_xy function
 
 
-def _envelope_xyz(xs: VALUES, ys: VALUES, zs: VALUES) -> Envelope:
+def _envelope_xyz(xs: ndarray, ys: ndarray, zs: ndarray) -> Envelope:
     """
     Envelope XYZ
     """
-    min_x, max_x = _min_max(xs)
-    min_y, max_y = _min_max(ys)
-    min_z, max_z = _min_max(zs)
+    min_x, max_x = nanmin(xs), nanmax(xs)
+    min_y, max_y = nanmin(ys), nanmax(ys)
+    min_z, max_z = nanmin(zs), nanmax(zs)
     return Envelope(code=2, min_x=min_x, max_x=max_x,
                     min_y=min_y, max_y=max_y,
                     min_z=min_z, max_z=max_z)
 # End _envelope_xyz function
 
 
-def _envelope_xym(xs: VALUES, ys: VALUES, ms: VALUES) -> Envelope:
+def _envelope_xym(xs: ndarray, ys: ndarray, ms: ndarray) -> Envelope:
     """
     Envelope XYM
     """
-    min_x, max_x = _min_max(xs)
-    min_y, max_y = _min_max(ys)
-    min_m, max_m = _min_max(ms)
+    min_x, max_x = nanmin(xs), nanmax(xs)
+    min_y, max_y = nanmin(ys), nanmax(ys)
+    min_m, max_m = nanmin(ms), nanmax(ms)
     return Envelope(code=3, min_x=min_x, max_x=max_x,
                     min_y=min_y, max_y=max_y,
                     min_m=min_m, max_m=max_m)
 # End _envelope_xym function
 
 
-def _envelope_xyzm(xs: VALUES, ys: VALUES, zs: VALUES, ms: VALUES) -> Envelope:
+def _envelope_xyzm(xs: ndarray, ys: ndarray,
+                   zs: ndarray, ms: ndarray) -> Envelope:
     """
     Envelope XYZM
     """
-    min_x, max_x = _min_max(xs)
-    min_y, max_y = _min_max(ys)
-    min_z, max_z = _min_max(zs)
-    min_m, max_m = _min_max(ms)
+    min_x, max_x = nanmin(xs), nanmax(xs)
+    min_y, max_y = nanmin(ys), nanmax(ys)
+    min_z, max_z = nanmin(zs), nanmax(zs)
+    min_m, max_m = nanmin(ms), nanmax(ms)
     return Envelope(
         code=4, min_x=min_x, max_x=max_x, min_y=min_y, max_y=max_y,
         min_z=min_z, max_z=max_z, min_m=min_m, max_m=max_m)
 # End _envelope_xyzm function
 
 
 if __name__ == '__main__':  # pragma: no cover
```

## Comparing `fudgeo-0.4.2.dist-info/LICENSE` & `fudgeo-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fudgeo-0.4.2.dist-info/RECORD` & `fudgeo-0.5.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-fudgeo/__init__.py,sha256=cfn0YWn5FEj8wmuqGYdPLxgfr48nxgwhRxVRhoq4R-4,117
+fudgeo/__init__.py,sha256=KozCNcZLFxSNF54wJ5akYLIN25MjKT2XuCIb6-JwA-Q,117
 fudgeo/constant.py,sha256=-fE2Lyobm43rnDNzxsLUhaCfMMlaO5cCUmOFEL05LCQ,2538
 fudgeo/enumeration.py,sha256=NvgtVBYxfULGVIks-J0rFLRxvGrtU2DM1bjZB0HxZRU,1157
 fudgeo/geopkg.py,sha256=LL5uO82kL5CgTlIdxbr_2hiUf-kqDVXdtz8vDASXj_g,20081
 fudgeo/geopkg.sql,sha256=Tt0Fi4w-ySR7tDUJsPt-5mA_Sw2oUs8co5rFGEleS24,2673
 fudgeo/sql.py,sha256=AJcNZAjvGHvmc88NCU1TTsfjJ0tVZ6muTyNzA8yZcW0,7768
 fudgeo/geometry/__init__.py,sha256=N4sf5FJB13JoNxB_GyyO9ohXbtKoSoVvbKTnltMXq-0,974
-fudgeo/geometry/base.py,sha256=hON9Oft3X-8uOkqiFV7s74ZIgDKORmWkZkQjiY2d21o,2000
-fudgeo/geometry/linestring.py,sha256=2zN-nYmZ0vSEUmGnp5JhKjFCuXMjvmaZEoFSiKWEZK4,18653
-fudgeo/geometry/point.py,sha256=t32pw6nY9xJZCupzuETgywu2MDVhy-Wkc8b0YKfT1CM,19794
-fudgeo/geometry/polygon.py,sha256=8fZjh19hCjyakvk8Bt7SgbKO6I2n8Ldyft4FEczVHJo,26366
-fudgeo/geometry/util.py,sha256=pszHc8-5sKBJLtq7e4aZJhFs61gOfoxU7BK3HWI29kQ,15891
-fudgeo-0.4.2.dist-info/LICENSE,sha256=kg8K68wjqhzaDoPNP6FWgXT2UuLmZbswzv72syix3Gw,1088
-fudgeo-0.4.2.dist-info/METADATA,sha256=9Qk1zxRwRUEv_l6WGVGmUykZ71Tozap-xyOGnGW_8uc,9095
-fudgeo-0.4.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fudgeo-0.4.2.dist-info/top_level.txt,sha256=RlcnukuWGTUINTexweATRDqQgM1d0q2iaOd6B6tBWWI,7
-fudgeo-0.4.2.dist-info/RECORD,,
+fudgeo/geometry/base.py,sha256=MF2b9lCrsbufB-IQrS8aE4p1PcRtyV8n0bxcuN_68jU,2012
+fudgeo/geometry/linestring.py,sha256=3Y0giqvXjjbHeOmSZKEgnivzxq0L8Xiazd8ggcpsXME,18786
+fudgeo/geometry/point.py,sha256=vGryK_D-04JIyLa4vDerLmPhOCUG4iJ1JzQJoxIzX9o,20019
+fudgeo/geometry/polygon.py,sha256=JkR0nHKv21Sjnxs1F7PB3qoTHwWbszPhA4nMkuuyKDs,26589
+fudgeo/geometry/util.py,sha256=9rjxRx4rS_e97N2vibO3l2x_QzT07DKgpmH6X93SEko,16275
+fudgeo-0.5.0.dist-info/LICENSE,sha256=kg8K68wjqhzaDoPNP6FWgXT2UuLmZbswzv72syix3Gw,1088
+fudgeo-0.5.0.dist-info/METADATA,sha256=balGUiS7dG9E1OjRJ74dj6BVYbgtipddDeH1h2n1PCM,12609
+fudgeo-0.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fudgeo-0.5.0.dist-info/top_level.txt,sha256=RlcnukuWGTUINTexweATRDqQgM1d0q2iaOd6B6tBWWI,7
+fudgeo-0.5.0.dist-info/RECORD,,
```

