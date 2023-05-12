# Comparing `tmp/featuremonkey3-0.1.0.tar.gz` & `tmp/featuremonkey3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featuremonkey3-0.1.0.tar", max compression
+gzip compressed data, was "featuremonkey3-0.1.1.tar", max compression
```

## Comparing `featuremonkey3-0.1.0.tar` & `featuremonkey3-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1083 2023-04-21 20:54:01.546860 featuremonkey3-0.1.0/LICENSE
--rw-r--r--   0        0        0      617 2023-04-21 20:54:01.547095 featuremonkey3-0.1.0/README.rst
--rw-r--r--   0        0        0      647 2023-05-11 19:54:48.923937 featuremonkey3-0.1.0/featuremonkey3/__init__.py
--rw-r--r--   0        0        0    12719 2023-04-21 20:54:01.550842 featuremonkey3-0.1.0/featuremonkey3/composer.py
--rw-r--r--   0        0        0     1017 2023-04-21 20:54:01.550951 featuremonkey3-0.1.0/featuremonkey3/helpers.py
--rw-r--r--   0        0        0     5553 2023-05-11 19:54:48.920345 featuremonkey3-0.1.0/featuremonkey3/importhooks.py
--rw-r--r--   0        0        0      578 2023-05-11 19:58:45.820594 featuremonkey3-0.1.0/featuremonkey3/test/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 20:54:01.551531 featuremonkey3-0.1.0/featuremonkey3/test/mock/__init__.py
--rw-r--r--   0        0        0     1425 2023-04-21 20:54:01.551668 featuremonkey3-0.1.0/featuremonkey3/test/mock/composer_mocks.py
--rw-r--r--   0        0        0      251 2023-04-21 20:54:01.551769 featuremonkey3-0.1.0/featuremonkey3/test/mock/testmodule1.py
--rw-r--r--   0        0        0        7 2023-04-21 20:54:01.551863 featuremonkey3-0.1.0/featuremonkey3/test/mock/testmodule2.py
--rw-r--r--   0        0        0        0 2023-04-21 20:54:01.551904 featuremonkey3-0.1.0/featuremonkey3/test/mock/testmodule3.py
--rw-r--r--   0        0        0       63 2023-04-21 20:54:01.552097 featuremonkey3-0.1.0/featuremonkey3/test/mock/testpackage1/__init__.py
--rw-r--r--   0        0        0       32 2023-04-27 14:03:41.570693 featuremonkey3-0.1.0/featuremonkey3/test/mock/testpackage1/submodule.py
--rw-r--r--   0        0        0    10129 2023-05-11 20:00:58.952706 featuremonkey3-0.1.0/featuremonkey3/test/test_composer.py
--rw-r--r--   0        0        0        0 2023-04-21 20:54:01.552286 featuremonkey3-0.1.0/featuremonkey3/tracing/__init__.py
--rw-r--r--   0        0        0      742 2023-04-21 20:54:01.552444 featuremonkey3-0.1.0/featuremonkey3/tracing/helper.py
--rw-r--r--   0        0        0     2292 2023-04-21 20:54:01.552672 featuremonkey3-0.1.0/featuremonkey3/tracing/logger.py
--rw-r--r--   0        0        0     4871 2023-04-21 20:54:01.552827 featuremonkey3-0.1.0/featuremonkey3/tracing/serializer.py
--rw-r--r--   0        0        0      442 2023-05-11 19:53:26.587803 featuremonkey3-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 featuremonkey3-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-05-12 15:29:33.644059 featuremonkey3-0.1.1/LICENSE
+-rw-r--r--   0        0        0      617 2023-05-12 15:29:33.644059 featuremonkey3-0.1.1/README.rst
+-rw-r--r--   0        0        0      647 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/__init__.py
+-rw-r--r--   0        0        0    12720 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/composer.py
+-rw-r--r--   0        0        0     1017 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/helpers.py
+-rw-r--r--   0        0        0     5556 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/importhooks.py
+-rw-r--r--   0        0        0      578 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/mock/__init__.py
+-rw-r--r--   0        0        0     1345 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/mock/composer_mocks.py
+-rw-r--r--   0        0        0      251 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/mock/testmodule1.py
+-rw-r--r--   0        0        0        7 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/mock/testmodule2.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/mock/testmodule3.py
+-rw-r--r--   0        0        0       63 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/mock/testpackage1/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/mock/testpackage1/submodule.py
+-rw-r--r--   0        0        0     9729 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/test/test_composer.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/tracing/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/tracing/helper.py
+-rw-r--r--   0        0        0     2292 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/tracing/logger.py
+-rw-r--r--   0        0        0     4871 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/featuremonkey3/tracing/serializer.py
+-rw-r--r--   0        0        0      499 2023-05-12 15:29:33.648059 featuremonkey3-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1307 1970-01-01 00:00:00.000000 featuremonkey3-0.1.1/PKG-INFO
```

### Comparing `featuremonkey3-0.1.0/LICENSE` & `featuremonkey3-0.1.1/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2012 Hendrik Speidel, http://schnapptack.de/
+Copyright (c) 2023 Adrian Wong
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `featuremonkey3-0.1.0/README.rst` & `featuremonkey3-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.0/featuremonkey3/__init__.py` & `featuremonkey3-0.1.1/featuremonkey3/__init__.py`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.0/featuremonkey3/composer.py` & `featuremonkey3-0.1.1/featuremonkey3/composer.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     message = """The logger ({logger}) set in the COMPOSITION_TRACER environment variable does not exist.\n
               Make sure the entered module/class exists, has the correct format ("path.to.module.LoggerClass")\n
               Unset the variable to use default logger (NullOperationLogger)."""
 
 
 # prevent errors; in case there is no operation logger defined, use the NullOperationLogger
 if not os.environ.get('COMPOSITION_TRACER'):
-    os.environ['COMPOSITION_TRACER'] = 'featuremonkey.tracing.logger.NullOperationLogger'
+    os.environ['COMPOSITION_TRACER'] = 'featuremonkey3.tracing.logger.NullOperationLogger'
 
 
 class Composer(object):
 
     def __init__(self):
         logger_class = self._get_logger_class()
         if logger_class:
```

### Comparing `featuremonkey3-0.1.0/featuremonkey3/helpers.py` & `featuremonkey3-0.1.1/featuremonkey3/helpers.py`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.0/featuremonkey3/importhooks.py` & `featuremonkey3-0.1.1/featuremonkey3/importhooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     @classmethod
     def add(cls, module_name, fsts, composer):
         '''
         add a couple of fsts to be superimposed on the module given
         by module_name as soon as it is imported.
 
-        internal - use featuremonkey.compose_later
+        internal - use featuremonkey3.compose_later
         '''
         cls._to_compose.setdefault(module_name, [])
         cls._to_compose[module_name].append(
             (list(fsts), composer)
         )
         cls._install()
 
@@ -113,16 +113,16 @@
     the import guard on that module is dropped again.
     Importing a guarded module results in an ImportGuard exception being thrown.
     Usually, you don`t want to catch these:
     better fail during the composition phase than continuing to run a miscomposed
     program.
 
     The existance of the import hook is considered an implementation detail.
-    The public API to import guards are ``featuremonkey.add_import_guard``
-    and ``featuremonkey.remove_import_guard``.
+    The public API to import guards are ``featuremonkey3.add_import_guard``
+    and ``featuremonkey3.remove_import_guard``.
     """
     _guards = dict()
     _num_entries = 0
 
     @classmethod
     def _insert_hook(cls):
         #the guard hook needs to be first
```

### Comparing `featuremonkey3-0.1.0/featuremonkey3/test/__init__.py` & `featuremonkey3-0.1.1/featuremonkey3/test/__init__.py`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.0/featuremonkey3/test/test_composer.py` & `featuremonkey3-0.1.1/featuremonkey3/test/test_composer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,200 +1,195 @@
-from __future__ import absolute_import
+# from __future__ import absolute_import
+from importlib import reload
 from featuremonkey3 import compose, compose_later
 from featuremonkey3.test.mock import composer_mocks as mocks
 from featuremonkey3.test.mock import testmodule1, testpackage1
-import unittest
+import pytest
 import sys
 
-try:
-    #python3
-    from imp import reload
-except ImportError:
-    #python2
-    pass
+@pytest.fixture
+def reload_mocks():
+    reload(mocks)
 
-class TestObjectComposition(unittest.TestCase):
 
-    def setUp(self):
-        pass
+class TestObjectComposition:
 
-    def test_noparam(self):
-        self.assertRaises(Exception, compose)
+    def test_noparam(self, reload_mocks):
+        with pytest.raises(Exception):
+            compose()
 
-    def test_singleparam(self):
-        self.assertEquals(self, compose(self))
+    def test_singleparam(self, reload_mocks):
+        assert self == compose(self)
 
-    def test_idendity(self):
+    def test_idendity(self, reload_mocks):
         instance = mocks.Base()
         composition = compose(mocks.MemberIntroduction(), instance)
-        self.assertEquals(instance, composition)
+        assert instance == composition
 
-    def test_member_introduction(self):
+    def test_member_introduction(self, reload_mocks):
         instance = mocks.Base()
         composition = compose(mocks.MemberIntroduction(), instance)
-        self.assertEquals(8, composition.base_prop)
-        self.assertEquals(1, composition.a)
+        assert composition.base_prop == 8
+        assert composition.a == 1
 
-    def test_existing_member_introduction(self):
+    def test_existing_member_introduction(self, reload_mocks):
         instance = mocks.Base()
-        self.assertRaises(Exception, compose, mocks.ExistingMemberIntroduction(), instance)
+        with pytest.raises(Exception):
+            compose(mocks.ExistingMemberIntroduction(), instance)
 
-    def test_method_introduction(self):
+    def test_method_introduction(self, reload_mocks):
         instance = mocks.Base()
         composition = compose(mocks.MethodIntroduction(), instance)
-        self.assertEquals(8, composition.base_prop)
-        self.assertTrue(composition.method())
+        assert composition.base_prop == 8
+        assert composition.method()
 
-    def test_method_refinement(self):
+    def test_method_refinement(self, reload_mocks):
         instance = mocks.Base()
         composition = compose(mocks.MethodRefinement(), instance)
-        self.assertEquals('Hellorefined', composition.base_method('Hello'))
+        assert composition.base_method("Hello") == "Hellorefined"
 
-    def test_staticmethod(self):
+    def test_staticmethod(self, reload_mocks):
         instance = mocks.StaticBase()
         instance2 = mocks.StaticBase()
-        self.assertEquals('Hello', instance.base_method('Hello'))
+        assert instance.base_method("Hello") == "Hello"
         composition = compose(mocks.StaticMethodRefinement(), instance)
-        self.assertEquals('Hellorefined', composition.base_method('Hello'))
-        self.assertEquals('Hello', instance2.base_method('Hello'))
+        assert composition.base_method("Hello") == "Hellorefined"
+        assert instance2.base_method("Hello") == "Hello"
 
-    def test_classmethod(self):
+    def test_classmethod(self, reload_mocks):
         instance = mocks.ClassMethodBase()
-        self.assertEquals('Hello', instance.base_method('Hello'))
+        assert instance.base_method("Hello") == "Hello"
         composition = compose(mocks.ClassMethodRefinement(), instance)
-        self.assertEquals('Hellorefined', composition.base_method('Hello'))
+        assert composition.base_method("Hello") == "Hellorefined"
 
+class TestClassComposition:
 
-class TestClassComposition(unittest.TestCase):
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        reload(mocks)
-
-    def test_idendity(self):
+    def test_idendity(self, reload_mocks):
         clss = mocks.Base
         composition = compose(mocks.MemberIntroduction, clss)
-        self.assertEquals(clss, composition)
+        assert composition == clss
 
-    def test_member_introduction(self):
+    def test_membr_introduction(self, reload_mocks):
         compose(mocks.MemberIntroduction, mocks.Base)
-        self.assertEquals(8, mocks.Base.base_prop)
-        self.assertEquals(1, mocks.Base.a)
+        assert mocks.Base.base_prop == 8
+        assert mocks.Base.a == 1
 
-    def test_existing_member_introduction(self):
-        self.assertRaises(Exception, compose, mocks.ExistingMemberIntroduction, mocks.Base)
+    def test_existing_member_introduction(self, reload_mocks):
+        with pytest.raises(Exception):
+            compose(mocks.ExistingMemberIntroduction, mocks.Base)
 
-    def test_method_introduction(self):
+    def test_method_introduction(self, reload_mocks):
         compose(mocks.MethodIntroduction(), mocks.Base)
-        self.assertEquals(8, mocks.Base.base_prop)
-        self.assertTrue(mocks.Base().method())
+        assert mocks.Base.base_prop == 8
+        assert mocks.Base().method()
 
-    def test_method_refinement(self):
+    def test_method_refinement(self, reload_mocks):
         compose(mocks.MethodRefinement2(), mocks.Base)
-        self.assertEquals('Hellorefined', mocks.Base().base_method('Hello'))
+        assert mocks.Base().base_method("Hello") == "Hellorefined"
 
-    def test_staticmethod(self):
-        self.assertEquals('Hello', mocks.StaticBase.base_method('Hello'))
-        self.assertEquals('Hello', mocks.StaticBase().base_method('Hello'))
+    def test_staticmethod(self, reload_mocks):
+        assert mocks.StaticBase.base_method("Hello") == "Hello"
+        assert mocks.StaticBase().base_method("Hello") == "Hello"
         compose(mocks.StaticMethodRefinement(), mocks.StaticBase)
-        self.assertEquals('Hellorefined', mocks.StaticBase.base_method('Hello'))
-        self.assertEquals('Hellorefined', mocks.StaticBase().base_method('Hello'))
+        assert mocks.StaticBase.base_method("Hello") == "Hellorefined"
+        assert mocks.StaticBase().base_method("Hello") == "Hellorefined"
 
-    def test_classmethod(self):
-        self.assertEquals('Hello', mocks.ClassMethodBase.base_method('Hello'))
-        self.assertEquals('Hello', mocks.ClassMethodBase().base_method('Hello'))
+    def test_classmethod(self, reload_mocks):
+        assert mocks.ClassMethodBase.base_method("Hello") == "Hello"
+        assert mocks.ClassMethodBase().base_method("Hello") == "Hello"
         compose(mocks.ClassMethodRefinement(), mocks.ClassMethodBase)
-        self.assertEquals('Hellorefined', mocks.ClassMethodBase.base_method('Hello'))
-        self.assertEquals('Hellorefined', mocks.ClassMethodBase().base_method('Hello'))
+        assert mocks.ClassMethodBase.base_method("Hello") == "Hellorefined"
+        assert mocks.ClassMethodBase().base_method("Hello") == "Hellorefined"
 
-class TestModuleComposition(unittest.TestCase):
+@pytest.fixture
+def reload_modules():
+    if hasattr(testmodule1, "module_introduction"):
+        del testmodule1.module_introduction
 
-    def setUp(self):
-        pass
+    reload(testmodule1)
+    reload(testpackage1)
 
-    def tearDown(self):
-        if hasattr(testmodule1, 'module_introduction'):
-            del testmodule1.module_introduction
-        reload(testmodule1)
-        reload(testpackage1)
+class TestModuleComposition:
 
-    def test_reloading_clears_composition(self):
+    def test_reloading_clears_composition(self, reload_modules):
 
-        self.assertEquals(False, hasattr(testmodule1, 'module_introduction'))
+        assert not hasattr(testmodule1, "module_introduction")
 
-    def test_member_introduction(self):
+    def test_member_introduction(self, reload_modules):
 
         class ModuleIntroduction(object):
 
             introduce_module_introduction = 478
 
         compose(ModuleIntroduction(), testmodule1)
-        self.assertEquals(True, hasattr(testmodule1, 'module_introduction'))
-        self.assertEquals(478, testmodule1.module_introduction)
+        assert hasattr(testmodule1, "module_introduction")
+        assert testmodule1.module_introduction == 478
 
-    def test_member_refinement(self):
+    def test_member_refinement(self, reload_modules):
 
         class ModuleRefinement(object):
 
             refine_attr_in_module = 234
 
-        self.assertEquals(123, testmodule1.attr_in_module)
+        assert testmodule1.attr_in_module == 123
         compose(ModuleRefinement(), testmodule1)
-        self.assertEquals(234, testmodule1.attr_in_module)
 
-    def test_function_introduction(self):
+        assert testmodule1.attr_in_module == 234
+
+    def test_function_introduction(self, reload_modules):
 
         class ModuleFunctionIntroduction(object):
 
             def introduce_my_function(self):
 
                 def my_function(x, y):
                     return x - y
 
                 return my_function
 
-        self.assertEquals(False, hasattr(testmodule1, 'my_function'))
+        assert not hasattr(testmodule1, "my_function")
         compose(ModuleFunctionIntroduction(), testmodule1)
-        self.assertEquals(0, testmodule1.my_function(3, 3))
 
-    def test_function_refinement(self):
+        assert testmodule1.my_function(3, 3) == 0
+
+    def test_function_refinement(self, reload_modules):
 
         class ModuleFunctionRefinement(object):
 
             def refine_func_in_module(self, original):
 
                 def func_in_module(x, y):
                     return original(x, y) * 2
 
                 return func_in_module
 
-        self.assertEquals(2, testmodule1.func_in_module(1, 1))
+        assert testmodule1.func_in_module(1, 1) == 2
         compose(ModuleFunctionRefinement(), testmodule1)
-        self.assertEquals(4, testmodule1.func_in_module(1, 1))
 
-    def test_tuple_refinement(self):
+        assert testmodule1.func_in_module(1, 1) == 4
+
+    def test_tuple_refinement(self, reload_modules):
 
         class ModuleTupleRefinement(object):
 
             def refine_tuple_in_module(self, original):
 
                 refinement = list(original)
                 refinement.append(4)
                 refinement = tuple(refinement)
 
                 return refinement
 
-        self.assertEquals(3, len(testmodule1.tuple_in_module))
+        assert len(testmodule1.tuple_in_module) == 3
         compose(ModuleTupleRefinement(), testmodule1)
-        self.assertEquals(4, len(testmodule1.tuple_in_module))
-        self.assertEquals(4, testmodule1.tuple_in_module[-1])
 
-    def test_class_deep_refinement(self):
+        assert len(testmodule1.tuple_in_module) == 4
+        assert testmodule1.tuple_in_module[-1] == 4
+
+    def test_class_deep_refinement(self, reload_modules):
 
         class ClassRefinement(object):
 
             introduce_a = 123
 
             def refine_attr_in_class(self, original):
                 return False
@@ -204,22 +199,23 @@
                     return (a + b) * 2
                 return plus
 
         class ModuleDeepRefinement(object):
 
             child_ClassInModule = ClassRefinement
 
-        self.assertEquals(False, hasattr(testmodule1.ClassInModule, 'a'))
-        self.assertEquals(2, testmodule1.ClassInModule().plus(1, 1))
-        self.assertEquals(True, testmodule1.ClassInModule().attr_in_class)
+        assert not hasattr(testmodule1.ClassInModule, "a")
+        assert testmodule1.ClassInModule().plus(1, 1) == 2
+        assert testmodule1.ClassInModule().attr_in_class
         compose(ModuleDeepRefinement(), testmodule1)
-        self.assertEquals(False, testmodule1.ClassInModule().attr_in_class)
-        self.assertEquals(4, testmodule1.ClassInModule().plus(1, 1))
 
-    def test_submodule_deep_refinement(self):
+        assert not testmodule1.ClassInModule().attr_in_class
+        assert testmodule1.ClassInModule().plus(1, 1) == 4
+
+    def test_submodule_deep_refinement(self, reload_modules):
 
         class SubmoduleRefinement(object):
 
             introduce_a = 123
 
             def introduce_afunction(self):
 
@@ -229,56 +225,59 @@
 
                 return afunction
 
         class PackageDeepRefinement(object):
 
             child_submodule = SubmoduleRefinement
 
-        self.assertEquals(False, hasattr(testpackage1.submodule, 'a'))
+        assert not hasattr(testpackage1.submodule, "a")
         compose(PackageDeepRefinement(), testpackage1)
-        self.assertEquals(123, testpackage1.submodule.a)
-        self.assertEquals(5, testpackage1.submodule.afunction(1, 5))
 
-    def test_submodule_function_refinement(self):
+        assert testpackage1.submodule.a == 123
+        assert testpackage1.submodule.afunction(1, 5) == 5
+
+    def test_submodule_function_refinement(self, reload_modules):
 
         class SubmoduleRefinement:
 
             def refine_add_one(self, original):
 
                 def add_one(x):
                     return original(x) + 1
 
                 return add_one
 
         class PackageDeepRefinement:
             child_submodule = SubmoduleRefinement
 
-        self.assertEquals(2, testpackage1.submodule.add_one(1))
+        assert testpackage1.submodule.add_one(1) == 2
         compose(PackageDeepRefinement(), testpackage1)
-        self.assertEquals(3, testpackage1.submodule.add_one(1))
 
-    def test_compose_later(self):
+        assert testpackage1.submodule.add_one(1) == 3
+
+    def test_compose_later(self, reload_modules):
 
         class LateModuleRefinement(object):
 
             introduce_a = 123
 
             def introduce_afunction(self):
 
                 def afunction(a, b):
                     return a * b
 
                 return afunction
 
-        self.assertEquals(True, 'featuremonkey3.test.mock.testmodule2' not in sys.modules)
+        assert 'featuremonkey3.test.mock.testmodule2' not in sys.modules
         compose_later(LateModuleRefinement(), 'featuremonkey3.test.mock.testmodule2')
         from featuremonkey3.test.mock import testmodule2
-        self.assertEquals(123, testmodule2.a)
 
-    def test_compose_later_composition_order(self):
+        assert testmodule2.a == 123
+
+    def test_compose_later_composition_order(self, reload_modules):
 
         class LateModuleRefinementA(object):
 
             introduce_a = 123
 
             def introduce_afunction(self):
 
@@ -294,16 +293,14 @@
             def refine_afunction(self, original):
 
                 def afunction(a, b):
                     return original(a, b) + 1
 
                 return afunction
 
-        self.assertEquals(True, 'featuremonkey3.test.mock.testmodule3' not in sys.modules)
+        assert "featuremonkey3.test.mock.testmodule3" not in sys.modules
         compose_later(LateModuleRefinementA(), 'featuremonkey3.test.mock.testmodule3')
         compose_later(LateModuleRefinementB(), 'featuremonkey3.test.mock.testmodule3')
         from featuremonkey3.test.mock import testmodule3
-        self.assertEquals(456, testmodule3.a)
-        self.assertEquals(5, testmodule3.afunction(2, 2))
 
-if __name__ == '__main__':
-    unittest.main()
+        assert testmodule3.a == 456
+        assert testmodule3.afunction(2, 2) == 5
```

### Comparing `featuremonkey3-0.1.0/featuremonkey3/tracing/helper.py` & `featuremonkey3-0.1.1/featuremonkey3/tracing/helper.py`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.0/featuremonkey3/tracing/logger.py` & `featuremonkey3-0.1.1/featuremonkey3/tracing/logger.py`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.0/featuremonkey3/tracing/serializer.py` & `featuremonkey3-0.1.1/featuremonkey3/tracing/serializer.py`

 * *Files identical despite different names*

### Comparing `featuremonkey3-0.1.0/PKG-INFO` & `featuremonkey3-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: featuremonkey3
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python 3.11 compatible fork of featuremonkey, a Python FOP framework first developed by Hendrik Speidel.
 License: MIT
 Author: Adrian Wong
 Author-email: adrianwong227@gmail.com
-Requires-Python: >=3.4,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: importlib (>=1.0.4,<2.0.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Description-Content-Type: text/x-rst
```

