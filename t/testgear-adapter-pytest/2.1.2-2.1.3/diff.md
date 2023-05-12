# Comparing `tmp/testgear-adapter-pytest-2.1.2.tar.gz` & `tmp/testgear-adapter-pytest-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgear-adapter-pytest-2.1.2.tar", last modified: Fri Apr 21 14:56:06 2023, max compression
+gzip compressed data, was "testgear-adapter-pytest-2.1.3.tar", last modified: Fri May 12 09:41:24 2023, max compression
```

## Comparing `testgear-adapter-pytest-2.1.2.tar` & `testgear-adapter-pytest-2.1.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:56:06.331037 testgear-adapter-pytest-2.1.2/
--rw-rw-rw-   0        0        0    12314 2023-04-21 14:56:06.331037 testgear-adapter-pytest-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    11760 2023-03-31 06:28:55.000000 testgear-adapter-pytest-2.1.2/README.md
--rw-rw-rw-   0        0        0      111 2023-04-21 13:48:08.000000 testgear-adapter-pytest-2.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 14:56:06.331037 testgear-adapter-pytest-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1007 2023-04-21 14:03:30.000000 testgear-adapter-pytest-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:56:06.315995 testgear-adapter-pytest-2.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 14:56:06.315995 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:47:37.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest/__init__.py
--rw-rw-rw-   0        0        0     7533 2023-04-21 13:57:30.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest/listener.py
--rw-rw-rw-   0        0        0     3621 2023-04-21 13:58:22.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest/plugin.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:56:06.331037 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest.egg-info/
--rw-rw-rw-   0        0        0    12314 2023-04-21 14:56:06.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-04-21 14:56:06.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:56:06.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-04-21 14:56:06.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-04-21 14:56:06.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-21 14:56:06.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:24.447960 testgear-adapter-pytest-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-05-12 09:41:24.447960 testgear-adapter-pytest-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-05-12 09:41:06.000000 testgear-adapter-pytest-2.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:41:24.447960 testgear-adapter-pytest-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-12 09:41:06.000000 testgear-adapter-pytest-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:24.447960 testgear-adapter-pytest-2.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:24.447960 testgear-adapter-pytest-2.1.3/src/testgear_adapter_pytest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:06.000000 testgear-adapter-pytest-2.1.3/src/testgear_adapter_pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-12 09:41:06.000000 testgear-adapter-pytest-2.1.3/src/testgear_adapter_pytest/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-12 09:41:06.000000 testgear-adapter-pytest-2.1.3/src/testgear_adapter_pytest/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:41:24.447960 testgear-adapter-pytest-2.1.3/src/testgear_adapter_pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-05-12 09:41:24.000000 testgear-adapter-pytest-2.1.3/src/testgear_adapter_pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-12 09:41:24.000000 testgear-adapter-pytest-2.1.3/src/testgear_adapter_pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:41:24.000000 testgear-adapter-pytest-2.1.3/src/testgear_adapter_pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-12 09:41:24.000000 testgear-adapter-pytest-2.1.3/src/testgear_adapter_pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 09:41:24.000000 testgear-adapter-pytest-2.1.3/src/testgear_adapter_pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 09:41:24.000000 testgear-adapter-pytest-2.1.3/src/testgear_adapter_pytest.egg-info/top_level.txt
```

### Comparing `testgear-adapter-pytest-2.1.2/setup.py` & `testgear-adapter-pytest-2.1.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from setuptools import find_packages, setup
-
-setup(
-    name='testgear-adapter-pytest',
-    version='2.1.2',
-    description='Pytest adapter for Test Gear',
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
-    py_modules=['testgear_adapter_pytest'],
-    packages=find_packages(where='src'),
-    package_dir={'': 'src'},
-    install_requires=['pytest', 'pytest-xdist', 'testgear-python-commons==2.1.2'],
-    entry_points={'pytest11': ['testgear_adapter_pytest = testgear_adapter_pytest.plugin']}
-)
+from setuptools import find_packages, setup
+
+setup(
+    name='testgear-adapter-pytest',
+    version='2.1.3',
+    description='Pytest adapter for Test Gear',
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
+    py_modules=['testgear_adapter_pytest'],
+    packages=find_packages(where='src'),
+    package_dir={'': 'src'},
+    install_requires=['pytest', 'pytest-xdist', 'testgear-python-commons==2.1.3'],
+    entry_points={'pytest11': ['testgear_adapter_pytest = testgear_adapter_pytest.plugin']}
+)
```

### Comparing `testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest/listener.py` & `testgear-adapter-pytest-2.1.3/src/testgear_adapter_pytest/listener.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,198 +1,198 @@
-import pickle
-
-from packaging import version
-
-import pytest
-
-import testgear_python_commons.services as adapter
-from testgear_python_commons.models.outcome_type import OutcomeType
-from testgear_python_commons.services import AdapterManager, Utils
-from testgear_python_commons.step import Step
-
-STATUS = {
-    'passed': OutcomeType.PASSED,
-    'failed': OutcomeType.FAILED,
-    'skipped': OutcomeType.SKIPPED
-}
-
-
-class TmsListener(object):
-    __executable_test = None
-    __pytest_check_info = None
-    __failures = None
-
-    def __init__(self, adapter_manager: AdapterManager):
-        self.__adapter_manager = adapter_manager
-
-    @pytest.hookimpl
-    def pytest_configure(self, config):
-        if not hasattr(config, "workerinput") and not hasattr(self, "test_run_id"):
-            config.test_run_id = self.__adapter_manager.get_test_run_id()
-        else:
-            config.test_run_id = pickle.loads(config.workerinput["test_run_id"])
-
-        self.__adapter_manager.set_test_run_id(config.test_run_id)
-
-    @pytest.hookimpl
-    def pytest_configure_node(self, node):
-        if not hasattr(self, "test_run_id"):
-            node.workerinput["test_run_id"] = pickle.dumps(node.config.test_run_id)
-
-    @adapter.hookimpl
-    def get_pytest_check_outcome(self):
-        if self.__pytest_check_info:
-            if version.parse(self.__pytest_check_info.version) < version.parse("1.1.0"):
-                from pytest_check import check_methods as logs
-            else:
-                from pytest_check import check_log as logs
-
-            failures = logs.get_failures()
-
-            if failures and self.__failures != failures:
-                self.__failures = failures[:]
-                return 'Failed'
-        return 'Passed'
-
-    @pytest.hookimpl
-    def pytest_collection_modifyitems(self, config, items):
-        index = 0
-        selected_items = []
-        deselected_items = []
-        plugin_info = config.pluginmanager.list_plugin_distinfo()
-
-        for plugin, dist in plugin_info:
-            if 'pytest-check' == dist.project_name:
-                self.__pytest_check_info = dist
-                break
-
-        resolved_autotests = self.__adapter_manager.get_autotests_for_launch()
-
-        for item in items:
-            if not hasattr(item.function, 'test_external_id'):
-                item.test_external_id = Utils.get_hash(item.nodeid + item.function.__name__)
-
-            if hasattr(item.function, 'test_external_id'):
-                if item.own_markers:
-                    for mark in item.own_markers:
-                        if mark.name == 'parametrize':
-                            if not hasattr(item, 'array_parametrize_mark_id'):
-                                item.array_parametrize_mark_id = []
-                            item.array_parametrize_mark_id.append(
-                                item.own_markers.index(mark))
-
-                params = Utils.get_params(item)
-                item.test_external_id = Utils.param_attribute_collector(
-                    item.function.test_external_id,
-                    params)
-
-                item.index = index
-                item_id = items.index(item)
-                index = index + 1 if len(items) > item_id + 1 and items[item_id + 1].originalname == item.originalname \
-                    else 0
-
-                if resolved_autotests \
-                        and item.test_external_id in resolved_autotests:
-                    selected_items.append(item)
-        if resolved_autotests:
-            if not selected_items:
-                print('The specified tests were not found!')
-                raise SystemExit
-
-            config.hook.pytest_deselected(items=deselected_items)
-            items[:] = selected_items
-
-    @pytest.hookimpl
-    def pytest_runtest_protocol(self, item):
-        if not hasattr(item.function, 'test_external_id'):
-            item.test_external_id = Utils.get_hash(item.nodeid + item.function.__name__)
-
-        if not hasattr(item.function, 'test_displayname'):
-            item.test_displayname = item.function.__doc__ if \
-                item.function.__doc__ else item.function.__name__
-        else:
-            params = Utils.get_params(item)
-
-            item.test_displayname = Utils.param_attribute_collector(
-                item.function.test_displayname,
-                params)
-
-        self.__executable_test = Utils.form_test(item)
-
-    @pytest.hookimpl(hookwrapper=True)
-    def pytest_fixture_setup(self, fixturedef):
-        yield
-        if self.__executable_test:
-            steps_data, results_steps_data = Step.get_steps_data()
-
-            if fixturedef.scope == 'function':
-                self.__executable_test['setUp'] += steps_data
-                self.__executable_test['setUpResults'] += results_steps_data
-
-    @pytest.hookimpl(hookwrapper=True, trylast=True)
-    def pytest_runtest_call(self):
-        yield
-
-        if not self.__executable_test:
-            return
-
-        test_steps, test_results_steps = Step.get_steps_data()
-        self.__executable_test['steps'] = test_steps
-        self.__executable_test['stepResults'] = test_results_steps
-
-    @pytest.hookimpl
-    def pytest_fixture_post_finalizer(self, fixturedef):
-        if not self.__executable_test:
-            return
-
-        teardown_steps, teardown_results_steps = Step.get_steps_data()
-
-        if fixturedef.scope == 'function':
-            self.__executable_test['tearDown'] += teardown_steps
-            self.__executable_test['tearDownResults'] += teardown_results_steps
-
-    @pytest.hookimpl
-    def pytest_runtest_logreport(self, report):
-        if self.__executable_test:
-            if report.when == 'setup':
-                self.__executable_test['outcome'] = STATUS.get(report.outcome, None)
-                if report.longreprtext:
-                    self.__executable_test['message'] = report.longreprtext
-
-            if report.when == 'call':
-                self.__executable_test['outcome'] = STATUS.get(report.outcome, None)
-
-            if report.failed or hasattr(report, 'wasxfail') \
-                    and not report.passed or report.outcome == 'rerun':
-                self.__executable_test['outcome'] = STATUS.get('failed', None)
-
-                if report.longreprtext:
-                    self.__executable_test['traces'] = report.longreprtext
-
-            self.__executable_test['duration'] += report.duration * 1000
-
-    @pytest.hookimpl
-    def pytest_runtest_logfinish(self):
-        if not self.__executable_test:
-            return
-
-        self.__adapter_manager.write_test(self.__executable_test)
-
-    @adapter.hookimpl
-    def add_link(self, link):
-        if self.__executable_test:
-            self.__executable_test['resultLinks'].append(link)
-
-    @adapter.hookimpl
-    def add_message(self, test_message):
-        if self.__executable_test:
-            self.__executable_test['message'] = str(test_message)
-
-    @adapter.hookimpl
-    def add_attachments(self, attach_paths: list or tuple):
-        if self.__executable_test:
-            self.__executable_test['attachments'] += self.__adapter_manager.load_attachments(attach_paths)
-
-    @adapter.hookimpl
-    def create_attachment(self, body, name: str):
-        if self.__executable_test:
-            self.__executable_test['attachments'] += self.__adapter_manager.create_attachment(body, name)
+import pickle
+
+from packaging import version
+
+import pytest
+
+import testgear_python_commons.services as adapter
+from testgear_python_commons.models.outcome_type import OutcomeType
+from testgear_python_commons.services import AdapterManager, Utils
+from testgear_python_commons.step import Step
+
+STATUS = {
+    'passed': OutcomeType.PASSED,
+    'failed': OutcomeType.FAILED,
+    'skipped': OutcomeType.SKIPPED
+}
+
+
+class TmsListener(object):
+    __executable_test = None
+    __pytest_check_info = None
+    __failures = None
+
+    def __init__(self, adapter_manager: AdapterManager):
+        self.__adapter_manager = adapter_manager
+
+    @pytest.hookimpl
+    def pytest_configure(self, config):
+        if not hasattr(config, "workerinput") and not hasattr(self, "test_run_id"):
+            config.test_run_id = self.__adapter_manager.get_test_run_id()
+        else:
+            config.test_run_id = pickle.loads(config.workerinput["test_run_id"])
+
+        self.__adapter_manager.set_test_run_id(config.test_run_id)
+
+    @pytest.hookimpl
+    def pytest_configure_node(self, node):
+        if not hasattr(self, "test_run_id"):
+            node.workerinput["test_run_id"] = pickle.dumps(node.config.test_run_id)
+
+    @adapter.hookimpl
+    def get_pytest_check_outcome(self):
+        if self.__pytest_check_info:
+            if version.parse(self.__pytest_check_info.version) < version.parse("1.1.0"):
+                from pytest_check import check_methods as logs
+            else:
+                from pytest_check import check_log as logs
+
+            failures = logs.get_failures()
+
+            if failures and self.__failures != failures:
+                self.__failures = failures[:]
+                return 'Failed'
+        return 'Passed'
+
+    @pytest.hookimpl
+    def pytest_collection_modifyitems(self, config, items):
+        index = 0
+        selected_items = []
+        deselected_items = []
+        plugin_info = config.pluginmanager.list_plugin_distinfo()
+
+        for plugin, dist in plugin_info:
+            if 'pytest-check' == dist.project_name:
+                self.__pytest_check_info = dist
+                break
+
+        resolved_autotests = self.__adapter_manager.get_autotests_for_launch()
+
+        for item in items:
+            if not hasattr(item.function, 'test_external_id'):
+                item.test_external_id = Utils.get_hash(item.nodeid + item.function.__name__)
+
+            if hasattr(item.function, 'test_external_id'):
+                if item.own_markers:
+                    for mark in item.own_markers:
+                        if mark.name == 'parametrize':
+                            if not hasattr(item, 'array_parametrize_mark_id'):
+                                item.array_parametrize_mark_id = []
+                            item.array_parametrize_mark_id.append(
+                                item.own_markers.index(mark))
+
+                params = Utils.get_params(item)
+                item.test_external_id = Utils.param_attribute_collector(
+                    item.function.test_external_id,
+                    params)
+
+                item.index = index
+                item_id = items.index(item)
+                index = index + 1 if len(items) > item_id + 1 and items[item_id + 1].originalname == item.originalname \
+                    else 0
+
+                if resolved_autotests \
+                        and item.test_external_id in resolved_autotests:
+                    selected_items.append(item)
+        if resolved_autotests:
+            if not selected_items:
+                print('The specified tests were not found!')
+                raise SystemExit
+
+            config.hook.pytest_deselected(items=deselected_items)
+            items[:] = selected_items
+
+    @pytest.hookimpl
+    def pytest_runtest_protocol(self, item):
+        if not hasattr(item.function, 'test_external_id'):
+            item.test_external_id = Utils.get_hash(item.nodeid + item.function.__name__)
+
+        if not hasattr(item.function, 'test_displayname'):
+            item.test_displayname = item.function.__doc__ if \
+                item.function.__doc__ else item.function.__name__
+        else:
+            params = Utils.get_params(item)
+
+            item.test_displayname = Utils.param_attribute_collector(
+                item.function.test_displayname,
+                params)
+
+        self.__executable_test = Utils.form_test(item)
+
+    @pytest.hookimpl(hookwrapper=True)
+    def pytest_fixture_setup(self, fixturedef):
+        yield
+        if self.__executable_test:
+            steps_data, results_steps_data = Step.get_steps_data()
+
+            if fixturedef.scope == 'function':
+                self.__executable_test['setUp'] += steps_data
+                self.__executable_test['setUpResults'] += results_steps_data
+
+    @pytest.hookimpl(hookwrapper=True, trylast=True)
+    def pytest_runtest_call(self):
+        yield
+
+        if not self.__executable_test:
+            return
+
+        test_steps, test_results_steps = Step.get_steps_data()
+        self.__executable_test['steps'] = test_steps
+        self.__executable_test['stepResults'] = test_results_steps
+
+    @pytest.hookimpl
+    def pytest_fixture_post_finalizer(self, fixturedef):
+        if not self.__executable_test:
+            return
+
+        teardown_steps, teardown_results_steps = Step.get_steps_data()
+
+        if fixturedef.scope == 'function':
+            self.__executable_test['tearDown'] += teardown_steps
+            self.__executable_test['tearDownResults'] += teardown_results_steps
+
+    @pytest.hookimpl
+    def pytest_runtest_logreport(self, report):
+        if self.__executable_test:
+            if report.when == 'setup':
+                self.__executable_test['outcome'] = STATUS.get(report.outcome, None)
+                if report.longreprtext:
+                    self.__executable_test['message'] = report.longreprtext
+
+            if report.when == 'call':
+                self.__executable_test['outcome'] = STATUS.get(report.outcome, None)
+
+            if report.failed or hasattr(report, 'wasxfail') \
+                    and not report.passed or report.outcome == 'rerun':
+                self.__executable_test['outcome'] = STATUS.get('failed', None)
+
+                if report.longreprtext:
+                    self.__executable_test['traces'] = report.longreprtext
+
+            self.__executable_test['duration'] += report.duration * 1000
+
+    @pytest.hookimpl
+    def pytest_runtest_logfinish(self):
+        if not self.__executable_test:
+            return
+
+        self.__adapter_manager.write_test(self.__executable_test)
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

