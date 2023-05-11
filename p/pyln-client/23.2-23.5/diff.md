# Comparing `tmp/pyln_client-23.2.tar.gz` & `tmp/pyln-client-23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyln_client-23.2.tar", max compression
+gzip compressed data, was "pyln-client-23.5.tar", max compression
```

## Comparing `pyln_client-23.2.tar` & `pyln-client-23.5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     2929 2023-03-03 15:54:49.821873 pyln_client-23.2/README.md
--rw-r--r--   0        0        0      432 2023-03-03 15:54:49.821873 pyln_client-23.2/pyln/client/__init__.py
--rw-r--r--   0        0        0      889 2023-03-03 15:54:49.821873 pyln_client-23.2/pyln/client/clnutils.py
--rwxr-xr-x   0        0        0    12499 2023-03-03 15:54:49.821873 pyln_client-23.2/pyln/client/gossmap.py
--rw-r--r--   0        0        0    53156 2023-03-03 15:54:49.821873 pyln_client-23.2/pyln/client/lightning.py
--rw-r--r--   0        0        0    38901 2023-03-03 15:54:49.821873 pyln_client-23.2/pyln/client/plugin.py
--rw-r--r--   0        0        0      615 2023-03-03 15:54:49.821873 pyln_client-23.2/pyproject.toml
--rw-r--r--   0        0        0     3722 1970-01-01 00:00:00.000000 pyln_client-23.2/setup.py
--rw-r--r--   0        0        0     3616 1970-01-01 00:00:00.000000 pyln_client-23.2/PKG-INFO
+-rw-r--r--   0        0        0     2939 2023-05-11 17:43:49.801160 pyln-client-23.5/README.md
+-rw-r--r--   0        0        0      573 2023-05-11 17:43:49.801160 pyln-client-23.5/pyln/client/__init__.py
+-rw-r--r--   0        0        0      889 2023-05-11 17:43:49.801160 pyln-client-23.5/pyln/client/clnutils.py
+-rwxr-xr-x   0        0        0    26412 2023-05-11 17:43:49.801160 pyln-client-23.5/pyln/client/gossmap.py
+-rw-r--r--   0        0        0    14744 2023-05-11 17:43:49.801160 pyln-client-23.5/pyln/client/gossmapstats.py
+-rw-r--r--   0        0        0    53156 2023-05-11 17:43:49.801160 pyln-client-23.5/pyln/client/lightning.py
+-rw-r--r--   0        0        0    38901 2023-05-11 17:43:49.801160 pyln-client-23.5/pyln/client/plugin.py
+-rw-r--r--   0        0        0      615 2023-05-11 17:43:49.801160 pyln-client-23.5/pyproject.toml
+-rw-r--r--   0        0        0     3732 1970-01-01 00:00:00.000000 pyln-client-23.5/setup.py
+-rw-r--r--   0        0        0     3575 1970-01-01 00:00:00.000000 pyln-client-23.5/PKG-INFO
```

### Comparing `pyln_client-23.2/README.md` & `pyln-client-23.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 def init(options, configuration, plugin):
     plugin.log("Plugin helloworld.py initialized")
     # This can also return {'disabled': <reason>} to self-disable,
 	# but normally it returns None.
 
 
 @plugin.subscribe("connect")
-def on_connect(plugin, id, address):
+def on_connect(plugin, id, address, **kwargs):
     plugin.log("Received connect event for peer {}".format(id))
 
 
 plugin.add_option('greeting', 'Hello', 'The greeting I should use.')
 plugin.run()
 
 ```
```

### Comparing `pyln_client-23.2/pyln/client/clnutils.py` & `pyln-client-23.5/pyln/client/clnutils.py`

 * *Files identical despite different names*

### Comparing `pyln_client-23.2/pyln/client/lightning.py` & `pyln-client-23.5/pyln/client/lightning.py`

 * *Files identical despite different names*

### Comparing `pyln_client-23.2/pyln/client/plugin.py` & `pyln-client-23.5/pyln/client/plugin.py`

 * *Files identical despite different names*

### Comparing `pyln_client-23.2/pyproject.toml` & `pyln-client-23.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyln-client"
-version = "23.02"
+version = "23.05"
 description = "Client library and plugin library for Core Lightning"
 authors = ["Christian Decker <decker.christian@gmail.com>"]
 license = "BSD-MIT"
 readme = "README.md"
 
 packages = [
   { include = "pyln/client" },
```

### Comparing `pyln_client-23.2/setup.py` & `pyln-client-23.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['pyln-bolt7>=1.0', 'pyln-proto>=0.12']
 
 setup_kwargs = {
     'name': 'pyln-client',
-    'version': '23.2',
+    'version': '23.5',
     'description': 'Client library and plugin library for Core Lightning',
-    'long_description': '# pyln-client: A python client library for lightningd\n\nThis package implements the Unix socket based JSON-RPC protocol that\n`lightningd` exposes to the rest of the world. It can be used to call\narbitrary functions on the RPC interface, and serves as a basis for plugins\nwritten in python.\n\n\n## Installation\n\n`pyln-client` is available on `pip`:\n\n```\npip install pyln-client\n```\n\nAlternatively you can also install the development version to get access to\ncurrently unreleased features by checking out the Core Lightning source code and\ninstalling into your python3 environment:\n\n```bash\ngit clone https://github.com/ElementsProject/lightning.git\ncd lightning/contrib/pyln-client\npoetry install\n```\n\nThis will add links to the library into your environment so changing the\nchecked out source code will also result in the environment picking up these\nchanges. Notice however that unreleased versions may change API without\nwarning, so test thoroughly with the released version.\n\n## Examples\n\n\n### Using the JSON-RPC client\n```py\n"""\nGenerate invoice on one daemon and pay it on the other\n"""\nfrom pyln.client import LightningRpc\nimport random\n\n# Create two instances of the LightningRpc object using two different Core Lightning daemons on your computer\nl1 = LightningRpc("/tmp/lightning1/lightning-rpc")\nl5 = LightningRpc("/tmp/lightning5/lightning-rpc")\n\ninfo5 = l5.getinfo()\nprint(info5)\n\n# Create invoice for test payment\ninvoice = l5.invoice(100, "lbl{}".format(random.random()), "testpayment")\nprint(invoice)\n\n# Get route to l1\nroute = l1.getroute(info5[\'id\'], 100, 1)\nprint(route)\n\n# Pay invoice\nprint(l1.sendpay(route[\'route\'], invoice[\'payment_hash\']))\n```\n\n### Writing a plugin\n\nPlugins are programs that `lightningd` can be configured to execute alongside\nthe main daemon. They allow advanced interactions with and customizations to\nthe daemon.\n\n```python\n#!/usr/bin/env python3\nfrom pyln.client import Plugin\n\nplugin = Plugin()\n\n@plugin.method("hello")\ndef hello(plugin, name="world"):\n    """This is the documentation string for the hello-function.\n\n    It gets reported as the description when registering the function\n    as a method with `lightningd`.\n\n    If this returns (a dict), that\'s the JSON "result" returned.  If\n    it raises an exception, that causes a JSON "error" return (raising\n    pyln.client.RpcException allows finer control over the return).\n    """\n    greeting = plugin.get_option(\'greeting\')\n    s = \'{} {}\'.format(greeting, name)\n    plugin.log(s)\n    return s\n\n\n@plugin.init()\ndef init(options, configuration, plugin):\n    plugin.log("Plugin helloworld.py initialized")\n    # This can also return {\'disabled\': <reason>} to self-disable,\n\t# but normally it returns None.\n\n\n@plugin.subscribe("connect")\ndef on_connect(plugin, id, address):\n    plugin.log("Received connect event for peer {}".format(id))\n\n\nplugin.add_option(\'greeting\', \'Hello\', \'The greeting I should use.\')\nplugin.run()\n\n```\n',
+    'long_description': '# pyln-client: A python client library for lightningd\n\nThis package implements the Unix socket based JSON-RPC protocol that\n`lightningd` exposes to the rest of the world. It can be used to call\narbitrary functions on the RPC interface, and serves as a basis for plugins\nwritten in python.\n\n\n## Installation\n\n`pyln-client` is available on `pip`:\n\n```\npip install pyln-client\n```\n\nAlternatively you can also install the development version to get access to\ncurrently unreleased features by checking out the Core Lightning source code and\ninstalling into your python3 environment:\n\n```bash\ngit clone https://github.com/ElementsProject/lightning.git\ncd lightning/contrib/pyln-client\npoetry install\n```\n\nThis will add links to the library into your environment so changing the\nchecked out source code will also result in the environment picking up these\nchanges. Notice however that unreleased versions may change API without\nwarning, so test thoroughly with the released version.\n\n## Examples\n\n\n### Using the JSON-RPC client\n```py\n"""\nGenerate invoice on one daemon and pay it on the other\n"""\nfrom pyln.client import LightningRpc\nimport random\n\n# Create two instances of the LightningRpc object using two different Core Lightning daemons on your computer\nl1 = LightningRpc("/tmp/lightning1/lightning-rpc")\nl5 = LightningRpc("/tmp/lightning5/lightning-rpc")\n\ninfo5 = l5.getinfo()\nprint(info5)\n\n# Create invoice for test payment\ninvoice = l5.invoice(100, "lbl{}".format(random.random()), "testpayment")\nprint(invoice)\n\n# Get route to l1\nroute = l1.getroute(info5[\'id\'], 100, 1)\nprint(route)\n\n# Pay invoice\nprint(l1.sendpay(route[\'route\'], invoice[\'payment_hash\']))\n```\n\n### Writing a plugin\n\nPlugins are programs that `lightningd` can be configured to execute alongside\nthe main daemon. They allow advanced interactions with and customizations to\nthe daemon.\n\n```python\n#!/usr/bin/env python3\nfrom pyln.client import Plugin\n\nplugin = Plugin()\n\n@plugin.method("hello")\ndef hello(plugin, name="world"):\n    """This is the documentation string for the hello-function.\n\n    It gets reported as the description when registering the function\n    as a method with `lightningd`.\n\n    If this returns (a dict), that\'s the JSON "result" returned.  If\n    it raises an exception, that causes a JSON "error" return (raising\n    pyln.client.RpcException allows finer control over the return).\n    """\n    greeting = plugin.get_option(\'greeting\')\n    s = \'{} {}\'.format(greeting, name)\n    plugin.log(s)\n    return s\n\n\n@plugin.init()\ndef init(options, configuration, plugin):\n    plugin.log("Plugin helloworld.py initialized")\n    # This can also return {\'disabled\': <reason>} to self-disable,\n\t# but normally it returns None.\n\n\n@plugin.subscribe("connect")\ndef on_connect(plugin, id, address, **kwargs):\n    plugin.log("Received connect event for peer {}".format(id))\n\n\nplugin.add_option(\'greeting\', \'Hello\', \'The greeting I should use.\')\nplugin.run()\n\n```\n',
     'author': 'Christian Decker',
     'author_email': 'decker.christian@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pyln_client-23.2/PKG-INFO` & `pyln-client-23.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pyln-client
-Version: 23.2
+Version: 23.5
 Summary: Client library and plugin library for Core Lightning
 License: BSD-MIT
 Author: Christian Decker
 Author-email: decker.christian@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyln-bolt7 (>=1.0)
 Requires-Dist: pyln-proto (>=0.12)
 Description-Content-Type: text/markdown
 
 # pyln-client: A python client library for lightningd
 
 This package implements the Unix socket based JSON-RPC protocol that
@@ -111,15 +110,15 @@
 def init(options, configuration, plugin):
     plugin.log("Plugin helloworld.py initialized")
     # This can also return {'disabled': <reason>} to self-disable,
 	# but normally it returns None.
 
 
 @plugin.subscribe("connect")
-def on_connect(plugin, id, address):
+def on_connect(plugin, id, address, **kwargs):
     plugin.log("Received connect event for peer {}".format(id))
 
 
 plugin.add_option('greeting', 'Hello', 'The greeting I should use.')
 plugin.run()
 
 ```
```

