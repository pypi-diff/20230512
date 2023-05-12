# Comparing `tmp/cloudshell-shell-standards-2.0.1.zip` & `tmp/cloudshell-shell-standards-2.0.2.zip`

## zipinfo {}

```diff
@@ -1,69 +1,70 @@
-Zip file size: 56850 bytes, number of entries: 67
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell_shell_standards.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/
--rw-r--r--  2.0 unx       34 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/MANIFEST.in
--rw-r--r--  2.0 unx     1134 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tox.ini
--rw-r--r--  2.0 unx       71 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/dev_requirements.txt
--rw-r--r--  2.0 unx      908 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/README.md
--rw-r--r--  2.0 unx      288 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/PKG-INFO
--rw-r--r--  2.0 unx       18 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/test_requirements.txt
--rw-r--r--  2.0 unx      810 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/setup.py
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/version.txt
--rw-r--r--  2.0 unx       38 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/setup.cfg
--rw-r--r--  2.0 unx    97622 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/LICENSE.htm
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/requirements.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell_shell_standards.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     2223 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell_shell_standards.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      288 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell_shell_standards.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell_shell_standards.egg-info/requires.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell_shell_standards.egg-info/top_level.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/__init__.py
--rw-r--r--  2.0 unx     1803 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/conftest.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell_standards/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/__init__.py
--rw-r--r--  2.0 unx     8480 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell_standards/test_autoload_details_builder.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell_standards/__init__.py
--rw-r--r--  2.0 unx     2248 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell_standards/test_autoload_generic_models.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/__init__.py
--rw-r--r--  2.0 unx     3160 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/test_resource_config_generic_models.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/resource_conf/
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/__init__.py
--rw-r--r--  2.0 unx     1205 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/test_utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/resource_conf/__init__.py
--rw-r--r--  2.0 unx     1574 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/resource_conf/test_simple_conf.py
--rw-r--r--  2.0 unx      509 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/resource_conf/test_enum.py
--rw-r--r--  2.0 unx     3730 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/resource_conf/test_attrs_converters.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/
--rw-r--r--  2.0 unx     1529 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/attribute_names.py
--rw-r--r--  2.0 unx     8113 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/autoload_generic_models.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/__init__.py
--rw-r--r--  2.0 unx     4027 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/resource_config_generic_models.py
--rw-r--r--  2.0 unx      178 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/exceptions.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/autoload/
--rw-r--r--  2.0 unx     1802 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/__init__.py
--rw-r--r--  2.0 unx      113 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/namespace_type.py
--rw-r--r--  2.0 unx     3190 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/attrs_converters.py
--rw-r--r--  2.0 unx      322 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/__init__.py
--rw-r--r--  2.0 unx     1396 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/resource_attr.py
--rw-r--r--  2.0 unx     7217 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/attrs_converter.py
--rw-r--r--  2.0 unx      361 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/enum.py
--rw-r--r--  2.0 unx     1840 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/base_conf.py
--rw-r--r--  2.0 unx     5207 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/autoload/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/autoload/__init__.py
--rw-r--r--  2.0 unx     4961 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/autoload/core_entities.py
--rw-r--r--  2.0 unx     5626 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/autoload/resource_model.py
--rw-r--r--  2.0 unx     3641 b- defN 23-Mar-31 13:55 cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/autoload/existed_resource_info.py
-67 files, 176102 bytes uncompressed, 42108 bytes compressed:  76.1%
+Zip file size: 57843 bytes, number of entries: 68
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell_shell_standards.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/
+-rw-r--r--  2.0 unx       34 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/MANIFEST.in
+-rw-r--r--  2.0 unx     1134 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tox.ini
+-rw-r--r--  2.0 unx       71 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/dev_requirements.txt
+-rw-r--r--  2.0 unx      908 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/README.md
+-rw-r--r--  2.0 unx      288 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/PKG-INFO
+-rw-r--r--  2.0 unx       18 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/test_requirements.txt
+-rw-r--r--  2.0 unx      810 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/setup.py
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/version.txt
+-rw-r--r--  2.0 unx       38 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/setup.cfg
+-rw-r--r--  2.0 unx    97622 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/LICENSE.htm
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/requirements.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell_shell_standards.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     2285 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell_shell_standards.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      288 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell_shell_standards.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell_shell_standards.egg-info/requires.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell_shell_standards.egg-info/top_level.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/__init__.py
+-rw-r--r--  2.0 unx     1803 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/conftest.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell_standards/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/__init__.py
+-rw-r--r--  2.0 unx     8480 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell_standards/test_autoload_details_builder.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell_standards/__init__.py
+-rw-r--r--  2.0 unx     2248 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell_standards/test_autoload_generic_models.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/__init__.py
+-rw-r--r--  2.0 unx     3160 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/test_resource_config_generic_models.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/resource_conf/
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/__init__.py
+-rw-r--r--  2.0 unx     1205 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/test_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/resource_conf/__init__.py
+-rw-r--r--  2.0 unx     1574 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/resource_conf/test_simple_conf.py
+-rw-r--r--  2.0 unx      509 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/resource_conf/test_enum.py
+-rw-r--r--  2.0 unx     3697 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/resource_conf/test_attrs_converters.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/
+-rw-r--r--  2.0 unx     1529 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/attribute_names.py
+-rw-r--r--  2.0 unx     8113 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/autoload_generic_models.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/__init__.py
+-rw-r--r--  2.0 unx     4027 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/resource_config_generic_models.py
+-rw-r--r--  2.0 unx      178 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/exceptions.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/autoload/
+-rw-r--r--  2.0 unx     1802 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/__init__.py
+-rw-r--r--  2.0 unx      113 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/namespace_type.py
+-rw-r--r--  2.0 unx     3069 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/attrs_converters.py
+-rw-r--r--  2.0 unx     3712 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/attrs_getter.py
+-rw-r--r--  2.0 unx      316 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/__init__.py
+-rw-r--r--  2.0 unx     1847 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/resource_attr.py
+-rw-r--r--  2.0 unx     4551 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/attrs_converter.py
+-rw-r--r--  2.0 unx      361 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/enum.py
+-rw-r--r--  2.0 unx     2092 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/base_conf.py
+-rw-r--r--  2.0 unx     5207 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/autoload/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/autoload/__init__.py
+-rw-r--r--  2.0 unx     4961 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/autoload/core_entities.py
+-rw-r--r--  2.0 unx     5626 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/autoload/resource_model.py
+-rw-r--r--  2.0 unx     3641 b- defN 23-Apr-04 14:16 cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/autoload/existed_resource_info.py
+68 files, 177753 bytes uncompressed, 42837 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -1,202 +1,205 @@
-Filename: cloudshell-shell-standards-2.0.1/
+Filename: cloudshell-shell-standards-2.0.2/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell_shell_standards.egg-info/
+Filename: cloudshell-shell-standards-2.0.2/cloudshell_shell_standards.egg-info/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/
+Filename: cloudshell-shell-standards-2.0.2/tests/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/MANIFEST.in
+Filename: cloudshell-shell-standards-2.0.2/MANIFEST.in
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tox.ini
+Filename: cloudshell-shell-standards-2.0.2/tox.ini
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/dev_requirements.txt
+Filename: cloudshell-shell-standards-2.0.2/dev_requirements.txt
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/README.md
+Filename: cloudshell-shell-standards-2.0.2/README.md
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/PKG-INFO
+Filename: cloudshell-shell-standards-2.0.2/PKG-INFO
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/test_requirements.txt
+Filename: cloudshell-shell-standards-2.0.2/test_requirements.txt
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/setup.py
+Filename: cloudshell-shell-standards-2.0.2/setup.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/version.txt
+Filename: cloudshell-shell-standards-2.0.2/version.txt
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/setup.cfg
+Filename: cloudshell-shell-standards-2.0.2/setup.cfg
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/LICENSE.htm
+Filename: cloudshell-shell-standards-2.0.2/LICENSE.htm
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/requirements.txt
+Filename: cloudshell-shell-standards-2.0.2/requirements.txt
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell_shell_standards.egg-info/dependency_links.txt
+Filename: cloudshell-shell-standards-2.0.2/cloudshell_shell_standards.egg-info/dependency_links.txt
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell_shell_standards.egg-info/SOURCES.txt
+Filename: cloudshell-shell-standards-2.0.2/cloudshell_shell_standards.egg-info/SOURCES.txt
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell_shell_standards.egg-info/PKG-INFO
+Filename: cloudshell-shell-standards-2.0.2/cloudshell_shell_standards.egg-info/PKG-INFO
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell_shell_standards.egg-info/requires.txt
+Filename: cloudshell-shell-standards-2.0.2/cloudshell_shell_standards.egg-info/requires.txt
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell_shell_standards.egg-info/top_level.txt
+Filename: cloudshell-shell-standards-2.0.2/cloudshell_shell_standards.egg-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/__init__.py
+Filename: cloudshell-shell-standards-2.0.2/tests/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/conftest.py
+Filename: cloudshell-shell-standards-2.0.2/tests/conftest.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell_standards/
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell_standards/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/__init__.py
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell_standards/test_autoload_details_builder.py
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell_standards/test_autoload_details_builder.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell_standards/__init__.py
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell_standards/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell_standards/test_autoload_generic_models.py
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell_standards/test_autoload_generic_models.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/__init__.py
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/__init__.py
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/test_resource_config_generic_models.py
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/test_resource_config_generic_models.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/resource_conf/
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/resource_conf/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/__init__.py
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/test_utils.py
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/test_utils.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/resource_conf/__init__.py
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/resource_conf/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/resource_conf/test_simple_conf.py
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/resource_conf/test_simple_conf.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/resource_conf/test_enum.py
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/resource_conf/test_enum.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/resource_conf/test_attrs_converters.py
+Filename: cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/resource_conf/test_attrs_converters.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/__init__.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/__init__.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/attribute_names.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/attribute_names.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/autoload_generic_models.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/autoload_generic_models.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/__init__.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/resource_config_generic_models.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/resource_config_generic_models.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/exceptions.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/exceptions.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/autoload/
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/autoload/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/utils.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/utils.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/__init__.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/namespace_type.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/namespace_type.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/attrs_converters.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/attrs_converters.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/__init__.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/attrs_getter.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/resource_attr.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/attrs_converter.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/resource_attr.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/enum.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/attrs_converter.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/base_conf.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/enum.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/autoload/utils.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/base_conf.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/autoload/__init__.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/autoload/utils.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/autoload/core_entities.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/autoload/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/autoload/resource_model.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/autoload/core_entities.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/autoload/existed_resource_info.py
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/autoload/resource_model.py
+Comment: 
+
+Filename: cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/autoload/existed_resource_info.py
 Comment: 
 
 Zip file comment:
```

## Comparing `cloudshell-shell-standards-2.0.1/tox.ini` & `cloudshell-shell-standards-2.0.2/tox.ini`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/README.md` & `cloudshell-shell-standards-2.0.2/README.md`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/setup.py` & `cloudshell-shell-standards-2.0.2/setup.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/LICENSE.htm` & `cloudshell-shell-standards-2.0.2/LICENSE.htm`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/cloudshell_shell_standards.egg-info/SOURCES.txt` & `cloudshell-shell-standards-2.0.2/cloudshell_shell_standards.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 cloudshell/shell/standards/core/autoload/core_entities.py
 cloudshell/shell/standards/core/autoload/existed_resource_info.py
 cloudshell/shell/standards/core/autoload/resource_model.py
 cloudshell/shell/standards/core/autoload/utils.py
 cloudshell/shell/standards/core/resource_conf/__init__.py
 cloudshell/shell/standards/core/resource_conf/attrs_converter.py
 cloudshell/shell/standards/core/resource_conf/attrs_converters.py
+cloudshell/shell/standards/core/resource_conf/attrs_getter.py
 cloudshell/shell/standards/core/resource_conf/base_conf.py
 cloudshell/shell/standards/core/resource_conf/enum.py
 cloudshell/shell/standards/core/resource_conf/resource_attr.py
 cloudshell_shell_standards.egg-info/PKG-INFO
 cloudshell_shell_standards.egg-info/SOURCES.txt
 cloudshell_shell_standards.egg-info/dependency_links.txt
 cloudshell_shell_standards.egg-info/requires.txt
```

## Comparing `cloudshell-shell-standards-2.0.1/tests/conftest.py` & `cloudshell-shell-standards-2.0.2/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/tests/cloudshell/shell_standards/test_autoload_details_builder.py` & `cloudshell-shell-standards-2.0.2/tests/cloudshell/shell_standards/test_autoload_details_builder.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/tests/cloudshell/shell_standards/test_autoload_generic_models.py` & `cloudshell-shell-standards-2.0.2/tests/cloudshell/shell_standards/test_autoload_generic_models.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/test_resource_config_generic_models.py` & `cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/test_resource_config_generic_models.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/test_utils.py` & `cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/test_utils.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/resource_conf/test_simple_conf.py` & `cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/resource_conf/test_simple_conf.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/tests/cloudshell/shell/standards/core/resource_conf/test_attrs_converters.py` & `cloudshell-shell-standards-2.0.2/tests/cloudshell/shell/standards/core/resource_conf/test_attrs_converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,22 +65,22 @@
     def test_convert_error_handling(self):
         class FloatConverter(AbsConverter):
             type_ = float
 
             def _convert(self) -> float:
                 return float(self.val)
 
-        meta = AttrMeta("test_attr", NameSpaceType.SHELL_NAME, False)
-        converter = FloatConverter("abc", meta)
+        attr_name = "test_attr"
+        converter = FloatConverter("abc", attr_name)
         with pytest.raises(AttributeConvertError) as exc_info:
             converter.convert()
         assert exc_info.value.name == "test_attr"
         assert exc_info.value.str_type == "float"
         assert exc_info.value.val == "abc"
-        assert f"attribute '{meta.name}' should be of type float" in str(exc_info.value)
+        assert f"attribute '{attr_name}' should be of type float" in str(exc_info.value)
 
     def test_is_supported_type_invalid(self):
         class IntConverter(AbsConverter):
             type_ = int
 
             def _convert(self) -> int:
                 return int(self.val)
```

## Comparing `cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/attribute_names.py` & `cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/attribute_names.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/autoload_generic_models.py` & `cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/autoload_generic_models.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/resource_config_generic_models.py` & `cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/resource_config_generic_models.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/utils.py` & `cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/utils.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/attrs_converters.py` & `cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/attrs_converters.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import re
 from abc import ABC, abstractmethod
 from collections.abc import Iterator
 from typing import ClassVar
 
 from attrs import define
 
-from cloudshell.shell.standards.core.resource_conf.resource_attr import AttrMeta
 from cloudshell.shell.standards.core.utils import split_list_of_values
 from cloudshell.shell.standards.exceptions import ResourceConfigException
 
 
 @define
 class AttributeConvertError(ResourceConfigException):
     name: str
@@ -24,17 +23,17 @@
             f"{self.str_type} but the value '{self.val}' was provided"
         )
 
 
 class AbsConverter(ABC):
     type_: ClassVar[type]
 
-    def __init__(self, val: str, meta: AttrMeta):
+    def __init__(self, val: str, name: str):
         self.val = val
-        self.meta = meta
+        self.name = name
 
     @classmethod
     def get_str_type(cls) -> str:
         return cls.type_.__name__
 
     @classmethod
     def is_supported_type(cls, str_type: str) -> bool:
@@ -44,17 +43,15 @@
     def _convert(self) -> type_:
         ...
 
     def convert(self) -> type_:
         try:
             return self._convert()
         except Exception as e:
-            raise AttributeConvertError(
-                self.meta.name, self.get_str_type(), self.val
-            ) from e
+            raise AttributeConvertError(self.name, self.get_str_type(), self.val) from e
 
 
 class AbsCollectionConverter(AbsConverter):
     @classmethod
     def is_supported_type(cls, str_type: str) -> bool:
         raise NotImplementedError
```

## Comparing `cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/resource_attr.py` & `cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/resource_attr.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,56 @@
 from __future__ import annotations
 
 import enum
 from typing import TYPE_CHECKING, Any, Callable, ClassVar, Sequence, TypeVar, Union
 
 from attrs import field, frozen, setters
+from typing_extensions import Self
 
 from cloudshell.shell.standards.core.namespace_type import NameSpaceType
+from cloudshell.shell.standards.exceptions import ResourceConfigException
 
 if TYPE_CHECKING:
     # used for TypeVar
     from attrs import Attribute  # noqa: F401
 
     from cloudshell.shell.standards.core.resource_conf import BaseConfig  # noqa: F401
 
 
 CONFIG_TYPE = TypeVar("CONFIG_TYPE", bound="BaseConfig")
 VALUE_TYPE = TypeVar("VALUE_TYPE")
 VALIDATOR_TYPE = Callable[[CONFIG_TYPE, "Attribute[VALUE_TYPE]", VALUE_TYPE], None]
 VALIDATOR_ARG = Union[VALIDATOR_TYPE, Sequence[VALIDATOR_TYPE]]
 
 
+class WithoutMeta(ResourceConfigException):
+    pass
+
+
 class _Raise(enum.Enum):
     RAISE = enum.auto()
 
 
 RAISE = _Raise.RAISE
 
 
 @frozen
 class AttrMeta:
     DICT_KEY: ClassVar[str] = "_standard"
     name: str
     namespace_type: NameSpaceType
     is_password: bool
 
+    @classmethod
+    def from_field(cls, f: Attribute) -> Self:
+        meta = f.metadata.get(cls.DICT_KEY)
+        if not meta:
+            raise WithoutMeta
+        return meta
+
 
 def attr(
     name: str,
     namespace: NameSpaceType = NameSpaceType.SHELL_NAME,
     is_password: bool = False,
     default: Any = RAISE,
     converter: Callable[[Any], Any] | None = None,
@@ -48,7 +61,11 @@
         default=default,
         kw_only=True,
         on_setattr=setters.frozen,
         converter=converter,
         validator=validator,
         repr=not is_password,
     )
+
+
+def get_str_type(f: Attribute) -> str:
+    return f.type if isinstance(f.type, str) else f.type.__name__
```

## Comparing `cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/resource_conf/base_conf.py` & `cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/resource_conf/base_conf.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 
 from attrs import define
 from typing_extensions import Self
 
 from cloudshell.api.cloudshell_api import CloudShellAPISession
 
 from cloudshell.shell.standards.core.resource_conf.attrs_converter import (
+    AbsModelAttrsConverter,
+    ModelAttrsConverter,
+)
+from cloudshell.shell.standards.core.resource_conf.attrs_getter import (
     RESOURCE_CONTEXT_TYPES,
-    AbsResourceAttrsConverter,
-    ResourceAttrsConverter,
+    ResourceContextAttrsGetter,
 )
 
 
 @define(slots=False, str=False)
 class BaseConfig:
     """Base class for creating resource configs.
 
@@ -24,40 +27,44 @@
     @define(slots=False, str=False)
     class Config(BaseConfig):
         str_res_attr: str = attr("Str Attribute")
         int_res_attr: int = attr("Int Attribute")
         enum_res_attr: EnumSubClass = attr("Enum Attribute")
     """
 
-    _CONVERTER: ClassVar[type[AbsResourceAttrsConverter]] = ResourceAttrsConverter
+    _CONVERTER: ClassVar[type[AbsModelAttrsConverter]] = ModelAttrsConverter
+    _ATTR_GETTER: ClassVar[
+        type[ResourceContextAttrsGetter]
+    ] = ResourceContextAttrsGetter
     name: str
     shell_name: str
     family_name: str
     address: str
     api: CloudShellAPISession
 
     def __str__(self) -> str:
         cls_name = type(self).__name__
         return f"{cls_name}({self.name})"
 
     @classmethod
     def from_context(
         cls, context: RESOURCE_CONTEXT_TYPES, api: CloudShellAPISession
     ) -> Self:
-        converter = cls._CONVERTER(context, cls, _password_decryptor(api))
+        attrs = cls._ATTR_GETTER(cls, password_decryptor(api), context).get_attrs()
+        converter = cls._CONVERTER(cls, attrs)
 
         return cls(
             name=context.resource.name,
             shell_name=context.resource.model,
             family_name=context.resource.family,
             address=context.resource.address,
             api=api,
             # this should return kwargs but BaseConfig doesn't have any
-            **converter.get_attrs(),  # noqa
+            **converter.convert(),  # noqa
         )
 
 
-def _password_decryptor(api: CloudShellAPISession) -> Callable[[str], str]:
+def password_decryptor(api: CloudShellAPISession) -> Callable[[str], str]:
     def wrapped(val: str) -> str:
         return api.DecryptPassword(val).Value
 
     return wrapped
```

## Comparing `cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/autoload/utils.py` & `cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/autoload/utils.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/autoload/core_entities.py` & `cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/autoload/core_entities.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/autoload/resource_model.py` & `cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/autoload/resource_model.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.1/cloudshell/shell/standards/core/autoload/existed_resource_info.py` & `cloudshell-shell-standards-2.0.2/cloudshell/shell/standards/core/autoload/existed_resource_info.py`

 * *Files identical despite different names*

