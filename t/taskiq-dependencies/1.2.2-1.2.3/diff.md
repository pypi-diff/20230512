# Comparing `tmp/taskiq_dependencies-1.2.2.tar.gz` & `tmp/taskiq_dependencies-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_dependencies-1.2.2.tar", max compression
+gzip compressed data, was "taskiq_dependencies-1.2.3.tar", max compression
```

## Comparing `taskiq_dependencies-1.2.2.tar` & `taskiq_dependencies-1.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4801 2023-04-27 14:42:34.438436 taskiq_dependencies-1.2.2/README.md
--rw-r--r--   0        0        0     1621 2023-04-27 14:42:34.438436 taskiq_dependencies-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      386 2023-04-27 14:42:34.438436 taskiq_dependencies-1.2.2/taskiq_dependencies/__init__.py
--rw-r--r--   0        0        0    11543 2023-04-27 14:42:34.438436 taskiq_dependencies-1.2.2/taskiq_dependencies/ctx.py
--rw-r--r--   0        0        0     3189 2023-04-27 14:42:34.438436 taskiq_dependencies-1.2.2/taskiq_dependencies/dependency.py
--rw-r--r--   0        0        0     7669 2023-04-27 14:42:34.438436 taskiq_dependencies-1.2.2/taskiq_dependencies/graph.py
--rw-r--r--   0        0        0        0 2023-04-27 14:42:34.438436 taskiq_dependencies-1.2.2/taskiq_dependencies/py.typed
--rw-r--r--   0        0        0      573 2023-04-27 14:42:34.438436 taskiq_dependencies-1.2.2/taskiq_dependencies/utils.py
--rw-r--r--   0        0        0     5933 1970-01-01 00:00:00.000000 taskiq_dependencies-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     6368 2023-05-12 12:01:10.208098 taskiq_dependencies-1.2.3/README.md
+-rw-r--r--   0        0        0     1621 2023-05-12 12:01:10.208098 taskiq_dependencies-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0      386 2023-05-12 12:01:10.208098 taskiq_dependencies-1.2.3/taskiq_dependencies/__init__.py
+-rw-r--r--   0        0        0    11543 2023-05-12 12:01:10.208098 taskiq_dependencies-1.2.3/taskiq_dependencies/ctx.py
+-rw-r--r--   0        0        0     3273 2023-05-12 12:01:10.208098 taskiq_dependencies-1.2.3/taskiq_dependencies/dependency.py
+-rw-r--r--   0        0        0     9626 2023-05-12 12:01:10.208098 taskiq_dependencies-1.2.3/taskiq_dependencies/graph.py
+-rw-r--r--   0        0        0        0 2023-05-12 12:01:10.208098 taskiq_dependencies-1.2.3/taskiq_dependencies/py.typed
+-rw-r--r--   0        0        0      573 2023-05-12 12:01:10.208098 taskiq_dependencies-1.2.3/taskiq_dependencies/utils.py
+-rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 taskiq_dependencies-1.2.3/PKG-INFO
```

### Comparing `taskiq_dependencies-1.2.2/README.md` & `taskiq_dependencies-1.2.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -172,7 +172,91 @@
 graph = DependencyGraph(target_func)
 
 with graph.sync_ctx(exception_propagation=False) as ctx:
     print(ctx.resolve_kwargs())
 
 
 ```
+
+
+## Generics support
+
+We support generics substitution for class-based dependencies.
+For example, let's define an interface and a class. This class can be
+parameterized with some type and we consider this type a dependency.
+
+```python
+import abc
+from typing import Any, Generic, TypeVar
+
+class MyInterface(abc.ABC):
+    @abc.abstractmethod
+    def getval(self) -> Any:
+        ...
+
+
+_T = TypeVar("_T", bound=MyInterface)
+
+
+class MyClass(Generic[_T]):
+    # We don't know exact type, but we assume
+    # that it can be used as a dependency.
+    def __init__(self, resource: _T = Depends()):
+        self.resource = resource
+
+    @property
+    def my_value(self) -> Any:
+        return self.resource.getval()
+
+```
+
+Now let's create several implementation of defined interface:
+
+```python
+
+def getstr() -> str:
+    return "strstr"
+
+
+def getint() -> int:
+    return 100
+
+
+class MyDep1(MyInterface):
+    def __init__(self, s: str = Depends(getstr)) -> None:
+        self.s = s
+
+    def getval(self) -> str:
+        return self.s
+
+
+class MyDep2(MyInterface):
+    def __init__(self, i: int = Depends(getint)) -> None:
+        self.i = i
+
+    def getval(self) -> int:
+        return self.i
+
+```
+
+Now you can use these dependencies by just setting proper type hints.
+
+```python
+def my_target(
+    d1: MyClass[MyDep1] = Depends(),
+    d2: MyClass[MyDep2] = Depends(),
+) -> None:
+    print(d1.my_value)
+    print(d2.my_value)
+
+
+with DependencyGraph(my_target).sync_ctx() as ctx:
+    my_target(**ctx.resolve_kwargs())
+
+```
+
+This code will is going to print:
+
+```
+strstr
+100
+```
```

### Comparing `taskiq_dependencies-1.2.2/pyproject.toml` & `taskiq_dependencies-1.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq-dependencies"
-version = "1.2.2"
+version = "1.2.3"
 description = "FastAPI like dependency injection implementation"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 packages = [{include = "taskiq_dependencies"}]
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
```

### Comparing `taskiq_dependencies-1.2.2/taskiq_dependencies/ctx.py` & `taskiq_dependencies-1.2.3/taskiq_dependencies/ctx.py`

 * *Files identical despite different names*

### Comparing `taskiq_dependencies-1.2.2/taskiq_dependencies/dependency.py` & `taskiq_dependencies-1.2.3/taskiq_dependencies/dependency.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,28 +98,30 @@
     Class to mark parameter as a dependency.
 
     This class is used to mark parameters of a function,
     or a class as injectables, so taskiq can resolve it
     and calculate before execution.
     """
 
-    def __init__(  # noqa: WPS234
+    def __init__(  # noqa: WPS211, WPS234
         self,
         dependency: Optional[Union[Type[Any], Callable[..., Any]]] = None,
         *,
         use_cache: bool = True,
         kwargs: Optional[Dict[str, Any]] = None,
         signature: Optional[inspect.Parameter] = None,
+        parent: "Optional[Dependency]" = None,
     ) -> None:
         self._id = uuid.uuid4()
         self.dependency = dependency
         self.use_cache = use_cache
         self.param_name = ""
         self.kwargs = kwargs or {}
         self.signature = signature
+        self.parent = parent
 
     def __hash__(self) -> int:
         return hash(self._id)
 
     def __eq__(self, rhs: object) -> bool:
         """
         Overriden eq operation.
```

### Comparing `taskiq_dependencies-1.2.2/taskiq_dependencies/graph.py` & `taskiq_dependencies-1.2.3/taskiq_dependencies/graph.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 from collections import defaultdict, deque
 from graphlib import TopologicalSorter
-from typing import Any, Callable, Dict, List, Optional, get_type_hints
+from typing import Any, Callable, Dict, List, Optional, TypeVar, get_type_hints
 
 from taskiq_dependencies.ctx import AsyncResolveContext, SyncResolveContext
 from taskiq_dependencies.dependency import Dependency
 
 try:
     from fastapi.params import Depends as FastapiDepends  # noqa: WPS433
 except ImportError:
@@ -99,26 +99,63 @@
             dep = dep_deque.popleft()
             # Skip adding dependency if it's already present.
             if dep in self.dependencies:
                 continue
             if dep.dependency is None:
                 continue
             # Get signature and type hints.
-            sign = inspect.signature(dep.dependency)
-            if inspect.isclass(dep.dependency):
+            origin = getattr(dep.dependency, "__origin__", None)
+            if origin is None:
+                origin = dep.dependency
+
+            # If we found the typevar.
+            # It means, that somebody depend on generic type.
+            if isinstance(origin, TypeVar):
+                if dep.parent is None:
+                    raise ValueError(f"Cannot resolve generic {dep.dependency}")
+                parent_cls = dep.parent.dependency
+                parent_cls_origin = getattr(parent_cls, "__origin__", None)
+                # If we cannot find origin, than means, that we cannot resolve
+                # generic parameters. So exiting.
+                if parent_cls_origin is None:
+                    raise ValueError(
+                        f"Unknown generic argument {origin}. "
+                        + f"Please provide a type in param `{dep.parent.param_name}`"
+                        + f" of `{dep.parent.dependency}`",
+                    )
+                # We zip together names of parameters and the subsctituted values
+                # In parameters we would see TypeVars in args
+                # we would find actual classes.
+                generics = zip(
+                    parent_cls_origin.__parameters__,
+                    parent_cls.__args__,  # type: ignore
+                )
+                for tvar, type_param in generics:
+                    # If we found the typevar we're currently try to resolve,
+                    # we need to find origin of the substituted class.
+                    if tvar == origin:
+                        dep.dependency = type_param
+                        origin = getattr(type_param, "__origin__", None)
+                        if origin is None:
+                            origin = type_param
+
+            if inspect.isclass(origin):
                 # If this is a class, we need to get signature of
                 # an __init__ method.
-                hints = get_type_hints(dep.dependency.__init__)  # noqa: WPS609
+                hints = get_type_hints(origin.__init__)  # noqa: WPS609
+                sign = inspect.signature(origin.__init__)  # noqa: WPS609
             elif inspect.isfunction(dep.dependency):
                 # If this is function or an instance of a class, we get it's type hints.
                 hints = get_type_hints(dep.dependency)
+                sign = inspect.signature(origin)  # type: ignore
             else:
                 hints = get_type_hints(
                     dep.dependency.__call__,  # type: ignore # noqa: WPS609
                 )
+                sign = inspect.signature(origin)  # type: ignore
 
             # Now we need to iterate over parameters, to
             # find all parameters, that have TaskiqDepends as it's
             # default vaule.
             for param_name, param in sign.parameters.items():
                 default_value = param.default
 
@@ -168,14 +205,15 @@
                 # Now we construct new TaskiqDepends instance
                 # with correct dependency function and cache.
                 dep_obj = Dependency(
                     dependency_func,
                     use_cache=default_value.use_cache,
                     kwargs=default_value.kwargs,
                     signature=param,
+                    parent=dep,
                 )
                 # Also we set the parameter name,
                 # it will help us in future when
                 # we're going to resolve all dependencies.
                 dep_obj.param_name = param_name
 
                 # We append current dependency
```

### Comparing `taskiq_dependencies-1.2.2/taskiq_dependencies/utils.py` & `taskiq_dependencies-1.2.3/taskiq_dependencies/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq_dependencies-1.2.2/PKG-INFO` & `taskiq_dependencies-1.2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-dependencies
-Version: 1.2.2
+Version: 1.2.3
 Summary: FastAPI like dependency injection implementation
 Keywords: taskiq,dependencies,injection,async,DI
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -200,7 +200,91 @@
 
 with graph.sync_ctx(exception_propagation=False) as ctx:
     print(ctx.resolve_kwargs())
 
 
 ```
 
+
+## Generics support
+
+We support generics substitution for class-based dependencies.
+For example, let's define an interface and a class. This class can be
+parameterized with some type and we consider this type a dependency.
+
+```python
+import abc
+from typing import Any, Generic, TypeVar
+
+class MyInterface(abc.ABC):
+    @abc.abstractmethod
+    def getval(self) -> Any:
+        ...
+
+
+_T = TypeVar("_T", bound=MyInterface)
+
+
+class MyClass(Generic[_T]):
+    # We don't know exact type, but we assume
+    # that it can be used as a dependency.
+    def __init__(self, resource: _T = Depends()):
+        self.resource = resource
+
+    @property
+    def my_value(self) -> Any:
+        return self.resource.getval()
+
+```
+
+Now let's create several implementation of defined interface:
+
+```python
+
+def getstr() -> str:
+    return "strstr"
+
+
+def getint() -> int:
+    return 100
+
+
+class MyDep1(MyInterface):
+    def __init__(self, s: str = Depends(getstr)) -> None:
+        self.s = s
+
+    def getval(self) -> str:
+        return self.s
+
+
+class MyDep2(MyInterface):
+    def __init__(self, i: int = Depends(getint)) -> None:
+        self.i = i
+
+    def getval(self) -> int:
+        return self.i
+
+```
+
+Now you can use these dependencies by just setting proper type hints.
+
+```python
+def my_target(
+    d1: MyClass[MyDep1] = Depends(),
+    d2: MyClass[MyDep2] = Depends(),
+) -> None:
+    print(d1.my_value)
+    print(d2.my_value)
+
+
+with DependencyGraph(my_target).sync_ctx() as ctx:
+    my_target(**ctx.resolve_kwargs())
+
+```
+
+This code will is going to print:
+
+```
+strstr
+100
+```
+
```

