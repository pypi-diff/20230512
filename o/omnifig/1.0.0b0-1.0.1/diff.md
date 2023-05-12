# Comparing `tmp/omnifig-1.0.0b0.tar.gz` & `tmp/omnifig-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/omnifig-1.0.0b0.tar", last modified: Fri Jan 13 01:53:18 2023, max compression
+gzip compressed data, was "omnifig-1.0.1.tar", last modified: Fri May 12 19:40:22 2023, max compression
```

## Comparing `omnifig-1.0.0b0.tar` & `omnifig-1.0.1.tar`

### file list

```diff
@@ -1,47 +1,45 @@
-drwxr-xr-x   0 fleeb     (1000) fleeb     (1000)        0 2023-01-13 01:53:18.523240 omnifig-1.0.0b0/
--rw-r--r--   0 fleeb     (1000) fleeb     (1000)     1069 2023-01-08 20:07:06.000000 omnifig-1.0.0b0/LICENSE
--rw-r--r--   0 fleeb     (1000) fleeb     (1000)     4098 2023-01-13 01:53:18.521207 omnifig-1.0.0b0/PKG-INFO
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     3573 2023-01-13 01:53:07.000000 omnifig-1.0.0b0/README.rst
-drwxr-xr-x   0 fleeb     (1000) fleeb     (1000)        0 2023-01-13 01:53:17.876368 omnifig-1.0.0b0/examples/
-drwxr-xr-x   0 fleeb     (1000) fleeb     (1000)        0 2023-01-13 01:53:17.937500 omnifig-1.0.0b0/examples/deep_fake/
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)        0 2023-01-12 15:10:56.000000 omnifig-1.0.0b0/examples/deep_fake/__init__.py
-drwxr-xr-x   0 fleeb     (1000) fleeb     (1000)        0 2023-01-13 01:53:18.023738 omnifig-1.0.0b0/examples/deep_fake/src/
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)       95 2023-01-12 15:12:40.000000 omnifig-1.0.0b0/examples/deep_fake/src/__init__.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     3695 2023-01-12 15:10:56.000000 omnifig-1.0.0b0/examples/deep_fake/src/data_loading.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     1928 2023-01-12 15:10:56.000000 omnifig-1.0.0b0/examples/deep_fake/src/deep_models.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)      662 2023-01-12 15:12:40.000000 omnifig-1.0.0b0/examples/deep_fake/src/util.py
-drwxr-xr-x   0 fleeb     (1000) fleeb     (1000)        0 2023-01-13 01:53:18.143318 omnifig-1.0.0b0/omnifig/
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)      625 2023-01-12 15:51:08.000000 omnifig-1.0.0b0/omnifig/__init__.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     1089 2023-01-13 01:47:02.000000 omnifig-1.0.0b0/omnifig/_info.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)    42470 2023-01-12 15:12:40.000000 omnifig-1.0.0b0/omnifig/abstract.py
-drwxr-xr-x   0 fleeb     (1000) fleeb     (1000)        0 2023-01-13 01:53:18.343154 omnifig-1.0.0b0/omnifig/behaviors/
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)       88 2023-01-12 15:12:40.000000 omnifig-1.0.0b0/omnifig/behaviors/__init__.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     3459 2023-01-12 15:12:40.000000 omnifig-1.0.0b0/omnifig/behaviors/base.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     2154 2023-01-12 15:12:40.000000 omnifig-1.0.0b0/omnifig/behaviors/debug.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     7379 2023-01-12 15:12:40.000000 omnifig-1.0.0b0/omnifig/behaviors/help.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     1432 2023-01-12 15:12:40.000000 omnifig-1.0.0b0/omnifig/behaviors/quiet.py
-drwxr-xr-x   0 fleeb     (1000) fleeb     (1000)        0 2023-01-13 01:53:18.420033 omnifig-1.0.0b0/omnifig/config/
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)      119 2023-01-12 15:12:40.000000 omnifig-1.0.0b0/omnifig/config/__init__.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     3425 2023-01-12 15:12:40.000000 omnifig-1.0.0b0/omnifig/config/abstract.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)    14162 2023-01-12 15:12:40.000000 omnifig-1.0.0b0/omnifig/config/manager.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)    58542 2023-01-12 18:31:53.000000 omnifig-1.0.0b0/omnifig/config/nodes.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     8065 2023-01-12 15:12:41.000000 omnifig-1.0.0b0/omnifig/configurable.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     2060 2023-01-12 15:12:41.000000 omnifig-1.0.0b0/omnifig/exporting.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     4321 2023-01-12 15:12:41.000000 omnifig-1.0.0b0/omnifig/mixins.py
-drwxr-xr-x   0 fleeb     (1000) fleeb     (1000)        0 2023-01-13 01:53:18.501099 omnifig-1.0.0b0/omnifig/organization/
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)      136 2023-01-12 15:12:41.000000 omnifig-1.0.0b0/omnifig/organization/__init__.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)    17882 2023-01-12 15:12:41.000000 omnifig-1.0.0b0/omnifig/organization/default.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)    11483 2023-01-12 15:12:41.000000 omnifig-1.0.0b0/omnifig/organization/profiles.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)    24298 2023-01-12 15:12:41.000000 omnifig-1.0.0b0/omnifig/organization/workspaces.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)    11749 2023-01-12 15:12:41.000000 omnifig-1.0.0b0/omnifig/registration.py
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     6433 2023-01-12 15:12:41.000000 omnifig-1.0.0b0/omnifig/top.py
-drwxr-xr-x   0 fleeb     (1000) fleeb     (1000)        0 2023-01-13 01:53:18.239318 omnifig-1.0.0b0/omnifig.egg-info/
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)     4098 2023-01-13 01:53:17.000000 omnifig-1.0.0b0/omnifig.egg-info/PKG-INFO
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)      951 2023-01-13 01:53:17.000000 omnifig-1.0.0b0/omnifig.egg-info/SOURCES.txt
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)        1 2023-01-13 01:53:17.000000 omnifig-1.0.0b0/omnifig.egg-info/dependency_links.txt
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)       43 2023-01-13 01:53:17.000000 omnifig-1.0.0b0/omnifig.egg-info/entry_points.txt
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)        2 2020-05-29 19:19:41.000000 omnifig-1.0.0b0/omnifig.egg-info/not-zip-safe
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)       37 2023-01-13 01:53:17.000000 omnifig-1.0.0b0/omnifig.egg-info/requires.txt
--rwxrwxrwx   0 fleeb     (1000) fleeb     (1000)        8 2023-01-13 01:53:17.000000 omnifig-1.0.0b0/omnifig.egg-info/top_level.txt
--rw-r--r--   0 fleeb     (1000) fleeb     (1000)       38 2023-01-13 01:53:18.524212 omnifig-1.0.0b0/setup.cfg
--rw-r--r--   0 fleeb     (1000) fleeb     (1000)     1525 2023-01-08 20:07:08.000000 omnifig-1.0.0b0/setup.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2023-05-12 19:40:22.449625 omnifig-1.0.1/
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1069 2022-01-21 09:21:43.000000 omnifig-1.0.1/LICENSE
+-rw-r--r--   0 fleeb     (7343) is        (1040)     5296 2023-05-12 19:40:22.447626 omnifig-1.0.1/PKG-INFO
+-rw-r--r--   0 fleeb     (7343) is        (1040)     5866 2023-05-12 19:40:14.000000 omnifig-1.0.1/README.rst
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2023-05-12 19:40:22.165624 omnifig-1.0.1/omnifig/
+-rw-r--r--   0 fleeb     (7343) is        (1040)      625 2023-01-13 10:56:47.000000 omnifig-1.0.1/omnifig/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1084 2023-05-12 19:32:28.000000 omnifig-1.0.1/omnifig/_info.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    42470 2023-01-11 19:12:39.000000 omnifig-1.0.1/omnifig/abstract.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2023-05-12 19:40:22.320625 omnifig-1.0.1/omnifig/behaviors/
+-rw-r--r--   0 fleeb     (7343) is        (1040)       88 2023-01-11 19:07:48.000000 omnifig-1.0.1/omnifig/behaviors/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3459 2023-01-11 19:07:48.000000 omnifig-1.0.1/omnifig/behaviors/base.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     2154 2023-01-11 19:07:48.000000 omnifig-1.0.1/omnifig/behaviors/debug.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     7379 2023-01-11 19:07:48.000000 omnifig-1.0.1/omnifig/behaviors/help.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1432 2023-01-11 19:07:48.000000 omnifig-1.0.1/omnifig/behaviors/quiet.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2023-05-12 19:40:22.356625 omnifig-1.0.1/omnifig/config/
+-rw-r--r--   0 fleeb     (7343) is        (1040)      119 2023-01-11 19:07:48.000000 omnifig-1.0.1/omnifig/config/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3425 2023-01-11 19:07:48.000000 omnifig-1.0.1/omnifig/config/abstract.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    14162 2023-01-11 19:12:39.000000 omnifig-1.0.1/omnifig/config/manager.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    59019 2023-05-12 19:32:48.000000 omnifig-1.0.1/omnifig/config/nodes.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     8075 2023-02-20 09:22:22.000000 omnifig-1.0.1/omnifig/configurable.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     2060 2023-01-11 19:07:48.000000 omnifig-1.0.1/omnifig/exporting.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     4321 2023-01-11 19:07:48.000000 omnifig-1.0.1/omnifig/mixins.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2023-05-12 19:40:22.408627 omnifig-1.0.1/omnifig/organization/
+-rw-r--r--   0 fleeb     (7343) is        (1040)      136 2023-01-11 19:07:48.000000 omnifig-1.0.1/omnifig/organization/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    17882 2023-01-11 19:12:39.000000 omnifig-1.0.1/omnifig/organization/default.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    11483 2023-01-11 19:07:48.000000 omnifig-1.0.1/omnifig/organization/profiles.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    24298 2023-01-11 19:12:39.000000 omnifig-1.0.1/omnifig/organization/workspaces.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    11749 2023-01-11 19:07:48.000000 omnifig-1.0.1/omnifig/registration.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     6433 2023-01-11 19:12:52.000000 omnifig-1.0.1/omnifig/top.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2023-05-12 19:40:22.253628 omnifig-1.0.1/omnifig.egg-info/
+-rw-r--r--   0 fleeb     (7343) is        (1040)     5296 2023-05-12 19:40:21.000000 omnifig-1.0.1/omnifig.egg-info/PKG-INFO
+-rw-r--r--   0 fleeb     (7343) is        (1040)      902 2023-05-12 19:40:21.000000 omnifig-1.0.1/omnifig.egg-info/SOURCES.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)        1 2023-05-12 19:40:21.000000 omnifig-1.0.1/omnifig.egg-info/dependency_links.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)       42 2023-05-12 19:40:21.000000 omnifig-1.0.1/omnifig.egg-info/entry_points.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)        1 2020-09-28 09:57:42.000000 omnifig-1.0.1/omnifig.egg-info/not-zip-safe
+-rw-r--r--   0 fleeb     (7343) is        (1040)       37 2023-05-12 19:40:21.000000 omnifig-1.0.1/omnifig.egg-info/requires.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)        8 2023-05-12 19:40:21.000000 omnifig-1.0.1/omnifig.egg-info/top_level.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)       38 2023-05-12 19:40:22.450627 omnifig-1.0.1/setup.cfg
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1525 2022-01-21 09:21:43.000000 omnifig-1.0.1/setup.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2023-05-12 19:40:22.441627 omnifig-1.0.1/tests/
+-rw-r--r--   0 fleeb     (7343) is        (1040)    14251 2023-05-12 19:32:02.000000 omnifig-1.0.1/tests/test_config.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     2234 2023-01-11 19:07:50.000000 omnifig-1.0.1/tests/test_configurable.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     9205 2023-01-11 19:07:50.000000 omnifig-1.0.1/tests/test_projects.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3977 2023-01-11 19:07:50.000000 omnifig-1.0.1/tests/test_running.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     5044 2023-01-15 14:59:36.000000 omnifig-1.0.1/tests/test_running_behaviors.py
```

### Comparing `omnifig-1.0.0b0/LICENSE` & `omnifig-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omnifig-1.0.0b0/omnifig/__init__.py` & `omnifig-1.0.1/omnifig/__init__.py`

 * *Files identical despite different names*

### Comparing `omnifig-1.0.0b0/omnifig/_info.py` & `omnifig-1.0.1/omnifig/_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 name = 'omnifig'
 long_name = 'omni-fig'
 
-version = '1.0.0-beta'
+version = '1.0.1'
 
 url = 'https://github.com/felixludos/omni-fig'
 
 description = 'Unleashing Project Configuration and Organization'
 
 author = 'Felix Leeb'
 author_email = 'felixludos.info@gmail.com'
```

### Comparing `omnifig-1.0.0b0/omnifig/abstract.py` & `omnifig-1.0.1/omnifig/abstract.py`

 * *Files identical despite different names*

### Comparing `omnifig-1.0.0b0/omnifig/behaviors/base.py` & `omnifig-1.0.1/omnifig/behaviors/base.py`

 * *Files identical despite different names*

### Comparing `omnifig-1.0.0b0/omnifig/behaviors/debug.py` & `omnifig-1.0.1/omnifig/behaviors/debug.py`

 * *Files identical despite different names*

### Comparing `omnifig-1.0.0b0/omnifig/behaviors/help.py` & `omnifig-1.0.1/omnifig/behaviors/help.py`

 * *Files identical despite different names*

### Comparing `omnifig-1.0.0b0/omnifig/behaviors/quiet.py` & `omnifig-1.0.1/omnifig/behaviors/quiet.py`

 * *Files identical despite different names*

### Comparing `omnifig-1.0.0b0/omnifig/config/abstract.py` & `omnifig-1.0.1/omnifig/config/abstract.py`

 * *Files identical despite different names*

### Comparing `omnifig-1.0.0b0/omnifig/config/manager.py` & `omnifig-1.0.1/omnifig/config/manager.py`

 * *Files identical despite different names*

### Comparing `omnifig-1.0.0b0/omnifig/config/nodes.py` & `omnifig-1.0.1/omnifig/config/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,15 @@
 				queries = queries.copy()
 				queries[0] = f'({queries[0]})'  # if getattr(search.parent_search[0]
 
 			if len(queries) > self.max_num_aliases:
 				key = self.alias_fmt.join([queries[0], '...', queries[-1]])
 			else:
 				key = self.alias_fmt.join(queries)
-			return key
+			return key.replace('_', '-')
 
 
 		def _stylize(self, node: 'ConfigNode', line: str) -> str:
 			'''
 			Stylizes the line based on the search origin's depth and the reporter's flair.
 
 			Args:
@@ -1716,14 +1716,36 @@
 
 
 
 class ConfigSparseNode(AutoTreeSparseNode, ConfigNode):
 	'''A config node that treats its children as being in a dict.'''
 	_python_structure = dict
 
+	def _get(self, addr: str):
+		try:
+			return super()._get(addr)
+		except self._MissingKey:
+			try:
+				return super()._get(addr.replace('-', '_'))
+			except self._MissingKey:
+				pass
+			raise
+
+	def _set(self, addr: str, node):
+		return super()._set(addr, node)
+
+	def _remove(self, addr: str):
+		if addr in self._children:
+			del self._children[addr]
+
+	def _has(self, addr: str):
+		return addr in self._children or addr.replace('-', '_') in self._children
+
+
+
 
 
 class ConfigDenseNode(AutoTreeDenseNode, ConfigNode):
 	'''A config node that treats its children as being in a list.'''
 	_python_structure = list
```

### Comparing `omnifig-1.0.0b0/omnifig/configurable.py` & `omnifig-1.0.1/omnifig/configurable.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 	'''
 	Simple mix-in to make the initialization of classes through the config a two-stage process.
 	The first stage calls the ``__init__`` method, and then after that is complete, the ``__certify__`` method
 	is called, which can return a new object to replace the original one.
 
 	Note, that ``__certify__`` is only called if the object is initialized through the config (e.g. through ``pull()``).
 	'''
-	def __certify__(self, config: AbstractConfig):
+	def __certify__(self, config: AbstractConfig, **kwargs):
 		return self
 
 
 
 class silent_config_args:
 	'''Decorator to silence the config when extracting arguments from the config'''
 	def __init__(self, *args: str):
```

### Comparing `omnifig-1.0.0b0/omnifig/exporting.py` & `omnifig-1.0.1/omnifig/exporting.py`

 * *Files identical despite different names*

### Comparing `omnifig-1.0.0b0/omnifig/mixins.py` & `omnifig-1.0.1/omnifig/mixins.py`

 * *Files identical despite different names*

### Comparing `omnifig-1.0.0b0/omnifig/organization/default.py` & `omnifig-1.0.1/omnifig/organization/default.py`

 * *Files identical despite different names*

### Comparing `omnifig-1.0.0b0/omnifig/organization/profiles.py` & `omnifig-1.0.1/omnifig/organization/profiles.py`

 * *Files identical despite different names*

### Comparing `omnifig-1.0.0b0/omnifig/organization/workspaces.py` & `omnifig-1.0.1/omnifig/organization/workspaces.py`

 * *Files identical despite different names*

### Comparing `omnifig-1.0.0b0/omnifig/registration.py` & `omnifig-1.0.1/omnifig/registration.py`

 * *Files identical despite different names*

### Comparing `omnifig-1.0.0b0/omnifig/top.py` & `omnifig-1.0.1/omnifig/top.py`

 * *Files identical despite different names*

### Comparing `omnifig-1.0.0b0/setup.py` & `omnifig-1.0.1/setup.py`

 * *Files identical despite different names*

