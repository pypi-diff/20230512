# Comparing `tmp/SimpleTFLinter-0.1.0.tar.gz` & `tmp/SimpleTFLinter-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleTFLinter-0.1.0.tar", last modified: Wed May 10 13:14:11 2023, max compression
+gzip compressed data, was "SimpleTFLinter-0.2.2.tar", last modified: Fri May 12 03:15:12 2023, max compression
```

## Comparing `SimpleTFLinter-0.1.0.tar` & `SimpleTFLinter-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-05-10 13:14:11.054631 SimpleTFLinter-0.1.0/
--rw-r--r--   0 wwang2     (501) staff       (20)     1069 2023-05-03 23:40:57.000000 SimpleTFLinter-0.1.0/LICENSE
--rw-r--r--   0 wwang2     (501) staff       (20)     6596 2023-05-10 13:14:11.054486 SimpleTFLinter-0.1.0/PKG-INFO
--rw-r--r--   0 wwang2     (501) staff       (20)     5569 2023-05-10 12:54:17.000000 SimpleTFLinter-0.1.0/README.md
--rw-r--r--   0 wwang2     (501) staff       (20)       38 2023-05-10 13:14:11.054683 SimpleTFLinter-0.1.0/setup.cfg
--rw-r--r--   0 wwang2     (501) staff       (20)     1587 2023-05-10 13:03:25.000000 SimpleTFLinter-0.1.0/setup.py
-drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-05-10 13:14:11.050928 SimpleTFLinter-0.1.0/src/
-drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-05-10 13:14:11.052228 SimpleTFLinter-0.1.0/src/SimpleTFLinter.egg-info/
--rw-r--r--   0 wwang2     (501) staff       (20)     6596 2023-05-10 13:14:11.000000 SimpleTFLinter-0.1.0/src/SimpleTFLinter.egg-info/PKG-INFO
--rw-r--r--   0 wwang2     (501) staff       (20)      474 2023-05-10 13:14:11.000000 SimpleTFLinter-0.1.0/src/SimpleTFLinter.egg-info/SOURCES.txt
--rw-r--r--   0 wwang2     (501) staff       (20)        1 2023-05-10 13:14:11.000000 SimpleTFLinter-0.1.0/src/SimpleTFLinter.egg-info/dependency_links.txt
--rw-r--r--   0 wwang2     (501) staff       (20)       47 2023-05-10 13:14:11.000000 SimpleTFLinter-0.1.0/src/SimpleTFLinter.egg-info/entry_points.txt
--rw-r--r--   0 wwang2     (501) staff       (20)       32 2023-05-10 13:14:11.000000 SimpleTFLinter-0.1.0/src/SimpleTFLinter.egg-info/requires.txt
--rw-r--r--   0 wwang2     (501) staff       (20)       21 2023-05-10 13:14:11.000000 SimpleTFLinter-0.1.0/src/SimpleTFLinter.egg-info/top_level.txt
--rw-r--r--   0 wwang2     (501) staff       (20)     2301 2023-05-10 12:37:28.000000 SimpleTFLinter-0.1.0/src/cli.py
-drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-05-10 13:14:11.054013 SimpleTFLinter-0.1.0/src/simple_tf_linter/
--rw-r--r--   0 wwang2     (501) staff       (20)      125 2023-05-10 07:45:28.000000 SimpleTFLinter-0.1.0/src/simple_tf_linter/__init__.py
--rw-r--r--   0 wwang2     (501) staff       (20)      885 2023-05-10 05:56:04.000000 SimpleTFLinter-0.1.0/src/simple_tf_linter/compare_path.py
--rw-r--r--   0 wwang2     (501) staff       (20)      714 2023-05-10 06:01:54.000000 SimpleTFLinter-0.1.0/src/simple_tf_linter/iterate_dict.py
--rw-r--r--   0 wwang2     (501) staff       (20)     2794 2023-05-10 05:56:04.000000 SimpleTFLinter-0.1.0/src/simple_tf_linter/key_value_rule.py
--rw-r--r--   0 wwang2     (501) staff       (20)     2474 2023-05-09 20:42:55.000000 SimpleTFLinter-0.1.0/src/simple_tf_linter/linter_basic.py
+drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-05-12 03:15:12.483083 SimpleTFLinter-0.2.2/
+-rw-r--r--   0 wwang2     (501) staff       (20)     1069 2023-05-03 23:40:57.000000 SimpleTFLinter-0.2.2/LICENSE
+-rw-r--r--   0 wwang2     (501) staff       (20)     6592 2023-05-12 03:15:12.482935 SimpleTFLinter-0.2.2/PKG-INFO
+-rw-r--r--   0 wwang2     (501) staff       (20)     5565 2023-05-10 13:19:42.000000 SimpleTFLinter-0.2.2/README.md
+-rw-r--r--   0 wwang2     (501) staff       (20)       38 2023-05-12 03:15:12.483134 SimpleTFLinter-0.2.2/setup.cfg
+-rw-r--r--   0 wwang2     (501) staff       (20)     1587 2023-05-12 03:14:29.000000 SimpleTFLinter-0.2.2/setup.py
+drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-05-12 03:15:12.479596 SimpleTFLinter-0.2.2/src/
+drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-05-12 03:15:12.480716 SimpleTFLinter-0.2.2/src/SimpleTFLinter.egg-info/
+-rw-r--r--   0 wwang2     (501) staff       (20)     6592 2023-05-12 03:15:12.000000 SimpleTFLinter-0.2.2/src/SimpleTFLinter.egg-info/PKG-INFO
+-rw-r--r--   0 wwang2     (501) staff       (20)      474 2023-05-12 03:15:12.000000 SimpleTFLinter-0.2.2/src/SimpleTFLinter.egg-info/SOURCES.txt
+-rw-r--r--   0 wwang2     (501) staff       (20)        1 2023-05-12 03:15:12.000000 SimpleTFLinter-0.2.2/src/SimpleTFLinter.egg-info/dependency_links.txt
+-rw-r--r--   0 wwang2     (501) staff       (20)       47 2023-05-12 03:15:12.000000 SimpleTFLinter-0.2.2/src/SimpleTFLinter.egg-info/entry_points.txt
+-rw-r--r--   0 wwang2     (501) staff       (20)       32 2023-05-12 03:15:12.000000 SimpleTFLinter-0.2.2/src/SimpleTFLinter.egg-info/requires.txt
+-rw-r--r--   0 wwang2     (501) staff       (20)       21 2023-05-12 03:15:12.000000 SimpleTFLinter-0.2.2/src/SimpleTFLinter.egg-info/top_level.txt
+-rw-r--r--   0 wwang2     (501) staff       (20)     2295 2023-05-12 03:06:29.000000 SimpleTFLinter-0.2.2/src/cli.py
+drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-05-12 03:15:12.482580 SimpleTFLinter-0.2.2/src/simple_tf_linter/
+-rw-r--r--   0 wwang2     (501) staff       (20)      125 2023-05-10 07:45:28.000000 SimpleTFLinter-0.2.2/src/simple_tf_linter/__init__.py
+-rw-r--r--   0 wwang2     (501) staff       (20)      885 2023-05-10 05:56:04.000000 SimpleTFLinter-0.2.2/src/simple_tf_linter/compare_path.py
+-rw-r--r--   0 wwang2     (501) staff       (20)      714 2023-05-10 06:01:54.000000 SimpleTFLinter-0.2.2/src/simple_tf_linter/iterate_dict.py
+-rw-r--r--   0 wwang2     (501) staff       (20)     2794 2023-05-10 05:56:04.000000 SimpleTFLinter-0.2.2/src/simple_tf_linter/key_value_rule.py
+-rw-r--r--   0 wwang2     (501) staff       (20)     2474 2023-05-09 20:42:55.000000 SimpleTFLinter-0.2.2/src/simple_tf_linter/linter_basic.py
```

### Comparing `SimpleTFLinter-0.1.0/LICENSE` & `SimpleTFLinter-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SimpleTFLinter-0.1.0/PKG-INFO` & `SimpleTFLinter-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleTFLinter
-Version: 0.1.0
+Version: 0.2.2
 Summary: Simple Terraform Linter is a lightweight command-line tool for checking Terraform configuration files against custom rules. It supports input from Terraform folders or JSON files, with easy customization and extensibility through user-defined rules defined in YAML files.
 Home-page: https://github.com/AutomationLover/TerraformLinter
 Author: William Wang
 Author-email: williamwangatsydney@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -33,19 +33,19 @@
 
 ## Installation
 
 1. Make sure you have Python 3 installed on your computer.
 2. Install the Terraform Linter CLI package using pip:
 
 ```
-pip install simple-tf-linter
+pip install simpleTFLinter
 ```
 ## Usage
 
-After installing the `simple-tf-linter` package, you can use the `simple_tf_linter` command to run the linter.
+After installing the `simpleTFLinter` package, you can use the `simple_tf_linter` command to run the linter.
 
 1. Set up your rule YAML file with the desired rules. You can either create your own or use the default `.tf_linter_rule.yaml` provided in the `examples` directory.
 2. Run the Terraform Linter CLI using the following command:
 
 ```
 simple_tf_linter -p [input_path] -r [rule_yaml_path] -t [input_type]
 ```
```

### Comparing `SimpleTFLinter-0.1.0/README.md` & `SimpleTFLinter-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 ## Installation
 
 1. Make sure you have Python 3 installed on your computer.
 2. Install the Terraform Linter CLI package using pip:
 
 ```
-pip install simple-tf-linter
+pip install simpleTFLinter
 ```
 ## Usage
 
-After installing the `simple-tf-linter` package, you can use the `simple_tf_linter` command to run the linter.
+After installing the `simpleTFLinter` package, you can use the `simple_tf_linter` command to run the linter.
 
 1. Set up your rule YAML file with the desired rules. You can either create your own or use the default `.tf_linter_rule.yaml` provided in the `examples` directory.
 2. Run the Terraform Linter CLI using the following command:
 
 ```
 simple_tf_linter -p [input_path] -r [rule_yaml_path] -t [input_type]
 ```
```

### Comparing `SimpleTFLinter-0.1.0/setup.py` & `SimpleTFLinter-0.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="SimpleTFLinter",
-    version="0.1.0",
+    version="0.2.2",
     author="William Wang",
     author_email="williamwangatsydney@gmail.com",
     description="Simple Terraform Linter is a lightweight command-line tool for checking Terraform configuration files against custom rules. It supports input from Terraform folders or JSON files, with easy customization and extensibility through user-defined rules defined in YAML files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AutomationLover/TerraformLinter",
     packages=find_packages("src"),
```

### Comparing `SimpleTFLinter-0.1.0/src/SimpleTFLinter.egg-info/PKG-INFO` & `SimpleTFLinter-0.2.2/src/SimpleTFLinter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleTFLinter
-Version: 0.1.0
+Version: 0.2.2
 Summary: Simple Terraform Linter is a lightweight command-line tool for checking Terraform configuration files against custom rules. It supports input from Terraform folders or JSON files, with easy customization and extensibility through user-defined rules defined in YAML files.
 Home-page: https://github.com/AutomationLover/TerraformLinter
 Author: William Wang
 Author-email: williamwangatsydney@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -33,19 +33,19 @@
 
 ## Installation
 
 1. Make sure you have Python 3 installed on your computer.
 2. Install the Terraform Linter CLI package using pip:
 
 ```
-pip install simple-tf-linter
+pip install simpleTFLinter
 ```
 ## Usage
 
-After installing the `simple-tf-linter` package, you can use the `simple_tf_linter` command to run the linter.
+After installing the `simpleTFLinter` package, you can use the `simple_tf_linter` command to run the linter.
 
 1. Set up your rule YAML file with the desired rules. You can either create your own or use the default `.tf_linter_rule.yaml` provided in the `examples` directory.
 2. Run the Terraform Linter CLI using the following command:
 
 ```
 simple_tf_linter -p [input_path] -r [rule_yaml_path] -t [input_type]
 ```
```

### Comparing `SimpleTFLinter-0.1.0/src/cli.py` & `SimpleTFLinter-0.2.2/src/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,23 +23,23 @@
     # Get the Terraform code path or JSON file path
     input_path = os.path.abspath(args.path)
 
     # Get the rule YAML location
     if args.rule_yaml:
         rule_yaml_path = os.path.abspath(args.rule_yaml)
     else:
-        current_folder_yaml = os.path.join('', '../examples/.tf_linter_rule.yaml')
-        home_folder_yaml = os.path.join(os.path.expanduser('~'), '../examples/.tf_linter_rule.yaml')
+        current_folder_yaml = os.path.join(os.getcwd(), '.tf_linter_rule.yaml')
+        home_folder_yaml = os.path.join(os.path.expanduser('~'), '/.tf_linter_rule.yaml')
         if os.path.exists(current_folder_yaml):
             rule_yaml_path = os.path.abspath(current_folder_yaml)
         elif os.path.exists(home_folder_yaml):
             rule_yaml_path = home_folder_yaml
         else:
             raise FileNotFoundError('.tf_linter_rule.yaml file not found in the current folder or ~/.')
-
+        
     # Print the paths for demonstration purposes
     print("Input Path:", input_path)
     print("Rule YAML Path:", rule_yaml_path)
 
     # Add your linter logic here
     linter = TerraformLinter()
     rules = read_rules_from_yaml(rule_yaml_path)
```

### Comparing `SimpleTFLinter-0.1.0/src/simple_tf_linter/compare_path.py` & `SimpleTFLinter-0.2.2/src/simple_tf_linter/compare_path.py`

 * *Files identical despite different names*

### Comparing `SimpleTFLinter-0.1.0/src/simple_tf_linter/iterate_dict.py` & `SimpleTFLinter-0.2.2/src/simple_tf_linter/iterate_dict.py`

 * *Files identical despite different names*

### Comparing `SimpleTFLinter-0.1.0/src/simple_tf_linter/key_value_rule.py` & `SimpleTFLinter-0.2.2/src/simple_tf_linter/key_value_rule.py`

 * *Files identical despite different names*

### Comparing `SimpleTFLinter-0.1.0/src/simple_tf_linter/linter_basic.py` & `SimpleTFLinter-0.2.2/src/simple_tf_linter/linter_basic.py`

 * *Files identical despite different names*

