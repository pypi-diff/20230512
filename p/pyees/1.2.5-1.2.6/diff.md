# Comparing `tmp/pyees-1.2.5.tar.gz` & `tmp/pyees-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.2.5.tar", last modified: Thu May 11 18:59:49 2023, max compression
+gzip compressed data, was "pyees-1.2.6.tar", last modified: Fri May 12 12:17:01 2023, max compression
```

## Comparing `pyees-1.2.5.tar` & `pyees-1.2.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 18:59:49.409227 pyees-1.2.5/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-05-11 18:59:49.417206 pyees-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 18:59:49.101053 pyees-1.2.5/pyees/
--rw-rw-rw-   0        0        0      323 2023-05-11 18:59:34.000000 pyees-1.2.5/pyees/__init__.py
--rw-rw-rw-   0        0        0    12829 2023-05-11 09:38:32.000000 pyees-1.2.5/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.2.5/pyees/profilePyees.py
--rw-rw-rw-   0        0        0     9126 2023-05-11 09:38:14.000000 pyees-1.2.5/pyees/prop.py
--rw-rw-rw-   0        0        0    17661 2023-05-11 18:51:21.000000 pyees-1.2.5/pyees/readData.py
--rw-rw-rw-   0        0        0    10193 2023-04-21 12:20:02.000000 pyees-1.2.5/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.2.5/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7669 2023-04-27 10:39:41.000000 pyees-1.2.5/pyees/testFit.py
--rw-rw-rw-   0        0        0    12431 2023-05-11 09:11:30.000000 pyees-1.2.5/pyees/testProp.py
--rw-rw-rw-   0        0        0     1059 2023-05-11 18:59:48.854708 pyees-1.2.5/pyees/testPyees.py
--rw-rw-rw-   0        0        0    15674 2023-04-24 15:13:29.000000 pyees-1.2.5/pyees/testReadData.py
--rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.2.5/pyees/testSolve.py
--rw-rw-rw-   0        0        0     8958 2023-04-15 19:26:44.000000 pyees-1.2.5/pyees/testUnit.py
--rw-rw-rw-   0        0        0    81533 2023-05-11 18:59:49.041211 pyees-1.2.5/pyees/testVariable.py
--rw-rw-rw-   0        0        0    44518 2023-05-11 12:21:25.000000 pyees-1.2.5/pyees/unit.py
--rw-rw-rw-   0        0        0    35130 2023-05-11 11:54:28.000000 pyees-1.2.5/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-05-11 18:59:49.362354 pyees-1.2.5/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-05-11 18:59:47.000000 pyees-1.2.5/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-05-11 18:59:48.000000 pyees-1.2.5/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 18:59:47.000000 pyees-1.2.5/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-05-11 18:59:47.000000 pyees-1.2.5/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-11 18:59:47.000000 pyees-1.2.5/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-11 18:59:49.460091 pyees-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-05-11 18:59:39.000000 pyees-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 12:17:00.895885 pyees-1.2.6/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.2.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-05-12 12:17:00.958459 pyees-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 12:17:00.023430 pyees-1.2.6/pyees/
+-rw-rw-rw-   0        0        0      320 2023-05-12 12:16:06.000000 pyees-1.2.6/pyees/__init__.py
+-rw-rw-rw-   0        0        0    12829 2023-05-11 09:38:32.000000 pyees-1.2.6/pyees/fit.py
+-rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.2.6/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0     9126 2023-05-11 09:38:14.000000 pyees-1.2.6/pyees/prop.py
+-rw-rw-rw-   0        0        0    17726 2023-05-12 12:15:59.000000 pyees-1.2.6/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10193 2023-04-21 12:20:02.000000 pyees-1.2.6/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.2.6/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7669 2023-04-27 10:39:41.000000 pyees-1.2.6/pyees/testFit.py
+-rw-rw-rw-   0        0        0    12431 2023-05-11 09:11:30.000000 pyees-1.2.6/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1059 2023-05-11 18:48:30.000000 pyees-1.2.6/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    15674 2023-04-24 15:13:29.000000 pyees-1.2.6/pyees/testReadData.py
+-rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.2.6/pyees/testSolve.py
+-rw-rw-rw-   0        0        0     9094 2023-05-12 06:37:13.000000 pyees-1.2.6/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    81858 2023-05-12 06:34:53.000000 pyees-1.2.6/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    44518 2023-05-11 12:21:25.000000 pyees-1.2.6/pyees/unit.py
+-rw-rw-rw-   0        0        0    35130 2023-05-11 11:54:28.000000 pyees-1.2.6/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-05-12 12:17:00.755256 pyees-1.2.6/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-05-12 12:16:54.000000 pyees-1.2.6/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-05-12 12:16:55.000000 pyees-1.2.6/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 12:16:54.000000 pyees-1.2.6/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-05-12 12:16:54.000000 pyees-1.2.6/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-12 12:16:54.000000 pyees-1.2.6/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-12 12:17:01.020891 pyees-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-05-12 12:16:49.000000 pyees-1.2.6/setup.py
```

### Comparing `pyees-1.2.5/LICENSE.txt` & `pyees-1.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.2.5/PKG-INFO` & `pyees-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.2.5
+Version: 1.2.6
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.2.5/README.md` & `pyees-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.2.5/pyees/fit.py` & `pyees-1.2.6/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.5/pyees/profilePyees.py` & `pyees-1.2.6/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.5/pyees/prop.py` & `pyees-1.2.6/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.5/pyees/readData.py` & `pyees-1.2.6/pyees/sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     from variable import variable, scalarVariable
 except ImportError:
     from pyees.variable import variable, scalarVariable
 
 
 
 def fileFromSheets(sheets, fileName):
+    if not isinstance(sheets, list):
+        sheets = [sheets]
     _fileFromSheets(sheets, fileName)
 
 class _fileFromSheets():
     def __init__(self, sheets, fileName) -> None:
         
         self.fileName = fileName
         self.sheets = sheets
```

### Comparing `pyees-1.2.5/pyees/solve.py` & `pyees-1.2.6/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.5/pyees/stackOverflowODR.py` & `pyees-1.2.6/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.5/pyees/testFit.py` & `pyees-1.2.6/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.5/pyees/testProp.py` & `pyees-1.2.6/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.5/pyees/testPyees.py` & `pyees-1.2.6/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.5/pyees/testReadData.py` & `pyees-1.2.6/pyees/testReadData.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.5/pyees/testSolve.py` & `pyees-1.2.6/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.5/pyees/testUnit.py` & `pyees-1.2.6/pyees/testUnit.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,27 +134,32 @@
         converter = a.getConverter('J/kg-F')
         self.assertAlmostEqual(converter.convert(1, useOffset=False), 555.555555555555)
 
         a = unit('K')
         converter = a.getConverter('F')
         self.assertAlmostEqual(converter.convert(300, useOffset=True), 80.33)
 
+        a = unit('mm2')
+        converter = a.getConverter('m2')
+        self.assertAlmostEqual(converter.convert(1), 1/1000 * 1/1000)
+
+
         a = unit('A')
         b = unit('V')
         c = a * b
         c = unit(c)
         converter = c.getConverter('W')
         
         a = unit('A')
         b = unit('ohm')
         c = a * b
         c = unit(c)
         converter = c.getConverter('V')
         
-        self.assertAlmostEqual(converter.convert(1, useOffset=True), 1)
+        self.assertEqual(converter.convert(1, useOffset=True), 1)
 
         with self.assertRaises(Exception) as context:
             a = unit('mu')
         self.assertEqual('''The unit (mu) was not found. Therefore it was interpreted as a prefix and a unit. The prefix was identified as "mu" and the unit was identified as "1". However, the unit "1" cannot have a prefix''', str(context.exception))
 
         with self.assertRaises(Exception) as context:
             a = unit('1/M')
```

### Comparing `pyees-1.2.5/pyees/testVariable.py` & `pyees-1.2.6/pyees/testVariable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1273,25 +1273,33 @@
         ub = np.array([1.2, 2.4, 4.7], dtype = float)
         uab = np.array([2, 3, 4], dtype = float)
 
         uc = np.sqrt((dcda * ua)**2 + (dcdb * ub)**2 + 2 * dcda * dcdb * uab)
         np.testing.assert_equal(c.uncert, uc)
 
     def testConvert(self):
-        a = variable(1, 'km')
-        b = variable(1, 'm')
+        a = variable(1, 'km', 0.1)
+        b = variable(1, 'm', 0.1)
         c = a * b
         c.convert('mm2')
+        self.assertEqual(c.value, 1e9)
+        self.assertEqual(c.unit, 'mm2')
+        self.assertEqual(c.uncert,  np.sqrt((1 * 1000 * 0.1 * 1000*1000)**2 + (1 * 1000*1000 * 0.1 * 1000)**2))
         
-        
-        diameter = variable(40, 'cm')
+        diameter = variable(40, 'cm', 0.2)
         area = np.pi / 4 * diameter ** 2
         area.convert('m2')
         self.assertEqual(area.value, 0.12566370614359172953850573)
-        self.assertEqual(area.unit, 'm2')       
+        self.assertEqual(area.unit, 'm2')
+        self.assertEqual(area.uncert, np.sqrt((2 * np.pi / 4 * 0.4 * 0.002)**2))
+        
+        
+        
+        
+         
         
 
     def testCompare(self):
         a = variable(1, 'm')
         b = variable([2, 3, 4], 'm')
         np.testing.assert_equal(a < b, [True, True, True])
         np.testing.assert_equal(a <= b, [True, True, True])
```

### Comparing `pyees-1.2.5/pyees/unit.py` & `pyees-1.2.6/pyees/unit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.5/pyees/variable.py` & `pyees-1.2.6/pyees/variable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.5/pyees.egg-info/PKG-INFO` & `pyees-1.2.6/pyees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.2.5
+Version: 1.2.6
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.2.5/setup.py` & `pyees-1.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.2.5',
+    version='1.2.6',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

