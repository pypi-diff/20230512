# Comparing `tmp/PyHaier-0.1.7.tar.gz` & `tmp/PyHaier-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHaier-0.1.7.tar", last modified: Fri May 12 11:36:10 2023, max compression
+gzip compressed data, was "PyHaier-0.1.8.tar", last modified: Fri May 12 11:51:15 2023, max compression
```

## Comparing `PyHaier-0.1.7.tar` & `PyHaier-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-05-12 11:36:10.302902 PyHaier-0.1.7/
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)     5932 2023-05-12 11:36:10.302902 PyHaier-0.1.7/PKG-INFO
-drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-05-12 11:36:10.301902 PyHaier-0.1.7/PyHaier/
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      164 2023-05-12 11:34:28.000000 PyHaier-0.1.7/PyHaier/GetCHTemp.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)       24 2023-05-12 11:34:28.000000 PyHaier-0.1.7/PyHaier/GetCompFreq.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      174 2023-05-12 11:34:28.000000 PyHaier-0.1.7/PyHaier/GetDHWCurTemp.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      155 2023-05-12 11:34:28.000000 PyHaier-0.1.7/PyHaier/GetDHWTemp.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      271 2023-05-12 11:34:28.000000 PyHaier-0.1.7/PyHaier/GetMode.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      776 2023-05-12 11:34:28.000000 PyHaier-0.1.7/PyHaier/GetState.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      570 2023-05-12 11:34:28.000000 PyHaier-0.1.7/PyHaier/GetTwiTwo.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      458 2023-05-12 11:34:28.000000 PyHaier-0.1.7/PyHaier/SetCHTemp.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      463 2023-05-12 11:34:28.000000 PyHaier-0.1.7/PyHaier/SetDHWTemp.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      248 2023-05-12 11:34:28.000000 PyHaier-0.1.7/PyHaier/SetMode.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)     1283 2023-05-12 11:34:28.000000 PyHaier-0.1.7/PyHaier/SetState.py
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      399 2023-05-12 11:34:28.000000 PyHaier-0.1.7/PyHaier/__init__.py
-drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-05-12 11:36:10.302902 PyHaier-0.1.7/PyHaier.egg-info/
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)     5932 2023-05-12 11:36:10.000000 PyHaier-0.1.7/PyHaier.egg-info/PKG-INFO
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      401 2023-05-12 11:36:10.000000 PyHaier-0.1.7/PyHaier.egg-info/SOURCES.txt
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)        1 2023-05-12 11:36:10.000000 PyHaier-0.1.7/PyHaier.egg-info/dependency_links.txt
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)        8 2023-05-12 11:36:10.000000 PyHaier-0.1.7/PyHaier.egg-info/top_level.txt
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)     5325 2023-05-12 11:34:28.000000 PyHaier-0.1.7/README.md
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)      608 2023-05-12 11:34:28.000000 PyHaier-0.1.7/pyproject.toml
--rw-r--r--   0 jacekb    (1000) jacekb    (1000)       38 2023-05-12 11:36:10.302902 PyHaier-0.1.7/setup.cfg
+drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-05-12 11:51:15.559497 PyHaier-0.1.8/
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)     5969 2023-05-12 11:51:15.559497 PyHaier-0.1.8/PKG-INFO
+drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-05-12 11:51:15.558497 PyHaier-0.1.8/PyHaier/
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      164 2023-05-12 11:50:48.000000 PyHaier-0.1.8/PyHaier/GetCHTemp.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)       24 2023-05-12 11:50:48.000000 PyHaier-0.1.8/PyHaier/GetCompFreq.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      174 2023-05-12 11:50:48.000000 PyHaier-0.1.8/PyHaier/GetDHWCurTemp.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      155 2023-05-12 11:50:48.000000 PyHaier-0.1.8/PyHaier/GetDHWTemp.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      271 2023-05-12 11:50:48.000000 PyHaier-0.1.8/PyHaier/GetMode.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      776 2023-05-12 11:50:48.000000 PyHaier-0.1.8/PyHaier/GetState.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      570 2023-05-12 11:50:48.000000 PyHaier-0.1.8/PyHaier/GetTwiTwo.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      458 2023-05-12 11:50:48.000000 PyHaier-0.1.8/PyHaier/SetCHTemp.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      463 2023-05-12 11:50:48.000000 PyHaier-0.1.8/PyHaier/SetDHWTemp.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      248 2023-05-12 11:50:48.000000 PyHaier-0.1.8/PyHaier/SetMode.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)     1282 2023-05-12 11:50:48.000000 PyHaier-0.1.8/PyHaier/SetState.py
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      399 2023-05-12 11:50:48.000000 PyHaier-0.1.8/PyHaier/__init__.py
+drwxr-xr-x   0 jacekb    (1000) jacekb    (1000)        0 2023-05-12 11:51:15.558497 PyHaier-0.1.8/PyHaier.egg-info/
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)     5969 2023-05-12 11:51:15.000000 PyHaier-0.1.8/PyHaier.egg-info/PKG-INFO
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      401 2023-05-12 11:51:15.000000 PyHaier-0.1.8/PyHaier.egg-info/SOURCES.txt
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)        1 2023-05-12 11:51:15.000000 PyHaier-0.1.8/PyHaier.egg-info/dependency_links.txt
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)        8 2023-05-12 11:51:15.000000 PyHaier-0.1.8/PyHaier.egg-info/top_level.txt
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)     5362 2023-05-12 11:50:48.000000 PyHaier-0.1.8/README.md
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)      608 2023-05-12 11:50:48.000000 PyHaier-0.1.8/pyproject.toml
+-rw-r--r--   0 jacekb    (1000) jacekb    (1000)       38 2023-05-12 11:51:15.559497 PyHaier-0.1.8/setup.cfg
```

### Comparing `PyHaier-0.1.7/PKG-INFO` & `PyHaier-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyHaier
-Version: 0.1.7
+Version: 0.1.8
 Summary: Very simple library to manipulate the basic parameters of the Haier heat pump.
 Author-email: Jacek Brzozowski <jacekbrzozowski.pld@gmail.com>
 Project-URL: Homepage, https://github.com/ktostam/PyHaier
 Project-URL: Bug Tracker, https://github.com/ktostam/PyHaier/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -25,14 +25,17 @@
 
 [<img width="150px" src="https://buycoffee.to/btn/buycoffeeto-btn-primary.svg">](https://buycoffee.to/jacekbrzozz)
 
 ## Support
 For support, join our Discord channel https://discord.gg/7aF38puD
 
 ## Version
+### 0.1.8
+- fix for previous fix :D
+
 ### 0.1.7
 - fix turning on pump in SetState function
 
 ### 0.1.6
 - Just for pip upload
 
 ### 0.1.5
```

### Comparing `PyHaier-0.1.7/PyHaier/GetState.py` & `PyHaier-0.1.8/PyHaier/GetState.py`

 * *Files identical despite different names*

### Comparing `PyHaier-0.1.7/PyHaier/GetTwiTwo.py` & `PyHaier-0.1.8/PyHaier/GetTwiTwo.py`

 * *Files identical despite different names*

### Comparing `PyHaier-0.1.7/PyHaier/SetState.py` & `PyHaier-0.1.8/PyHaier/SetState.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         if new == "off":
             if int(hex(current[0])[4:6])%2 == 1:
                 state=int(hex(current[0])[4:6])-1
             else:
                 return -1
         elif new == "on":
-            if int(hex(current[0])[4:6])%2) == 0:
+            if int(hex(current[0])[4:6])%2 == 0:
                 state=int(hex(current[0])[4:6])+1
             else:
                 return -1
         elif new == "C":
             state=3
         elif new == "H":
             state=5
```

### Comparing `PyHaier-0.1.7/PyHaier.egg-info/PKG-INFO` & `PyHaier-0.1.8/PyHaier.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyHaier
-Version: 0.1.7
+Version: 0.1.8
 Summary: Very simple library to manipulate the basic parameters of the Haier heat pump.
 Author-email: Jacek Brzozowski <jacekbrzozowski.pld@gmail.com>
 Project-URL: Homepage, https://github.com/ktostam/PyHaier
 Project-URL: Bug Tracker, https://github.com/ktostam/PyHaier/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -25,14 +25,17 @@
 
 [<img width="150px" src="https://buycoffee.to/btn/buycoffeeto-btn-primary.svg">](https://buycoffee.to/jacekbrzozz)
 
 ## Support
 For support, join our Discord channel https://discord.gg/7aF38puD
 
 ## Version
+### 0.1.8
+- fix for previous fix :D
+
 ### 0.1.7
 - fix turning on pump in SetState function
 
 ### 0.1.6
 - Just for pip upload
 
 ### 0.1.5
```

### Comparing `PyHaier-0.1.7/README.md` & `PyHaier-0.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 [<img width="150px" src="https://buycoffee.to/btn/buycoffeeto-btn-primary.svg">](https://buycoffee.to/jacekbrzozz)
 
 ## Support
 For support, join our Discord channel https://discord.gg/7aF38puD
 
 ## Version
+### 0.1.8
+- fix for previous fix :D
+
 ### 0.1.7
 - fix turning on pump in SetState function
 
 ### 0.1.6
 - Just for pip upload
 
 ### 0.1.5
```

### Comparing `PyHaier-0.1.7/pyproject.toml` & `PyHaier-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PyHaier"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Jacek Brzozowski", email="jacekbrzozowski.pld@gmail.com" },
 ]
 description = "Very simple library to manipulate the basic parameters of the Haier heat pump."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

