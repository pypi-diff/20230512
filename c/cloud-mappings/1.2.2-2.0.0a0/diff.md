# Comparing `tmp/cloud-mappings-1.2.2.tar.gz` & `tmp/cloud-mappings-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cloud-mappings/cloud-mappings/dist/tmpj1dr6jew/cloud-mappings-1.2.2.tar", last modified: Mon Aug 29 13:44:12 2022, max compression
+gzip compressed data, was "/home/runner/work/cloud-mappings/cloud-mappings/dist/.tmp-6y3loxyk/cloud-mappings-2.0.0a0.tar", last modified: Fri May 12 03:32:19 2023, max compression
```

## Comparing `cloud-mappings-1.2.2.tar` & `cloud-mappings-2.0.0a0.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 13:44:12.000000 cloud-mappings-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-08-29 13:43:43.000000 cloud-mappings-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6595 2022-08-29 13:44:12.000000 cloud-mappings-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5878 2022-08-29 13:43:43.000000 cloud-mappings-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-08-29 13:43:43.000000 cloud-mappings-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-08-29 13:44:12.000000 cloud-mappings-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 13:44:12.000000 cloud-mappings-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 13:44:12.000000 cloud-mappings-1.2.2/src/cloud_mappings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6595 2022-08-29 13:44:12.000000 cloud-mappings-1.2.2/src/cloud_mappings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-08-29 13:44:12.000000 cloud-mappings-1.2.2/src/cloud_mappings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-29 13:44:12.000000 cloud-mappings-1.2.2/src/cloud_mappings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-08-29 13:44:12.000000 cloud-mappings-1.2.2/src/cloud_mappings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-29 13:44:12.000000 cloud-mappings-1.2.2/src/cloud_mappings.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 13:44:12.000000 cloud-mappings-1.2.2/src/cloudmappings/
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-08-29 13:43:43.000000 cloud-mappings-1.2.2/src/cloudmappings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11678 2022-08-29 13:43:43.000000 cloud-mappings-1.2.2/src/cloudmappings/cloudstoragemapping.py
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-08-29 13:43:43.000000 cloud-mappings-1.2.2/src/cloudmappings/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 13:44:12.000000 cloud-mappings-1.2.2/src/cloudmappings/storageproviders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-29 13:43:43.000000 cloud-mappings-1.2.2/src/cloudmappings/storageproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4997 2022-08-29 13:43:43.000000 cloud-mappings-1.2.2/src/cloudmappings/storageproviders/awss3.py
--rw-r--r--   0 runner    (1001) docker     (121)     4087 2022-08-29 13:43:43.000000 cloud-mappings-1.2.2/src/cloudmappings/storageproviders/azureblobstorage.py
--rw-r--r--   0 runner    (1001) docker     (121)     5292 2022-08-29 13:43:43.000000 cloud-mappings-1.2.2/src/cloudmappings/storageproviders/azuretablestorage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2939 2022-08-29 13:43:43.000000 cloud-mappings-1.2.2/src/cloudmappings/storageproviders/googlecloudstorage.py
--rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-08-29 13:43:43.000000 cloud-mappings-1.2.2/src/cloudmappings/storageproviders/storageprovider.py
--rw-r--r--   0 runner    (1001) docker     (121)     4959 2022-08-29 13:43:43.000000 cloud-mappings-1.2.2/src/cloudmappings/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14037 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloud_mappings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloud_mappings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloud_mappings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloud_mappings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloud_mappings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloud_mappings.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloudmappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/_cloudmappinginternal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/awss3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/azureblobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/azuretablestorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/googlecloudstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/cloudmapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/cloudstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:32:19.000000 cloud-mappings-2.0.0a0/src/cloudmappings/serialisers/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/serialisers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/serialisers/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/serialisers/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/serialisers/serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-12 03:31:50.000000 cloud-mappings-2.0.0a0/src/cloudmappings/storageprovider.py
```

### Comparing `cloud-mappings-1.2.2/LICENSE` & `cloud-mappings-2.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-mappings-1.2.2/setup.cfg` & `cloud-mappings-2.0.0a0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cloud-mappings
-version = 1.2.2
+version = attr: cloudmappings.__version__
 author = Lucas Sargent
 author_email = lucas.sargent@outlook.com
 description = MutableMapping interfaces for common cloud storage providers
 keywords = mutable dict aws s3 azure gcp
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JJ11teen/cloud-mappings
@@ -18,18 +18,18 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
 
 [options.extras_require]
-azureblob = azure-identity==1.10.0; azure-storage-blob==12.13.1
-azuretable = azure-identity==1.10.0; azure-data-tables==12.4.0
-gcpstorage = google-cloud-storage==2.5.0
-awss3 = boto3==1.24.54
+azureblob = azure-identity==1.12.0; azure-storage-blob==12.16.0
+azuretable = azure-identity==1.12.0; azure-data-tables==12.4.2
+gcpstorage = google-cloud-storage==2.9.0
+awss3 = boto3==1.26.129
 tests = pytest==7.1.2
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `cloud-mappings-1.2.2/src/cloud_mappings.egg-info/SOURCES.txt` & `cloud-mappings-2.0.0a0/src/cloud_mappings.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -4,16 +4,21 @@
 setup.cfg
 src/cloud_mappings.egg-info/PKG-INFO
 src/cloud_mappings.egg-info/SOURCES.txt
 src/cloud_mappings.egg-info/dependency_links.txt
 src/cloud_mappings.egg-info/requires.txt
 src/cloud_mappings.egg-info/top_level.txt
 src/cloudmappings/__init__.py
-src/cloudmappings/cloudstoragemapping.py
+src/cloudmappings/_cloudmappinginternal.py
+src/cloudmappings/cloudmapping.py
+src/cloudmappings/cloudstorage.py
 src/cloudmappings/errors.py
-src/cloudmappings/wrappers.py
-src/cloudmappings/storageproviders/__init__.py
-src/cloudmappings/storageproviders/awss3.py
-src/cloudmappings/storageproviders/azureblobstorage.py
-src/cloudmappings/storageproviders/azuretablestorage.py
-src/cloudmappings/storageproviders/googlecloudstorage.py
-src/cloudmappings/storageproviders/storageprovider.py
+src/cloudmappings/storageprovider.py
+src/cloudmappings/_storageproviders/__init__.py
+src/cloudmappings/_storageproviders/awss3.py
+src/cloudmappings/_storageproviders/azureblobstorage.py
+src/cloudmappings/_storageproviders/azuretablestorage.py
+src/cloudmappings/_storageproviders/googlecloudstorage.py
+src/cloudmappings/serialisers/__init__.py
+src/cloudmappings/serialisers/core.py
+src/cloudmappings/serialisers/pandas.py
+src/cloudmappings/serialisers/serialisation.py
```

### Comparing `cloud-mappings-1.2.2/src/cloudmappings/cloudstoragemapping.py` & `cloud-mappings-2.0.0a0/src/cloudmappings/cloudstorage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,286 +1,217 @@
-from functools import partial
-from typing import Any, Callable, Dict, List, MutableMapping
+from typing import Any, Optional, TypeVar
 
-from .storageproviders.storageprovider import StorageProvider
+from cloudmappings._cloudmappinginternal import CloudMappingInternal
+from cloudmappings.cloudmapping import CloudMapping
+from cloudmappings.serialisers import CloudMappingSerialisation
+from cloudmappings.serialisers.core import pickle
+from cloudmappings.storageprovider import StorageProvider
 
+T = TypeVar("T")
 
-class CloudMapping(MutableMapping):
-    """A cloud-mapping, a `MutableMapping` implementation backed by common cloud storage solutions.
 
-    Parameters
-    ----------
-    storage_provider : StorageProvider
-        The storage provider to use as the backing for the cloud-mapping.
-    sync_initially : bool, default=True
-        Whether to call `sync_with_cloud` initially
-    read_blindly : bool, default=False
-        Whether to read blindly or not by default. See `read_blindly` attribute for more
-        information.
-    read_blindly_error : bool, default=False
-        Whether to raise `KeyError`s when read_blindly is enabled and the key does not have a value
-        in the cloud.
-    read_blindly_default : Any, default=None
-        The value to return when read_blindly is enabled, the key does not have a value in the
-        cloud, and read_blindly_error is `False`.
-    ordered_dumps_funcs : List[Callable]
-        An ordered list of functions to pass values through before saving bytes to the cloud.
-        The last function must return a bytes-like object.
-    ordered_loads_funcs : List[Callable]
-        An ordered list of functions to pass values through before saving bytes to the cloud.
-        The first function must expect a bytes-like object as its input.
-    """
-
-    read_blindly: bool
-    """ Whether the cloud-mapping is currently set to read from the cloud blindly.
-
-        When read blindly is `False`, a cloud-mapping will raise a KeyError if a key that it
-        doesn't know about is accessed. If a key that it does know about is accessed but then
-        found to be out of sync with the cloud, a `cloudmappings.errors.KeySyncError` will be
-        raised.
-
-        When read blindly is `True`, a cloud-mapping will return the latest cloud version
-        for any key accessed, including keys it has no prior knowledge of (ie not in it's etag
-        dict). If there is no value for a key in the cloud, whether a `KeyValue` error is
-        raised is controlled by the `read_blindly_error` flag. If `False`, the current value of
-        `read_blindly_default` will be returned.
-
-        When read blindly is `True` a cloud-mapping will not raise `cloudmappings.errors.KeySyncError`
-        errors for read/get operations.
-
-        By default a cloud-mapping is instantiated with read blindly set to `False`.
-    """
-
-    read_blindly_error: bool
-    """Whether to raise a `KeyValue` error when read_blindly is `True` and the key does not have
-        a value in the cloud. If `True`, this takes prescedence over `read_blindly_default`.
-    """
-
-    read_blindly_default: Any
-    """The value to return when read_blindly is `True`, the key does not have a value in the cloud,
-        and read_blindly_error is `False`.
-    """
+class CloudStorage:
+    def __init__(self, storage_provider: StorageProvider) -> None:
+        self._storage_provider = storage_provider
 
-    def __init__(
+    @property
+    def storage_provider(self) -> StorageProvider:
+        return self._storage_provider
+
+    def create_mapping(
         self,
-        storage_provider: StorageProvider,
         sync_initially: bool = True,
         read_blindly: bool = False,
         read_blindly_error: bool = False,
         read_blindly_default: Any = None,
-        ordered_dumps_funcs: List[Callable] = None,
-        ordered_loads_funcs: List[Callable] = None,
-    ) -> None:
+        serialisation: CloudMappingSerialisation[T] = pickle(),
+        key_prefix: Optional[str] = None,
+    ) -> CloudMapping[T]:
         """A cloud-mapping, a `MutableMapping` implementation backed by common cloud storage solutions.
 
         Parameters
         ----------
-        storage_provider : StorageProvider
-            The storage provider to use as the backing for the cloud-mapping.
         sync_initially : bool, default=True
             Whether to call `sync_with_cloud` initially
         read_blindly : bool, default=False
-            Whether to read blindly or not by default. See `read_blindly` attribute for more
-            information
+            Whether the `CloudMapping` will read from the cloud without synchronising.
+            When `read_blindly=False`, a `CloudMapping` will raise a `KeyError` unless a key has been
+            previously written using the same `CloudMapping` instance, or `.sync_with_cloud` has been
+            called and the key was in the cloud. If the value in the cloud has changed since being
+            written or synchronised, a `cloudmappings.errors.KeySyncError` will be raised.
+            When `read_blindly=True`, a `CloudMapping` will directly query the cloud for any key
+            accessed, regardless of if it has previously written a value to that key. It will always get
+            the latest value from the cloud, and never raise a `cloudmappings.errors.KeySyncError` for
+            read operations. If there is no value for a key in the cloud, and `read_blindly_error=True`,
+            a `KeyError` will be raised. If there is no value for a key in the cloud and
+            `read_blindly_error=False`, `read_blindly_default` will be returned.
         read_blindly_error : bool, default=False
-            Whether to raise `KeyError`s when read_blindly is enabled and the key does not have a value
-            in the cloud
+            Whether to raise a `KeyValue` error when `read_blindly=True` and a key does not have
+            a value in the cloud. If `True`, this takes prescedence over `read_blindly_default`.
         read_blindly_default : Any, default=None
-            The value to return when read_blindly is enabled, the key does not have a value in the
-            cloud, and read_blindly_error is `False`
-        ordered_dumps_funcs : List[Callable], default=None
-            An ordered list of functions to pass values through before saving bytes to the cloud.
-            The last function must return a bytes-like object.
-        ordered_loads_funcs : List[Callable], default=None
-            An ordered list of functions to pass values through before saving bytes to the cloud.
-            The first function must expect a bytes-like object as its input.
-        """
-        self._storage_provider = storage_provider
-        self._etags = {}
-        self._ordered_dumps_funcs = ordered_dumps_funcs if ordered_dumps_funcs is not None else []
-        self._ordered_loads_funcs = ordered_loads_funcs if ordered_loads_funcs is not None else []
-
-        self.read_blindly = read_blindly
-        self.read_blindly_error = read_blindly_error
-        self.read_blindly_default = read_blindly_default
-
-        if self._storage_provider.create_if_not_exists() and sync_initially:
-            self.sync_with_cloud()
+            The value to return when `read_blindly=True`, a key does not have a value in the cloud,
+            and `read_blindly_error=False`.
+        serialiser : CloudMappingSerialiser, default=pickle()
+            CloudMappingSerialiser to use, defaults to `pickle`.
+        key_prefix : Optional[str], default=None
+            Prefix to apply to keys in cloud storage. Enables `CloudMapping`s to map to a subdirectory
+            within a cloud storage service, as opposed to the whole resource.
+        """
+        mapping = CloudMappingInternal()
+        mapping._storage_provider = self.storage_provider
+        mapping._etags = {}
+        mapping._serialisation = serialisation
+        mapping._key_prefix = key_prefix
+
+        mapping.read_blindly = read_blindly
+        mapping.read_blindly_error = read_blindly_error
+        mapping.read_blindly_default = read_blindly_default
 
-    def _encode_key(self, unsafe_key: str) -> str:
-        if not isinstance(unsafe_key, str):
-            raise TypeError("Key must be of type 'str'. Got key:", unsafe_key)
-        return self._storage_provider.encode_key(unsafe_key=unsafe_key)
+        if self.storage_provider.create_if_not_exists() and sync_initially:
+            mapping.sync_with_cloud()
 
-    def sync_with_cloud(self, key_prefix: str = None) -> None:
-        """Synchronise this cloud-mapping's etags with the cloud.
+        return mapping
 
-        This allows a cloud-mapping to reflect the most recent updates to the cloud resource,
-        including those made by other instances or users. This can allow destructive operations
-        as a user may sync to get the latest updates, and then overwrite or delete keys.
 
-        Consider calling this if you are encountering a `cloudmappings.errors.KeySyncError`,
-        and you are sure you would like to force the operation anyway.
-
-        This is called by default on instantiation of a cloud-mapping.
+class AzureBlobStorage(CloudStorage):
+    def __init__(
+        self,
+        container_name: str,
+        credential: Any,
+        account_url: str = None,
+        connection_string: str = None,
+        create_container_metadata=None,
+    ) -> None:
+        """A cloud-mapping backed by an Azure Blob Storage Container
 
         Parameters
         ----------
-        key_prefix : str, optional
-            Only sync keys beginning with the specified prefix
-        """
-        key_prefix = None if key_prefix is None else self._encode_key(key_prefix)
-        self._etags.update(
-            {
-                self._storage_provider.decode_key(k): i
-                for k, i in self._storage_provider.list_keys_and_etags(key_prefix).items()
-            }
-        )
-
-    @property
-    def etags(self) -> Dict:
-        """An internal dictionary of etags used to ensure the cloud-mapping is in sync with
-        the cloud storage resource. The dict is itself a mapping, mapping keys to their etags.
-
-        This dictionary is used as the cloud-mapping's expected view of the cloud. It is used
-        to determine if a key exists, and ensure that the value at each key is expected.
-
-        See: https://en.wikipedia.org/wiki/HTTP_ETag
-        """
-        return self._etags
-
-    def __getitem__(self, key: str) -> Any:
-        if not self.read_blindly and key not in self._etags:
-            raise KeyError(key)
-        value = self._storage_provider.download_data(
-            key=self._encode_key(key), etag=None if self.read_blindly else self._etags[key]
-        )
-        if self.read_blindly and value is None:
-            if self.read_blindly_error:
-                raise KeyError(key)
-            return self.read_blindly_default
-        for loads in self._ordered_loads_funcs:
-            value = loads(value)
-        return value
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        for dumps in self._ordered_dumps_funcs:
-            value = dumps(value)
-        self._etags[key] = self._storage_provider.upload_data(
-            key=self._encode_key(key),
-            etag=self._etags.get(key, None),
-            data=value,
+        container_name : str
+            The name of the Azure Storage Blob Container to use within the Azure Storage Account
+        credential : Any
+            A credential object from `azure.identity`
+        account_url : str, default=None
+            The url of the Azure Storage Account to use
+        connection_string : str, default=None
+            A connection string to use for the Azure Blob Storage Container. Takes precedence over
+            `account_url` and `credential` if given
+
+        See Also
+        --------
+        cloud-mapping : `CloudMapping`
+        """
+        from cloudmappings._storageproviders.azureblobstorage import (
+            AzureBlobStorageProvider,
+        )
+
+        super().__init__(
+            AzureBlobStorageProvider(
+                container_name=container_name,
+                credential=credential,
+                account_url=account_url,
+                connection_string=connection_string,
+                create_container_metadata=create_container_metadata,
+            )
         )
 
-    def __delitem__(self, key: str) -> None:
-        if key not in self._etags:
-            raise KeyError(key)
-        self._storage_provider.delete_data(key=self._encode_key(key), etag=self._etags[key])
-        del self._etags[key]
 
-    def __contains__(self, key: str) -> bool:
-        return key in self._etags
-
-    def keys(self):
-        return iter(self._etags.keys())
-
-    __iter__ = keys
-
-    def __len__(self) -> int:
-        return len(self._etags)
-
-    def __repr__(self) -> str:
-        return f"cloudmapping<{self._storage_provider.logical_name()}>"
+class AzureTableStorage(CloudStorage):
+    def __init__(
+        self,
+        table_name: str,
+        credential: Any,
+        endpoint: str = None,
+        connection_string: str = None,
+    ) -> None:
+        """A cloud-mapping backed by an Azure Table Storage Table
 
-    @classmethod
-    def with_pickle(cls, *args, **kwargs) -> "CloudMapping":
-        """Create a cloud-mapping instance that pickles values using pythons `pickle`
+        Note that Azure Table Storage has a 1MB size limit per entity. This mapping distributes
+        bytes across dummy attributes within an entity to ensure attribute level limits are not
+        hit. This results in a 1MB limit for each value stored in this mapping.
 
         Parameters
         ----------
-        *args : tuple, optional
-            Additional positional arguments to pass to the CloudMapping constructor
-        **kwargs : dict, optional
-            Additional keyword arguments to pass to the CloudMapping constructor
-
-        Returns
-        -------
-        CloudMapping
-            A new cloud-mapping setup with pickle serialisation
-        """
-        import pickle
-
-        kwargs.update(
-            dict(
-                ordered_dumps_funcs=[pickle.dumps],
-                ordered_loads_funcs=[pickle.loads],
+        table_name : str
+            The name of the Azure Storage Table to use within the Azure Storage Account
+        credential : Any
+            A credential object from `azure.identity`
+        endpoint : str, default=None
+            The table endpoint of the Azure Storage Account to use
+        connection_string : str, default=None
+            A connection string to use for the Azure Table Storage Table. Takes precedence over
+            `endpoint` and `credential` if given
+
+        See Also
+        --------
+        cloud-mapping : `CloudMapping`
+        """
+        from cloudmappings._storageproviders.azuretablestorage import (
+            AzureTableStorageProvider,
+        )
+
+        super().__init__(
+            AzureTableStorageProvider(
+                table_name=table_name,
+                credential=credential,
+                endpoint=endpoint,
+                connection_string=connection_string,
             )
         )
-        return cls(*args, **kwargs)
 
-    @classmethod
-    def with_json(cls, encoding="utf-8", *args, **kwargs) -> "CloudMapping":
-        """Create a cloud-mapping instance that serialises values to JSON strings
+
+class GoogleCloudStorage(CloudStorage):
+    def __init__(
+        self,
+        bucket_name: str,
+        project: str,
+        credentials: Any = None,
+    ) -> None:
+        """A cloud-mapping backed by a Google Cloud Storage Bucket
 
         Parameters
         ----------
-        encoding : str, default="utf-8"
-            The string encoding to use, passed to bytes() and str() for dumps and loads respectively.
-        *args : tuple, optional
-            Additional positional arguments to pass to the CloudMapping constructor
-        **kwargs : dict, optional
-            Additional keyword arguments to pass to the CloudMapping constructor
-
-        Returns
-        -------
-        CloudMapping
-            A new cloud-mapping setup with JSON string serialisation
-        """
-        import json
+        bucket_name : str
+            The name of the Storage Bucket to use within Google Cloud Storage
+        project : str
+            The GCP project to use
+        credentials : optional
+            A credentials object from various google client libraries
 
-        kwargs.update(
-            dict(
-                ordered_dumps_funcs=[partial(json.dumps, sort_keys=True), partial(bytes, encoding=encoding)],
-                ordered_loads_funcs=[partial(str, encoding=encoding), json.loads],
-            )
+        See Also
+        --------
+        cloud-mapping : `CloudMapping`
+        """
+        from cloudmappings._storageproviders.googlecloudstorage import (
+            GoogleCloudStorageProvider,
         )
-        return cls(*args, **kwargs)
 
-    @classmethod
-    def with_json_zlib(cls, encoding="utf-8", *args, **kwargs) -> "CloudMapping":
-        """Create a cloud-mapping instance that serialises values to compressed JSON strings
+        super().__init__(GoogleCloudStorageProvider(bucket_name=bucket_name, project=project, credentials=credentials))
 
-        Uses zlib to compress values after serialising them JSON strings.
+
+class AWSS3Storage(CloudStorage):
+    def __init__(
+        self,
+        bucket_name: str,
+        silence_warning: bool = False,
+    ) -> None:
+        """A cloud-mapping backed by an AWS S3 Bucket
+
+        Note that AWS S3 does not support service-side atomic requests, which means there is
+        a race condition when multiple clients are uploading data at the same time. Because of
+        this, *AWS S3 is not recommended for concurrent use*. Consider using Azure or GCP is
+        you need concurrent access. A warning about this will be logged by default when using
+        `AWSS3Mapping`. This warning can be silenced with `silence_warning=True`.
 
         Parameters
         ----------
-        encoding : str, default="utf-8"
-            The string encoding to use, passed to bytes() and str() for dumps and loads
-            respectively.
-        *args : tuple, optional
-            Additional positional arguments to pass to the CloudMapping constructor
-        **kwargs : dict, optional
-            Additional keyword arguments to pass to the CloudMapping constructor
-
-        Returns
-        -------
-        CloudMapping
-            A new cloud-mapping setup with zlib compression and JSON string serialisation
+        bucket_name : str
+            The name of the S3 Bucket to use within AWS
+        silence_warning : bool, default=False
+            Whether to silence the warning logged about using S3 backed cloud-mappings concurrently
+
+        See Also
+        --------
+        cloud-mapping : `CloudMapping`
         """
-        import json
-        import zlib
+        from cloudmappings._storageproviders.awss3 import AWSS3Provider
 
-        kwargs.update(
-            dict(
-                ordered_dumps_funcs=[
-                    partial(json.dumps, sort_keys=True),
-                    partial(bytes, encoding=encoding),
-                    zlib.compress,
-                ],
-                ordered_loads_funcs=[
-                    zlib.decompress,
-                    partial(str, encoding=encoding),
-                    json.loads,
-                ],
-            )
-        )
-        return cls(*args, **kwargs)
+        super().__init__(AWSS3Provider(bucket_name=bucket_name, silence_warning=silence_warning))
```

### Comparing `cloud-mappings-1.2.2/src/cloudmappings/errors.py` & `cloud-mappings-2.0.0a0/src/cloudmappings/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class KeySyncError(ValueError):
+class KeySyncError(KeyError):
     storage_provider_name: str
     key: str
     expected_etag: str
 
     def __init__(self, storage_provider_name: str, key: str, etag: str) -> None:
         self.storage_provider_name = storage_provider_name
         self.key = key
```

### Comparing `cloud-mappings-1.2.2/src/cloudmappings/storageproviders/awss3.py` & `cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/awss3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import logging
 from typing import Dict
 from uuid import uuid4
 
 import boto3
 
-from .storageprovider import StorageProvider
+from cloudmappings.errors import KeySyncError
+from cloudmappings.storageprovider import StorageProvider
+
+logger = logging.getLogger(__name__)
 
 _metadata_etag_key = "cloud-mappings-etag"
 
 
 class AWSS3Provider(StorageProvider):
     def __init__(
         self,
         bucket_name: str,
         silence_warning: bool = False,
     ) -> None:
         self._client = boto3.client("s3")
         self._bucket_name = bucket_name
         if not silence_warning:
-            logging.warning(
+            logger.warning(
                 msg=(
                     "AWS S3 does not support server-side atomic requests, it is not recommended for concurrent use.\n",
                     "Consider using another provider such as Azure or GCP if you need concurrent access.\n",
                     "You may silence this warning with silence_warning=True.",
                 ),
             )
 
@@ -65,25 +68,25 @@
             )
         except self._client.exceptions.NoSuchKey:
             return (None, None, None)
 
     def download_data(self, key: str, etag: str) -> bytes:
         body, existing_etag, _ = self._get_body_etag_version_id_if_exists(key)
         if etag is not None and (body is None or etag != existing_etag):
-            self.raise_key_sync_error(key=key, etag=etag)
+            raise KeySyncError(storage_provider_name=self.logical_name(), key=key, etag=etag)
         if body is None:
             return None
         return body.read()
 
     def upload_data(self, key: str, etag: str, data: bytes) -> str:
         if not isinstance(data, bytes):
-            raise ValueError("Data must be bytes like")
+            raise ValueError(f"Data must be bytes like, got {type(data)}")
         _, existing_etag, _ = self._get_body_etag_version_id_if_exists(key)
         if etag != existing_etag:
-            self.raise_key_sync_error(key=key, etag=etag)
+            raise KeySyncError(storage_provider_name=self.logical_name(), key=key, etag=etag)
         # Note: There is a race condition here:
         # If blob is changed after the etag is fetched but before the put_object call succeeds.
         # Currently, the S3 API does not appear to support any parameters that would enable server-side
         # conflict checking.
         # TODO: Monitor S3 API to see if a parameter to support atomic requests is added.
         new_etag = str(uuid4())
         self._client.put_object(
@@ -95,25 +98,25 @@
             },
         )
         return new_etag
 
     def delete_data(self, key: str, etag: str) -> None:
         body, existing_etag, version_id = self._get_body_etag_version_id_if_exists(key)
         if body is None or etag != existing_etag:
-            self.raise_key_sync_error(key=key, etag=etag)
+            raise KeySyncError(storage_provider_name=self.logical_name(), key=key, etag=etag)
         # Note: There is a race condition here:
         # If blob is changed after the etag is fetched but before the delete_object call succeeds.
         # Currently, the S3 API does not appear to support any parameters that would enable server-side
         # conflict checking.
         # TODO: Monitor S3 API to see if a parameter to support atomic requests is added.
         self._client.delete_object(
             Bucket=self._bucket_name,
             Key=key,
             VersionId=version_id,
         )
 
     def list_keys_and_etags(self, key_prefix: str) -> Dict[str, str]:
         bucket = boto3.resource("s3").Bucket(self._bucket_name)
         kwargs = {}
-        if key_prefix is not None:
+        if key_prefix:
             kwargs["Prefix"] = key_prefix
         return {o.key: o.Object().metadata[_metadata_etag_key] for o in bucket.objects.filter(**kwargs)}
```

### Comparing `cloud-mappings-1.2.2/src/cloudmappings/storageproviders/azureblobstorage.py` & `cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/azureblobstorage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import json
-from typing import Dict
+from typing import Any, Dict
 
 from azure.core import MatchConditions
 from azure.core.exceptions import (
     ResourceExistsError,
     ResourceModifiedError,
     ResourceNotFoundError,
 )
-from azure.identity import DefaultAzureCredential
 from azure.storage.blob import ContainerClient
 
-from .storageprovider import StorageProvider
+from cloudmappings.errors import KeySyncError
+from cloudmappings.storageprovider import StorageProvider
 
 
 class AzureBlobStorageProvider(StorageProvider):
     def __init__(
         self,
         container_name: str,
+        credential: Any,
         account_url: str = None,
-        credential=DefaultAzureCredential(),
         connection_string: str = None,
         create_container_metadata=None,
     ) -> None:
         if connection_string:
             self._container_client = ContainerClient.from_connection_string(
                 conn_str=connection_string, container_name=container_name
             )
@@ -56,23 +56,23 @@
                     etag=etag,
                     match_condition=MatchConditions.IfNotModified,
                 )
             )
         try:
             return self._container_client.download_blob(**args).readall()
         except ResourceModifiedError as e:
-            self.raise_key_sync_error(key=key, etag=etag, inner_exception=e)
+            raise KeySyncError(storage_provider_name=self.logical_name(), key=key, etag=etag) from e
         except ResourceNotFoundError as e:
             if etag is None:
                 return None
-            self.raise_key_sync_error(key=key, etag=etag, inner_exception=e)
+            raise KeySyncError(storage_provider_name=self.logical_name(), key=key, etag=etag) from e
 
     def upload_data(self, key: str, etag: str, data: bytes) -> str:
         if not isinstance(data, bytes):
-            raise ValueError("Data must be bytes like")
+            raise ValueError(f"Data must be bytes like, got {type(data)}")
         expecting_blob = etag is not None
         args = dict(overwrite=expecting_blob)
         if expecting_blob:
             args.update(
                 dict(
                     etag=etag,
                     match_condition=MatchConditions.IfNotModified,
@@ -81,31 +81,31 @@
         bc = self._container_client.get_blob_client(blob=key)
         try:
             response = bc.upload_blob(
                 data=data,
                 **args,
             )
         except (ResourceExistsError, ResourceModifiedError) as e:
-            self.raise_key_sync_error(key=key, etag=etag, inner_exception=e)
+            raise KeySyncError(storage_provider_name=self.logical_name(), key=key, etag=etag) from e
         return json.loads(response["etag"])
 
     def delete_data(self, key: str, etag: str) -> None:
         try:
             self._container_client.delete_blob(
                 blob=key,
                 etag=etag,
                 match_condition=MatchConditions.IfNotModified,
             )
         except ResourceModifiedError as e:
-            self.raise_key_sync_error(key=key, etag=etag, inner_exception=e)
+            raise KeySyncError(storage_provider_name=self.logical_name(), key=key, etag=etag) from e
 
     def list_keys_and_etags(self, key_prefix: str) -> Dict[str, str]:
         # If the container has hierarchical namespaces enabled, this call
         # will return files as well as subdirectories.
         # Unforunately there is no serverside api to filter, so we
         # rely on checking the content_type & content_md5 hash
         # If both are None, we assume the listing is a dir skip it
         return {
             b.name: b.etag
             for b in self._container_client.list_blobs(name_starts_with=key_prefix)
-            if b.content_settings.content_type is not None and b.content_settings.content_md5 is not None
+            if b.content_settings.content_type is not None or b.content_settings.content_md5 is not None
         }
```

### Comparing `cloud-mappings-1.2.2/src/cloudmappings/storageproviders/azuretablestorage.py` & `cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/azuretablestorage.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Dict
+from typing import Any, Dict
 from urllib.parse import quote, unquote
 
 from azure.core import MatchConditions
 from azure.core.exceptions import (
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
 )
 from azure.data.tables import TableClient, UpdateMode
-from azure.identity import DefaultAzureCredential
 
-from .storageprovider import StorageProvider
+from cloudmappings.errors import KeySyncError, ValueSizeError
+from cloudmappings.storageprovider import StorageProvider
 
 
 def _chunk_bytes(data: bytes) -> Dict[str, bytes]:
     # Max property size in azure tables is 64KiB
     max_property_size = 64 * 1024
     return {f"d_{k}": data[i : i + max_property_size] for k, i in enumerate(range(0, len(data), max_property_size))}
 
@@ -23,16 +23,16 @@
     return b"".join([v for k, v in entity.items() if k.startswith("d_")])
 
 
 class AzureTableStorageProvider(StorageProvider):
     def __init__(
         self,
         table_name: str,
+        credential: Any,
         endpoint: str = None,
-        credential=DefaultAzureCredential(),
         connection_string: str = None,
     ) -> None:
         if connection_string is not None:
             self._table_client = TableClient.from_connection_string(conn_str=connection_string, table_name=table_name)
         else:
             self._table_client = TableClient(
                 endpoint=endpoint,
@@ -65,23 +65,23 @@
             entity = self._table_client.get_entity(
                 partition_key=key,
                 row_key="cm",
             )
         except ResourceNotFoundError as e:
             if etag is None:
                 return None
-            self.raise_key_sync_error(key=key, etag=etag, inner_exception=e)
+            raise KeySyncError(storage_provider_name=self.logical_name(), key=key, etag=etag) from e
         else:
             if etag is not None and etag != entity.metadata["etag"]:
-                self.raise_key_sync_error(key=key, etag=etag)
+                raise KeySyncError(storage_provider_name=self.logical_name(), key=key, etag=etag)
             return _dechunk_entity(entity)
 
     def upload_data(self, key: str, etag: str, data: bytes) -> str:
         if not isinstance(data, bytes):
-            raise ValueError("Data must be bytes like")
+            raise ValueError(f"Data must be bytes like, got {type(data)}")
         entity = {
             "PartitionKey": key,
             "RowKey": "cm",
             **_chunk_bytes(data=data),
         }
         try:
             if etag is None:  # Not expecting existing data
@@ -90,28 +90,28 @@
                 response = self._table_client.update_entity(
                     entity=entity,
                     mode=UpdateMode.REPLACE,
                     etag=etag,
                     match_condition=MatchConditions.IfNotModified,
                 )
         except ResourceExistsError as e:
-            self.raise_key_sync_error(key=key, etag=etag, inner_exception=e)
+            raise KeySyncError(storage_provider_name=self.logical_name(), key=key, etag=etag) from e
         except HttpResponseError as e:
             if "update condition specified in the request was not satisfied" in e.exc_msg or (
                 "etag value" in e.exc_msg and "is not valid" in e.exc_msg
             ):
-                self.raise_key_sync_error(key=key, etag=etag, inner_exception=e)
+                raise KeySyncError(storage_provider_name=self.logical_name(), key=key, etag=etag) from e
             elif (
                 e.model is not None
                 and e.model.additional_properties is not None
                 and "odata.error" in e.model.additional_properties
                 and "code" in e.model.additional_properties["odata.error"]
                 and e.model.additional_properties["odata.error"]["code"] == "EntityTooLarge"
             ):
-                self.raise_value_size_error(key=key, inner_exception=e)
+                raise ValueSizeError(storage_provider_name=self.logical_name(), key=key) from e
             else:
                 raise e
         return response["etag"]
 
     def delete_data(self, key: str, etag: str) -> None:
         try:
             self._table_client.delete_entity(
@@ -120,20 +120,20 @@
                 etag=etag,
                 match_condition=MatchConditions.IfNotModified,
             )
         except HttpResponseError as e:
             if "update condition specified in the request was not satisfied" in e.exc_msg or (
                 "etag value" in e.exc_msg and "is not valid" in e.exc_msg
             ):
-                self.raise_key_sync_error(key=key, etag=etag, inner_exception=e)
+                raise KeySyncError(storage_provider_name=self.logical_name(), key=key, etag=etag) from e
             else:
                 raise e
 
     def list_keys_and_etags(self, key_prefix: str) -> Dict[str, str]:
-        if key_prefix is None:
+        if not key_prefix:
             query = self._table_client.list_entities()
         else:
             key_prefix_stop = key_prefix[:-1] + chr(ord(key_prefix[-1]) + 1)
             query = self._table_client.query_entities(
                 f"PartitionKey ge '{key_prefix}' and PartitionKey lt '{key_prefix_stop}'"
             )
         return {e["PartitionKey"]: e.metadata["etag"] for e in query}
```

### Comparing `cloud-mappings-1.2.2/src/cloudmappings/storageproviders/googlecloudstorage.py` & `cloud-mappings-2.0.0a0/src/cloudmappings/_storageproviders/googlecloudstorage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Dict
 
 from google.cloud import storage
 from google.cloud.exceptions import Conflict
 from google.cloud.storage.blob import Blob
 
-from .storageprovider import StorageProvider
+from cloudmappings.errors import KeySyncError
+from cloudmappings.storageprovider import StorageProvider
 
 
 class GoogleCloudStorageProvider(StorageProvider):
     def __init__(
         self,
         bucket_name: str,
         project: str,
@@ -46,30 +47,30 @@
 
     def download_data(self, key: str, etag: str) -> bytes:
         b = self._bucket.get_blob(
             blob_name=key,
         )
         existing_etag = self._parse_etag(b)
         if etag is not None and etag != existing_etag:
-            self.raise_key_sync_error(key=key, etag=etag)
+            raise KeySyncError(storage_provider_name=self.logical_name(), key=key, etag=etag)
         if b is None:
             return None
         return b.download_as_bytes(
             if_generation_match=b.generation,
         )
 
     def upload_data(self, key: str, etag: str, data: bytes) -> str:
         if not isinstance(data, bytes):
-            raise ValueError("Data must be bytes like")
+            raise ValueError(f"Data must be bytes like, got {type(data)}")
         b = self._bucket.get_blob(
             blob_name=key,
         )
         existing_etag = self._parse_etag(b)
         if etag != existing_etag:
-            self.raise_key_sync_error(key=key, etag=etag)
+            raise KeySyncError(storage_provider_name=self.logical_name(), key=key, etag=etag)
         if b is None:
             b = self._bucket.blob(
                 blob_name=key,
             )
         b.upload_from_string(
             data=data,
             if_generation_match=b.generation,
@@ -78,15 +79,15 @@
 
     def delete_data(self, key: str, etag: str) -> None:
         b = self._bucket.get_blob(
             blob_name=key,
         )
         existing_etag = self._parse_etag(b)
         if etag != existing_etag:
-            self.raise_key_sync_error(key=key, etag=etag)
+            raise KeySyncError(storage_provider_name=self.logical_name(), key=key, etag=etag)
         self._bucket.delete_blob(
             blob_name=key,
             if_generation_match=b.generation,
         )
 
     def list_keys_and_etags(self, key_prefix: str) -> Dict[str, str]:
         keys_and_ids = {
```

### Comparing `cloud-mappings-1.2.2/src/cloudmappings/storageproviders/storageprovider.py` & `cloud-mappings-2.0.0a0/src/cloudmappings/storageprovider.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,13 @@
 from abc import ABC, abstractmethod
 from typing import Dict
 from urllib.parse import quote, unquote
 
-from ..errors import KeySyncError, ValueSizeError
-
 
 class StorageProvider(ABC):
-    def raise_key_sync_error(self, key: str, etag: str, inner_exception: Exception = None):
-        raise KeySyncError(storage_provider_name=self.logical_name(), key=key, etag=etag) from inner_exception
-
-    def raise_value_size_error(self, key: str, inner_exception: Exception = None):
-        raise ValueSizeError(storage_provider_name=self.logical_name(), key=key) from inner_exception
-
-    def encode_key(self, unsafe_key) -> str:
-        return quote(unsafe_key, errors="strict")
-
-    def decode_key(self, encoded_key) -> str:
-        return unquote(encoded_key, errors="strict")
-
     @abstractmethod
     def logical_name(self) -> str:
         """Returns a human readable string identifying the current implementation, and which
         logical cloud resouce it is currently mapping to. Does not include any credential or
         secret information.
 
         Returns
@@ -43,14 +29,46 @@
         Returns
         -------
         bool
             `True` if the parent cloud resouce already existed, otherwise `False`.
         """
         pass
 
+    def encode_key(self, unsafe_key) -> str:
+        """Encode a possibly unsafe input string input a safe value to use as a key in the
+        storage service. Defaults to `urllib.parse.quote`
+
+        Parameters
+        ----------
+        unsafe_key: str
+            The unsafe key to encode
+
+        Returns
+        -------
+        str
+            Safely encoded key
+        """
+        return quote(unsafe_key, errors="strict")
+
+    def decode_key(self, encoded_key) -> str:
+        """Decodes a previously encoded key back to it's original value.
+        Defaults to `urllib.parse.unquote`
+
+        Parameters
+        ----------
+        encoded_key: str
+            The encoded key to decode
+
+        Returns
+        -------
+        str
+            Decoded key
+        """
+        return unquote(encoded_key, errors="strict")
+
     @abstractmethod
     def download_data(self, key: str, etag: str) -> bytes:
         """Download data from cloud storage
 
         Downloads the data at the specified key and with the specified etag from cloud storage.
 
         If `None` is passed for etag the latest version in the cloud will be downloaded.
@@ -95,14 +113,16 @@
 
         Raises
         ------
         KeySyncError
             When the etag specified does not match the value in the cloud
         ValueError
             When data is not bytes-like
+        ValueSizeError
+            When data is too large for storage provider
 
         Returns
         -------
         str
             Etag of the newly uploaded data
         """
         pass
```

