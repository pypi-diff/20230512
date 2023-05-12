# Comparing `tmp/troposphere_awscommunity_applicationautoscaling_scheduledaction-0.0.1.tar.gz` & `tmp/troposphere_awscommunity_applicationautoscaling_scheduledaction-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troposphere_awscommunity_applicationautoscaling_scheduledaction-0.0.1.tar", max compression
+gzip compressed data, was "troposphere_awscommunity_applicationautoscaling_scheduledaction-0.1.1.tar", max compression
```

## Comparing `troposphere_awscommunity_applicationautoscaling_scheduledaction-0.0.1.tar` & `troposphere_awscommunity_applicationautoscaling_scheduledaction-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1090 2023-05-12 06:59:39.930028 troposphere_awscommunity_applicationautoscaling_scheduledaction-0.0.1/LICENSE
--rw-r--r--   0        0        0     1804 2023-05-12 06:58:32.550209 troposphere_awscommunity_applicationautoscaling_scheduledaction-0.0.1/README.md
--rw-r--r--   0        0        0     2172 2023-05-12 07:12:14.565224 troposphere_awscommunity_applicationautoscaling_scheduledaction-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1540 2023-05-12 07:10:21.301899 troposphere_awscommunity_applicationautoscaling_scheduledaction-0.0.1/troposphere_awscommunity_applicationautoscaling_scheduledaction/__init__.py
--rw-r--r--   0        0        0      952 2023-05-12 07:04:54.625923 troposphere_awscommunity_applicationautoscaling_scheduledaction-0.0.1/troposphere_awscommunity_applicationautoscaling_scheduledaction/validators.py
--rw-r--r--   0        0        0     3143 1970-01-01 00:00:00.000000 troposphere_awscommunity_applicationautoscaling_scheduledaction-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-05-12 06:59:39.930028 troposphere_awscommunity_applicationautoscaling_scheduledaction-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1875 2023-05-12 07:17:51.402244 troposphere_awscommunity_applicationautoscaling_scheduledaction-0.1.1/README.md
+-rw-r--r--   0        0        0     2172 2023-05-12 07:21:09.881622 troposphere_awscommunity_applicationautoscaling_scheduledaction-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1540 2023-05-12 07:21:09.881622 troposphere_awscommunity_applicationautoscaling_scheduledaction-0.1.1/troposphere_awscommunity_applicationautoscaling_scheduledaction/__init__.py
+-rw-r--r--   0        0        0      986 2023-05-12 07:16:03.163952 troposphere_awscommunity_applicationautoscaling_scheduledaction-0.1.1/troposphere_awscommunity_applicationautoscaling_scheduledaction/validators.py
+-rw-r--r--   0        0        0     3214 1970-01-01 00:00:00.000000 troposphere_awscommunity_applicationautoscaling_scheduledaction-0.1.1/PKG-INFO
```

### Comparing `troposphere_awscommunity_applicationautoscaling_scheduledaction-0.0.1/LICENSE` & `troposphere_awscommunity_applicationautoscaling_scheduledaction-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `troposphere_awscommunity_applicationautoscaling_scheduledaction-0.0.1/README.md` & `troposphere_awscommunity_applicationautoscaling_scheduledaction-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 ```yaml
 Resources:
   MyAction:
     Properties:
       ResourceId: table/awscommunityscheduledactiontesttable
       ScalableDimension: dynamodb:table:ReadCapacityUnits
       ScalableTargetAction:
-        MaxCapacity: null
-        MinCapacity: null
-      Schedule: null
+        MaxCapacity: 4
+        MinCapacity: 1
+      Schedule: cron(5 2 ? * FRI)
       ScheduledActionName: cfn-testing-resource
       ServiceNamespace: dynamodb
       Timezone: Europe/London
+    Type: AwsCommunity::ApplicationAutoscaling::ScheduledAction
 ```
```

### Comparing `troposphere_awscommunity_applicationautoscaling_scheduledaction-0.0.1/pyproject.toml` & `troposphere_awscommunity_applicationautoscaling_scheduledaction-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troposphere-awscommunity-applicationautoscaling-scheduledaction"
-version = "0.0.1"
+version = "0.1.1"
 description = "Troposphere resource for AwsCommunity::ApplicationAutoscaling::ScheduledAction"
 authors = ["John \"Preston\" Mille <john@ews-network.net>"]
 readme = "README.md"
 packages = [{include = "troposphere_awscommunity_applicationautoscaling_scheduledaction"}]
 keywords = ["troposphere", "aws-cloudformation"]
 classifiers = [
   "Development Status :: 3 - Alpha",
@@ -52,15 +52,15 @@
 use_parentheses = true
 known_first_party = "kelvin"
 
 [tool.tbump]
 github_url = "https://github.com/JohnPreston/troposphere-awscommunity-applicationautoscaling-scheduledaction.git"
 
 [tool.tbump.version]
-current = "0.0.1"
+current = "0.1.1"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `troposphere_awscommunity_applicationautoscaling_scheduledaction-0.0.1/troposphere_awscommunity_applicationautoscaling_scheduledaction/__init__.py` & `troposphere_awscommunity_applicationautoscaling_scheduledaction-0.1.1/troposphere_awscommunity_applicationautoscaling_scheduledaction/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #  SPDX-License-Identifier: MIT
 #  Copyright 2023 John Mille <john@ews-network.net>
 
 __author__ = """John Mille"""
 __email__ = "john@ews-network.net"
-__version__ = "0.0.1"
+__version__ = "0.1.1"
 
 
 """Troposphere resource to cover AwsCommunity::ApplicationAutoscaling::ScheduledAction"""
 
 from troposphere import AWSObject, AWSProperty, PropsDictType
 
 from troposphere_awscommunity_applicationautoscaling_scheduledaction.validators import (
```

### Comparing `troposphere_awscommunity_applicationautoscaling_scheduledaction-0.0.1/troposphere_awscommunity_applicationautoscaling_scheduledaction/validators.py` & `troposphere_awscommunity_applicationautoscaling_scheduledaction-0.1.1/troposphere_awscommunity_applicationautoscaling_scheduledaction/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,20 @@
     """Validates the Min & Max Capacity are valid"""
     if not isinstance(value, (int, AWSHelperFn)):
         raise TypeError("MinCapacity/MaxCapacity must be a positive integer", int)
     if isinstance(value, int) and value < 0:
         raise ValueError(
             "MinCapacity/MaxCapacity must be a positive integer. Got", value
         )
+    return value
 
 
 def validate_schedule(value: str):
     if not isinstance(value, (str, AWSHelperFn)):
         raise TypeError(f"Schedule must be a string. Got {type(value)}", str)
     if isinstance(value, str) and not (
         value.startswith("at(")
         or value.startswith("cron(")
         or value.startswith("rate(")
     ):
         raise ValueError(f"Schedule start with either at(|cron(|rate(. Got {value}")
+    return value
```

### Comparing `troposphere_awscommunity_applicationautoscaling_scheduledaction-0.0.1/PKG-INFO` & `troposphere_awscommunity_applicationautoscaling_scheduledaction-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troposphere-awscommunity-applicationautoscaling-scheduledaction
-Version: 0.0.1
+Version: 0.1.1
 Summary: Troposphere resource for AwsCommunity::ApplicationAutoscaling::ScheduledAction
 License: LICENSE
 Keywords: troposphere,aws-cloudformation
 Author: John "Preston" Mille
 Author-email: john@ews-network.net
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -71,15 +71,16 @@
 ```yaml
 Resources:
   MyAction:
     Properties:
       ResourceId: table/awscommunityscheduledactiontesttable
       ScalableDimension: dynamodb:table:ReadCapacityUnits
       ScalableTargetAction:
-        MaxCapacity: null
-        MinCapacity: null
-      Schedule: null
+        MaxCapacity: 4
+        MinCapacity: 1
+      Schedule: cron(5 2 ? * FRI)
       ScheduledActionName: cfn-testing-resource
       ServiceNamespace: dynamodb
       Timezone: Europe/London
+    Type: AwsCommunity::ApplicationAutoscaling::ScheduledAction
 ```
```

