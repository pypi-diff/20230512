# Comparing `tmp/tomato-cooker-0.0.1.tar.gz` & `tmp/tomato-cooker-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomato-cooker-0.0.1.tar", last modified: Fri May  5 19:12:41 2023, max compression
+gzip compressed data, was "tomato-cooker-0.1.0.tar", last modified: Fri May 12 10:23:14 2023, max compression
```

## Comparing `tomato-cooker-0.0.1.tar` & `tomato-cooker-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:12:41.280001 tomato-cooker-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-05 19:12:27.000000 tomato-cooker-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-05 19:12:41.280001 tomato-cooker-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-05 19:12:27.000000 tomato-cooker-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 19:12:41.280001 tomato-cooker-0.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-05-05 19:12:27.000000 tomato-cooker-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:12:41.280001 tomato-cooker-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-05 19:12:27.000000 tomato-cooker-0.0.1/tests/test_grill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:12:41.280001 tomato-cooker-0.0.1/tomato_cooker/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 19:12:27.000000 tomato-cooker-0.0.1/tomato_cooker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:12:41.280001 tomato-cooker-0.0.1/tomato_cooker/grill/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-05 19:12:27.000000 tomato-cooker-0.0.1/tomato_cooker/grill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-05 19:12:27.000000 tomato-cooker-0.0.1/tomato_cooker/grill/grill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:12:41.280001 tomato-cooker-0.0.1/tomato_cooker/models/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-05 19:12:27.000000 tomato-cooker-0.0.1/tomato_cooker/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-05 19:12:27.000000 tomato-cooker-0.0.1/tomato_cooker/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:12:41.280001 tomato-cooker-0.0.1/tomato_cooker/models/tomatic/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-05 19:12:27.000000 tomato-cooker-0.0.1/tomato_cooker/models/tomatic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 19:12:27.000000 tomato-cooker-0.0.1/tomato_cooker/models/tomatic/tomatic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:12:41.280001 tomato-cooker-0.0.1/tomato_cooker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-05 19:12:27.000000 tomato-cooker-0.0.1/tomato_cooker/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:12:41.280001 tomato-cooker-0.0.1/tomato_cooker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-05 19:12:41.000000 tomato-cooker-0.0.1/tomato_cooker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-05 19:12:41.000000 tomato-cooker-0.0.1/tomato_cooker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:12:41.000000 tomato-cooker-0.0.1/tomato_cooker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 19:12:41.000000 tomato-cooker-0.0.1/tomato_cooker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 19:12:41.000000 tomato-cooker-0.0.1/tomato_cooker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:12:41.000000 tomato-cooker-0.0.1/tomato_cooker.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:23:14.551118 tomato-cooker-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-12 10:23:14.551118 tomato-cooker-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:23:14.555117 tomato-cooker-0.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1555 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:23:14.547118 tomato-cooker-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tests/test_grill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:23:14.547118 tomato-cooker-0.1.0/tomato_cooker/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:23:14.551118 tomato-cooker-0.1.0/tomato_cooker/grill/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/grill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/grill/grill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:23:14.551118 tomato-cooker-0.1.0/tomato_cooker/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:23:14.551118 tomato-cooker-0.1.0/tomato_cooker/models/tomatic/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/models/tomatic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/models/tomatic/phone_grill.mzn
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/models/tomatic/tomatic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:23:14.551118 tomato-cooker-0.1.0/tomato_cooker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:23:14.551118 tomato-cooker-0.1.0/tomato_cooker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-12 10:23:14.000000 tomato-cooker-0.1.0/tomato_cooker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-12 10:23:14.000000 tomato-cooker-0.1.0/tomato_cooker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:23:14.000000 tomato-cooker-0.1.0/tomato_cooker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-12 10:23:14.000000 tomato-cooker-0.1.0/tomato_cooker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 10:23:14.000000 tomato-cooker-0.1.0/tomato_cooker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:23:14.000000 tomato-cooker-0.1.0/tomato_cooker.egg-info/zip-safe
```

### Comparing `tomato-cooker-0.0.1/LICENSE` & `tomato-cooker-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tomato-cooker-0.0.1/PKG-INFO` & `tomato-cooker-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomato-cooker
-Version: 0.0.1
+Version: 0.1.0
 Summary: Minizinc problem solver
 Home-page: https://github.com/Som-Energia/Som-Minizinc
 Author: Som Energia SCCL
 Author-email: info@somenergia.coop
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tomato-cooker-0.0.1/README.md` & `tomato-cooker-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tomato-cooker-0.0.1/setup.py` & `tomato-cooker-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,17 @@
     packages=find_packages(exclude=["*[tT]est*"]),
     python_requires=">=3.8.0",
     zip_safe=True,
     setup_requires=[],
     install_requires=required,
     extras_require=extras,
     scripts=[],
+    package_data={
+        'tomato_cooker.models.tomatic': ['*mzn']
+    },
     include_package_data=True,
     test_suite="pytest",
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Intended Audience :: Developers",
```

### Comparing `tomato-cooker-0.0.1/tests/test_grill.py` & `tomato-cooker-0.1.0/tests/test_grill.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,14 +33,45 @@
         for slot in day:
             assert (
                 tomatic_instance.nLinies - tomatic_instance.nNingus
                 <= len(slot)
                 <= tomatic_instance.nLinies
             )
 
+@pytest.mark.asyncio
+async def test__grid_tomato_cooker__cook__especial_one_day_two_consecutive_slots_same_person(
+    # given a solver
+    tomato_cooker,
+    # problem instance
+    tomatic_instance_one_day_three_people,
+):
+    # When we start a new grid execution
+    results = await tomato_cooker.cook(tomatic_instance_one_day_three_people)
+
+    # Then a valid phone schedule is generated
+    assert len(results.solution.ocupacioSlot) == tomatic_instance_one_day_three_people.nDies
+    for day in results.solution.ocupacioSlot:
+        assert len(day) == tomatic_instance_one_day_three_people.nSlots
+        for slot in day:
+            assert (
+                tomatic_instance_one_day_three_people.nLinies - tomatic_instance_one_day_three_people.nNingus
+                <= len(slot)
+                <= tomatic_instance_one_day_three_people.nLinies
+            )
+            assert (
+                1 in results.solution.ocupacioSlot[0][0]
+            )
+            assert (
+                2 in results.solution.ocupacioSlot[0][1] or
+                3 in results.solution.ocupacioSlot[0][1]
+            )
+            assert (
+                2 in results.solution.ocupacioSlot[0][2] or
+                3 in results.solution.ocupacioSlot[0][2]
+            )
 
 @pytest.mark.asyncio
 async def test__grid_tomato_cooker__indisponibilities(
     # given a solver
     tomato_cooker,
     # problem instance
     tomatic_instance,
```

### Comparing `tomato-cooker-0.0.1/tomato_cooker/grill/grill.py` & `tomato-cooker-0.1.0/tomato_cooker/grill/grill.py`

 * *Files identical despite different names*

### Comparing `tomato-cooker-0.0.1/tomato_cooker/utils/__init__.py` & `tomato-cooker-0.1.0/tomato_cooker/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tomato-cooker-0.0.1/tomato_cooker.egg-info/PKG-INFO` & `tomato-cooker-0.1.0/tomato_cooker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomato-cooker
-Version: 0.0.1
+Version: 0.1.0
 Summary: Minizinc problem solver
 Home-page: https://github.com/Som-Energia/Som-Minizinc
 Author: Som Energia SCCL
 Author-email: info@somenergia.coop
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tomato-cooker-0.0.1/tomato_cooker.egg-info/SOURCES.txt` & `tomato-cooker-0.1.0/tomato_cooker.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -10,9 +10,10 @@
 tomato_cooker.egg-info/top_level.txt
 tomato_cooker.egg-info/zip-safe
 tomato_cooker/grill/__init__.py
 tomato_cooker/grill/grill.py
 tomato_cooker/models/__init__.py
 tomato_cooker/models/base.py
 tomato_cooker/models/tomatic/__init__.py
+tomato_cooker/models/tomatic/phone_grill.mzn
 tomato_cooker/models/tomatic/tomatic.py
 tomato_cooker/utils/__init__.py
```

