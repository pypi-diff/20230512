# Comparing `tmp/devpytools-0.1.0.dev4.tar.gz` & `tmp/devpytools-0.1.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\devpytools-0.1.0.dev4.tar", last modified: Sun Apr 30 16:03:47 2023, max compression
+gzip compressed data, was "dist\devpytools-0.1.0.dev5.tar", last modified: Fri May 12 19:53:06 2023, max compression
```

## Comparing `devpytools-0.1.0.dev4.tar` & `devpytools-0.1.0.dev5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 16:03:47.615880 devpytools-0.1.0.dev4/
--rw-rw-rw-   0        0        0     1950 2022-10-05 19:38:35.000000 devpytools-0.1.0.dev4/.gitignore
--rw-rw-rw-   0        0        0     1085 2022-04-16 14:06:14.000000 devpytools-0.1.0.dev4/LICENSE
--rw-rw-rw-   0        0        0     3950 2023-04-30 16:03:47.609894 devpytools-0.1.0.dev4/PKG-INFO
--rw-rw-rw-   0        0        0     2144 2023-04-30 14:53:21.000000 devpytools-0.1.0.dev4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 16:03:47.484230 devpytools-0.1.0.dev4/devpytools/
--rw-rw-rw-   0        0        0       45 2022-04-23 18:37:52.000000 devpytools-0.1.0.dev4/devpytools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:03:47.586961 devpytools-0.1.0.dev4/devpytools/cacher/
--rw-rw-rw-   0        0        0      154 2022-10-09 09:16:26.000000 devpytools-0.1.0.dev4/devpytools/cacher/__init__.py
--rw-rw-rw-   0        0        0     2785 2022-10-10 18:41:26.000000 devpytools-0.1.0.dev4/devpytools/cacher/cache_provider.py
--rw-rw-rw-   0        0        0     8201 2023-04-30 14:44:50.000000 devpytools-0.1.0.dev4/devpytools/cacher/cacher.py
--rw-rw-rw-   0        0        0      654 2022-10-05 20:22:46.000000 devpytools-0.1.0.dev4/devpytools/cacher/extensions.py
--rw-rw-rw-   0        0        0       72 2022-10-09 09:13:32.000000 devpytools-0.1.0.dev4/devpytools/cacher/general.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:03:47.592940 devpytools-0.1.0.dev4/devpytools/other/
--rw-rw-rw-   0        0        0       34 2022-04-23 18:37:34.000000 devpytools-0.1.0.dev4/devpytools/other/__init__.py
--rw-rw-rw-   0        0        0     1408 2022-10-10 19:40:39.000000 devpytools-0.1.0.dev4/devpytools/other/replace.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:03:47.564017 devpytools-0.1.0.dev4/devpytools.egg-info/
--rw-rw-rw-   0        0        0     3950 2023-04-30 16:03:46.000000 devpytools-0.1.0.dev4/devpytools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      541 2023-04-30 16:03:47.000000 devpytools-0.1.0.dev4/devpytools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 16:03:46.000000 devpytools-0.1.0.dev4/devpytools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-10 20:08:29.000000 devpytools-0.1.0.dev4/devpytools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-04-30 16:03:46.000000 devpytools-0.1.0.dev4/devpytools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-30 16:03:46.000000 devpytools-0.1.0.dev4/devpytools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 16:03:47.616879 devpytools-0.1.0.dev4/setup.cfg
--rw-rw-rw-   0        0        0     1426 2023-04-30 16:03:24.000000 devpytools-0.1.0.dev4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:03:47.606902 devpytools-0.1.0.dev4/tests/
--rw-rw-rw-   0        0        0        0 2022-04-18 15:01:59.000000 devpytools-0.1.0.dev4/tests/__init__.py
--rw-rw-rw-   0        0        0     7239 2022-10-10 19:45:53.000000 devpytools-0.1.0.dev4/tests/test_cacher.py
--rw-rw-rw-   0        0        0      720 2022-10-10 19:39:51.000000 devpytools-0.1.0.dev4/tests/test_other.py
--rw-rw-rw-   0        0        0      183 2022-10-10 19:56:35.000000 devpytools-0.1.0.dev4/tox.ini
+drwxrwxrwx   0        0        0        0 2023-05-12 19:53:06.062369 devpytools-0.1.0.dev5/
+-rw-rw-rw-   0        0        0     1950 2022-10-05 19:38:35.000000 devpytools-0.1.0.dev5/.gitignore
+-rw-rw-rw-   0        0        0     1085 2022-04-16 14:06:14.000000 devpytools-0.1.0.dev5/LICENSE
+-rw-rw-rw-   0        0        0     3946 2023-05-12 19:53:06.060374 devpytools-0.1.0.dev5/PKG-INFO
+-rw-rw-rw-   0        0        0     2140 2023-05-11 16:51:43.000000 devpytools-0.1.0.dev5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 19:53:05.967623 devpytools-0.1.0.dev5/devpytools/
+-rw-rw-rw-   0        0        0       45 2022-04-23 18:37:52.000000 devpytools-0.1.0.dev5/devpytools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:53:06.043420 devpytools-0.1.0.dev5/devpytools/cacher/
+-rw-rw-rw-   0        0        0      154 2022-10-09 09:16:26.000000 devpytools-0.1.0.dev5/devpytools/cacher/__init__.py
+-rw-rw-rw-   0        0        0     2785 2022-10-10 18:41:26.000000 devpytools-0.1.0.dev5/devpytools/cacher/cache_provider.py
+-rw-rw-rw-   0        0        0     8290 2023-05-12 19:49:43.000000 devpytools-0.1.0.dev5/devpytools/cacher/cacher.py
+-rw-rw-rw-   0        0        0      654 2022-10-05 20:22:46.000000 devpytools-0.1.0.dev5/devpytools/cacher/extensions.py
+-rw-rw-rw-   0        0        0      175 2023-05-12 19:42:30.000000 devpytools-0.1.0.dev5/devpytools/cacher/general.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:53:06.050409 devpytools-0.1.0.dev5/devpytools/other/
+-rw-rw-rw-   0        0        0       34 2022-04-23 18:37:34.000000 devpytools-0.1.0.dev5/devpytools/other/__init__.py
+-rw-rw-rw-   0        0        0     1408 2022-10-10 19:40:39.000000 devpytools-0.1.0.dev5/devpytools/other/replace.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:53:06.029460 devpytools-0.1.0.dev5/devpytools.egg-info/
+-rw-rw-rw-   0        0        0     3946 2023-05-12 19:53:05.000000 devpytools-0.1.0.dev5/devpytools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      541 2023-05-12 19:53:05.000000 devpytools-0.1.0.dev5/devpytools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 19:53:05.000000 devpytools-0.1.0.dev5/devpytools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-12 19:53:05.000000 devpytools-0.1.0.dev5/devpytools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-05-12 19:53:05.000000 devpytools-0.1.0.dev5/devpytools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-12 19:53:05.000000 devpytools-0.1.0.dev5/devpytools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 19:53:06.062369 devpytools-0.1.0.dev5/setup.cfg
+-rw-rw-rw-   0        0        0     1426 2023-05-12 19:51:52.000000 devpytools-0.1.0.dev5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:53:06.057382 devpytools-0.1.0.dev5/tests/
+-rw-rw-rw-   0        0        0        0 2022-04-18 15:01:59.000000 devpytools-0.1.0.dev5/tests/__init__.py
+-rw-rw-rw-   0        0        0     7546 2023-05-12 19:49:06.000000 devpytools-0.1.0.dev5/tests/test_cacher.py
+-rw-rw-rw-   0        0        0      720 2022-10-10 19:39:51.000000 devpytools-0.1.0.dev5/tests/test_other.py
+-rw-rw-rw-   0        0        0      183 2022-10-10 19:56:35.000000 devpytools-0.1.0.dev5/tox.ini
```

### Comparing `devpytools-0.1.0.dev4/.gitignore` & `devpytools-0.1.0.dev5/.gitignore`

 * *Files identical despite different names*

### Comparing `devpytools-0.1.0.dev4/LICENSE` & `devpytools-0.1.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `devpytools-0.1.0.dev4/PKG-INFO` & `devpytools-0.1.0.dev5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpytools
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: Various dev tools.
 Home-page: https://github.com/glowlex/devpytools
 Author: glowlex
 Author-email: antonioavocado777@gmail.com
 License: MIT
 Description: # devpytools
         Tools for development.
@@ -31,15 +31,15 @@
         c = Cacher(name='dev', tmpDirPath='./tmp')
         ```
         
         Get previously configured cacher in other file and use
         ```python
         from devpytools import getCacher
         c = getCacher("dev")
-        @c.cache()
+        @c.cache
         def a(b):
             ...
         ```
         
         Example
         ```python
         from devpytools import Cacher
@@ -50,15 +50,15 @@
             name="dev",
             tmpDirPath="./tmp",
             isEnable=IS_DEV,  # work only if run in dev environment
             isExpired=extensions.expireAfterHours(1),  # recache if cached data older than 1 hour
             isSavable=lambda result: bool(result),  # only cache positive function call results
         )
         
-        @devCacher.cache()
+        @devCacher.cache
         def a(b):
             ...
         
         # works with the same params as devCacher but saves caches to ./tmp1 folder
         @devCacher.cache(tmpDirPath="./tmp1")
         def a1(b):
             ...
```

### Comparing `devpytools-0.1.0.dev4/README.md` & `devpytools-0.1.0.dev5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 c = Cacher(name='dev', tmpDirPath='./tmp')
 ```
 
 Get previously configured cacher in other file and use
 ```python
 from devpytools import getCacher
 c = getCacher("dev")
-@c.cache()
+@c.cache
 def a(b):
     ...
 ```
 
 Example
 ```python
 from devpytools import Cacher
@@ -42,15 +42,15 @@
     name="dev",
     tmpDirPath="./tmp",
     isEnable=IS_DEV,  # work only if run in dev environment
     isExpired=extensions.expireAfterHours(1),  # recache if cached data older than 1 hour
     isSavable=lambda result: bool(result),  # only cache positive function call results
 )
 
-@devCacher.cache()
+@devCacher.cache
 def a(b):
     ...
 
 # works with the same params as devCacher but saves caches to ./tmp1 folder
 @devCacher.cache(tmpDirPath="./tmp1")
 def a1(b):
     ...
```

### Comparing `devpytools-0.1.0.dev4/devpytools/cacher/cache_provider.py` & `devpytools-0.1.0.dev5/devpytools/cacher/cache_provider.py`

 * *Files identical despite different names*

### Comparing `devpytools-0.1.0.dev4/devpytools/cacher/cacher.py` & `devpytools-0.1.0.dev5/devpytools/cacher/cacher.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,41 +117,41 @@
     def _getArgsHash(self, arguments) -> str:
         return hashlib.sha256((";".join(map(lambda x: json.dumps(x, default=self.__defaultSerializeArgs),
                                             arguments))).encode()).hexdigest()
 
     @overload
     def cache(self, func: FuncType, *, tmpDirPath: Optional[Union[str, PathLike]] = None,
               isExpired: Optional[Callable[[int, Any], bool]] = None,
-              uniqueKey: Optional[Union[UniqueKeyType, Iterable[str]]] = None, isEnable: bool = True,
+              uniqueKey: Optional[Union[UniqueKeyType, Iterable[str]]] = None, isEnable: Optional[bool] = None,
               cacheProvider: Optional[CacheProviderABC] = None,
               isSavable: Optional[Callable[[FuncResult], bool]] = None,
-              version=1,) -> FuncType:
+              version=None,) -> FuncType:
         ...
 
     @overload
     def cache(self, func=None, *, tmpDirPath: Optional[Union[str, PathLike]] = None,
               isExpired: Optional[Callable[[int, Any], bool]] = None,
-              uniqueKey: Optional[Union[UniqueKeyType, Iterable[str]]] = None, isEnable: bool = True,
+              uniqueKey: Optional[Union[UniqueKeyType, Iterable[str]]] = None, isEnable: Optional[bool] = None,
               cacheProvider: Optional[CacheProviderABC] = None,
               isSavable: Optional[Callable[[FuncResult], bool]] = None,
-              version=1,) -> Callable[[FuncType], FuncType]:
+              version=None,) -> Callable[[FuncType], FuncType]:
         ...
 
-    def cache(self, func: Optional[FuncType] = None, *, tmpDirPath: Optional[Union[str, PathLike]] = None,
-              isExpired: Optional[Callable[[int, Any], bool]] = None,
-              uniqueKey: Optional[Union[UniqueKeyType, Iterable[str]]] = None, isEnable: bool = True,
-              cacheProvider: Optional[CacheProviderABC] = None,
-              isSavable: Optional[Callable[[FuncResult], bool]] = None,
-              version=1,):
+    def cache(self, func: Optional[FuncType] = None, *, tmpDirPath: Optional[Union[str, PathLike]] = _NoValue,
+              isExpired: Optional[Callable[[int, Any], bool]] = _NoValue,
+              uniqueKey: Optional[Union[UniqueKeyType, Iterable[str]]] = _NoValue, isEnable: Optional[bool] = _NoValue,
+              cacheProvider: Optional[CacheProviderABC] = _NoValue,
+              isSavable: Optional[Callable[[FuncResult], bool]] = _NoValue,
+              version=_NoValue,):
         '''
         when additional params is passed creates new local Cacher object that merges original Cacher params and the new
         '''
         if not func:
             signature = inspect.signature(self.cache)
-            kwargs = {k: v for k, v in locals().items() if k in signature.parameters}
+            kwargs = {k: v for k, v in locals().items() if k in signature.parameters and v is not _NoValue}
             newself = Cacher(**{**self.__dict__, **kwargs, 'isLocal': True})
 
             def dec(func):
                 return self._getDecorated(func, newself)
             return dec
         return self._getDecorated(func, self)
```

### Comparing `devpytools-0.1.0.dev4/devpytools/cacher/extensions.py` & `devpytools-0.1.0.dev5/devpytools/cacher/extensions.py`

 * *Files identical despite different names*

### Comparing `devpytools-0.1.0.dev4/devpytools/other/replace.py` & `devpytools-0.1.0.dev5/devpytools/other/replace.py`

 * *Files identical despite different names*

### Comparing `devpytools-0.1.0.dev4/devpytools.egg-info/PKG-INFO` & `devpytools-0.1.0.dev5/devpytools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpytools
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: Various dev tools.
 Home-page: https://github.com/glowlex/devpytools
 Author: glowlex
 Author-email: antonioavocado777@gmail.com
 License: MIT
 Description: # devpytools
         Tools for development.
@@ -31,15 +31,15 @@
         c = Cacher(name='dev', tmpDirPath='./tmp')
         ```
         
         Get previously configured cacher in other file and use
         ```python
         from devpytools import getCacher
         c = getCacher("dev")
-        @c.cache()
+        @c.cache
         def a(b):
             ...
         ```
         
         Example
         ```python
         from devpytools import Cacher
@@ -50,15 +50,15 @@
             name="dev",
             tmpDirPath="./tmp",
             isEnable=IS_DEV,  # work only if run in dev environment
             isExpired=extensions.expireAfterHours(1),  # recache if cached data older than 1 hour
             isSavable=lambda result: bool(result),  # only cache positive function call results
         )
         
-        @devCacher.cache()
+        @devCacher.cache
         def a(b):
             ...
         
         # works with the same params as devCacher but saves caches to ./tmp1 folder
         @devCacher.cache(tmpDirPath="./tmp1")
         def a1(b):
             ...
```

### Comparing `devpytools-0.1.0.dev4/devpytools.egg-info/SOURCES.txt` & `devpytools-0.1.0.dev5/devpytools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devpytools-0.1.0.dev4/setup.py` & `devpytools-0.1.0.dev5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='devpytools',
-    version='0.1.0.dev4',
+    version='0.1.0.dev5',
     description='Various dev tools.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/glowlex/devpytools',
     author='glowlex',
     author_email='antonioavocado777@gmail.com',
     license='MIT',
```

### Comparing `devpytools-0.1.0.dev4/tests/test_cacher.py` & `devpytools-0.1.0.dev5/tests/test_cacher.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,7 +344,18 @@
     @c.cache
     def a(a, b, c, d, e):
         return var
     assert a("a", (1, 2), ([1],), {}, A()) == 4
     var = 7
     assert a("a", (1, 2), ([1],), {}, A()) == 4
 
+
+def test_updatedCache(inmemResourceSetup):
+    c = Cacher(name='test', uniqueKey=('a', 'b'), version=2, tmpDirPath=TMP_DIR_PATH)
+    var = 4
+
+    @c.cache(uniqueKey=('a', 'b'))
+    def a1(a, b, c):
+        return var
+    assert a1(1, b=2, c=3) == 4
+    var = 7
+    assert a1(b=2, a=1, c=1) == 4
```

### Comparing `devpytools-0.1.0.dev4/tests/test_other.py` & `devpytools-0.1.0.dev5/tests/test_other.py`

 * *Files identical despite different names*

