# Comparing `tmp/redmage-0.0.5.tar.gz` & `tmp/redmage-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redmage-0.0.5.tar", max compression
+gzip compressed data, was "redmage-0.1.0.tar", max compression
```

## Comparing `redmage-0.0.5.tar` & `redmage-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.0.5/LICENSE
--rw-r--r--   0        0        0    14693 2023-04-30 22:37:22.299063 redmage-0.0.5/README.md
--rw-r--r--   0        0        0      624 2023-05-01 01:05:35.169429 redmage-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      328 2023-04-21 18:11:35.917318 redmage-0.0.5/redmage/__init__.py
--rw-r--r--   0        0        0     6371 2023-05-01 00:05:27.298095 redmage-0.0.5/redmage/components.py
--rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.0.5/redmage/convertors.py
--rw-r--r--   0        0        0     6979 2023-04-30 21:11:15.121820 redmage-0.0.5/redmage/core.py
--rw-r--r--   0        0        0     9605 2023-04-30 17:34:15.446362 redmage-0.0.5/redmage/elements.py
--rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.0.5/redmage/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.0.5/redmage/py.typed
--rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.0.5/redmage/targets.py
--rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.0.5/redmage/triggers.py
--rw-r--r--   0        0        0     1314 2023-05-01 00:53:46.268926 redmage-0.0.5/redmage/types.py
--rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.0.5/redmage/utils.py
--rw-r--r--   0        0        0    15394 1970-01-01 00:00:00.000000 redmage-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.1.0/LICENSE
+-rw-r--r--   0        0        0    14351 2023-05-12 14:17:31.917169 redmage-0.1.0/README.md
+-rw-r--r--   0        0        0      660 2023-05-12 14:55:28.760619 redmage-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      333 2023-05-12 13:48:08.901451 redmage-0.1.0/redmage/__init__.py
+-rw-r--r--   0        0        0     6689 2023-05-12 14:38:21.207931 redmage-0.1.0/redmage/components.py
+-rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.1.0/redmage/convertors.py
+-rw-r--r--   0        0        0     7186 2023-05-12 14:51:43.484701 redmage-0.1.0/redmage/core.py
+-rw-r--r--   0        0        0     9605 2023-04-30 17:34:15.446362 redmage-0.1.0/redmage/elements.py
+-rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.1.0/redmage/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.1.0/redmage/py.typed
+-rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.1.0/redmage/targets.py
+-rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.1.0/redmage/triggers.py
+-rw-r--r--   0        0        0     1314 2023-05-01 00:53:46.268926 redmage-0.1.0/redmage/types.py
+-rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.1.0/redmage/utils.py
+-rw-r--r--   0        0        0    15052 1970-01-01 00:00:00.000000 redmage-0.1.0/PKG-INFO
```

### Comparing `redmage-0.0.5/LICENSE` & `redmage-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redmage-0.0.5/README.md` & `redmage-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,14 @@
 Consider the example below.
 
 ```
 from redmage import Component, Redmage, Target
 from redmage.elements import Button, Div, H1, Script
 
 
-app = Redmage()
-
-
 class Counter(Component, routes=("/",)):
     count: int
 
     def __init__(self):
         self.count = 0
 
     def render(self):
@@ -50,46 +47,25 @@
 
 Redmage is available on pypi.
 
 ```
 pip install redmage
 ```
 
-## Redmage application
-
-
-The first thing you need to do is create an instance of the Redmage class.
-
-```
-from redmage import Redmage
-
-
-app = Redmage()
-```
-
-At this point our app won't do anything because we haven't registered any routes by sublassing Component. But you can start it up using your favorite ASGI server like uvicorn.
-
-```
-uvicorn <module>:<filename>:app.starlette
-```
-
 
 ## First Component
 
 
 Let's create a Component. In the example we just returned a **div** element. This works but we're going to want to create a proper html page with **html**, **header**, **body** tags etc.
 
 ```
-from redmage import Component, Redmage
+from redmage import Component, app
 from redmage.elements import Body, Doc, H1, Head, Html, Script, Title
 
 
-app = Redmage()
-
-
 class Index(Component, routes=("/",)):
 
     def render(self):
         return Doc(
             Html(
                 Head(
                     Title("Example"),
@@ -102,14 +78,20 @@
         )
 ```
 
 This tells our app to register the **Index** component with the route "/". When you navigate to _localhost:8000/_ an instance of **Index** will be created and it's render method will be called to generate the html.
 
 The **Component** class is abstract and has a single abstract base method, **render**, that must be implemented and return and instance of **redmage.elements.Element**.
 
+You can start the application using your favorite ASGI server like uvicorn.
+
+```
+uvicorn <module>:<filename>:app.starlette
+```
+
 
 ## Elements
 
 Redmage internally uses python classes associated with each html tag (**Div**, **Body**, **H1** etc.). They can all be imported from **redmage.elements**. Each of these classes subclasses **redmage.elements.Element**. Pass the elements inner html as positional arguments and add attributes with keyword arguments.
 
 ```
 from redmage.elements import Div
@@ -160,21 +142,17 @@
 
 ## Nesting Components
 
 
 Components can be easily nested by using them just like you would use any other html **Element** object.
 
 ```
-from redmage import Redmage
 from redmage.elements import Body, Doc, H1, Head, Html, Script, Title
 
 
-app = Redmage()
-
-
 class Index(Component, routes=("/",)):
 
     def render(self):
         return Doc(
             Html(
                 Head(
                     Title("Todo App"),
```

### Comparing `redmage-0.0.5/pyproject.toml` & `redmage-0.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redmage"
-version = "0.0.5"
+version = "0.1.0"
 description = "A component based library for building htmx powered applications."
 authors = ["Scott Russell <me@scottrussell.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -16,14 +16,16 @@
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pycodestyle = "^2.10.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 httpx = "^0.24.0"
 jinja2 = "^3.1.2"
+mypy = "^1.2.0"
+uvicorn = "^0.22.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `redmage-0.0.5/redmage/components.py` & `redmage-0.1.0/redmage/components.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,15 +111,20 @@
             ):
                 if (
                     param_value.default != Parameter.empty
                     and param_value.kind != Parameter.POSITIONAL_ONLY
                     and param_value.name != "self"
                     and len(positional_or_keyword_params) >= n
                 ):
-                    convertor = starlette_convertors[param_value.annotation.__name__]
+                    ann = (
+                        param_value.annotation
+                        if isinstance(param_value.annotation, str)
+                        else param_value.annotation.__name__
+                    )
+                    convertor = starlette_convertors[ann]
                     value = convertor.to_string(
                         positional_or_keyword_params[n - offset]
                     )
                     path += f"{method_name}__{param_value.name}="
                     path += f"{value}&"
 
             path = path[:-1]  # Have to remove whatever the last character is
@@ -128,18 +133,20 @@
             params = signature(method_fn).parameters
             for param_value in params.values():
                 if (
                     param_value.default == Parameter.empty
                     and param_value.kind != Parameter.POSITIONAL_ONLY
                     and param_value.name != "self"
                 ):
-                    path += (
-                        f"/{{{method_name}__{param_value.name}:"
-                        f"{param_value.annotation.__name__}}}"
+                    ann = (
+                        param_value.annotation
+                        if isinstance(param_value.annotation, str)
+                        else param_value.annotation.__name__
                     )
+                    path += f"/{{{method_name}__{param_value.name}:{ann}}}"
 
         return path
 
     @property
     def id(self) -> str:
         if not hasattr(self, "_id"):
             self._id = f"{self.__class__.__name__}-{str(uuid1())}"
```

### Comparing `redmage-0.0.5/redmage/convertors.py` & `redmage-0.1.0/redmage/convertors.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.5/redmage/core.py` & `redmage-0.1.0/redmage/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 logger = logging.getLogger("redmage")
 
 
 ComponentClass = Type[Component]
 
 
 class Redmage:
-    def __init__(self, debug: bool = False):
-        self.debug = debug
+    def __init__(self) -> None:
+        self.debug = False
         self.routes: List[Route] = []
         # Could cuase problems if multiple apps are created
         Component.set_app(self)
 
     @property
     def starlette(self) -> Starlette:
         if not hasattr(self, "_starlette"):
@@ -94,15 +94,20 @@
             return HTMLResponse(str(instance))
 
         return route_function
 
     def _convert_value(self, key: str, value: str, fn: Callable) -> Any:
         params = signature(fn).parameters
         if key in params:
-            type_name = params[key].annotation.__name__
+            ann = (
+                params[key].annotation
+                if isinstance(params[key].annotation, str)
+                else params[key].annotation.__name__
+            )
+            type_name = ann
             value = starlette_convertors[type_name].convert(value)
         return value
 
     def _split_params(
         self,
         params: Union[Dict[str, Any], QueryParams],
         method_name: str,
@@ -150,14 +155,15 @@
         return target_method
 
     def _register_routes(
         self, cls: ComponentClass, routes: Tuple[str]
     ) -> ComponentClass:
         for route in routes:
             logger.debug(route)
+            print(route)
             self.routes.append(
                 Route(
                     route,
                     self._get_explicit_route_function(cls),
                     methods=[
                         HTTPMethod.GET,
                     ],
@@ -178,20 +184,24 @@
     def _register_target(
         self, cls: ComponentClass, method: Tuple[str, FunctionType]
     ) -> None:
         method_name, method_fn = method
         path = cls.get_base_path()
         path += cls.get_target_path(method_name)
         logger.debug(path)
+        print(path)
         route_function = self._get_route_function(cls, method_name, method_fn)
 
         self.routes.append(
             Route(
                 path,
                 route_function,
                 name=method_name,
                 methods=[method_fn.target_method],  # type: ignore
             )
         )
 
         target_method = self._get_target_method(method_name, method_fn)
         setattr(cls, method_name, target_method)
+
+
+app = Redmage()
```

### Comparing `redmage-0.0.5/redmage/elements.py` & `redmage-0.1.0/redmage/elements.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.5/redmage/targets.py` & `redmage-0.1.0/redmage/targets.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.5/redmage/triggers.py` & `redmage-0.1.0/redmage/triggers.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.5/redmage/types.py` & `redmage-0.1.0/redmage/types.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.5/redmage/utils.py` & `redmage-0.1.0/redmage/utils.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.5/PKG-INFO` & `redmage-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redmage
-Version: 0.0.5
+Version: 0.1.0
 Summary: A component based library for building htmx powered applications.
 License: MIT
 Author: Scott Russell
 Author-email: me@scottrussell.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -32,17 +32,14 @@
 Consider the example below.
 
 ```
 from redmage import Component, Redmage, Target
 from redmage.elements import Button, Div, H1, Script
 
 
-app = Redmage()
-
-
 class Counter(Component, routes=("/",)):
     count: int
 
     def __init__(self):
         self.count = 0
 
     def render(self):
@@ -69,46 +66,25 @@
 
 Redmage is available on pypi.
 
 ```
 pip install redmage
 ```
 
-## Redmage application
-
-
-The first thing you need to do is create an instance of the Redmage class.
-
-```
-from redmage import Redmage
-
-
-app = Redmage()
-```
-
-At this point our app won't do anything because we haven't registered any routes by sublassing Component. But you can start it up using your favorite ASGI server like uvicorn.
-
-```
-uvicorn <module>:<filename>:app.starlette
-```
-
 
 ## First Component
 
 
 Let's create a Component. In the example we just returned a **div** element. This works but we're going to want to create a proper html page with **html**, **header**, **body** tags etc.
 
 ```
-from redmage import Component, Redmage
+from redmage import Component, app
 from redmage.elements import Body, Doc, H1, Head, Html, Script, Title
 
 
-app = Redmage()
-
-
 class Index(Component, routes=("/",)):
 
     def render(self):
         return Doc(
             Html(
                 Head(
                     Title("Example"),
@@ -121,14 +97,20 @@
         )
 ```
 
 This tells our app to register the **Index** component with the route "/". When you navigate to _localhost:8000/_ an instance of **Index** will be created and it's render method will be called to generate the html.
 
 The **Component** class is abstract and has a single abstract base method, **render**, that must be implemented and return and instance of **redmage.elements.Element**.
 
+You can start the application using your favorite ASGI server like uvicorn.
+
+```
+uvicorn <module>:<filename>:app.starlette
+```
+
 
 ## Elements
 
 Redmage internally uses python classes associated with each html tag (**Div**, **Body**, **H1** etc.). They can all be imported from **redmage.elements**. Each of these classes subclasses **redmage.elements.Element**. Pass the elements inner html as positional arguments and add attributes with keyword arguments.
 
 ```
 from redmage.elements import Div
@@ -179,21 +161,17 @@
 
 ## Nesting Components
 
 
 Components can be easily nested by using them just like you would use any other html **Element** object.
 
 ```
-from redmage import Redmage
 from redmage.elements import Body, Doc, H1, Head, Html, Script, Title
 
 
-app = Redmage()
-
-
 class Index(Component, routes=("/",)):
 
     def render(self):
         return Doc(
             Html(
                 Head(
                     Title("Todo App"),
```

