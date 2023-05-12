# Comparing `tmp/rmmbr-0.0.4.tar.gz` & `tmp/rmmbr-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmmbr-0.0.4.tar", last modified: Tue May  9 13:05:15 2023, max compression
+gzip compressed data, was "rmmbr-0.0.5.tar", last modified: Fri May 12 11:53:26 2023, max compression
```

## Comparing `rmmbr-0.0.4.tar` & `rmmbr-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:05:15.798818 rmmbr-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-09 13:05:15.798818 rmmbr-0.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:05:15.798818 rmmbr-0.0.4/rmmbr/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 13:05:03.000000 rmmbr-0.0.4/rmmbr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-09 13:05:03.000000 rmmbr-0.0.4/rmmbr/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-09 13:05:03.000000 rmmbr-0.0.4/rmmbr/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-09 13:05:03.000000 rmmbr-0.0.4/rmmbr/main_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 13:05:03.000000 rmmbr-0.0.4/rmmbr/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:05:15.798818 rmmbr-0.0.4/rmmbr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-09 13:05:15.000000 rmmbr-0.0.4/rmmbr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-09 13:05:15.000000 rmmbr-0.0.4/rmmbr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:05:15.000000 rmmbr-0.0.4/rmmbr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-09 13:05:15.000000 rmmbr-0.0.4/rmmbr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-09 13:05:15.000000 rmmbr-0.0.4/rmmbr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 13:05:15.000000 rmmbr-0.0.4/rmmbr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:05:15.798818 rmmbr-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-09 13:05:03.000000 rmmbr-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:53:26.492429 rmmbr-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-12 11:53:26.492429 rmmbr-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:53:26.492429 rmmbr-0.0.5/rmmbr/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-12 11:53:17.000000 rmmbr-0.0.5/rmmbr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-12 11:53:17.000000 rmmbr-0.0.5/rmmbr/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-12 11:53:17.000000 rmmbr-0.0.5/rmmbr/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-12 11:53:17.000000 rmmbr-0.0.5/rmmbr/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-12 11:53:17.000000 rmmbr-0.0.5/rmmbr/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:53:26.492429 rmmbr-0.0.5/rmmbr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-12 11:53:26.000000 rmmbr-0.0.5/rmmbr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-12 11:53:26.000000 rmmbr-0.0.5/rmmbr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:53:26.000000 rmmbr-0.0.5/rmmbr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 11:53:26.000000 rmmbr-0.0.5/rmmbr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-12 11:53:26.000000 rmmbr-0.0.5/rmmbr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 11:53:26.000000 rmmbr-0.0.5/rmmbr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:53:26.492429 rmmbr-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-12 11:53:17.000000 rmmbr-0.0.5/setup.py
```

### Comparing `rmmbr-0.0.4/PKG-INFO` & `rmmbr-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: rmmbr
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple persistent caching.
 Home-page: https://github.com/uriva/rmmbr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-`rmmbr` gives you a decorator you can place around async functions to have them be cached, locally or in the cloud.
+`rmmbr` is the simplest way to cache your async functions, locally or in the cloud.
 
 Usage:
 
 ```sh
 npm i rmmbr
 ```
 
 ```js
 import { cloudCache, localCache } from "rmmbr";
 
-const cacher = localCache({ id: "some-id" });
+const cacher = localCache({ id: "name of cache for my function" });
 
 let nCalled = 0;
 const f = (x: number) => {
   nCalled++;
   return Promise.resolve(x);
 };
 const fCached = cacher(f);
@@ -32,40 +32,57 @@
 // nCalled is 1 here
 ```
 
 The local cache stores data in a text file under a `.rmmbr` directory.
 
 There is also a `memCache`, if you are feeling nostalgic 😉 and just want to store stuff in memory.
 
-If you want to persist across devices, we offer a free to use cloud service:
+To persist the cache across devices, we offer a use cloud service, which is free to use up to a quota.
+
+To use it, you can install the CLI tool:
+
+`source <(curl -s https://raw.githubusercontent.com/uriva/rmmbr/main/cli/install.sh)`
+
+Then
+
+```sh
+rmmbr login
+rmmbr api-token
+```
+
+You can then use your token with the API as follows:
 
 ```js
 const cacher = cloudCache({
   token: "service-token",
+  cacheId: "some name for the cache",
   url: "https://uriva-rmmbr.deno.dev",
   ttl: 60 * 60 * 24, // Values will expire after one day, omission of this field implies max.
 });
 ```
 
-If your data is sensitive, you can encrypt it by adding an `encryptionKey` parameter:
+If your data is sensitive, you can e2e encrypt it by adding an `encryptionKey` parameter.
+
+To produce an encryption key:
+
+```sh
+rmmbr secret
+```
+
+Then use it like so:
 
 ```js
 const cacher = cloudCache({
   token: "service-token",
+  cacheId: "some name for the cache",
   url: "https://uriva-rmmbr.deno.dev",
   encryptionKey: "eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee",
 });
 ```
 
-Note that this is implemented as e2e encryption.
-
-At the moment this service is with no guarantees, but we are working on a production tier as well. Please contact us or post an issue if you want to try it out!
-
-We also accept issues for feature requests 👩‍🔧
-
 ## Python
 
 ```sh
 pip install rmmbr
 ```
 
 The python api mimicks the js one, with exported decorators named `mem_cache`, `local_cache` and `cloud_cache`.
```

### Comparing `rmmbr-0.0.4/rmmbr/crypto.py` & `rmmbr-0.0.5/rmmbr/crypto.py`

 * *Files identical despite different names*

### Comparing `rmmbr-0.0.4/rmmbr/main.py` & `rmmbr-0.0.5/rmmbr/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,31 +122,37 @@
                 "Authorization": f"Bearer {token}",
             },
         )
         return response.json()
 
 
 def _set_remote(
-    token: str, url: str, ttl: Optional[int], serialize: Callable[[Serializable], str]
+    url: str,
+    token: str,
+    cache_id: str,
+    ttl: Optional[int],
+    serialize: Callable[[Serializable], str],
 ):
     async def func(key, value):
-        params = {"key": key, "value": serialize(value)}
+        params = {"key": key, "value": serialize(value), "cacheId": cache_id}
         if ttl is not None:
             params["ttl"] = ttl
         await _call_api(url, token, "set", params)
 
     return func
 
 
 _Key = str
 
 
-def _get_remote(token: str, url: str, deserialize: Callable[[str], Serializable]):
+def _get_remote(
+    url: str, token: str, cache_id: str, deserialize: Callable[[str], Serializable]
+):
     async def func(key: _Key):
-        value = await _call_api(url, token, "get", {"key": key})
+        value = await _call_api(url, token, "get", {"key": key, "cacheId": cache_id})
         if value is not None:
             value = deserialize(value)
         return value
 
     return func
 
 
@@ -159,16 +165,17 @@
 
 
 def _decrypt_and_deserialize_output(encryptor: Encryptor, data: str) -> Serializable:
     return deserialize_output(decrypt(encryptor, data))
 
 
 def cloud_cache(
-    token: str,
     url: str,
+    token: str,
+    cache_id: str,
     ttl: Optional[int],
     encryption_key: Optional[str],
 ):
     if encryption_key is not None:
         encryptor = encryptor_from_key(encryption_key.encode())
         key_arguments_func = partial(_private_key_arguments, encryption_key.encode())
         serialize_output_func = partial(_serialize_and_encrypt_output, encryptor)
@@ -179,12 +186,12 @@
         serialize_output_func = serialize_output
         deserialize_output_func = deserialize_output
 
     def inner_func(f):
         return _abstract_cache_params(
             key_arguments_func,
             f,
-            _get_remote(token, url, deserialize_output_func),
-            _set_remote(token, url, ttl, serialize_output_func),
+            _get_remote(url, token, cache_id, deserialize_output_func),
+            _set_remote(url, token, cache_id, ttl, serialize_output_func),
         )
 
     return inner_func
```

### Comparing `rmmbr-0.0.4/rmmbr/main_test.py` & `rmmbr-0.0.5/rmmbr/main_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,28 +69,29 @@
 _port = _env_param("PORT")
 _mock_backend_url = f"http://localhost:{_port}"
 
 
 async def test_cloud_cache():
     await _clean_redis()
     await _cache_test_helper(False, False)(
-        cloud_cache("some-token", _mock_backend_url, None, None)
+        cloud_cache(_mock_backend_url, "some-token", "my_function_name", None, None)
     )
 
 
 async def test_cloud_cache_expiration():
     await _clean_redis()
     await _cache_test_helper(False, True)(
-        cloud_cache("some-token", _mock_backend_url, 1, None)
+        cloud_cache(_mock_backend_url, "some-token", "my_function_name", 1, None)
     )
 
 
 async def test_cloud_cache_encryption():
     await _clean_redis()
     await _cache_test_helper(False, False)(
         cloud_cache(
-            "some-token",
             _mock_backend_url,
+            "some-token",
+            "my_function_name",
             None,
             "Cqq33cbHu9AEUaP_wS3LCDQN7wy40XKWzALoPHbU5S8=",
         )
     )
```

### Comparing `rmmbr-0.0.4/rmmbr.egg-info/PKG-INFO` & `rmmbr-0.0.5/rmmbr.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: rmmbr
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple persistent caching.
 Home-page: https://github.com/uriva/rmmbr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-`rmmbr` gives you a decorator you can place around async functions to have them be cached, locally or in the cloud.
+`rmmbr` is the simplest way to cache your async functions, locally or in the cloud.
 
 Usage:
 
 ```sh
 npm i rmmbr
 ```
 
 ```js
 import { cloudCache, localCache } from "rmmbr";
 
-const cacher = localCache({ id: "some-id" });
+const cacher = localCache({ id: "name of cache for my function" });
 
 let nCalled = 0;
 const f = (x: number) => {
   nCalled++;
   return Promise.resolve(x);
 };
 const fCached = cacher(f);
@@ -32,40 +32,57 @@
 // nCalled is 1 here
 ```
 
 The local cache stores data in a text file under a `.rmmbr` directory.
 
 There is also a `memCache`, if you are feeling nostalgic 😉 and just want to store stuff in memory.
 
-If you want to persist across devices, we offer a free to use cloud service:
+To persist the cache across devices, we offer a use cloud service, which is free to use up to a quota.
+
+To use it, you can install the CLI tool:
+
+`source <(curl -s https://raw.githubusercontent.com/uriva/rmmbr/main/cli/install.sh)`
+
+Then
+
+```sh
+rmmbr login
+rmmbr api-token
+```
+
+You can then use your token with the API as follows:
 
 ```js
 const cacher = cloudCache({
   token: "service-token",
+  cacheId: "some name for the cache",
   url: "https://uriva-rmmbr.deno.dev",
   ttl: 60 * 60 * 24, // Values will expire after one day, omission of this field implies max.
 });
 ```
 
-If your data is sensitive, you can encrypt it by adding an `encryptionKey` parameter:
+If your data is sensitive, you can e2e encrypt it by adding an `encryptionKey` parameter.
+
+To produce an encryption key:
+
+```sh
+rmmbr secret
+```
+
+Then use it like so:
 
 ```js
 const cacher = cloudCache({
   token: "service-token",
+  cacheId: "some name for the cache",
   url: "https://uriva-rmmbr.deno.dev",
   encryptionKey: "eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee",
 });
 ```
 
-Note that this is implemented as e2e encryption.
-
-At the moment this service is with no guarantees, but we are working on a production tier as well. Please contact us or post an issue if you want to try it out!
-
-We also accept issues for feature requests 👩‍🔧
-
 ## Python
 
 ```sh
 pip install rmmbr
 ```
 
 The python api mimicks the js one, with exported decorators named `mem_cache`, `local_cache` and `cloud_cache`.
```

### Comparing `rmmbr-0.0.4/setup.py` & `rmmbr-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages, setup
 
 _repo_dir = os.environ.get("GITHUB_WORKSPACE")
 assert _repo_dir
 setup(
     name="rmmbr",
-    version="0.0.4",
+    version="0.0.5",
     description="Simple persistent caching.",
     long_description=(pathlib.Path(_repo_dir) / "README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/uriva/rmmbr",
     packages=find_packages(),
     install_requires=[
         "redis>=3.5.3",
```

