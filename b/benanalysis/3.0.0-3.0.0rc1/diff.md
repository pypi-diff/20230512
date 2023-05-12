# Comparing `tmp/benanalysis-3.0.0-cp39-cp39-win_amd64.whl.zip` & `tmp/benanalysis-3.0.0rc1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,32 @@
-Zip file size: 1435003 bytes, number of entries: 21
--rw-rw-rw-  2.0 fat      343 b- defN 23-May-12 13:06 benanalysis/__init__.py
--rw-rw-rw-  2.0 fat     7850 b- defN 23-May-12 13:06 benanalysis/__init__.pyi
--rw-rw-rw-  2.0 fat   383488 b- defN 23-May-12 13:33 benanalysis/_benpy_core.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat  2668544 b- defN 23-May-12 13:26 benanalysis/gsl.dll
--rw-rw-rw-  2.0 fat   417792 b- defN 23-May-12 13:26 benanalysis/gslcblas.dll
--rw-rw-rw-  2.0 fat      202 b- defN 23-May-12 13:06 benanalysis/colorimetry/__init__.py
--rw-rw-rw-  2.0 fat     9607 b- defN 23-May-12 13:06 benanalysis/colorimetry/__init__.pyi
--rw-rw-rw-  2.0 fat      195 b- defN 23-May-12 13:06 benanalysis/data/__init__.py
--rw-rw-rw-  2.0 fat      129 b- defN 23-May-12 13:06 benanalysis/data/__init__.pyi
--rw-rw-rw-  2.0 fat      207 b- defN 23-May-12 13:06 benanalysis/data/colorimetry/__init__.py
--rw-rw-rw-  2.0 fat     6734 b- defN 23-May-12 13:06 benanalysis/data/colorimetry/__init__.pyi
--rw-rw-rw-  2.0 fat      204 b- defN 23-May-12 13:06 benanalysis/monochromator/__init__.py
--rw-rw-rw-  2.0 fat      140 b- defN 23-May-12 13:06 benanalysis/monochromator/__init__.pyi
--rw-rw-rw-  2.0 fat       65 b- defN 23-May-12 13:06 benanalysis/monochromator/slit_function/__init__.py
--rw-rw-rw-  2.0 fat      885 b- defN 23-May-12 13:06 benanalysis/monochromator/slit_function/__init__.pyi
--rw-rw-rw-  2.0 fat      257 b- defN 23-May-12 13:06 benanalysis/utils/__init__.py
--rw-rw-rw-  2.0 fat      745 b- defN 23-May-12 13:06 benanalysis/utils/__init__.pyi
--rw-rw-rw-  2.0 fat      753 b- defN 23-May-12 13:33 benanalysis-3.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-12 13:33 benanalysis-3.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-12 13:33 benanalysis-3.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1856 b- defN 23-May-12 13:33 benanalysis-3.0.0.dist-info/RECORD
-21 files, 3500108 bytes uncompressed, 1431941 bytes compressed:  59.1%
+Zip file size: 5020589 bytes, number of entries: 30
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 12:15 benanalysis.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 12:15 benanalysis/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 12:15 benanalysis-3.0.0rc1.dist-info/
+-rwxr-xr-x  2.0 unx  1424553 b- defN 23-May-12 12:15 benanalysis.libs/libgslcblas-9bc550a1.so.0.0.0
+-rwxr-xr-x  2.0 unx 15884169 b- defN 23-May-12 12:15 benanalysis.libs/libgsl-26724a50.so.25.1.0
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 12:15 benanalysis/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 12:15 benanalysis/colorimetry/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 12:15 benanalysis/data/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 12:15 benanalysis/monochromator/
+-rwxr-xr-x  2.0 unx   700953 b- defN 23-May-12 12:15 benanalysis/_benpy_core.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      329 b- defN 23-May-12 12:15 benanalysis/__init__.py
+-rw-r--r--  2.0 unx     7622 b- defN 23-May-12 12:15 benanalysis/__init__.pyi
+-rw-r--r--  2.0 unx      249 b- defN 23-May-12 12:15 benanalysis/utils/__init__.py
+-rw-r--r--  2.0 unx      716 b- defN 23-May-12 12:15 benanalysis/utils/__init__.pyi
+-rw-r--r--  2.0 unx      195 b- defN 23-May-12 12:15 benanalysis/colorimetry/__init__.py
+-rw-r--r--  2.0 unx     9326 b- defN 23-May-12 12:15 benanalysis/colorimetry/__init__.pyi
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 12:15 benanalysis/data/colorimetry/
+-rw-r--r--  2.0 unx      188 b- defN 23-May-12 12:15 benanalysis/data/__init__.py
+-rw-r--r--  2.0 unx      120 b- defN 23-May-12 12:15 benanalysis/data/__init__.pyi
+-rw-r--r--  2.0 unx      200 b- defN 23-May-12 12:15 benanalysis/data/colorimetry/__init__.py
+-rw-r--r--  2.0 unx     6568 b- defN 23-May-12 12:15 benanalysis/data/colorimetry/__init__.pyi
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 12:15 benanalysis/monochromator/slit_function/
+-rw-r--r--  2.0 unx      197 b- defN 23-May-12 12:15 benanalysis/monochromator/__init__.py
+-rw-r--r--  2.0 unx      131 b- defN 23-May-12 12:15 benanalysis/monochromator/__init__.pyi
+-rw-r--r--  2.0 unx       65 b- defN 23-May-12 12:15 benanalysis/monochromator/slit_function/__init__.py
+-rw-r--r--  2.0 unx      862 b- defN 23-May-12 12:15 benanalysis/monochromator/slit_function/__init__.pyi
+-rw-rw-r--  2.0 unx     1949 b- defN 23-May-12 12:15 benanalysis-3.0.0rc1.dist-info/RECORD
+-rw-r--r--  2.0 unx      152 b- defN 23-May-12 12:15 benanalysis-3.0.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-12 12:15 benanalysis-3.0.0rc1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      723 b- defN 23-May-12 12:15 benanalysis-3.0.0rc1.dist-info/METADATA
+30 files, 18039279 bytes uncompressed, 5016275 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -1,64 +1,91 @@
-Filename: benanalysis/__init__.py
+Filename: benanalysis.libs/
 Comment: 
 
-Filename: benanalysis/__init__.pyi
+Filename: benanalysis/
+Comment: 
+
+Filename: benanalysis-3.0.0rc1.dist-info/
+Comment: 
+
+Filename: benanalysis.libs/libgslcblas-9bc550a1.so.0.0.0
+Comment: 
+
+Filename: benanalysis.libs/libgsl-26724a50.so.25.1.0
+Comment: 
+
+Filename: benanalysis/utils/
+Comment: 
+
+Filename: benanalysis/colorimetry/
+Comment: 
+
+Filename: benanalysis/data/
+Comment: 
+
+Filename: benanalysis/monochromator/
+Comment: 
+
+Filename: benanalysis/_benpy_core.cpython-311-x86_64-linux-gnu.so
 Comment: 
 
-Filename: benanalysis/_benpy_core.cp39-win_amd64.pyd
+Filename: benanalysis/__init__.py
 Comment: 
 
-Filename: benanalysis/gsl.dll
+Filename: benanalysis/__init__.pyi
 Comment: 
 
-Filename: benanalysis/gslcblas.dll
+Filename: benanalysis/utils/__init__.py
+Comment: 
+
+Filename: benanalysis/utils/__init__.pyi
 Comment: 
 
 Filename: benanalysis/colorimetry/__init__.py
 Comment: 
 
 Filename: benanalysis/colorimetry/__init__.pyi
 Comment: 
 
+Filename: benanalysis/data/colorimetry/
+Comment: 
+
 Filename: benanalysis/data/__init__.py
 Comment: 
 
 Filename: benanalysis/data/__init__.pyi
 Comment: 
 
 Filename: benanalysis/data/colorimetry/__init__.py
 Comment: 
 
 Filename: benanalysis/data/colorimetry/__init__.pyi
 Comment: 
 
+Filename: benanalysis/monochromator/slit_function/
+Comment: 
+
 Filename: benanalysis/monochromator/__init__.py
 Comment: 
 
 Filename: benanalysis/monochromator/__init__.pyi
 Comment: 
 
 Filename: benanalysis/monochromator/slit_function/__init__.py
 Comment: 
 
 Filename: benanalysis/monochromator/slit_function/__init__.pyi
 Comment: 
 
-Filename: benanalysis/utils/__init__.py
-Comment: 
-
-Filename: benanalysis/utils/__init__.pyi
-Comment: 
-
-Filename: benanalysis-3.0.0.dist-info/METADATA
+Filename: benanalysis-3.0.0rc1.dist-info/RECORD
 Comment: 
 
-Filename: benanalysis-3.0.0.dist-info/WHEEL
+Filename: benanalysis-3.0.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: benanalysis-3.0.0.dist-info/top_level.txt
+Filename: benanalysis-3.0.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: benanalysis-3.0.0.dist-info/RECORD
+Filename: benanalysis-3.0.0rc1.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## benanalysis/__init__.py

 * *Ordering differences only*

```diff
@@ -1,15 +1,15 @@
-#
-# @file __init__.py
-# @author Markus Führer
-# @date 5 May 2023
-# @copyright Copyright © 2023 Bentham Instruments Ltd. All Rights Reserved.
-#
-
-#
-# @file __init__.py
-# @author Markus Führer
-# @date 5 May 2023
-# @copyright Copyright © 2023 Bentham Instruments Ltd. All Rights Reserved.
-#
-
+#
+# @file __init__.py
+# @author Markus Führer
+# @date 5 May 2023
+# @copyright Copyright © 2023 Bentham Instruments Ltd. All Rights Reserved.
+#
+
+#
+# @file __init__.py
+# @author Markus Führer
+# @date 5 May 2023
+# @copyright Copyright © 2023 Bentham Instruments Ltd. All Rights Reserved.
+#
+
 from benanalysis._benpy_core import *
```

## benanalysis/__init__.pyi

 * *Ordering differences only*

```diff
@@ -1,228 +1,228 @@
-"""Bentham Instruments spectral analysis package."""
-from __future__ import annotations
-import benanalysis._benpy_core
-import typing
-
-__all__ = [
-    "Interpolation",
-    "Scan",
-    "colorimetry",
-    "data",
-    "log",
-    "log10",
-    "monochromator",
-    "utils"
-]
-
-
-class Interpolation():
-    """
-    Members:
-
-      NONE
-
-      AKIMA
-
-      CUBIC
-
-      LINEAR
-
-      POLYNOMIAL
-    """
-    def __eq__(self, other: object) -> bool: ...
-    def __getstate__(self) -> int: ...
-    def __hash__(self) -> int: ...
-    def __index__(self) -> int: ...
-    def __init__(self, value: int) -> None: ...
-    def __int__(self) -> int: ...
-    def __ne__(self, other: object) -> bool: ...
-    def __repr__(self) -> str: ...
-    def __setstate__(self, state: int) -> None: ...
-    @property
-    def name(self) -> str:
-        """
-        :type: str
-        """
-    @property
-    def value(self) -> int:
-        """
-        :type: int
-        """
-    AKIMA: benanalysis._benpy_core.Interpolation # value = <Interpolation.AKIMA: 1>
-    CUBIC: benanalysis._benpy_core.Interpolation # value = <Interpolation.CUBIC: 2>
-    LINEAR: benanalysis._benpy_core.Interpolation # value = <Interpolation.LINEAR: 3>
-    NONE: benanalysis._benpy_core.Interpolation # value = <Interpolation.NONE: 0>
-    POLYNOMIAL: benanalysis._benpy_core.Interpolation # value = <Interpolation.POLYNOMIAL: 4>
-    __members__: dict # value = {'NONE': <Interpolation.NONE: 0>, 'AKIMA': <Interpolation.AKIMA: 1>, 'CUBIC': <Interpolation.CUBIC: 2>, 'LINEAR': <Interpolation.LINEAR: 3>, 'POLYNOMIAL': <Interpolation.POLYNOMIAL: 4>}
-    pass
-class Scan():
-    """
-    Class to manipulate spectral data consisting of wavelength and value pairs.
-
-
-    Usage:
-    >>> scan1 = Scan() # create empty scan object
-    >>> scan1 = Scan(epsilon=0.001) # ... with wavelength float comparison epsilon
-    >>> scan1 = Scan(interpolation=SplineType.LINEAR) # ... allowing interpolation
-    >>> scan1[400] = 1.1  # start assigning values to wavelengths
-    >>> print(scan1[400]) # and retrieving them
-    1.1
-    >>> scan2 = benpy.Scan([400,405,410,415,420],[1,2,3,4,5],  # initialise with list or numpy arrays
-    ...   epsilon=0.001, interpolation=benpy.SplineType.AKIMA)
-    >>> scan2(402) # call with one value to interpolate
-    2.4
-    >>> scan2(402,415) # call with one value to integrate
-    35.1
-    >>> scan3 = log10(scan1+1) * scan2  # do complex maths
-    Scan(400→420[5], epsilon=0.001, interpolation=AKIMA)
-    >>> scan3.to_numpy()
-    [[4.00000000e+02 4.05000000e+02 4.10000000e+02 4.15000000e+02
-      4.20000000e+02]
-     [9.06190583e-02 2.27644692e-01 3.62476233e-01 4.88559067e-01
-      6.05519368e-01]]
-    """
-    @typing.overload
-    def __add__(self, arg0: Scan) -> Scan: ...
-    @typing.overload
-    def __add__(self, arg0: float) -> Scan: ...
-    @typing.overload
-    def __call__(self, wavelength: float) -> float: 
-        """
-        Indirect access to the data to allow interpolation. Note does not
-        extrapolate or throw, returns zero if wavelength is out of bounds.
-
-
-
-        The numerical integral result of the interpolated function over
-        the range [wavelength_from, wavelength_to].
-        """
-    @typing.overload
-    def __call__(self, wavelength_from: float, wavelength_to: float) -> float: ...
-    def __eq__(self, arg0: Scan) -> bool: ...
-    def __getitem__(self, arg0: float) -> float: ...
-    @typing.overload
-    def __iadd__(self, arg0: Scan) -> Scan: ...
-    @typing.overload
-    def __iadd__(self, arg0: float) -> Scan: ...
-    @typing.overload
-    def __imul__(self, arg0: Scan) -> Scan: ...
-    @typing.overload
-    def __imul__(self, arg0: float) -> Scan: ...
-    @typing.overload
-    def __init__(self, epsilon: float = 1e-20, interpolation: Interpolation = Interpolation.NONE) -> None: 
-        """
-        Initialise an empty Scan, storing epsilon and interpolation.
-
-        Initialise a scan with lists of wavelength and values, wavelength epsilon, and interpolation type
-        """
-    @typing.overload
-    def __init__(self, wavelength_array: typing.List[float], value_array: typing.List[float], epsilon: float = 1e-20, interpolation: Interpolation = Interpolation.NONE) -> None: ...
-    @typing.overload
-    def __isub__(self, arg0: Scan) -> Scan: ...
-    @typing.overload
-    def __isub__(self, arg0: float) -> Scan: ...
-    def __iter__(self) -> typing.Iterator: ...
-    @typing.overload
-    def __itruediv__(self, arg0: Scan) -> Scan: ...
-    @typing.overload
-    def __itruediv__(self, arg0: float) -> Scan: ...
-    @typing.overload
-    def __mul__(self, arg0: Scan) -> Scan: ...
-    @typing.overload
-    def __mul__(self, arg0: float) -> Scan: ...
-    def __neg__(self) -> Scan: ...
-    @typing.overload
-    def __pow__(self, arg0: Scan) -> Scan: ...
-    @typing.overload
-    def __pow__(self, arg0: float) -> Scan: ...
-    def __radd__(self, arg0: float) -> Scan: ...
-    def __repr__(self) -> str: ...
-    def __rmul__(self, arg0: float) -> Scan: ...
-    def __rpow__(self, arg0: float) -> Scan: ...
-    def __rsub__(self, arg0: float) -> Scan: ...
-    def __rtruediv__(self, arg0: float) -> Scan: ...
-    def __setitem__(self, arg0: float, arg1: float) -> None: ...
-    def __str__(self) -> str: ...
-    @typing.overload
-    def __sub__(self, arg0: Scan) -> Scan: ...
-    @typing.overload
-    def __sub__(self, arg0: float) -> Scan: ...
-    @typing.overload
-    def __truediv__(self, arg0: Scan) -> Scan: ...
-    @typing.overload
-    def __truediv__(self, arg0: float) -> Scan: ...
-    def add(self, wavelength: float, value: float) -> None: 
-        """
-        Add a wavelength, value point to the scan.
-        """
-    def init_spline(self) -> None: 
-        """
-        Initialise the spline with the current interpolation type.
-        """
-    def is_interpolated(self) -> bool: 
-        """
-        Returns whether or not the scan uses interpolation (a SplineType other than NONE).
-        """
-    def items(self) -> typing.Iterator: ...
-    def populate_from_csv(self, file_path: str) -> None: 
-        """
-        Populate from csv (or general char delimited) file.
-        """
-    def to_lists(self) -> typing.List[typing.List[float]]: 
-        """
-        Convert Scan object to a pair of lists
-        """
-    def to_numpy(self) -> numpy.ndarray[numpy.float64]: 
-        """
-        Convert Scan object to a 2D numpy array where index 0 and 1 are arrays of wavelengths and values respectively
-        """
-    def values(self) -> typing.List[float]: 
-        """
-        return the values from the scan object
-        """
-    def wavelengths(self) -> typing.List[float]: 
-        """
-        return the wavelengths from the scan object
-        """
-    @property
-    def epsilon(self) -> float:
-        """
-        :type: float
-        """
-    @epsilon.setter
-    def epsilon(self, arg1: float) -> None:
-        pass
-    @property
-    def interpolation(self) -> Interpolation:
-        """
-        :type: Interpolation
-        """
-    @interpolation.setter
-    def interpolation(self, arg1: Interpolation) -> None:
-        pass
-    __hash__ = None
-    pass
-@typing.overload
-def log(arg0: Scan) -> Scan:
-    """
-    Compute natural logarithm of a scan.
-
-    Compute logarithm base [Scan] of a Scan
-
-    Compute logarithm base [float] of a [Scan]
-
-    Compute logarithm base [Scan] of a [float]
-    """
-@typing.overload
-def log(arg0: Scan, arg1: Scan) -> Scan:
-    pass
-@typing.overload
-def log(arg0: Scan, arg1: float) -> Scan:
-    pass
-@typing.overload
-def log(arg0: float, arg1: Scan) -> Scan:
-    pass
-def log10(arg0: Scan) -> Scan:
-    """
-    Compute logarithm base 10 of a scan.
-    """
+"""Bentham Instruments spectral analysis package."""
+from __future__ import annotations
+import benanalysis._benpy_core
+import typing
+
+__all__ = [
+    "Interpolation",
+    "Scan",
+    "colorimetry",
+    "data",
+    "log",
+    "log10",
+    "monochromator",
+    "utils"
+]
+
+
+class Interpolation():
+    """
+    Members:
+
+      NONE
+
+      AKIMA
+
+      CUBIC
+
+      LINEAR
+
+      POLYNOMIAL
+    """
+    def __eq__(self, other: object) -> bool: ...
+    def __getstate__(self) -> int: ...
+    def __hash__(self) -> int: ...
+    def __index__(self) -> int: ...
+    def __init__(self, value: int) -> None: ...
+    def __int__(self) -> int: ...
+    def __ne__(self, other: object) -> bool: ...
+    def __repr__(self) -> str: ...
+    def __setstate__(self, state: int) -> None: ...
+    @property
+    def name(self) -> str:
+        """
+        :type: str
+        """
+    @property
+    def value(self) -> int:
+        """
+        :type: int
+        """
+    AKIMA: benanalysis._benpy_core.Interpolation # value = <Interpolation.AKIMA: 1>
+    CUBIC: benanalysis._benpy_core.Interpolation # value = <Interpolation.CUBIC: 2>
+    LINEAR: benanalysis._benpy_core.Interpolation # value = <Interpolation.LINEAR: 3>
+    NONE: benanalysis._benpy_core.Interpolation # value = <Interpolation.NONE: 0>
+    POLYNOMIAL: benanalysis._benpy_core.Interpolation # value = <Interpolation.POLYNOMIAL: 4>
+    __members__: dict # value = {'NONE': <Interpolation.NONE: 0>, 'AKIMA': <Interpolation.AKIMA: 1>, 'CUBIC': <Interpolation.CUBIC: 2>, 'LINEAR': <Interpolation.LINEAR: 3>, 'POLYNOMIAL': <Interpolation.POLYNOMIAL: 4>}
+    pass
+class Scan():
+    """
+    Class to manipulate spectral data consisting of wavelength and value pairs.
+
+
+    Usage:
+    >>> scan1 = Scan() # create empty scan object
+    >>> scan1 = Scan(epsilon=0.001) # ... with wavelength float comparison epsilon
+    >>> scan1 = Scan(interpolation=SplineType.LINEAR) # ... allowing interpolation
+    >>> scan1[400] = 1.1  # start assigning values to wavelengths
+    >>> print(scan1[400]) # and retrieving them
+    1.1
+    >>> scan2 = benpy.Scan([400,405,410,415,420],[1,2,3,4,5],  # initialise with list or numpy arrays
+    ...   epsilon=0.001, interpolation=benpy.SplineType.AKIMA)
+    >>> scan2(402) # call with one value to interpolate
+    2.4
+    >>> scan2(402,415) # call with one value to integrate
+    35.1
+    >>> scan3 = log10(scan1+1) * scan2  # do complex maths
+    Scan(400→420[5], epsilon=0.001, interpolation=AKIMA)
+    >>> scan3.to_numpy()
+    [[4.00000000e+02 4.05000000e+02 4.10000000e+02 4.15000000e+02
+      4.20000000e+02]
+     [9.06190583e-02 2.27644692e-01 3.62476233e-01 4.88559067e-01
+      6.05519368e-01]]
+    """
+    @typing.overload
+    def __add__(self, arg0: Scan) -> Scan: ...
+    @typing.overload
+    def __add__(self, arg0: float) -> Scan: ...
+    @typing.overload
+    def __call__(self, wavelength: float) -> float: 
+        """
+        Indirect access to the data to allow interpolation. Note does not
+        extrapolate or throw, returns zero if wavelength is out of bounds.
+
+
+
+        The numerical integral result of the interpolated function over
+        the range [wavelength_from, wavelength_to].
+        """
+    @typing.overload
+    def __call__(self, wavelength_from: float, wavelength_to: float) -> float: ...
+    def __eq__(self, arg0: Scan) -> bool: ...
+    def __getitem__(self, arg0: float) -> float: ...
+    @typing.overload
+    def __iadd__(self, arg0: Scan) -> Scan: ...
+    @typing.overload
+    def __iadd__(self, arg0: float) -> Scan: ...
+    @typing.overload
+    def __imul__(self, arg0: Scan) -> Scan: ...
+    @typing.overload
+    def __imul__(self, arg0: float) -> Scan: ...
+    @typing.overload
+    def __init__(self, epsilon: float = 1e-20, interpolation: Interpolation = Interpolation.NONE) -> None: 
+        """
+        Initialise an empty Scan, storing epsilon and interpolation.
+
+        Initialise a scan with lists of wavelength and values, wavelength epsilon, and interpolation type
+        """
+    @typing.overload
+    def __init__(self, wavelength_array: typing.List[float], value_array: typing.List[float], epsilon: float = 1e-20, interpolation: Interpolation = Interpolation.NONE) -> None: ...
+    @typing.overload
+    def __isub__(self, arg0: Scan) -> Scan: ...
+    @typing.overload
+    def __isub__(self, arg0: float) -> Scan: ...
+    def __iter__(self) -> typing.Iterator: ...
+    @typing.overload
+    def __itruediv__(self, arg0: Scan) -> Scan: ...
+    @typing.overload
+    def __itruediv__(self, arg0: float) -> Scan: ...
+    @typing.overload
+    def __mul__(self, arg0: Scan) -> Scan: ...
+    @typing.overload
+    def __mul__(self, arg0: float) -> Scan: ...
+    def __neg__(self) -> Scan: ...
+    @typing.overload
+    def __pow__(self, arg0: Scan) -> Scan: ...
+    @typing.overload
+    def __pow__(self, arg0: float) -> Scan: ...
+    def __radd__(self, arg0: float) -> Scan: ...
+    def __repr__(self) -> str: ...
+    def __rmul__(self, arg0: float) -> Scan: ...
+    def __rpow__(self, arg0: float) -> Scan: ...
+    def __rsub__(self, arg0: float) -> Scan: ...
+    def __rtruediv__(self, arg0: float) -> Scan: ...
+    def __setitem__(self, arg0: float, arg1: float) -> None: ...
+    def __str__(self) -> str: ...
+    @typing.overload
+    def __sub__(self, arg0: Scan) -> Scan: ...
+    @typing.overload
+    def __sub__(self, arg0: float) -> Scan: ...
+    @typing.overload
+    def __truediv__(self, arg0: Scan) -> Scan: ...
+    @typing.overload
+    def __truediv__(self, arg0: float) -> Scan: ...
+    def add(self, wavelength: float, value: float) -> None: 
+        """
+        Add a wavelength, value point to the scan.
+        """
+    def init_spline(self) -> None: 
+        """
+        Initialise the spline with the current interpolation type.
+        """
+    def is_interpolated(self) -> bool: 
+        """
+        Returns whether or not the scan uses interpolation (a SplineType other than NONE).
+        """
+    def items(self) -> typing.Iterator: ...
+    def populate_from_csv(self, file_path: str) -> None: 
+        """
+        Populate from csv (or general char delimited) file.
+        """
+    def to_lists(self) -> typing.List[typing.List[float]]: 
+        """
+        Convert Scan object to a pair of lists
+        """
+    def to_numpy(self) -> numpy.ndarray[numpy.float64]: 
+        """
+        Convert Scan object to a 2D numpy array where index 0 and 1 are arrays of wavelengths and values respectively
+        """
+    def values(self) -> typing.List[float]: 
+        """
+        return the values from the scan object
+        """
+    def wavelengths(self) -> typing.List[float]: 
+        """
+        return the wavelengths from the scan object
+        """
+    @property
+    def epsilon(self) -> float:
+        """
+        :type: float
+        """
+    @epsilon.setter
+    def epsilon(self, arg1: float) -> None:
+        pass
+    @property
+    def interpolation(self) -> Interpolation:
+        """
+        :type: Interpolation
+        """
+    @interpolation.setter
+    def interpolation(self, arg1: Interpolation) -> None:
+        pass
+    __hash__ = None
+    pass
+@typing.overload
+def log(arg0: Scan) -> Scan:
+    """
+    Compute natural logarithm of a scan.
+
+    Compute logarithm base [Scan] of a Scan
+
+    Compute logarithm base [float] of a [Scan]
+
+    Compute logarithm base [Scan] of a [float]
+    """
+@typing.overload
+def log(arg0: Scan, arg1: Scan) -> Scan:
+    pass
+@typing.overload
+def log(arg0: Scan, arg1: float) -> Scan:
+    pass
+@typing.overload
+def log(arg0: float, arg1: Scan) -> Scan:
+    pass
+def log10(arg0: Scan) -> Scan:
+    """
+    Compute logarithm base 10 of a scan.
+    """
```

## benanalysis/colorimetry/__init__.py

 * *Ordering differences only*

```diff
@@ -1,8 +1,8 @@
-#
-# @file __init__.py
-# @author Markus Führer
-# @date 5 May 2023
-# @copyright Copyright © 2023 Bentham Instruments Ltd. All Rights Reserved.
-#
-
+#
+# @file __init__.py
+# @author Markus Führer
+# @date 5 May 2023
+# @copyright Copyright © 2023 Bentham Instruments Ltd. All Rights Reserved.
+#
+
 from benanalysis._benpy_core.colorimetry import *
```

## benanalysis/colorimetry/__init__.pyi

 * *Ordering differences only*

```diff
@@ -1,281 +1,281 @@
-from __future__ import annotations
-import benanalysis._benpy_core.colorimetry
-import typing
-import benanalysis._benpy_core
-
-__all__ = [
-    "ANSI_Z80_3_tau_signal",
-    "ANSI_Z80_3_tau_spectral_min",
-    "ANSI_Z80_3_tau_uva",
-    "ANSI_Z80_3_tau_uvb",
-    "ANSI_Z80_3_tau_v",
-    "ASNZS1067_2016_tau_suva",
-    "CIELAB",
-    "CIELAB_f",
-    "CIELAB_tristimulus_values",
-    "CIEXYZ",
-    "CIE_tristimulus_values",
-    "ISO12311_tau_sb",
-    "ISO8980_3_tau_signal_incandescent",
-    "ISO8980_3_tau_signal_led",
-    "ISO8980_3_tau_suva",
-    "ISO8980_3_tau_suvb",
-    "ISO8980_3_tau_uva",
-    "ISO8980_3_tau_v",
-    "Observer",
-    "RYG",
-    "RYGB",
-    "f1_prime",
-    "f2"
-]
-
-
-class CIELAB():
-    """
-    CIE 1976 (L*, a*, b*) color space (CIELAB) coordinates
-    """
-    @typing.overload
-    def __init__(self) -> None: ...
-    @typing.overload
-    def __init__(self, L_star: float, a_star: float, b_star: float) -> None: ...
-    def __repr__(self) -> str: ...
-    def __str__(self) -> str: ...
-    @property
-    def L_star(self) -> float:
-        """
-        :type: float
-        """
-    @L_star.setter
-    def L_star(self, arg0: float) -> None:
-        pass
-    @property
-    def a_star(self) -> float:
-        """
-        :type: float
-        """
-    @a_star.setter
-    def a_star(self, arg0: float) -> None:
-        pass
-    @property
-    def b_star(self) -> float:
-        """
-        :type: float
-        """
-    @b_star.setter
-    def b_star(self, arg0: float) -> None:
-        pass
-    pass
-class CIEXYZ():
-    """
-    CIE 1931 (X, Y, Z) color space (CIEXYZ) coordinates
-    """
-    @typing.overload
-    def __init__(self) -> None: ...
-    @typing.overload
-    def __init__(self, X: float, Y: float, Z: float) -> None: ...
-    def __repr__(self) -> str: ...
-    def __str__(self) -> str: ...
-    @property
-    def X(self) -> float:
-        """
-        :type: float
-        """
-    @X.setter
-    def X(self, arg0: float) -> None:
-        pass
-    @property
-    def Y(self) -> float:
-        """
-        :type: float
-        """
-    @Y.setter
-    def Y(self, arg0: float) -> None:
-        pass
-    @property
-    def Z(self) -> float:
-        """
-        :type: float
-        """
-    @Z.setter
-    def Z(self, arg0: float) -> None:
-        pass
-    pass
-class Observer():
-    """
-    Observer struct
-    """
-    def __init__(self, x: benanalysis._benpy_core.Scan, y: benanalysis._benpy_core.Scan, z: benanalysis._benpy_core.Scan) -> None: ...
-    def __repr__(self) -> str: ...
-    @property
-    def x(self) -> benanalysis._benpy_core.Scan:
-        """
-        :type: benanalysis._benpy_core.Scan
-        """
-    @property
-    def y(self) -> benanalysis._benpy_core.Scan:
-        """
-        :type: benanalysis._benpy_core.Scan
-        """
-    @property
-    def z(self) -> benanalysis._benpy_core.Scan:
-        """
-        :type: benanalysis._benpy_core.Scan
-        """
-    pass
-class RYG():
-    """
-    Red, Yellow, Green coordinates
-    """
-    @typing.overload
-    def __init__(self) -> None: ...
-    @typing.overload
-    def __init__(self, red: float, yellow: float, green: float) -> None: ...
-    def __repr__(self) -> str: ...
-    def __str__(self) -> str: ...
-    @property
-    def green(self) -> float:
-        """
-        :type: float
-        """
-    @green.setter
-    def green(self, arg0: float) -> None:
-        pass
-    @property
-    def red(self) -> float:
-        """
-        :type: float
-        """
-    @red.setter
-    def red(self, arg0: float) -> None:
-        pass
-    @property
-    def yellow(self) -> float:
-        """
-        :type: float
-        """
-    @yellow.setter
-    def yellow(self, arg0: float) -> None:
-        pass
-    pass
-class RYGB():
-    """
-    Red, Yellow, Green, Blue coordinates
-    """
-    @typing.overload
-    def __init__(self) -> None: ...
-    @typing.overload
-    def __init__(self, red: float, yellow: float, green: float, blue: float) -> None: ...
-    def __repr__(self) -> str: ...
-    def __str__(self) -> str: ...
-    @property
-    def blue(self) -> float:
-        """
-        :type: float
-        """
-    @blue.setter
-    def blue(self, arg0: float) -> None:
-        pass
-    @property
-    def green(self) -> float:
-        """
-        :type: float
-        """
-    @green.setter
-    def green(self, arg0: float) -> None:
-        pass
-    @property
-    def red(self) -> float:
-        """
-        :type: float
-        """
-    @red.setter
-    def red(self, arg0: float) -> None:
-        pass
-    @property
-    def yellow(self) -> float:
-        """
-        :type: float
-        """
-    @yellow.setter
-    def yellow(self, arg0: float) -> None:
-        pass
-    pass
-def ANSI_Z80_3_tau_signal(trans: benanalysis._benpy_core.Scan) -> RYG:
-    """
-    Returns the luminous transmittance of the lens for the spectral radiant power distribution of the incandescent traffic signal light.
-    """
-def ANSI_Z80_3_tau_spectral_min(trans: benanalysis._benpy_core.Scan) -> float:
-    """
-    Returns the minimum of the spectral transmittance tau(lambda) of the lens between 475nm and 650nm.
-    """
-def ANSI_Z80_3_tau_uva(trans: benanalysis._benpy_core.Scan) -> float:
-    """
-    Returns the mean UV-A transmittance (tau_UVA). The mean transmittance between 315 nm and 380 nm.
-    """
-def ANSI_Z80_3_tau_uvb(trans: benanalysis._benpy_core.Scan) -> float:
-    """
-    Returns the mean UV-B transmittance (tau_UVB). The mean transmittance between 280 nm and 315 nm.
-    """
-def ANSI_Z80_3_tau_v(trans: benanalysis._benpy_core.Scan) -> float:
-    """
-    Returns the luminous transmittance (tau_V). The ratio of the luminous flux transmitted by the lens or filter to the incident luminous flux.
-    """
-def ASNZS1067_2016_tau_suva(trans: benanalysis._benpy_core.Scan) -> float:
-    """
-    Returns the solar UV-A transmittance (tau_SUVA). The mean of the spectral transmittance between 315 nm and 400 nm weighted by the solar radiation distribution Es(λ) at sea level, for air mass 2, and the relative spectral effectiveness function for UV radiation S(λ).
-    """
-def CIELAB_f(t: float) -> float:
-    """
-    Non-linear function used in the forward transformation from the CIEXYZ color space to the CIELAB.
-    """
-def CIELAB_tristimulus_values(scan: benanalysis._benpy_core.Scan, white_point_reference: benanalysis._benpy_core.Scan, observer: Observer) -> CIELAB:
-    """
-    Returns the CIE 1976 (L*, a*, b*) color space coordinates for a given spectrum given a specific observer and white point reference.
-    """
-def CIE_tristimulus_values(scan: benanalysis._benpy_core.Scan, observer: Observer) -> CIEXYZ:
-    """
-    Calculate the CIE Tristimulus Values for a given observer and spectrum.
-
-    Args:
-        scan (Scan): A scan object containing the spectrum data.
-        observer (Observer): An observer object containing color matching functions.
-
-    Returns:
-        CIEXYZ: A CIEXYZ object containing the calculated CIE Tristimulus Values.
-    """
-def ISO12311_tau_sb(trans: benanalysis._benpy_core.Scan) -> float:
-    """
-    Returns the solar blue-light transmittance tau_sb. Solar blue-light transmittance is the result of the mean of the spectral transmittance between 380 nm and 500 nm and appropriate weighting functions.
-    """
-def ISO8980_3_tau_signal_incandescent(trans: benanalysis._benpy_core.Scan) -> RYGB:
-    """
-    Returns the luminous transmittance of the lens for the spectral radiant power distribution of the incandescent traffic signal light.
-    """
-def ISO8980_3_tau_signal_led(trans: benanalysis._benpy_core.Scan) -> RYGB:
-    """
-    Returns the luminous transmittance of the lens for the spectral radiant power distribution of the LED traffic signal light.
-    """
-def ISO8980_3_tau_suva(trans: benanalysis._benpy_core.Scan) -> float:
-    """
-    Returns the solar UV-A transmittance (tau_SUVA). The mean of the spectral transmittance between 315 nm and 380 nm weighted by the solar radiation distribution Es(λ) at sea level, for air mass 2, and the relative spectral effectiveness function for UV radiation S(λ).
-    """
-def ISO8980_3_tau_suvb(trans: benanalysis._benpy_core.Scan) -> float:
-    """
-    Returns the solar UV-B transmittance (tau_SUVB). The mean of the spectral transmittance between 280 nm and 315 nm weighted by the solar radiation distribution Es(λ) at sea level, for air mass 2, and the relative spectral effectiveness function for UV radiation S(λ).
-    """
-def ISO8980_3_tau_uva(trans: benanalysis._benpy_core.Scan) -> float:
-    """
-    Returns the mean UV-A transmittance (tau_UVA). The mean transmittance between 315 nm and 380 nm.
-    """
-def ISO8980_3_tau_v(trans: benanalysis._benpy_core.Scan) -> float:
-    """
-    Returns the luminous transmittancev (tau_V). The ratio of the luminous flux transmitted by the lens or filter to the incident luminous flux.
-    """
-def f1_prime(scan: benanalysis._benpy_core.Scan) -> float:
-    """
-    The integral parameter f1' describes the quality of the spectral match between a specified spectrum and the CIE 1931 standard colorimetric observer (CIE 1931 2° Standard Observer) Color Matching Function y.
-    """
-def f2(Y_0: benanalysis._benpy_core.Scan, Y_pi_2: benanalysis._benpy_core.Scan) -> float:
-    """
-    f2 is the deviation in directional response to the incident radiation of a photometer with a plane input window measuring planar illuminances.
-    """
+from __future__ import annotations
+import benanalysis._benpy_core.colorimetry
+import typing
+import benanalysis._benpy_core
+
+__all__ = [
+    "ANSI_Z80_3_tau_signal",
+    "ANSI_Z80_3_tau_spectral_min",
+    "ANSI_Z80_3_tau_uva",
+    "ANSI_Z80_3_tau_uvb",
+    "ANSI_Z80_3_tau_v",
+    "ASNZS1067_2016_tau_suva",
+    "CIELAB",
+    "CIELAB_f",
+    "CIELAB_tristimulus_values",
+    "CIEXYZ",
+    "CIE_tristimulus_values",
+    "ISO12311_tau_sb",
+    "ISO8980_3_tau_signal_incandescent",
+    "ISO8980_3_tau_signal_led",
+    "ISO8980_3_tau_suva",
+    "ISO8980_3_tau_suvb",
+    "ISO8980_3_tau_uva",
+    "ISO8980_3_tau_v",
+    "Observer",
+    "RYG",
+    "RYGB",
+    "f1_prime",
+    "f2"
+]
+
+
+class CIELAB():
+    """
+    CIE 1976 (L*, a*, b*) color space (CIELAB) coordinates
+    """
+    @typing.overload
+    def __init__(self) -> None: ...
+    @typing.overload
+    def __init__(self, L_star: float, a_star: float, b_star: float) -> None: ...
+    def __repr__(self) -> str: ...
+    def __str__(self) -> str: ...
+    @property
+    def L_star(self) -> float:
+        """
+        :type: float
+        """
+    @L_star.setter
+    def L_star(self, arg0: float) -> None:
+        pass
+    @property
+    def a_star(self) -> float:
+        """
+        :type: float
+        """
+    @a_star.setter
+    def a_star(self, arg0: float) -> None:
+        pass
+    @property
+    def b_star(self) -> float:
+        """
+        :type: float
+        """
+    @b_star.setter
+    def b_star(self, arg0: float) -> None:
+        pass
+    pass
+class CIEXYZ():
+    """
+    CIE 1931 (X, Y, Z) color space (CIEXYZ) coordinates
+    """
+    @typing.overload
+    def __init__(self) -> None: ...
+    @typing.overload
+    def __init__(self, X: float, Y: float, Z: float) -> None: ...
+    def __repr__(self) -> str: ...
+    def __str__(self) -> str: ...
+    @property
+    def X(self) -> float:
+        """
+        :type: float
+        """
+    @X.setter
+    def X(self, arg0: float) -> None:
+        pass
+    @property
+    def Y(self) -> float:
+        """
+        :type: float
+        """
+    @Y.setter
+    def Y(self, arg0: float) -> None:
+        pass
+    @property
+    def Z(self) -> float:
+        """
+        :type: float
+        """
+    @Z.setter
+    def Z(self, arg0: float) -> None:
+        pass
+    pass
+class Observer():
+    """
+    Observer struct
+    """
+    def __init__(self, x: benanalysis._benpy_core.Scan, y: benanalysis._benpy_core.Scan, z: benanalysis._benpy_core.Scan) -> None: ...
+    def __repr__(self) -> str: ...
+    @property
+    def x(self) -> benanalysis._benpy_core.Scan:
+        """
+        :type: benanalysis._benpy_core.Scan
+        """
+    @property
+    def y(self) -> benanalysis._benpy_core.Scan:
+        """
+        :type: benanalysis._benpy_core.Scan
+        """
+    @property
+    def z(self) -> benanalysis._benpy_core.Scan:
+        """
+        :type: benanalysis._benpy_core.Scan
+        """
+    pass
+class RYG():
+    """
+    Red, Yellow, Green coordinates
+    """
+    @typing.overload
+    def __init__(self) -> None: ...
+    @typing.overload
+    def __init__(self, red: float, yellow: float, green: float) -> None: ...
+    def __repr__(self) -> str: ...
+    def __str__(self) -> str: ...
+    @property
+    def green(self) -> float:
+        """
+        :type: float
+        """
+    @green.setter
+    def green(self, arg0: float) -> None:
+        pass
+    @property
+    def red(self) -> float:
+        """
+        :type: float
+        """
+    @red.setter
+    def red(self, arg0: float) -> None:
+        pass
+    @property
+    def yellow(self) -> float:
+        """
+        :type: float
+        """
+    @yellow.setter
+    def yellow(self, arg0: float) -> None:
+        pass
+    pass
+class RYGB():
+    """
+    Red, Yellow, Green, Blue coordinates
+    """
+    @typing.overload
+    def __init__(self) -> None: ...
+    @typing.overload
+    def __init__(self, red: float, yellow: float, green: float, blue: float) -> None: ...
+    def __repr__(self) -> str: ...
+    def __str__(self) -> str: ...
+    @property
+    def blue(self) -> float:
+        """
+        :type: float
+        """
+    @blue.setter
+    def blue(self, arg0: float) -> None:
+        pass
+    @property
+    def green(self) -> float:
+        """
+        :type: float
+        """
+    @green.setter
+    def green(self, arg0: float) -> None:
+        pass
+    @property
+    def red(self) -> float:
+        """
+        :type: float
+        """
+    @red.setter
+    def red(self, arg0: float) -> None:
+        pass
+    @property
+    def yellow(self) -> float:
+        """
+        :type: float
+        """
+    @yellow.setter
+    def yellow(self, arg0: float) -> None:
+        pass
+    pass
+def ANSI_Z80_3_tau_signal(trans: benanalysis._benpy_core.Scan) -> RYG:
+    """
+    Returns the luminous transmittance of the lens for the spectral radiant power distribution of the incandescent traffic signal light.
+    """
+def ANSI_Z80_3_tau_spectral_min(trans: benanalysis._benpy_core.Scan) -> float:
+    """
+    Returns the minimum of the spectral transmittance tau(lambda) of the lens between 475nm and 650nm.
+    """
+def ANSI_Z80_3_tau_uva(trans: benanalysis._benpy_core.Scan) -> float:
+    """
+    Returns the mean UV-A transmittance (tau_UVA). The mean transmittance between 315 nm and 380 nm.
+    """
+def ANSI_Z80_3_tau_uvb(trans: benanalysis._benpy_core.Scan) -> float:
+    """
+    Returns the mean UV-B transmittance (tau_UVB). The mean transmittance between 280 nm and 315 nm.
+    """
+def ANSI_Z80_3_tau_v(trans: benanalysis._benpy_core.Scan) -> float:
+    """
+    Returns the luminous transmittance (tau_V). The ratio of the luminous flux transmitted by the lens or filter to the incident luminous flux.
+    """
+def ASNZS1067_2016_tau_suva(trans: benanalysis._benpy_core.Scan) -> float:
+    """
+    Returns the solar UV-A transmittance (tau_SUVA). The mean of the spectral transmittance between 315 nm and 400 nm weighted by the solar radiation distribution Es(λ) at sea level, for air mass 2, and the relative spectral effectiveness function for UV radiation S(λ).
+    """
+def CIELAB_f(t: float) -> float:
+    """
+    Non-linear function used in the forward transformation from the CIEXYZ color space to the CIELAB.
+    """
+def CIELAB_tristimulus_values(scan: benanalysis._benpy_core.Scan, white_point_reference: benanalysis._benpy_core.Scan, observer: Observer) -> CIELAB:
+    """
+    Returns the CIE 1976 (L*, a*, b*) color space coordinates for a given spectrum given a specific observer and white point reference.
+    """
+def CIE_tristimulus_values(scan: benanalysis._benpy_core.Scan, observer: Observer) -> CIEXYZ:
+    """
+    Calculate the CIE Tristimulus Values for a given observer and spectrum.
+
+    Args:
+        scan (Scan): A scan object containing the spectrum data.
+        observer (Observer): An observer object containing color matching functions.
+
+    Returns:
+        CIEXYZ: A CIEXYZ object containing the calculated CIE Tristimulus Values.
+    """
+def ISO12311_tau_sb(trans: benanalysis._benpy_core.Scan) -> float:
+    """
+    Returns the solar blue-light transmittance tau_sb. Solar blue-light transmittance is the result of the mean of the spectral transmittance between 380 nm and 500 nm and appropriate weighting functions.
+    """
+def ISO8980_3_tau_signal_incandescent(trans: benanalysis._benpy_core.Scan) -> RYGB:
+    """
+    Returns the luminous transmittance of the lens for the spectral radiant power distribution of the incandescent traffic signal light.
+    """
+def ISO8980_3_tau_signal_led(trans: benanalysis._benpy_core.Scan) -> RYGB:
+    """
+    Returns the luminous transmittance of the lens for the spectral radiant power distribution of the LED traffic signal light.
+    """
+def ISO8980_3_tau_suva(trans: benanalysis._benpy_core.Scan) -> float:
+    """
+    Returns the solar UV-A transmittance (tau_SUVA). The mean of the spectral transmittance between 315 nm and 380 nm weighted by the solar radiation distribution Es(λ) at sea level, for air mass 2, and the relative spectral effectiveness function for UV radiation S(λ).
+    """
+def ISO8980_3_tau_suvb(trans: benanalysis._benpy_core.Scan) -> float:
+    """
+    Returns the solar UV-B transmittance (tau_SUVB). The mean of the spectral transmittance between 280 nm and 315 nm weighted by the solar radiation distribution Es(λ) at sea level, for air mass 2, and the relative spectral effectiveness function for UV radiation S(λ).
+    """
+def ISO8980_3_tau_uva(trans: benanalysis._benpy_core.Scan) -> float:
+    """
+    Returns the mean UV-A transmittance (tau_UVA). The mean transmittance between 315 nm and 380 nm.
+    """
+def ISO8980_3_tau_v(trans: benanalysis._benpy_core.Scan) -> float:
+    """
+    Returns the luminous transmittancev (tau_V). The ratio of the luminous flux transmitted by the lens or filter to the incident luminous flux.
+    """
+def f1_prime(scan: benanalysis._benpy_core.Scan) -> float:
+    """
+    The integral parameter f1' describes the quality of the spectral match between a specified spectrum and the CIE 1931 standard colorimetric observer (CIE 1931 2° Standard Observer) Color Matching Function y.
+    """
+def f2(Y_0: benanalysis._benpy_core.Scan, Y_pi_2: benanalysis._benpy_core.Scan) -> float:
+    """
+    f2 is the deviation in directional response to the incident radiation of a photometer with a plane input window measuring planar illuminances.
+    """
```

## benanalysis/data/__init__.py

 * *Ordering differences only*

```diff
@@ -1,8 +1,8 @@
-#
-# @file __init__.py
-# @author Markus Führer
-# @date 5 May 2023
-# @copyright Copyright © 2023 Bentham Instruments Ltd. All Rights Reserved.
-#
-
+#
+# @file __init__.py
+# @author Markus Führer
+# @date 5 May 2023
+# @copyright Copyright © 2023 Bentham Instruments Ltd. All Rights Reserved.
+#
+
 from benanalysis._benpy_core.data import *
```

## benanalysis/data/__init__.pyi

 * *Ordering differences only*

```diff
@@ -1,9 +1,9 @@
-from __future__ import annotations
-import benanalysis._benpy_core.data
-import typing
-
-__all__ = [
-    "colorimetry"
-]
-
-
+from __future__ import annotations
+import benanalysis._benpy_core.data
+import typing
+
+__all__ = [
+    "colorimetry"
+]
+
+
```

## benanalysis/data/colorimetry/__init__.py

 * *Ordering differences only*

```diff
@@ -1,8 +1,8 @@
-#
-# @file __init__.py
-# @author Markus Führer
-# @date 5 May 2023
-# @copyright Copyright © 2023 Bentham Instruments Ltd. All Rights Reserved.
-#
-
+#
+# @file __init__.py
+# @author Markus Führer
+# @date 5 May 2023
+# @copyright Copyright © 2023 Bentham Instruments Ltd. All Rights Reserved.
+#
+
 from benanalysis._benpy_core.data.colorimetry import *
```

## benanalysis/data/colorimetry/__init__.pyi

 * *Ordering differences only*

```diff
@@ -1,166 +1,166 @@
-from __future__ import annotations
-import benanalysis._benpy_core.data.colorimetry
-import typing
-import benanalysis._benpy_core
-
-__all__ = [
-    "ANSI_Z80_3_2015_green_signal_transmittance",
-    "ANSI_Z80_3_2015_red_signal_transmittance",
-    "ANSI_Z80_3_2015_yellow_signal_transmittance",
-    "ISO8980_3_incandescent_blue",
-    "ISO8980_3_incandescent_green",
-    "ISO8980_3_incandescent_red",
-    "ISO8980_3_incandescent_yellow",
-    "ISO8980_3_led_blue",
-    "ISO8980_3_led_green",
-    "ISO8980_3_led_red",
-    "ISO8980_3_led_yellow",
-    "aphake_hazard",
-    "blue_light_hazard",
-    "cie_1931_standard_observer_x",
-    "cie_1931_standard_observer_y",
-    "cie_1931_standard_observer_z",
-    "cie_1964_standard_observer_x",
-    "cie_1964_standard_observer_y",
-    "cie_1964_standard_observer_z",
-    "cie_illuminant_a",
-    "cie_illuminant_c",
-    "cie_illuminant_d65",
-    "relative_spectral_effectiveness",
-    "solar_spectral_irradiance"
-]
-
-
-def ANSI_Z80_3_2015_green_signal_transmittance() -> benanalysis._benpy_core.Scan:
-    """
-    Transmittance of the green traffic signal lens specified in ANSI Z80.3-2015
-    """
-def ANSI_Z80_3_2015_red_signal_transmittance() -> benanalysis._benpy_core.Scan:
-    """
-    Transmittance of the red traffic signal lens specified in ANSI Z80.3-2015
-    """
-def ANSI_Z80_3_2015_yellow_signal_transmittance() -> benanalysis._benpy_core.Scan:
-    """
-    Transmittance of the yellow traffic signal lens specified in ANSI Z80.3-2015
-    """
-def ISO8980_3_incandescent_blue() -> benanalysis._benpy_core.Scan:
-    """
-    Relative spectral distribution of radiation emitted by incandescent signal lights,
-    ESignal(λ), weighted by the spectral luminous efficiency function of the average
-    human eye for daylight vision, V(λ), as specified in ISO 11664-1.
-    Blue Signal
-    """
-def ISO8980_3_incandescent_green() -> benanalysis._benpy_core.Scan:
-    """
-    Relative spectral distribution of radiation emitted by incandescent signal lights,
-    ESignal(λ), weighted by the spectral luminous efficiency function of the average
-    human eye for daylight vision, V(λ), as specified in ISO 11664-1.
-    Green Signal
-    """
-def ISO8980_3_incandescent_red() -> benanalysis._benpy_core.Scan:
-    """
-    Relative spectral distribution of radiation emitted by incandescent signal lights,
-    ESignal(λ), weighted by the spectral luminous efficiency function of the average
-    human eye for daylight vision, V(λ), as specified in ISO 11664-1.
-    Red Signal
-    """
-def ISO8980_3_incandescent_yellow() -> benanalysis._benpy_core.Scan:
-    """
-    Relative spectral distribution of radiation emitted by incandescent signal lights,
-    ESignal(λ), weighted by the spectral luminous efficiency function of the average
-    human eye for daylight vision, V(λ), as specified in ISO 11664-1.
-    Yellow Signal
-    """
-def ISO8980_3_led_blue() -> benanalysis._benpy_core.Scan:
-    """
-    Relative spectral distribution of radiation emitted by LED signal lights,
-    ESignal(λ), weighted by the spectral luminous efficiency function of the average
-    human eye for daylight vision, V(λ), as specified in ISO 11664-1.
-    Blue Signal
-    """
-def ISO8980_3_led_green() -> benanalysis._benpy_core.Scan:
-    """
-    Relative spectral distribution of radiation emitted by LED signal lights,
-    ESignal(λ), weighted by the spectral luminous efficiency function of the average
-    human eye for daylight vision, V(λ), as specified in ISO 11664-1.
-    Green Signal
-    """
-def ISO8980_3_led_red() -> benanalysis._benpy_core.Scan:
-    """
-    Relative spectral distribution of radiation emitted by LED signal lights,
-    ESignal(λ), weighted by the spectral luminous efficiency function of the average
-    human eye for daylight vision, V(λ), as specified in ISO 11664-1.
-    Red Signal
-    """
-def ISO8980_3_led_yellow() -> benanalysis._benpy_core.Scan:
-    """
-    Relative spectral distribution of radiation emitted by LED signal lights,
-    ESignal(λ), weighted by the spectral luminous efficiency function of the average
-    human eye for daylight vision, V(λ), as specified in ISO 11664-1.
-    Yellow Signal
-    """
-def aphake_hazard() -> benanalysis._benpy_core.Scan:
-    """
-    Aphake hazard function A(λ)
-    """
-def blue_light_hazard() -> benanalysis._benpy_core.Scan:
-    """
-    Blue-light hazard function B(λ)
-    380nm to 500nm steps 5nm
-    """
-def cie_1931_standard_observer_x() -> benanalysis._benpy_core.Scan:
-    """
-    CIE 1931 standard colorimetric observer (CIE 1931 2° Standard Observer)
-    Color Matching Function x
-    """
-def cie_1931_standard_observer_y() -> benanalysis._benpy_core.Scan:
-    """
-    CIE 1931 standard colorimetric observer (CIE 1931 2° Standard Observer)
-    Color Matching Function y
-    """
-def cie_1931_standard_observer_z() -> benanalysis._benpy_core.Scan:
-    """
-    CIE 1931 standard colorimetric observer (CIE 1931 2° Standard Observer)
-    Color Matching Function z
-    """
-def cie_1964_standard_observer_x() -> benanalysis._benpy_core.Scan:
-    """
-    CIE 1964 standard colorimetric observer (CIE 1964 10° Standard Observer)
-    Color Matching Function x
-    """
-def cie_1964_standard_observer_y() -> benanalysis._benpy_core.Scan:
-    """
-    CIE 1964 standard colorimetric observer (CIE 1964 10° Standard Observer)
-    Color Matching Function y
-    """
-def cie_1964_standard_observer_z() -> benanalysis._benpy_core.Scan:
-    """
-    CIE 1964 standard colorimetric observer (CIE 1964 10° Standard Observer)
-    Color Matching Function z
-    """
-def cie_illuminant_a() -> benanalysis._benpy_core.Scan:
-    """
-    Relative spectral power distribution of CIE Standard Illuminant A
-    """
-def cie_illuminant_c() -> benanalysis._benpy_core.Scan:
-    """
-    Relative spectral power distribution of CIE Standard Illuminant C
-    """
-def cie_illuminant_d65() -> benanalysis._benpy_core.Scan:
-    """
-    Relative spectral power distribution of CIE Standard Illuminant D65
-    """
-def relative_spectral_effectiveness() -> benanalysis._benpy_core.Scan:
-    """
-    Relative spectral effectiveness function S(λ)
-    280nm to 400nm steps 5nm
-    see: The International commission on non-ionizing radiation protection (ICNIRP).
-    Guidelines on limits of exposure to ultraviolet radiation of wavelengths between
-    180 nm and 400 nm (incoherent optical radiation).
-    Health Phys. 2004, 87 (2) pp. 171-186
-    """
-def solar_spectral_irradiance() -> benanalysis._benpy_core.Scan:
-    """
-    Solar Spectral Irradiance (mW m-2 nm-1)
-    250nm to 500nm steps 5nm
-    """
+from __future__ import annotations
+import benanalysis._benpy_core.data.colorimetry
+import typing
+import benanalysis._benpy_core
+
+__all__ = [
+    "ANSI_Z80_3_2015_green_signal_transmittance",
+    "ANSI_Z80_3_2015_red_signal_transmittance",
+    "ANSI_Z80_3_2015_yellow_signal_transmittance",
+    "ISO8980_3_incandescent_blue",
+    "ISO8980_3_incandescent_green",
+    "ISO8980_3_incandescent_red",
+    "ISO8980_3_incandescent_yellow",
+    "ISO8980_3_led_blue",
+    "ISO8980_3_led_green",
+    "ISO8980_3_led_red",
+    "ISO8980_3_led_yellow",
+    "aphake_hazard",
+    "blue_light_hazard",
+    "cie_1931_standard_observer_x",
+    "cie_1931_standard_observer_y",
+    "cie_1931_standard_observer_z",
+    "cie_1964_standard_observer_x",
+    "cie_1964_standard_observer_y",
+    "cie_1964_standard_observer_z",
+    "cie_illuminant_a",
+    "cie_illuminant_c",
+    "cie_illuminant_d65",
+    "relative_spectral_effectiveness",
+    "solar_spectral_irradiance"
+]
+
+
+def ANSI_Z80_3_2015_green_signal_transmittance() -> benanalysis._benpy_core.Scan:
+    """
+    Transmittance of the green traffic signal lens specified in ANSI Z80.3-2015
+    """
+def ANSI_Z80_3_2015_red_signal_transmittance() -> benanalysis._benpy_core.Scan:
+    """
+    Transmittance of the red traffic signal lens specified in ANSI Z80.3-2015
+    """
+def ANSI_Z80_3_2015_yellow_signal_transmittance() -> benanalysis._benpy_core.Scan:
+    """
+    Transmittance of the yellow traffic signal lens specified in ANSI Z80.3-2015
+    """
+def ISO8980_3_incandescent_blue() -> benanalysis._benpy_core.Scan:
+    """
+    Relative spectral distribution of radiation emitted by incandescent signal lights,
+    ESignal(λ), weighted by the spectral luminous efficiency function of the average
+    human eye for daylight vision, V(λ), as specified in ISO 11664-1.
+    Blue Signal
+    """
+def ISO8980_3_incandescent_green() -> benanalysis._benpy_core.Scan:
+    """
+    Relative spectral distribution of radiation emitted by incandescent signal lights,
+    ESignal(λ), weighted by the spectral luminous efficiency function of the average
+    human eye for daylight vision, V(λ), as specified in ISO 11664-1.
+    Green Signal
+    """
+def ISO8980_3_incandescent_red() -> benanalysis._benpy_core.Scan:
+    """
+    Relative spectral distribution of radiation emitted by incandescent signal lights,
+    ESignal(λ), weighted by the spectral luminous efficiency function of the average
+    human eye for daylight vision, V(λ), as specified in ISO 11664-1.
+    Red Signal
+    """
+def ISO8980_3_incandescent_yellow() -> benanalysis._benpy_core.Scan:
+    """
+    Relative spectral distribution of radiation emitted by incandescent signal lights,
+    ESignal(λ), weighted by the spectral luminous efficiency function of the average
+    human eye for daylight vision, V(λ), as specified in ISO 11664-1.
+    Yellow Signal
+    """
+def ISO8980_3_led_blue() -> benanalysis._benpy_core.Scan:
+    """
+    Relative spectral distribution of radiation emitted by LED signal lights,
+    ESignal(λ), weighted by the spectral luminous efficiency function of the average
+    human eye for daylight vision, V(λ), as specified in ISO 11664-1.
+    Blue Signal
+    """
+def ISO8980_3_led_green() -> benanalysis._benpy_core.Scan:
+    """
+    Relative spectral distribution of radiation emitted by LED signal lights,
+    ESignal(λ), weighted by the spectral luminous efficiency function of the average
+    human eye for daylight vision, V(λ), as specified in ISO 11664-1.
+    Green Signal
+    """
+def ISO8980_3_led_red() -> benanalysis._benpy_core.Scan:
+    """
+    Relative spectral distribution of radiation emitted by LED signal lights,
+    ESignal(λ), weighted by the spectral luminous efficiency function of the average
+    human eye for daylight vision, V(λ), as specified in ISO 11664-1.
+    Red Signal
+    """
+def ISO8980_3_led_yellow() -> benanalysis._benpy_core.Scan:
+    """
+    Relative spectral distribution of radiation emitted by LED signal lights,
+    ESignal(λ), weighted by the spectral luminous efficiency function of the average
+    human eye for daylight vision, V(λ), as specified in ISO 11664-1.
+    Yellow Signal
+    """
+def aphake_hazard() -> benanalysis._benpy_core.Scan:
+    """
+    Aphake hazard function A(λ)
+    """
+def blue_light_hazard() -> benanalysis._benpy_core.Scan:
+    """
+    Blue-light hazard function B(λ)
+    380nm to 500nm steps 5nm
+    """
+def cie_1931_standard_observer_x() -> benanalysis._benpy_core.Scan:
+    """
+    CIE 1931 standard colorimetric observer (CIE 1931 2° Standard Observer)
+    Color Matching Function x
+    """
+def cie_1931_standard_observer_y() -> benanalysis._benpy_core.Scan:
+    """
+    CIE 1931 standard colorimetric observer (CIE 1931 2° Standard Observer)
+    Color Matching Function y
+    """
+def cie_1931_standard_observer_z() -> benanalysis._benpy_core.Scan:
+    """
+    CIE 1931 standard colorimetric observer (CIE 1931 2° Standard Observer)
+    Color Matching Function z
+    """
+def cie_1964_standard_observer_x() -> benanalysis._benpy_core.Scan:
+    """
+    CIE 1964 standard colorimetric observer (CIE 1964 10° Standard Observer)
+    Color Matching Function x
+    """
+def cie_1964_standard_observer_y() -> benanalysis._benpy_core.Scan:
+    """
+    CIE 1964 standard colorimetric observer (CIE 1964 10° Standard Observer)
+    Color Matching Function y
+    """
+def cie_1964_standard_observer_z() -> benanalysis._benpy_core.Scan:
+    """
+    CIE 1964 standard colorimetric observer (CIE 1964 10° Standard Observer)
+    Color Matching Function z
+    """
+def cie_illuminant_a() -> benanalysis._benpy_core.Scan:
+    """
+    Relative spectral power distribution of CIE Standard Illuminant A
+    """
+def cie_illuminant_c() -> benanalysis._benpy_core.Scan:
+    """
+    Relative spectral power distribution of CIE Standard Illuminant C
+    """
+def cie_illuminant_d65() -> benanalysis._benpy_core.Scan:
+    """
+    Relative spectral power distribution of CIE Standard Illuminant D65
+    """
+def relative_spectral_effectiveness() -> benanalysis._benpy_core.Scan:
+    """
+    Relative spectral effectiveness function S(λ)
+    280nm to 400nm steps 5nm
+    see: The International commission on non-ionizing radiation protection (ICNIRP).
+    Guidelines on limits of exposure to ultraviolet radiation of wavelengths between
+    180 nm and 400 nm (incoherent optical radiation).
+    Health Phys. 2004, 87 (2) pp. 171-186
+    """
+def solar_spectral_irradiance() -> benanalysis._benpy_core.Scan:
+    """
+    Solar Spectral Irradiance (mW m-2 nm-1)
+    250nm to 500nm steps 5nm
+    """
```

## benanalysis/monochromator/__init__.py

 * *Ordering differences only*

```diff
@@ -1,8 +1,8 @@
-#
-# @file __init__.py
-# @author Markus Führer
-# @date 5 May 2023
-# @copyright Copyright © 2023 Bentham Instruments Ltd. All Rights Reserved.
-#
-
+#
+# @file __init__.py
+# @author Markus Führer
+# @date 5 May 2023
+# @copyright Copyright © 2023 Bentham Instruments Ltd. All Rights Reserved.
+#
+
 from benanalysis._benpy_core.monochromator import *
```

## benanalysis/monochromator/__init__.pyi

 * *Ordering differences only*

```diff
@@ -1,9 +1,9 @@
-from __future__ import annotations
-import benanalysis._benpy_core.monochromator
-import typing
-
-__all__ = [
-    "slit_function"
-]
-
-
+from __future__ import annotations
+import benanalysis._benpy_core.monochromator
+import typing
+
+__all__ = [
+    "slit_function"
+]
+
+
```

## benanalysis/monochromator/slit_function/__init__.pyi

 * *Ordering differences only*

```diff
@@ -1,23 +1,23 @@
-from __future__ import annotations
-import benanalysis._benpy_core.monochromator.slit_function
-import typing
-import benanalysis._benpy_core
-
-__all__ = [
-    "uniform_fibres",
-    "uniform_fibres_value"
-]
-
-
-def uniform_fibres(center_wavelength: float, bandwidth: float, points: int) -> benanalysis._benpy_core.Scan:
-    """
-    Returns the slit function (normalized to 1) formed by the perfect image of
-    a uniform circular input fibre as it passes accross a circular exit fibre.
-    Input and exit fibres have equal diameters.
-    """
-def uniform_fibres_value(center_wavelength: float, bandwidth: float, wavelength: float) -> float:
-    """
-    Returns the slit function value (normalized to 1) formed by the perfect image
-    of a uniform circular input fibre as it passes accross a circular exit fibre.
-    Input and exit fibres have equal diameters.
-    """
+from __future__ import annotations
+import benanalysis._benpy_core.monochromator.slit_function
+import typing
+import benanalysis._benpy_core
+
+__all__ = [
+    "uniform_fibres",
+    "uniform_fibres_value"
+]
+
+
+def uniform_fibres(center_wavelength: float, bandwidth: float, points: int) -> benanalysis._benpy_core.Scan:
+    """
+    Returns the slit function (normalized to 1) formed by the perfect image of
+    a uniform circular input fibre as it passes accross a circular exit fibre.
+    Input and exit fibres have equal diameters.
+    """
+def uniform_fibres_value(center_wavelength: float, bandwidth: float, wavelength: float) -> float:
+    """
+    Returns the slit function value (normalized to 1) formed by the perfect image
+    of a uniform circular input fibre as it passes accross a circular exit fibre.
+    Input and exit fibres have equal diameters.
+    """
```

## benanalysis/utils/__init__.py

 * *Ordering differences only*

```diff
@@ -1,9 +1,9 @@
-#
-# @file __init__.py
-# @author Markus Führer
-# @date 5 May 2023
-# @copyright Copyright © 2023 Bentham Instruments Ltd. All Rights Reserved.
-#
-
-# import benanalysis._benpy_core.colorimetry as colorimetry
+#
+# @file __init__.py
+# @author Markus Führer
+# @date 5 May 2023
+# @copyright Copyright © 2023 Bentham Instruments Ltd. All Rights Reserved.
+#
+
+# import benanalysis._benpy_core.colorimetry as colorimetry
 from benanalysis._benpy_core.utils import *
```

## benanalysis/utils/__init__.pyi

 * *Ordering differences only*

```diff
@@ -1,29 +1,29 @@
-from __future__ import annotations
-import benanalysis._benpy_core.utils
-import typing
-import benanalysis._benpy_core
-
-__all__ = [
-    "find_key",
-    "find_peak",
-    "find_peaks",
-    "peak_width"
-]
-
-
-def find_key(scan: benanalysis._benpy_core.Scan, lo: float, hi: float, value: float) -> float:
-    """
-    The value to search for. 
-    """
-def find_peak(scan: benanalysis._benpy_core.Scan) -> float:
-    """
-    The scan to find the peak of.
-    """
-def find_peaks(scan: benanalysis._benpy_core.Scan) -> benanalysis._benpy_core.Scan:
-    """
-    The scan to find the peaks of.
-    """
-def peak_width(scan: benanalysis._benpy_core.Scan, height: float) -> float:
-    """
-    The height as a fraction of max
-    """
+from __future__ import annotations
+import benanalysis._benpy_core.utils
+import typing
+import benanalysis._benpy_core
+
+__all__ = [
+    "find_key",
+    "find_peak",
+    "find_peaks",
+    "peak_width"
+]
+
+
+def find_key(scan: benanalysis._benpy_core.Scan, lo: float, hi: float, value: float) -> float:
+    """
+    The value to search for. 
+    """
+def find_peak(scan: benanalysis._benpy_core.Scan) -> float:
+    """
+    The scan to find the peak of.
+    """
+def find_peaks(scan: benanalysis._benpy_core.Scan) -> benanalysis._benpy_core.Scan:
+    """
+    The scan to find the peaks of.
+    """
+def peak_width(scan: benanalysis._benpy_core.Scan, height: float) -> float:
+    """
+    The height as a fraction of max
+    """
```

## Comparing `benanalysis-3.0.0.dist-info/METADATA` & `benanalysis-3.0.0rc1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1
-Name: benanalysis
-Version: 3.0.0
-Summary: Bentham Spectral Analysis and Calibration Utilities Library
-Home-page: https://github.com/BenthamInstruments/BenAnalysis
-Author: Bentham Instruments Ltd
-Author-email: support@bentham.com
-Requires-Dist: numpy
-
-benanalysis
-===========
-
-Bentham Instruments spectral analysis library.
-
-Compatibility
--------------
-
-Wheels are built for python versions 3.8 - 3.11, for these systems:
-
-- Windows: win32, amd64
-- Linux: x86, x86_64
-- MacOS >10.9, universal2 (combined x86_64, arm64, requires pip version > 20.6 on intel, >21.0.1 on Apple Silicon)
-
-Note: Apple silicon build has not been tested.
-
-Installation
-------------
-
-`pip install benanalysis`
-
-Usage
------
-
+Metadata-Version: 2.1
+Name: benanalysis
+Version: 3.0.0rc1
+Summary: Bentham Spectral Analysis and Calibration Utilities Library
+Home-page: https://github.com/BenthamInstruments/BenAnalysis
+Author: Bentham Instruments Ltd
+Author-email: support@bentham.com
+Requires-Dist: numpy
+
+benanalysis
+===========
+
+Bentham Instruments spectral analysis library.
+
+Compatibility
+-------------
+
+Wheels are built for python versions 3.8 - 3.11, for these systems:
+
+- Windows: win32, amd64
+- Linux: x86, x86_64
+- MacOS >10.9, universal2 (combined x86_64, arm64, requires pip version > 20.6 on intel, >21.0.1 on Apple Silicon)
+
+Note: Apple silicon build has not been tested.
+
+Installation
+------------
+
+`pip install benanalysis`
+
+Usage
+-----
+
```

## Comparing `benanalysis-3.0.0.dist-info/RECORD` & `benanalysis-3.0.0rc1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-benanalysis/__init__.py,sha256=znQ9TAFqCPFXZzmRq_OVZaJe8xfTXaWNk2XsvwLB7-c,343
-benanalysis/__init__.pyi,sha256=gcCyXJkptXMXJ-hu3wl9F5yicvvhVDTTlnaXDHfqZ94,7850
-benanalysis/_benpy_core.cp39-win_amd64.pyd,sha256=c3unDVgqg7qHO802yhDtTxV1LSH29NREyM7fLzq9URM,383488
-benanalysis/gsl.dll,sha256=zq1XlzVYLrDOsMjSKyrW7jhqqGZ9Nex7HbWyRXW2_ts,2668544
-benanalysis/gslcblas.dll,sha256=bLhsIbNC1IVsl_07zG0Ttvhsbs1TTlkz0jJgoQgPZZc,417792
-benanalysis/colorimetry/__init__.py,sha256=bYR7SXdVrozgQafHmgJDZK8UL7FVClfeDxiDul-exmw,202
-benanalysis/colorimetry/__init__.pyi,sha256=k3aLe_Ed6cbIBVIxNGZJT9I0YQhm4TrgXxpkfFMc61M,9607
-benanalysis/data/__init__.py,sha256=0w4mTeB7KNzvgb95HaKXCNqdmu8l1FkqglbOu-C4940,195
-benanalysis/data/__init__.pyi,sha256=nmhQBPLCCti8J1_vya8xt2ePIjuu2f0OGk6riS2XLCw,129
-benanalysis/data/colorimetry/__init__.py,sha256=Grgeow9KxNT6XYldeBXffYO6NWppoH7mu8sx5bsL5Yc,207
-benanalysis/data/colorimetry/__init__.pyi,sha256=NU0Fy4iaYB4MawY1uyETBDvdI_O0OiJnvf91y8s8wlQ,6734
-benanalysis/monochromator/__init__.py,sha256=spYfo97oCfuj7szs59iTsRJfy_LO1YeZD8BFSp-C_WU,204
-benanalysis/monochromator/__init__.pyi,sha256=0ThS7FrddAACs1p2yK_gASSO5NFW1gWNJo_HZ9kezYU,140
-benanalysis/monochromator/slit_function/__init__.py,sha256=a4AM8LPiSVrgjnqDiHRuUxXamsko_wvJJLzIdoajUt8,65
-benanalysis/monochromator/slit_function/__init__.pyi,sha256=DRh8eXKgBdbI7NeZoyA6zWwRQ5tdFBx8V73KJ8TOH-8,885
-benanalysis/utils/__init__.py,sha256=Nml0MOrHNBB1K5ngis_K8iEZrKFqRm1Dynm9j3oKjIs,257
-benanalysis/utils/__init__.pyi,sha256=IhP-n010QAwCVFOJpZcQvsuNbFJ0dV1EQ7lr0kNUc68,745
-benanalysis-3.0.0.dist-info/METADATA,sha256=LF5IhGnG1tW1-ltAermeyHy-TlzD_ahy49kcnJVTrPs,753
-benanalysis-3.0.0.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-benanalysis-3.0.0.dist-info/top_level.txt,sha256=cBbFgqO507F1sDD_MLoUoqR4voa-dwFBbDBvQa16qks,12
-benanalysis-3.0.0.dist-info/RECORD,,
+benanalysis.libs/libgslcblas-9bc550a1.so.0.0.0,sha256=41AFVJsq3UHlDwfbm5uEAz6t2gjRVMsmRDaQIJTVylo,1424553
+benanalysis.libs/libgsl-26724a50.so.25.1.0,sha256=pxurBpo6hNPBW_eFZPiFHomdeIVw8ypcr13UtQfvrzI,15884169
+benanalysis/_benpy_core.cpython-311-x86_64-linux-gnu.so,sha256=LcL1izgHOGaA3rNnfV6XA5dLkp1J4_XVmf85QnHPnv0,700953
+benanalysis/__init__.py,sha256=-6hoSNXbxc0H71CsX0zjm_vuzN7bHzu18oUvLog1c20,329
+benanalysis/__init__.pyi,sha256=_iXSdn1e4oYPB8TCbtxa5OAeHDAnfB1-0k9dSnyF7tI,7622
+benanalysis/utils/__init__.py,sha256=nL5gWb0J-qiIwg4H1UdWEQA120uQHR_NhL6-bE0KzRE,249
+benanalysis/utils/__init__.pyi,sha256=50K2JtssgNK5a3m4r197hQXGf5QQQTTO4aTL1IAP95s,716
+benanalysis/colorimetry/__init__.py,sha256=H-kUMdhDtTTNwEpRmV8EvHDJG6oloZtQJursOrOJFHk,195
+benanalysis/colorimetry/__init__.pyi,sha256=KVr64dw2oGkYLoXYTLfOWvzwpZChLtfmsitj9zRYJjg,9326
+benanalysis/data/__init__.py,sha256=8cX2lZ4xnykfRBxqEilfBzrZJzHcpkuhnTeqbIuubBQ,188
+benanalysis/data/__init__.pyi,sha256=Z7CuvE0StCFOdC0tNCOUseBBbCKMJQjJXjzwbBSSPco,120
+benanalysis/data/colorimetry/__init__.py,sha256=UXJAt3THeJo9LLNCwW0Zr_N5cm5mtuUt0mFTl3PSR5o,200
+benanalysis/data/colorimetry/__init__.pyi,sha256=nmxhZymE_MUrJEqAUGdcKWBq1x8wYcdGG-0TeQbIGwo,6568
+benanalysis/monochromator/__init__.py,sha256=zNW0JJ91QQ07LphnCdorwjm0AhhXXCP63zb77SYYV8s,197
+benanalysis/monochromator/__init__.pyi,sha256=p0K-_F4AjjSNg-pCwHPN3U76bCDS4xu6vn7ULizf2cY,131
+benanalysis/monochromator/slit_function/__init__.py,sha256=a4AM8LPiSVrgjnqDiHRuUxXamsko_wvJJLzIdoajUt8,65
+benanalysis/monochromator/slit_function/__init__.pyi,sha256=LCSC3h2To6aB6eTZ8BVDpJNEndvpu3NBfaWpA7UuVDg,862
+benanalysis-3.0.0rc1.dist-info/RECORD,,
+benanalysis-3.0.0rc1.dist-info/WHEEL,sha256=8KU227XctfdX2qUwyjQUO-ciQuZtmyPUCKmeGV6Byto,152
+benanalysis-3.0.0rc1.dist-info/top_level.txt,sha256=cBbFgqO507F1sDD_MLoUoqR4voa-dwFBbDBvQa16qks,12
+benanalysis-3.0.0rc1.dist-info/METADATA,sha256=btDfpAmyS9fF65OJAI0o2BY5nYJTRFk-zO34ZltUWEc,723
```

