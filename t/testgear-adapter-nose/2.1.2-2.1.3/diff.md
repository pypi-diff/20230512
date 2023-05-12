# Comparing `tmp/testgear-adapter-nose-2.1.2.tar.gz` & `tmp/testgear-adapter-nose-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgear-adapter-nose-2.1.2.tar", last modified: Fri Apr 21 14:56:40 2023, max compression
+gzip compressed data, was "testgear-adapter-nose-2.1.3.tar", last modified: Fri May 12 09:41:07 2023, max compression
```

## Comparing `testgear-adapter-nose-2.1.2.tar` & `testgear-adapter-nose-2.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:56:40.198191 testgear-adapter-nose-2.1.2/
--rw-rw-rw-   0        0        0     7830 2023-04-21 14:56:40.198191 testgear-adapter-nose-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     7280 2023-03-31 06:28:55.000000 testgear-adapter-nose-2.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-21 14:56:40.198191 testgear-adapter-nose-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1061 2023-04-21 14:02:44.000000 testgear-adapter-nose-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:56:40.172878 testgear-adapter-nose-2.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 14:56:40.172878 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:47:37.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose/__init__.py
--rw-rw-rw-   0        0        0     1263 2023-04-21 13:59:17.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose/listener.py
--rw-rw-rw-   0        0        0      986 2023-04-21 13:59:17.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose/plugin.py
--rw-rw-rw-   0        0        0     8373 2023-04-21 13:59:17.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:56:40.198191 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose.egg-info/
--rw-rw-rw-   0        0        0     7830 2023-04-21 14:56:39.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-04-21 14:56:40.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:56:39.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-04-21 14:56:39.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-21 14:56:39.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-21 14:56:39.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:07.515226 testgear-adapter-nose-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-05-12 09:41:07.515226 testgear-adapter-nose-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-05-12 09:40:56.000000 testgear-adapter-nose-2.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:41:07.515226 testgear-adapter-nose-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-12 09:40:56.000000 testgear-adapter-nose-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:07.511225 testgear-adapter-nose-2.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:07.515226 testgear-adapter-nose-2.1.3/src/testgear_adapter_nose/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:40:56.000000 testgear-adapter-nose-2.1.3/src/testgear_adapter_nose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-12 09:40:56.000000 testgear-adapter-nose-2.1.3/src/testgear_adapter_nose/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-12 09:40:56.000000 testgear-adapter-nose-2.1.3/src/testgear_adapter_nose/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-05-12 09:40:56.000000 testgear-adapter-nose-2.1.3/src/testgear_adapter_nose/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:07.515226 testgear-adapter-nose-2.1.3/src/testgear_adapter_nose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-05-12 09:41:07.000000 testgear-adapter-nose-2.1.3/src/testgear_adapter_nose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-12 09:41:07.000000 testgear-adapter-nose-2.1.3/src/testgear_adapter_nose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:41:07.000000 testgear-adapter-nose-2.1.3/src/testgear_adapter_nose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-12 09:41:07.000000 testgear-adapter-nose-2.1.3/src/testgear_adapter_nose.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 09:41:07.000000 testgear-adapter-nose-2.1.3/src/testgear_adapter_nose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 09:41:07.000000 testgear-adapter-nose-2.1.3/src/testgear_adapter_nose.egg-info/top_level.txt
```

### Comparing `testgear-adapter-nose-2.1.2/setup.py` & `testgear-adapter-nose-2.1.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from setuptools import setup, find_packages
-
-setup(
-    name='testgear-adapter-nose',
-    version='2.1.2',
-    description='Nose adapter for Test Gear',
-    long_description=open('README.md', "r").read(),
-    long_description_content_type="text/markdown",
-    url='https://github.com/testgear-tms/adapters-python/',
-    author='Integration team',
-    author_email='integrations@test-gear.io',
-    license='Apache-2.0',
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-    ],
-    py_modules=['testgear_adapter_nose'],
-    packages=find_packages(where='src'),
-    package_dir={'': 'src'},
-    install_requires=['attrs', 'nose2', 'testgear-python-commons==2.1.2'],
-    entry_points={
-            'nose.plugins.0.10': [
-                'testgear_adapter_nose = testgear_adapter_nose.plugin:TmsPlugin',
-            ]
-    }
-)
+from setuptools import setup, find_packages
+
+setup(
+    name='testgear-adapter-nose',
+    version='2.1.3',
+    description='Nose adapter for Test Gear',
+    long_description=open('README.md', "r").read(),
+    long_description_content_type="text/markdown",
+    url='https://github.com/testgear-tms/adapters-python/',
+    author='Integration team',
+    author_email='integrations@test-gear.io',
+    license='Apache-2.0',
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+    ],
+    py_modules=['testgear_adapter_nose'],
+    packages=find_packages(where='src'),
+    package_dir={'': 'src'},
+    install_requires=['attrs', 'nose2', 'testgear-python-commons==2.1.3'],
+    entry_points={
+            'nose.plugins.0.10': [
+                'testgear_adapter_nose = testgear_adapter_nose.plugin:TmsPlugin',
+            ]
+    }
+)
```

### Comparing `testgear-adapter-nose-2.1.2/src/testgear_adapter_nose/listener.py` & `testgear-adapter-nose-2.1.3/src/testgear_adapter_nose/listener.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,61 @@
-from testgear_python_commons.services import AdapterManager
-from testgear_python_commons.step import Step
-from .utils import (
-    form_test,
-    get_outcome
-)
-
-
-class AdapterListener(object):
-    __executable_test = None
-
-    def __init__(self, adapter_manager: AdapterManager):
-        self.__adapter_manager = adapter_manager
-
-    def start_launch(self):
-        test_run_id = self.__adapter_manager.get_test_run_id()
-
-        self.__adapter_manager.set_test_run_id(test_run_id)
-
-    def get_tests_for_launch(self):
-        return self.__adapter_manager.get_autotests_for_launch()
-
-    def start_test(self, test):
-        self.__executable_test = form_test(test)
-
-    def set_outcome(self, event):
-        outcome, message, trace = get_outcome(event)
-
-        self.__executable_test['outcome'] = outcome
-        self.__executable_test['message'] = message
-        self.__executable_test['traces'] = trace
-
-    def stop_test(self):
-        test_steps, test_results_steps = Step.get_steps_data()
-
-        self.__executable_test['steps'] = test_steps
-        self.__executable_test['stepResults'] = test_results_steps
-
-        self.__adapter_manager.write_test(self.__executable_test)
-        self.__executable_test = None
+import testgear_python_commons.services as adapter
+from testgear_python_commons.services import AdapterManager
+from testgear_python_commons.step import Step
+from .utils import (
+    form_test,
+    get_outcome
+)
+
+
+class AdapterListener(object):
+    __executable_test = None
+
+    def __init__(self, adapter_manager: AdapterManager):
+        self.__adapter_manager = adapter_manager
+
+    def start_launch(self):
+        test_run_id = self.__adapter_manager.get_test_run_id()
+
+        self.__adapter_manager.set_test_run_id(test_run_id)
+
+    def get_tests_for_launch(self):
+        return self.__adapter_manager.get_autotests_for_launch()
+
+    def start_test(self, test):
+        self.__executable_test = form_test(test)
+
+    def set_outcome(self, event):
+        outcome, message, trace = get_outcome(event)
+
+        self.__executable_test['outcome'] = outcome
+        self.__executable_test['message'] = message
+        self.__executable_test['traces'] = trace
+
+    def stop_test(self):
+        test_steps, test_results_steps = Step.get_steps_data()
+
+        self.__executable_test['steps'] = test_steps
+        self.__executable_test['stepResults'] = test_results_steps
+
+        self.__adapter_manager.write_test(self.__executable_test)
+        self.__executable_test = None
+
+    @adapter.hookimpl
+    def add_link(self, link):
+        if self.__executable_test:
+            self.__executable_test['resultLinks'].append(link)
+
+    @adapter.hookimpl
+    def add_message(self, test_message):
+        if self.__executable_test:
+            self.__executable_test['message'] = str(test_message)
+
+    @adapter.hookimpl
+    def add_attachments(self, attach_paths: list or tuple):
+        if self.__executable_test:
+            self.__executable_test['attachments'] += self.__adapter_manager.load_attachments(attach_paths)
+
+    @adapter.hookimpl
+    def create_attachment(self, body, name: str):
+        if self.__executable_test:
+            self.__executable_test['attachments'] += self.__adapter_manager.create_attachment(body, name)
```

### Comparing `testgear-adapter-nose-2.1.2/src/testgear_adapter_nose/plugin.py` & `testgear-adapter-nose-2.1.3/src/testgear_adapter_nose/plugin.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from nose2.events import Plugin
-
-from testgear_python_commons.services import TmsPluginManager
-
-from .listener import AdapterListener
-
-
-class TmsPlugin(Plugin):
-    configSection = 'testgear'
-    commandLineSwitch = (None, 'testgear', 'TMS adapter for Nose')
-    __listener = None
-    __tests_for_launch = None
-
-    def __init__(self, *args, **kwargs):
-        super(TmsPlugin, self).__init__(*args, **kwargs)
-
-    def startTestRun(self, event):
-        self.__listener = AdapterListener(
-            TmsPluginManager.get_adapter_manager())
-
-        TmsPluginManager.get_plugin_manager().register(self.__listener)
-
-        self.__listener.start_launch()
-        self.__tests_for_launch = self.__listener.get_tests_for_launch()
-
-    def startTest(self, event):
-        self.__listener.start_test(event.test)
-
-    def stopTest(self, event):
-        self.__listener.stop_test()
-
-    def testOutcome(self, event):
-        self.__listener.set_outcome(event)
+from nose2.events import Plugin
+
+from testgear_python_commons.services import TmsPluginManager
+
+from .listener import AdapterListener
+
+
+class TmsPlugin(Plugin):
+    configSection = 'testgear'
+    commandLineSwitch = (None, 'testgear', 'TMS adapter for Nose')
+    __listener = None
+    __tests_for_launch = None
+
+    def __init__(self, *args, **kwargs):
+        super(TmsPlugin, self).__init__(*args, **kwargs)
+
+    def startTestRun(self, event):
+        self.__listener = AdapterListener(
+            TmsPluginManager.get_adapter_manager())
+
+        TmsPluginManager.get_plugin_manager().register(self.__listener)
+
+        self.__listener.start_launch()
+        self.__tests_for_launch = self.__listener.get_tests_for_launch()
+
+    def startTest(self, event):
+        self.__listener.start_test(event.test)
+
+    def stopTest(self, event):
+        self.__listener.stop_test()
+
+    def testOutcome(self, event):
+        self.__listener.set_outcome(event)
```

### Comparing `testgear-adapter-nose-2.1.2/src/testgear_adapter_nose/utils.py` & `testgear-adapter-nose-2.1.3/src/testgear_adapter_nose/utils.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,257 +1,257 @@
-from traceback import format_exception_only
-from nose2 import (
-    util,
-    result
-)
-import inspect
-
-from testgear_python_commons.services.utils import Utils
-from testgear_python_commons.models.outcome_type import OutcomeType
-
-
-def status_details(event):
-    message, trace = None, None
-    if event.exc_info:
-        exc_type, value, _ = event.exc_info
-        message = '\n'.join(format_exception_only(exc_type, value)) if exc_type or value else None
-        trace = ''.join(util.exc_info_to_string(event.exc_info, event.test))
-    elif event.reason:
-        message = event.reason
-
-    return message, trace
-
-
-def update_attrs(test, name, values):
-    if type(values) in (list, tuple, str) and name.isidentifier():
-        attrib = getattr(test, name, values)
-        if attrib and attrib != values:
-            attrib = sum(
-                [tuple(i) if type(i) in (tuple, list) else (i,) for i in (attrib, values)],
-                ()
-            )
-        setattr(test, name, attrib)
-
-
-def get_outcome(event):
-    outcome = None
-    message = None
-    trace = None
-
-    if event.outcome == result.PASS and event.expected:
-        outcome = OutcomeType.PASSED
-    elif event.outcome == result.PASS and not event.expected:
-        outcome = OutcomeType.PASSED
-        message = "test passes unexpectedly"
-    elif event.outcome == result.FAIL and not event.expected:
-        outcome = OutcomeType.FAILED
-        message, trace = status_details(event)
-    elif event.outcome == result.ERROR:
-        outcome = OutcomeType.BLOCKED
-        message, trace = status_details(event)
-    elif event.outcome == result.SKIP:
-        outcome = OutcomeType.SKIPPED
-        message, trace = status_details(event)
-
-    print(outcome, message, trace)
-
-    return outcome, message, trace
-
-
-def form_test(test):
-    data = {}
-    parameters = get_params(test)
-
-    if hasattr(test, "_testFunc"):
-        item = test._testFunc
-
-        if not hasattr(item, 'test_external_id'):
-            item.test_external_id = Utils.get_hash(item.__name__)
-
-        if not hasattr(item, 'test_displayname'):
-            item.test_displayname = item.__doc__ if \
-                item.__doc__ else item.__name__
-        else:
-            params = Utils.get_params(item)
-            item.test_displayname = Utils.param_attribute_collector(
-                item.test_displayname,
-                params)
-
-        data = {
-            'externalID': item.test_external_id,
-            'autoTestName': item.test_displayname,
-            'steps': [],
-            'stepResults': [],
-            'setUp': [],
-            'setUpResults': [],
-            'tearDown': [],
-            'tearDownResults': [],
-            'resultLinks': [],
-            'duration': 0,
-            'outcome': None,
-            'failureReasonName': None,
-            'traces': None,
-            'namespace': item.__module__,
-            'attachments': [],
-            'parameters': parameters,
-            'properties': get_properties_from(item),
-            'classname': get_classname_from(item),
-            'title': get_title_from(item),
-            'description': get_description_from(item),
-            'links': [],
-            'labels': [],
-            'workItemsID': [],
-            'message': None
-        }
-
-        if hasattr(item, 'test_links'):
-            set_links(item, data)
-
-        if hasattr(item, 'test_labels'):
-            set_labels(item, data)
-
-        if hasattr(item, 'test_workitems_id'):
-            data['workItemsID'] = item.test_workitems_id
-    elif hasattr(test, "_testMethodName"):
-        data = {
-            'externalID': Utils.get_hash(test._testMethodName),
-            'autoTestName': test.__doc__ if \
-                test.__doc__ else test._testMethodName,
-            'parameters': parameters
-        }
-
-    return data
-
-
-def get_properties_from(item):
-    if hasattr(item, 'test_properties'):
-        return item.test_properties
-    return None
-
-
-def get_classname_from(item):
-    i = item.__qualname__.find('.')
-    if i != -1:
-        return item.__qualname__[:i]
-    return None
-
-
-def set_links(item, data):
-    params = Utils.get_params(item)
-
-    if params:
-        for link in item.test_links:
-            data['links'].append({})
-            data['links'][-1]['url'] = Utils.param_attribute_collector(
-                link['url'],
-                params)
-            data['links'][-1]['title'] = Utils.param_attribute_collector(
-                link['title'],
-                params) if link['title'] else None
-            data['links'][-1]['type'] = Utils.param_attribute_collector(
-                link['type'],
-                params) if link['type'] else None
-            data['links'][-1]['description'] = Utils.param_attribute_collector(
-                link['description'],
-                params) if link['description'] else None
-    else:
-        data['links'] = item.test_links
-
-
-def get_title_from(item):
-    if not hasattr(item, 'test_title'):
-        return None
-
-    params = Utils.get_params(item)
-
-    if params:
-        return Utils.param_attribute_collector(
-            item.test_title,
-            params)
-    return item.test_title
-
-
-def get_description_from(item):
-    if not hasattr(item, 'test_description'):
-        return None
-
-    params = Utils.get_params(item)
-
-    if params:
-        return Utils.param_attribute_collector(
-            item.test_description,
-            params)
-    return item.test_description
-
-
-def set_labels(item, data):
-    if hasattr(item, 'array_parametrize_mark_id'):
-        for one_label in item.test_labels:
-            result, param_id = Utils.mass_param_attribute_collector(
-                one_label,
-                item.own_markers,
-                item.array_parametrize_mark_id,
-                item.index)
-            if param_id is not None and one_label[1:-1] in \
-                    item.name[(item.name.find('[') + 1):(item.name.rfind(']'))].split(
-                        '-')[param_id]:
-                for label in result:
-                    data['labels'].append({
-                        'name': label
-                    })
-            else:
-                data['labels'].append({
-                    'name': result
-                })
-    else:
-        for label in item.test_labels:
-            data['labels'].append({
-                'name': label
-            })
-
-
-def set_workitems_id(item, data):
-    if hasattr(item, 'array_parametrize_mark_id'):
-        result, param_id = Utils.mass_param_attribute_collector(
-            item.test_workitems_id[0], item.own_markers,
-            item.array_parametrize_mark_id, item.index)
-        if param_id is not None and item.test_workitems_id[0][1:-1] in \
-                item.name[(item.name.find('[') + 1):(item.name.rfind(']'))].split(
-                    '-')[param_id]:
-            data['workItemsID'] = result
-        else:
-            data['workItemsID'] = [result]
-    else:
-        data['workItemsID'] = item.test_workitems_id
-
-
-def fullname(event):
-    if hasattr(event.test, "_testFunc"):
-        test_module = event.test._testFunc.__module__
-        test_name = event.test._testFunc.__name__
-        return f"{test_module}.{test_name}"
-    test_id = event.test.id()
-    return test_id.split(":")[0]
-
-
-def get_params(test):
-    def _params(names, values):
-        return {name if name else f"param{values.index(value)}": value for name, value in zip(names, values)}
-
-    test_id = test.id()
-
-    if len(test_id.split("\n")) > 1:
-        if hasattr(test, "_testFunc"):
-            wrapper_arg_spec = inspect.getfullargspec(test._testFunc)
-            arg_set, obj = wrapper_arg_spec.defaults
-            test_arg_spec = inspect.getfullargspec(obj)
-            args = test_arg_spec.args
-
-            return _params(args, arg_set)
-        elif hasattr(test, "_testMethodName"):
-            method = getattr(test, test._testMethodName)
-            wrapper_arg_spec = inspect.getfullargspec(method)
-            obj, arg_set = wrapper_arg_spec.defaults
-            test_arg_spec = inspect.getfullargspec(obj)
-            args = test_arg_spec.args
-
-            return _params(args[1:], arg_set)
+from traceback import format_exception_only
+from nose2 import (
+    util,
+    result
+)
+import inspect
+
+from testgear_python_commons.services.utils import Utils
+from testgear_python_commons.models.outcome_type import OutcomeType
+
+
+def status_details(event):
+    message, trace = None, None
+    if event.exc_info:
+        exc_type, value, _ = event.exc_info
+        message = '\n'.join(format_exception_only(exc_type, value)) if exc_type or value else None
+        trace = ''.join(util.exc_info_to_string(event.exc_info, event.test))
+    elif event.reason:
+        message = event.reason
+
+    return message, trace
+
+
+def update_attrs(test, name, values):
+    if type(values) in (list, tuple, str) and name.isidentifier():
+        attrib = getattr(test, name, values)
+        if attrib and attrib != values:
+            attrib = sum(
+                [tuple(i) if type(i) in (tuple, list) else (i,) for i in (attrib, values)],
+                ()
+            )
+        setattr(test, name, attrib)
+
+
+def get_outcome(event):
+    outcome = None
+    message = None
+    trace = None
+
+    if event.outcome == result.PASS and event.expected:
+        outcome = OutcomeType.PASSED
+    elif event.outcome == result.PASS and not event.expected:
+        outcome = OutcomeType.PASSED
+        message = "test passes unexpectedly"
+    elif event.outcome == result.FAIL and not event.expected:
+        outcome = OutcomeType.FAILED
+        message, trace = status_details(event)
+    elif event.outcome == result.ERROR:
+        outcome = OutcomeType.BLOCKED
+        message, trace = status_details(event)
+    elif event.outcome == result.SKIP:
+        outcome = OutcomeType.SKIPPED
+        message, trace = status_details(event)
+
+    print(outcome, message, trace)
+
+    return outcome, message, trace
+
+
+def form_test(test):
+    data = {}
+    parameters = get_params(test)
+
+    if hasattr(test, "_testFunc"):
+        item = test._testFunc
+
+        if not hasattr(item, 'test_external_id'):
+            item.test_external_id = Utils.get_hash(item.__name__)
+
+        if not hasattr(item, 'test_displayname'):
+            item.test_displayname = item.__doc__ if \
+                item.__doc__ else item.__name__
+        else:
+            params = Utils.get_params(item)
+            item.test_displayname = Utils.param_attribute_collector(
+                item.test_displayname,
+                params)
+
+        data = {
+            'externalID': item.test_external_id,
+            'autoTestName': item.test_displayname,
+            'steps': [],
+            'stepResults': [],
+            'setUp': [],
+            'setUpResults': [],
+            'tearDown': [],
+            'tearDownResults': [],
+            'resultLinks': [],
+            'duration': 0,
+            'outcome': None,
+            'failureReasonName': None,
+            'traces': None,
+            'namespace': item.__module__,
+            'attachments': [],
+            'parameters': parameters,
+            'properties': get_properties_from(item),
+            'classname': get_classname_from(item),
+            'title': get_title_from(item),
+            'description': get_description_from(item),
+            'links': [],
+            'labels': [],
+            'workItemsID': [],
+            'message': None
+        }
+
+        if hasattr(item, 'test_links'):
+            set_links(item, data)
+
+        if hasattr(item, 'test_labels'):
+            set_labels(item, data)
+
+        if hasattr(item, 'test_workitems_id'):
+            data['workItemsID'] = item.test_workitems_id
+    elif hasattr(test, "_testMethodName"):
+        data = {
+            'externalID': Utils.get_hash(test._testMethodName),
+            'autoTestName': test.__doc__ if \
+                test.__doc__ else test._testMethodName,
+            'parameters': parameters
+        }
+
+    return data
+
+
+def get_properties_from(item):
+    if hasattr(item, 'test_properties'):
+        return item.test_properties
+    return None
+
+
+def get_classname_from(item):
+    i = item.__qualname__.find('.')
+    if i != -1:
+        return item.__qualname__[:i]
+    return None
+
+
+def set_links(item, data):
+    params = Utils.get_params(item)
+
+    if params:
+        for link in item.test_links:
+            data['links'].append({})
+            data['links'][-1]['url'] = Utils.param_attribute_collector(
+                link['url'],
+                params)
+            data['links'][-1]['title'] = Utils.param_attribute_collector(
+                link['title'],
+                params) if link['title'] else None
+            data['links'][-1]['type'] = Utils.param_attribute_collector(
+                link['type'],
+                params) if link['type'] else None
+            data['links'][-1]['description'] = Utils.param_attribute_collector(
+                link['description'],
+                params) if link['description'] else None
+    else:
+        data['links'] = item.test_links
+
+
+def get_title_from(item):
+    if not hasattr(item, 'test_title'):
+        return None
+
+    params = Utils.get_params(item)
+
+    if params:
+        return Utils.param_attribute_collector(
+            item.test_title,
+            params)
+    return item.test_title
+
+
+def get_description_from(item):
+    if not hasattr(item, 'test_description'):
+        return None
+
+    params = Utils.get_params(item)
+
+    if params:
+        return Utils.param_attribute_collector(
+            item.test_description,
+            params)
+    return item.test_description
+
+
+def set_labels(item, data):
+    if hasattr(item, 'array_parametrize_mark_id'):
+        for one_label in item.test_labels:
+            result, param_id = Utils.mass_param_attribute_collector(
+                one_label,
+                item.own_markers,
+                item.array_parametrize_mark_id,
+                item.index)
+            if param_id is not None and one_label[1:-1] in \
+                    item.name[(item.name.find('[') + 1):(item.name.rfind(']'))].split(
+                        '-')[param_id]:
+                for label in result:
+                    data['labels'].append({
+                        'name': label
+                    })
+            else:
+                data['labels'].append({
+                    'name': result
+                })
+    else:
+        for label in item.test_labels:
+            data['labels'].append({
+                'name': label
+            })
+
+
+def set_workitems_id(item, data):
+    if hasattr(item, 'array_parametrize_mark_id'):
+        result, param_id = Utils.mass_param_attribute_collector(
+            item.test_workitems_id[0], item.own_markers,
+            item.array_parametrize_mark_id, item.index)
+        if param_id is not None and item.test_workitems_id[0][1:-1] in \
+                item.name[(item.name.find('[') + 1):(item.name.rfind(']'))].split(
+                    '-')[param_id]:
+            data['workItemsID'] = result
+        else:
+            data['workItemsID'] = [result]
+    else:
+        data['workItemsID'] = item.test_workitems_id
+
+
+def fullname(event):
+    if hasattr(event.test, "_testFunc"):
+        test_module = event.test._testFunc.__module__
+        test_name = event.test._testFunc.__name__
+        return f"{test_module}.{test_name}"
+    test_id = event.test.id()
+    return test_id.split(":")[0]
+
+
+def get_params(test):
+    def _params(names, values):
+        return {name if name else f"param{values.index(value)}": value for name, value in zip(names, values)}
+
+    test_id = test.id()
+
+    if len(test_id.split("\n")) > 1:
+        if hasattr(test, "_testFunc"):
+            wrapper_arg_spec = inspect.getfullargspec(test._testFunc)
+            arg_set, obj = wrapper_arg_spec.defaults
+            test_arg_spec = inspect.getfullargspec(obj)
+            args = test_arg_spec.args
+
+            return _params(args, arg_set)
+        elif hasattr(test, "_testMethodName"):
+            method = getattr(test, test._testMethodName)
+            wrapper_arg_spec = inspect.getfullargspec(method)
+            obj, arg_set = wrapper_arg_spec.defaults
+            test_arg_spec = inspect.getfullargspec(obj)
+            args = test_arg_spec.args
+
+            return _params(args[1:], arg_set)
```

