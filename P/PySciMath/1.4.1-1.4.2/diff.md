# Comparing `tmp/PySciMath-1.4.1.tar.gz` & `tmp/PySciMath-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySciMath-1.4.1.tar", last modified: Thu May 11 15:32:21 2023, max compression
+gzip compressed data, was "PySciMath-1.4.2.tar", last modified: Thu May 11 16:19:21 2023, max compression
```

## Comparing `PySciMath-1.4.1.tar` & `PySciMath-1.4.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 15:32:21.231861 PySciMath-1.4.1/
--rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2591 2023-05-11 15:32:21.230862 PySciMath-1.4.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-11 15:32:21.211923 PySciMath-1.4.1/PySciMath/
--rw-rw-rw-   0        0        0     1720 2023-05-11 15:05:50.000000 PySciMath-1.4.1/PySciMath/Arithmetic.py
--rw-rw-rw-   0        0        0      677 2023-05-10 14:22:10.000000 PySciMath-1.4.1/PySciMath/ComplexNumbers.py
--rw-rw-rw-   0        0        0     4286 2023-05-10 14:05:32.000000 PySciMath-1.4.1/PySciMath/CoordinateGeometry.py
--rw-rw-rw-   0        0        0    17742 2023-05-11 15:13:15.000000 PySciMath-1.4.1/PySciMath/Geometry.py
--rw-rw-rw-   0        0        0      568 2023-05-10 10:26:42.000000 PySciMath-1.4.1/PySciMath/Quadratic.py
--rw-rw-rw-   0        0        0     1272 2023-05-11 15:14:07.000000 PySciMath-1.4.1/PySciMath/Statistics.py
--rw-rw-rw-   0        0        0      558 2023-05-10 09:51:46.000000 PySciMath-1.4.1/PySciMath/Trigonometry.py
--rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.4.1/PySciMath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:32:21.226874 PySciMath-1.4.1/PySciMath.egg-info/
--rw-rw-rw-   0        0        0     2591 2023-05-11 15:32:21.000000 PySciMath-1.4.1/PySciMath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2023-05-11 15:32:21.000000 PySciMath-1.4.1/PySciMath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 15:32:21.000000 PySciMath-1.4.1/PySciMath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-11 15:32:21.000000 PySciMath-1.4.1/PySciMath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2077 2023-05-11 15:31:15.000000 PySciMath-1.4.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 15:32:21.232857 PySciMath-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-05-11 15:31:24.000000 PySciMath-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:19:21.637057 PySciMath-1.4.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.4.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2591 2023-05-11 16:19:21.635061 PySciMath-1.4.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-11 16:19:21.616114 PySciMath-1.4.2/PySciMath/
+-rw-rw-rw-   0        0        0     2090 2023-05-11 16:14:33.000000 PySciMath-1.4.2/PySciMath/Arithmetic.py
+-rw-rw-rw-   0        0        0     4286 2023-05-10 14:05:32.000000 PySciMath-1.4.2/PySciMath/CoordinateGeometry.py
+-rw-rw-rw-   0        0        0    17742 2023-05-11 15:13:15.000000 PySciMath-1.4.2/PySciMath/Geometry.py
+-rw-rw-rw-   0        0        0      568 2023-05-10 10:26:42.000000 PySciMath-1.4.2/PySciMath/Quadratic.py
+-rw-rw-rw-   0        0        0     1272 2023-05-11 15:14:07.000000 PySciMath-1.4.2/PySciMath/Statistics.py
+-rw-rw-rw-   0        0        0      558 2023-05-10 09:51:46.000000 PySciMath-1.4.2/PySciMath/Trigonometry.py
+-rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.4.2/PySciMath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:19:21.631072 PySciMath-1.4.2/PySciMath.egg-info/
+-rw-rw-rw-   0        0        0     2591 2023-05-11 16:19:21.000000 PySciMath-1.4.2/PySciMath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-05-11 16:19:21.000000 PySciMath-1.4.2/PySciMath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 16:19:21.000000 PySciMath-1.4.2/PySciMath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 16:19:21.000000 PySciMath-1.4.2/PySciMath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2077 2023-05-11 16:16:40.000000 PySciMath-1.4.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 16:19:21.638054 PySciMath-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      903 2023-05-11 16:16:37.000000 PySciMath-1.4.2/setup.py
```

### Comparing `PySciMath-1.4.1/LICENSE.txt` & `PySciMath-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySciMath-1.4.1/PKG-INFO` & `PySciMath-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.4.1
+Version: 1.4.2
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/pyscimath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Calculations
@@ -18,15 +18,15 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.4.1</br>
+**Version** - 1.4.2</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
```

### Comparing `PySciMath-1.4.1/PySciMath/Arithmetic.py` & `PySciMath-1.4.2/PySciMath/Arithmetic.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 # PySciMath - Arithmetic
 
 ''' This is the "Arithmetic" sub-module. '''
 
+# Imports
+import cmath
+
+# Constants
+iota = "Iota, which is also referred to as 'i'. It's value is √-1."
+
 # Functions - Simple Arithmetic Operations
 def add(num1, num2): return num1 + num2
 def subtract(num1, num2): return num1 - num2
 def multiply(num1, num2): return num1 * num2
 def divide(num1, num2): return num1 / num2
 def modulus(num1, num2): return num1 % num2
 def floorDivision(num1, num2): return num1 // num2
 def power(base, exponent): return base ** exponent
 
+# Functions - Complex Numbers
+def modulusComplex(z): return abs(z)
+def conjugateComplex(z): return z.conjugate()
+def multiplicativeInverseComplex(z): return conjugateComplex(z) / power(modulusComplex(z), 2)
+def polarComplex(z): return cmath.polar(z)
+
 # Functions - Squares and Cubes
 def square(number): return power(number, 2)
 def cube(number): return power(number, 3)
 def squareRoot(number): return number ** 0.5
 def cubeRoot(number): return number ** (1/3)
 
 # Functions - Odd and Even
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PySciMath-1.4.1/PySciMath/CoordinateGeometry.py` & `PySciMath-1.4.2/PySciMath/CoordinateGeometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.4.1/PySciMath/Geometry.py` & `PySciMath-1.4.2/PySciMath/Geometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.4.1/PySciMath/Quadratic.py` & `PySciMath-1.4.2/PySciMath/Quadratic.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.4.1/PySciMath/Statistics.py` & `PySciMath-1.4.2/PySciMath/Statistics.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.4.1/PySciMath/Trigonometry.py` & `PySciMath-1.4.2/PySciMath/Trigonometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.4.1/PySciMath.egg-info/PKG-INFO` & `PySciMath-1.4.2/PySciMath.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.4.1
+Version: 1.4.2
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/pyscimath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Calculations
@@ -18,15 +18,15 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.4.1</br>
+**Version** - 1.4.2</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
```

### Comparing `PySciMath-1.4.1/README.md` & `PySciMath-1.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.4.1</br>
+**Version** - 1.4.2</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
```

### Comparing `PySciMath-1.4.1/setup.py` & `PySciMath-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PySciMath",
-    version="1.4.1",
+    version="1.4.2",
     description="PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
```

