# Comparing `tmp/dialog-workflow-local-python-package-0.0.13.tar.gz` & `tmp/dialog-workflow-local-python-package-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-python-package-0.0.13.tar", last modified: Fri May 12 06:37:51 2023, max compression
+gzip compressed data, was "dialog-workflow-local-python-package-0.0.14.tar", last modified: Fri May 12 07:20:38 2023, max compression
```

## Comparing `dialog-workflow-local-python-package-0.0.13.tar` & `dialog-workflow-local-python-package-0.0.14.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:37:51.544427 dialog-workflow-local-python-package-0.0.13/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-12 06:37:51.544427 dialog-workflow-local-python-package-0.0.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-12 06:37:35.000000 dialog-workflow-local-python-package-0.0.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:37:51.540427 dialog-workflow-local-python-package-0.0.13/dialog_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-05-12 06:37:35.000000 dialog-workflow-local-python-package-0.0.13/dialog_workflow/Act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-12 06:37:35.000000 dialog-workflow-local-python-package-0.0.13/dialog_workflow/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-12 06:37:35.000000 dialog-workflow-local-python-package-0.0.13/dialog_workflow/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-12 06:37:35.000000 dialog-workflow-local-python-package-0.0.13/dialog_workflow/TablesAsObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 06:37:35.000000 dialog-workflow-local-python-package-0.0.13/dialog_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-12 06:37:35.000000 dialog-workflow-local-python-package-0.0.13/dialog_workflow/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-05-12 06:37:35.000000 dialog-workflow-local-python-package-0.0.13/dialog_workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:37:51.544427 dialog-workflow-local-python-package-0.0.13/dialog_workflow_local_python_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-12 06:37:51.000000 dialog-workflow-local-python-package-0.0.13/dialog_workflow_local_python_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-12 06:37:51.000000 dialog-workflow-local-python-package-0.0.13/dialog_workflow_local_python_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 06:37:51.000000 dialog-workflow-local-python-package-0.0.13/dialog_workflow_local_python_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 06:37:51.000000 dialog-workflow-local-python-package-0.0.13/dialog_workflow_local_python_package.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-12 06:37:35.000000 dialog-workflow-local-python-package-0.0.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 06:37:51.544427 dialog-workflow-local-python-package-0.0.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-12 06:37:35.000000 dialog-workflow-local-python-package-0.0.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:20:38.702298 dialog-workflow-local-python-package-0.0.14/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-12 07:20:38.702298 dialog-workflow-local-python-package-0.0.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-12 07:20:26.000000 dialog-workflow-local-python-package-0.0.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:20:38.702298 dialog-workflow-local-python-package-0.0.14/dialog_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-05-12 07:20:26.000000 dialog-workflow-local-python-package-0.0.14/dialog_workflow/Act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-12 07:20:26.000000 dialog-workflow-local-python-package-0.0.14/dialog_workflow/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-12 07:20:26.000000 dialog-workflow-local-python-package-0.0.14/dialog_workflow/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-12 07:20:26.000000 dialog-workflow-local-python-package-0.0.14/dialog_workflow/TablesAsObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:20:26.000000 dialog-workflow-local-python-package-0.0.14/dialog_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-12 07:20:26.000000 dialog-workflow-local-python-package-0.0.14/dialog_workflow/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-05-12 07:20:26.000000 dialog-workflow-local-python-package-0.0.14/dialog_workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:20:38.702298 dialog-workflow-local-python-package-0.0.14/dialog_workflow_local_python_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-12 07:20:38.000000 dialog-workflow-local-python-package-0.0.14/dialog_workflow_local_python_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-12 07:20:38.000000 dialog-workflow-local-python-package-0.0.14/dialog_workflow_local_python_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 07:20:38.000000 dialog-workflow-local-python-package-0.0.14/dialog_workflow_local_python_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 07:20:38.000000 dialog-workflow-local-python-package-0.0.14/dialog_workflow_local_python_package.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-12 07:20:26.000000 dialog-workflow-local-python-package-0.0.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 07:20:38.702298 dialog-workflow-local-python-package-0.0.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-12 07:20:26.000000 dialog-workflow-local-python-package-0.0.14/setup.py
```

### Comparing `dialog-workflow-local-python-package-0.0.13/dialog_workflow/Act.py` & `dialog-workflow-local-python-package-0.0.14/dialog_workflow/Act.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-python-package-0.0.13/dialog_workflow/Constants.py` & `dialog-workflow-local-python-package-0.0.14/dialog_workflow/Constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     PRESENT_CHILD_GROUPS_NAMES_BY_ID = 13
     PRESENT_GROUPS_WITH_CERTAIN_TEXT = 14
     INSERT_MISSING_DATA = 15
 
 class communication_type_enum(Enum):
     CONSOLE = 1
     WEBSOCKET = 2
-COMMUNICATION_TYPE = 1
+COMMUNICATION_TYPE = 2
 
 VARIABLE_NAMES_DICT = {1 : "Person Id" , 2 : "User Id", 3 : "Profile Id", 4 : "Lang Code", 
                        5 : "Name Prefix", 6 : "First Name", 7 : "Middle Name" , 
                        8 : "Last Name", 9 : "Name Suffix",  10 : "Full Name", 
                        11 : "Country", 12 : "State" , 13 : "County" , 14 : "City", 
                        15 : "Neighborhood", 16 : "Street", 17 : "House", 18 : "Suite/Apartment", 
                        19 : "Zip Code", 20 : "Post Result", 21 : "Age", 22 : "Result"}
```

### Comparing `dialog-workflow-local-python-package-0.0.13/dialog_workflow/DialogWorkflow.py` & `dialog-workflow-local-python-package-0.0.14/dialog_workflow/DialogWorkflow.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-python-package-0.0.13/dialog_workflow/TablesAsObjects.py` & `dialog-workflow-local-python-package-0.0.14/dialog_workflow/TablesAsObjects.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-python-package-0.0.13/dialog_workflow/test.py` & `dialog-workflow-local-python-package-0.0.14/dialog_workflow/test.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-python-package-0.0.13/dialog_workflow/utils.py` & `dialog-workflow-local-python-package-0.0.14/dialog_workflow/utils.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-python-package-0.0.13/setup.py` & `dialog-workflow-local-python-package-0.0.14/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='dialog-workflow-local-python-package',  
-     version='0.0.13',
+     version='0.0.14',
      author="Circles",
      author_email="info@circle.life",
      description="PyPI Package for dialog workflow",
      long_description="This is a package for running the dialog workflow",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

