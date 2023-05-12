# Comparing `tmp/autometrics-0.4.tar.gz` & `tmp/autometrics-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autometrics-0.4.tar", max compression
+gzip compressed data, was "autometrics-0.5.tar", max compression
```

## Comparing `autometrics-0.4.tar` & `autometrics-0.5.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0     1022 2023-03-06 16:22:27.425939 autometrics-0.4/LICENSE
--rw-r--r--   0        0        0     5439 2023-04-13 10:20:53.040055 autometrics-0.4/README.md
--rw-r--r--   0        0        0     1825 2023-04-13 10:53:46.784179 autometrics-0.4/pyproject.toml
--rw-r--r--   0        0        0       25 2023-04-13 09:01:12.452935 autometrics-0.4/src/autometrics/__init__.py
--rw-r--r--   0        0        0      843 2023-04-13 10:20:53.042912 autometrics-0.4/src/autometrics/constants.py
--rw-r--r--   0        0        0     1913 2023-04-13 10:20:53.043762 autometrics-0.4/src/autometrics/decorator.py
--rw-r--r--   0        0        0     2158 2023-04-13 10:20:53.044169 autometrics-0.4/src/autometrics/emit.py
--rw-r--r--   0        0        0     3050 2023-04-13 10:20:53.044607 autometrics-0.4/src/autometrics/objectives.py
--rw-r--r--   0        0        0     1956 2023-04-13 10:20:53.045139 autometrics-0.4/src/autometrics/prometheus_url.py
--rw-r--r--   0        0        0     6787 2023-04-13 10:20:53.045649 autometrics-0.4/src/autometrics/test_decorator.py
--rw-r--r--   0        0        0     1401 2023-04-13 10:20:53.045977 autometrics-0.4/src/autometrics/test_prometheus_url.py
--rw-r--r--   0        0        0     1535 2023-04-13 10:20:53.046402 autometrics-0.4/src/autometrics/utils.py
--rw-r--r--   0        0        0     6416 1970-01-01 00:00:00.000000 autometrics-0.4/PKG-INFO
+-rw-r--r--   0        0        0     1022 2023-04-12 17:23:29.278864 autometrics-0.5/LICENSE
+-rw-r--r--   0        0        0     7398 2023-05-11 14:31:00.584949 autometrics-0.5/README.md
+-rw-r--r--   0        0        0     2052 2023-05-12 08:30:51.478225 autometrics-0.5/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-05-11 14:31:00.585437 autometrics-0.5/src/autometrics/__init__.py
+-rw-r--r--   0        0        0     1269 2023-05-11 12:02:53.378510 autometrics-0.5/src/autometrics/constants.py
+-rw-r--r--   0        0        0     3979 2023-05-11 14:31:00.585878 autometrics-0.5/src/autometrics/decorator.py
+-rw-r--r--   0        0        0     3050 2023-04-13 12:18:19.449416 autometrics-0.5/src/autometrics/objectives.py
+-rw-r--r--   0        0        0     2197 2023-05-11 12:02:53.378737 autometrics-0.5/src/autometrics/prometheus_url.py
+-rw-r--r--   0        0        0     9729 2023-05-10 12:22:44.149925 autometrics-0.5/src/autometrics/test_decorator.py
+-rw-r--r--   0        0        0     3065 2023-05-11 12:02:53.378981 autometrics-0.5/src/autometrics/test_prometheus_url.py
+-rw-r--r--   0        0        0       23 2023-05-05 10:51:08.826284 autometrics-0.5/src/autometrics/tracker/__init__.py
+-rw-r--r--   0        0        0     4565 2023-05-11 12:02:53.379215 autometrics-0.5/src/autometrics/tracker/opentelemetry.py
+-rw-r--r--   0        0        0     3520 2023-05-11 12:02:53.379424 autometrics-0.5/src/autometrics/tracker/prometheus.py
+-rw-r--r--   0        0        0     2693 2023-05-11 12:02:53.379696 autometrics-0.5/src/autometrics/tracker/test_tracker.py
+-rw-r--r--   0        0        0     2277 2023-05-11 12:02:53.380041 autometrics-0.5/src/autometrics/tracker/tracker.py
+-rw-r--r--   0        0        0     1820 2023-05-10 15:25:28.523451 autometrics-0.5/src/autometrics/utils.py
+-rw-r--r--   0        0        0     8547 1970-01-01 00:00:00.000000 autometrics-0.5/PKG-INFO
```

### Comparing `autometrics-0.4/LICENSE` & `autometrics-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autometrics-0.4/README.md` & `autometrics-0.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 
 ## Features
 
 - ✨ `autometrics` decorator instruments any function or class method to track the
   most useful metrics
 - 💡 Writes Prometheus queries so you can understand the data generated without
   knowing PromQL
-- 🔗 Create links to live Prometheus charts directly into each functions docstrings (with tooltips coming soon!)
-- 📊 (Coming Soon!) Grafana dashboard showing the performance of all
-  instrumented functions
-- 🚨 Enable Prometheus alerts using SLO best practices from simple annotations in your code
+- 🔗 Create links to live Prometheus charts directly into each function's docstring
+- [🔍 Identify commits](#identifying-commits-that-introduced-problems) that introduced errors or increased latency
+- [🚨 Define alerts](#alerts--slos) using SLO best practices directly in your source code
+- [📊 Grafana dashboards](#dashboards) work out of the box to visualize the performance of instrumented functions & SLOs
+- [⚙️ Configurable](#metrics-libraries) metric collection library (`opentelemetry`, `prometheus`, or `metrics`)
 - ⚡ Minimal runtime overhead
 
 ## Using autometrics-py
 
 - Set up a [Prometheus instance](https://prometheus.io/download/)
 - Configure prometheus to scrape your application ([check our instructions if you need help](https://github.com/autometrics-dev#5-configuring-prometheus))
 - Include a .env file with your prometheus endpoint `PROMETHEUS_URL=your endpoint`. If this is not defined, the default endpoint will be `http://localhost:9090/`
@@ -42,14 +43,18 @@
 
 - To access the PromQL queries for your decorated functions, run `help(yourfunction)` or `print(yourfunction.__doc__)`.
 
 - To show tooltips over decorated functions in VSCode, with links to Prometheus queries, try installing [the VSCode extension](https://marketplace.visualstudio.com/items?itemName=Fiberplane.autometrics).
 
 > Note that we cannot support tooltips without a VSCode extension due to behavior of the [static analyzer](https://github.com/davidhalter/jedi/issues/1921) used in VSCode.
 
+## Dashboards
+
+Autometrics provides [Grafana dashboards](https://github.com/autometrics-dev/autometrics-shared#dashboards) that will work for any project instrumented with the library.
+
 ## Alerts / SLOs
 
 Autometrics makes it easy to add Prometheus alerts using Service-Level Objectives (SLOs) to a function or group of functions.
 
 In order to receive alerts you need to add a set of rules to your Prometheus set up. You can find out more about those rules here: [Prometheus alerting rules](https://github.com/autometrics-dev/autometrics-shared#prometheus-recording--alerting-rules). Once added, most of the recording rules are dormant. They are enabled by specific metric labels that can be automatically attached by autometrics.
 
 To use autometrics SLOs and alerts, create one or multiple `Objective`s based on the function(s) success rate and/or latency, as shown below. The `Objective` can be passed as an argument to the `autometrics` macro to include the given function in that objective.
@@ -99,14 +104,36 @@
 ```py
 @autometrics
 @noop
 def api_handler():
   # ...
 ```
 
+#### Metrics Libraries
+
+Configure the crate that autometrics will use to produce metrics by using one of the following feature flags:
+
+- `opentelemetry` - (enabled by default, can also be explicitly set using the AUTOMETRICS_TRACKER="OPEN_TELEMETERY" env var) uses
+- `prometheus` - (using the AUTOMETRICS_TRACKER env var set to "PROMETHEUS")
+
+## Identifying commits that introduced problems
+
+> **NOTE** - As of writing, `build_info` will not work correctly when using the default tracker (`AUTOMETRICS_TRACKER=OPEN_TELEMETRY`).
+> This will be fixed once the following PR is merged on the opentelemetry-python project: https://github.com/open-telemetry/opentelemetry-python/pull/3306
+>
+> autometrics-py will track support for build_info using the OpenTelemetry tracker via #38
+
+Autometrics makes it easy to identify if a specific version or commit introduced errors or increased latencies.
+
+It uses a separate metric (`build_info`) to track the version and, optionally, git commit of your service. It then writes queries that group metrics by the `version` and `commit` labels so you can spot correlations between those and potential issues.
+
+The `version` is read from the `AUTOMETRICS_VERSION` environment variable, and the `commit` value uses the environment variable `AUTOMETRICS_COMMIT`.
+
+This follows the method outlined in [Exposing the software version to Prometheus](https://www.robustperception.io/exposing-the-software-version-to-prometheus/).
+
 ## Development of the package
 
 This package uses [poetry](https://python-poetry.org) as a package manager, with all dependencies separated into three groups:
 
 - root level dependencies, required
 - `dev`, everything that is needed for development or in ci
 - `examples`, dependencies of everything in `examples/` directory
@@ -134,8 +161,10 @@
 ```sh
 # Formatting using black
 poetry run black .
 # Lint using pyright
 poetry run pyright
 # Run the tests using pytest
 poetry run pytest
+# Run a single test, and clear the cache
+poetry run pytest --cache-clear -k test_tracker
 ```
```

### Comparing `autometrics-0.4/pyproject.toml` & `autometrics-0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 [tool.poetry]
 name = "autometrics"
-version = "0.4"
+version = "0.5"
 description = "Easily add metrics to your system – and actually understand them using automatically customized Prometheus queries"
 authors = ["Fiberplane <info@fiberplane.com>"]
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/autometrics-dev/autometrics-py"
 homepage = "https://github.com/autometrics-dev/autometrics-py"
 keywords = ["metrics", "telemetry", "prometheus", "monitoring", "observability", "instrumentation"]
 # classifiers = [
 #     "Topic :: Software Development :: Build Tools",
 #     "Topic :: Software Development :: Libraries :: Python Modules"
 # ]
 packages = [{include = "autometrics", from = "src"}]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+opentelemetry-api = "^1.17.0"
+opentelemetry-exporter-prometheus = "^1.12.0rc1"
+opentelemetry-sdk = "^1.17.0"
 prometheus-client = "0.16.0"
+python = "^3.8"
 python-dotenv = "1.0.0"
 typing-extensions = "^4.5.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-pyright = "^1.1.302"
+pyright = "^1.1.307"
 pytest = "^7.3.0"
+pytest-asyncio = "^0.21.0"
 black = "^23.3.0"
 
 [tool.poetry.group.examples]
 optional = true
 
 [tool.poetry.group.examples.dependencies]
 anyio = "3.6.2"
 bleach = "6.0.0"
 build = "0.10.0"
 certifi = "2022.12.7"
 charset-normalizer = "3.1.0"
 click = "8.1.3"
+django = "^4.2"
 docutils = "0.19"
 fastapi = "0.95.0"
 h11 = "0.14.0"
 idna = "3.4"
-importlib-metadata = "6.1.0"
+# pinned importlib-metadat to version ~6.0.0 because of opentelemetry-api
+importlib-metadata = "~6.0.0"
 jaraco-classes = "3.2.3"
 keyring = "23.13.1"
 markdown-it-py = "2.2.0"
 mdurl = "0.1.2"
 more-itertools = "9.1.0"
 packaging = "23.0"
 pkginfo = "1.9.6"
```

### Comparing `autometrics-0.4/src/autometrics/constants.py` & `autometrics-0.5/src/autometrics/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,28 @@
 """Constants used by autometrics"""
 
+COUNTER_NAME = "function.calls.count"
+HISTOGRAM_NAME = "function.calls.duration"
+# NOTE - The Rust implementation does not use `build.info`, instead opts for just `build_info`
+BUILD_INFO_NAME = "build_info"
+
+COUNTER_NAME_PROMETHEUS = COUNTER_NAME.replace(".", "_")
+HISTOGRAM_NAME_PROMETHEUS = HISTOGRAM_NAME.replace(".", "_")
+
 COUNTER_DESCRIPTION = "Autometrics counter for tracking function calls"
 HISTOGRAM_DESCRIPTION = "Autometrics histogram for tracking function call duration"
+BUILD_INFO_DESCRIPTION = (
+    "Autometrics info metric for tracking software version and build details"
+)
 
 # The following constants are used to create the labels
-OBJECTIVE_NAME = "objective.name".replace(".", "_")
-OBJECTIVE_PERCENTILE = "objective.percentile".replace(".", "_")
-OBJECTIVE_LATENCY_THRESHOLD = "objective.latency_threshold".replace(".", "_")
+OBJECTIVE_NAME = "objective.name"
+OBJECTIVE_PERCENTILE = "objective.percentile"
+OBJECTIVE_LATENCY_THRESHOLD = "objective.latency_threshold"
+VERSION_KEY = "version"
+COMMIT_KEY = "commit"
 
 # The values are updated to use underscores instead of periods to avoid issues with prometheus.
 # A similar thing is done in the rust library, which supports multiple exporters
 OBJECTIVE_NAME_PROMETHEUS = OBJECTIVE_NAME.replace(".", "_")
 OBJECTIVE_PERCENTILE_PROMETHEUS = OBJECTIVE_PERCENTILE.replace(".", "_")
 OBJECTIVE_LATENCY_THRESHOLD_PROMETHEUS = OBJECTIVE_LATENCY_THRESHOLD.replace(".", "_")
```

### Comparing `autometrics-0.4/src/autometrics/objectives.py` & `autometrics-0.5/src/autometrics/objectives.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.4/src/autometrics/prometheus_url.py` & `autometrics-0.5/src/autometrics/prometheus_url.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import urllib.parse
 import os
 from typing import Optional
 from dotenv import load_dotenv
 
+ADD_BUILD_INFO_LABELS = "* on (instance, job) group_left(version, commit) (last_over_time(build_info[1s]) or on (instance, job) up)"
+
 
 def cleanup_url(url: str) -> str:
     """Remove the trailing slash if there is one."""
     if url[-1] == "/":
         url = url[:-1]
     return url
 
@@ -22,27 +24,29 @@
         self.module_name = module_name
 
         url = base_url or os.getenv("PROMETHEUS_URL") or "http://localhost:9090"
         self.base_url = cleanup_url(url)
 
     def create_urls(self):
         """Create the prometheus query urls for the function and module."""
-        request_rate_query = f'sum by (function, module) (rate (function_calls_count_total{{function="{self.function_name}",module="{self.module_name}"}}[5m]))'
-        latency_query = f'sum by (le, function, module) (rate(function_calls_duration_bucket{{function="{self.function_name}",module="{self.module_name}"}}[5m]))'
-        error_ratio_query = f'sum by (function, module) (rate (function_calls_count_total{{function="{self.function_name}",module="{self.module_name}", result="error"}}[5m])) / {request_rate_query}'
+        request_rate_query = f'sum by (function, module, commit, version) (rate (function_calls_count_total{{function="{self.function_name}",module="{self.module_name}"}}[5m]) {ADD_BUILD_INFO_LABELS})'
+        latency_query = f'sum by (le, function, module, commit, version) (rate(function_calls_duration_bucket{{function="{self.function_name}",module="{self.module_name}"}}[5m]) {ADD_BUILD_INFO_LABELS})'
+        error_ratio_query = f'sum by (function, module, commit, version) (rate (function_calls_count_total{{function="{self.function_name}",module="{self.module_name}", result="error"}}[5m]) {ADD_BUILD_INFO_LABELS}) / {request_rate_query}'
+
+        queries = {
+            "Request rate URL": request_rate_query,
+            "Latency URL": latency_query,
+            "Error Ratio URL": error_ratio_query,
+        }
 
-        queries = [request_rate_query, latency_query, error_ratio_query]
-        names = ["Request rate URL", "Latency URL", "Error Ratio URL"]
         urls = {}
-        for name in names:
-            for query in queries:
-                generated_url = self.create_prometheus_url(query)
-                urls[name] = generated_url
-                queries.remove(query)
-                break
+        for [name, query] in queries.items():
+            # for query in queries:
+            generated_url = self.create_prometheus_url(query)
+            urls[name] = generated_url
         return urls
 
     def create_prometheus_url(self, query: str):
         """Create a the full query url for a given query."""
         encoded_query = urllib.parse.quote(query)
         url = f"{self.base_url}/graph?g0.expr={encoded_query}&g0.tab=0"
         return url
```

### Comparing `autometrics-0.4/src/autometrics/test_decorator.py` & `autometrics-0.5/src/autometrics/test_decorator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,140 +1,215 @@
 """Test the autometrics decorator."""
+import time
+import asyncio
 from prometheus_client.exposition import generate_latest
-from prometheus_client import registry, Metric
-from pytest import raises
+import pytest
 
 from .decorator import autometrics
 from .objectives import ObjectiveLatency, Objective, ObjectivePercentile
+
+from .tracker import set_tracker, TrackerType
 from .utils import get_caller_function
 
 
-def basic_function():
+def basic_function(sleep_duration: float = 0.0):
     """This is a basic function."""
+    time.sleep(sleep_duration)
     return True
 
 
-def find_metric_with_name(metrics: "list[Metric]", name: str):
-    """Find a metric with a given name."""
-    for metric in metrics:
-        if metric.name == name:
-            return metric
-
-    return None
-
-
-def test_basic():
-    """This is a basic test."""
-
-    # set up the function + basic variables
-    caller = get_caller_function(depth=1)
-    assert caller is not None
-    assert caller != ""
-    function_name = basic_function.__name__
-    wrapped_function = autometrics(basic_function)
-    wrapped_function()
-
-    # get the metrics
-    blob = generate_latest(registry.REGISTRY)
-    assert blob is not None
-    data = blob.decode("utf-8")
-
-    total_count = f"""function_calls_count_total{{caller="{caller}",function="{function_name}",module="test_decorator",objective_name="",objective_percentile="",result="ok"}} 1.0"""
-    assert total_count in data
-    count_created = f"""function_calls_count_created{{caller="{caller}",function="{function_name}",module="test_decorator",objective_name="",objective_percentile="",result="ok"}}"""
-    assert count_created in data
-
-    for latency in ObjectiveLatency:
-        query = f"""function_calls_duration_bucket{{function="{function_name}",le="{latency.value}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
-        assert query in data
-
-    duration_count = f"""function_calls_duration_count{{function="{function_name}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
-    assert duration_count in data
-
-    duration_sum = f"""function_calls_duration_sum{{function="{function_name}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
-    assert duration_sum in data
-
-    duration_created = f"""function_calls_duration_created{{function="{function_name}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
-    assert duration_created in data
-
-
-def test_objectives():
-    """This is a test that covers objectives."""
-
-    # set up the function + objective variables
-    caller = get_caller_function(depth=1)
-    assert caller is not None
-    assert caller != ""
-    objective_name = "test_objective"
-    success_rate = ObjectivePercentile.P90
-    latency = (ObjectiveLatency.Ms100, ObjectivePercentile.P99)
-    objective = Objective(
-        name=objective_name, success_rate=success_rate, latency=latency
-    )
-    function_name = basic_function.__name__
-    wrapped_function = autometrics(objective=objective)(basic_function)
-
-    # call the function
-    wrapped_function()
-
-    # get the metrics
-    blob = generate_latest(registry.REGISTRY)
-    assert blob is not None
-    data = blob.decode("utf-8")
-
-    total_count = f"""function_calls_count_total{{caller="{caller}",function="{function_name}",module="test_decorator",objective_name="{objective_name}",objective_percentile="{success_rate.value}",result="ok"}} 1.0"""
-    assert total_count in data
-    count_created = f"""function_calls_count_created{{caller="{caller}",function="{function_name}",module="test_decorator",objective_name="{objective_name}",objective_percentile="{success_rate.value}",result="ok"}}"""
-    assert count_created in data
-
-    for objective in ObjectiveLatency:
-        query = f"""function_calls_duration_bucket{{function="{function_name}",le="{objective.value}",module="test_decorator",objective_latency_threshold="{latency[0].value}",objective_name="{objective_name}",objective_percentile="{latency[1].value}"}}"""
-        assert query in data
-
-    duration_count = f"""function_calls_duration_count{{function="{function_name}",module="test_decorator",objective_latency_threshold="{latency[0].value}",objective_name="{objective_name}",objective_percentile="{latency[1].value}"}}"""
-    assert duration_count in data
+def error_function():
+    """This is a function that raises an error."""
+    raise RuntimeError("This is a test error")
 
-    duration_sum = f"""function_calls_duration_sum{{function="{function_name}",module="test_decorator",objective_latency_threshold="{latency[0].value}",objective_name="{objective_name}",objective_percentile="{latency[1].value}"}}"""
-    assert duration_sum in data
 
-    duration_created = f"""function_calls_duration_created{{function="{function_name}",module="test_decorator",objective_latency_threshold="{latency[0].value}",objective_name="{objective_name}",objective_percentile="{latency[1].value}"}}"""
-    assert duration_created in data
+async def basic_async_function(sleep_duration: float = 1.0):
+    """This is a basic async function."""
+    await asyncio.sleep(sleep_duration)
+    return True
 
 
-def error_function():
-    """This is a function that raises an error."""
+async def error_async_function():
+    """This is an async function that raises an error."""
+    await asyncio.sleep(0.5)
     raise RuntimeError("This is a test error")
 
 
-def test_exception():
-    caller = get_caller_function(depth=1)
-    assert caller is not None
-    assert caller != ""
-    function_name = error_function.__name__
-    wrapped_function = autometrics(error_function)
-    with raises(RuntimeError) as exception:
-        wrapped_function()
-    assert "This is a test error" in str(exception.value)
+tracker_types = [TrackerType.PROMETHEUS, TrackerType.OPENTELEMETRY]
+
+
+@pytest.fixture(scope="class", params=tracker_types)
+def setup_tracker_type(request):
+    """Force the use of a specific metrics tracker"""
+    set_tracker(request.param)
+
 
-    # get the metrics
-    blob = generate_latest(registry.REGISTRY)
-    assert blob is not None
-    data = blob.decode("utf-8")
-    print("data", data)
-
-    total_count = f"""function_calls_count_total{{caller="{caller}",function="{function_name}",module="test_decorator",objective_name="",objective_percentile="",result="error"}} 1.0"""
-    assert total_count in data
-    count_created = f"""function_calls_count_created{{caller="{caller}",function="{function_name}",module="test_decorator",objective_name="",objective_percentile="",result="error"}}"""
-    assert count_created in data
-
-    for latency in ObjectiveLatency:
-        query = f"""function_calls_duration_bucket{{function="{function_name}",le="{latency.value}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
-        assert query in data
+@pytest.mark.usefixtures("setup_tracker_type")
+class TestDecoratorClass:
+    """Test the autometrics decorator. These tests are run multiple times with different trackers."""
+
+    def test_basic(self):
+        """This is a basic test."""
+
+        # set up the function + basic variables
+        caller = get_caller_function(depth=1)
+        assert caller is not None
+        assert caller != ""
+        function_name = basic_function.__name__
+        wrapped_function = autometrics(basic_function)
+        wrapped_function()
 
-    duration_count = f"""function_calls_duration_count{{function="{function_name}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
-    assert duration_count in data
+        blob = generate_latest()
+        assert blob is not None
+        data = blob.decode("utf-8")
+
+        total_count = f"""function_calls_count_total{{caller="{caller}",function="{function_name}",module="test_decorator",objective_name="",objective_percentile="",result="ok"}} 1.0"""
+        assert total_count in data
+
+        for latency in ObjectiveLatency:
+            query = f"""function_calls_duration_bucket{{function="{function_name}",le="{latency.value}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
+            assert query in data
+
+        duration_count = f"""function_calls_duration_count{{function="{function_name}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
+        assert duration_count in data
+
+        duration_sum = f"""function_calls_duration_sum{{function="{function_name}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
+        assert duration_sum in data
+
+    @pytest.mark.asyncio
+    async def test_basic_async(self):
+        """This is a basic test."""
+
+        # set up the function + basic variables
+        caller = get_caller_function(depth=1)
+        assert caller is not None
+        assert caller != ""
+        function_name = basic_async_function.__name__
+        wrapped_function = autometrics(basic_async_function)
+
+        # Test that the function is *still* async after we wrap it
+        assert asyncio.iscoroutinefunction(wrapped_function) == True
+
+        await wrapped_function()
+
+        blob = generate_latest()
+        assert blob is not None
+        data = blob.decode("utf-8")
+
+        total_count = f"""function_calls_count_total{{caller="{caller}",function="{function_name}",module="test_decorator",objective_name="",objective_percentile="",result="ok"}} 1.0"""
+        assert total_count in data
+
+        for latency in ObjectiveLatency:
+            query = f"""function_calls_duration_bucket{{function="{function_name}",le="{latency.value}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
+            assert query in data
+
+        duration_count = f"""function_calls_duration_count{{function="{function_name}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
+        assert duration_count in data
+
+        duration_sum = f"""function_calls_duration_sum{{function="{function_name}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
+        assert duration_sum in data
+
+    def test_objectives(self):
+        """This is a test that covers objectives."""
+
+        # set up the function + objective variables
+        caller = get_caller_function(depth=1)
+        assert caller is not None
+        assert caller != ""
+        objective_name = "test_objective"
+        success_rate = ObjectivePercentile.P90
+        latency = (ObjectiveLatency.Ms100, ObjectivePercentile.P99)
+        objective = Objective(
+            name=objective_name, success_rate=success_rate, latency=latency
+        )
+        function_name = basic_function.__name__
+        wrapped_function = autometrics(objective=objective)(basic_function)
+
+        sleep_duration = 0.25
+        # call the function
+        wrapped_function(sleep_duration)
+
+        # get the metrics
+        blob = generate_latest()
+        assert blob is not None
+        data = blob.decode("utf-8")
+
+        total_count = f"""function_calls_count_total{{caller="{caller}",function="{function_name}",module="test_decorator",objective_name="{objective_name}",objective_percentile="{success_rate.value}",result="ok"}} 1.0"""
+        assert total_count in data
+
+        # Check the latency buckets
+        for objective in ObjectiveLatency:
+            count = 0 if float(objective.value) <= sleep_duration else 1
+            query = f"""function_calls_duration_bucket{{function="{function_name}",le="{objective.value}",module="test_decorator",objective_latency_threshold="{latency[0].value}",objective_name="{objective_name}",objective_percentile="{latency[1].value}"}} {count}"""
+            assert query in data
+
+        duration_count = f"""function_calls_duration_count{{function="{function_name}",module="test_decorator",objective_latency_threshold="{latency[0].value}",objective_name="{objective_name}",objective_percentile="{latency[1].value}"}}"""
+        assert duration_count in data
+
+        duration_sum = f"""function_calls_duration_sum{{function="{function_name}",module="test_decorator",objective_latency_threshold="{latency[0].value}",objective_name="{objective_name}",objective_percentile="{latency[1].value}"}}"""
+        assert duration_sum in data
+
+    def test_exception(self):
+        """This is a test that covers exceptions."""
+        caller = get_caller_function(depth=1)
+        assert caller is not None
+        assert caller != ""
+
+        function_name = error_function.__name__
+        wrapped_function = autometrics(error_function)
+
+        with pytest.raises(RuntimeError) as exception:
+            wrapped_function()
+        assert "This is a test error" in str(exception.value)
+
+        # get the metrics
+        blob = generate_latest()
+        assert blob is not None
+        data = blob.decode("utf-8")
+
+        total_count = f"""function_calls_count_total{{caller="{caller}",function="{function_name}",module="test_decorator",objective_name="",objective_percentile="",result="error"}} 1.0"""
+        assert total_count in data
+
+        for latency in ObjectiveLatency:
+            query = f"""function_calls_duration_bucket{{function="{function_name}",le="{latency.value}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
+            assert query in data
+
+        duration_count = f"""function_calls_duration_count{{function="{function_name}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
+        assert duration_count in data
+
+        duration_sum = f"""function_calls_duration_sum{{function="{function_name}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
+        assert duration_sum in data
+
+    @pytest.mark.asyncio
+    async def test_async_exception(self):
+        """This is a test that covers exceptions."""
+        caller = get_caller_function(depth=1)
+        assert caller is not None
+        assert caller != ""
+
+        function_name = error_async_function.__name__
+        wrapped_function = autometrics(error_async_function)
+
+        # Test that the function is *still* async after we wrap it
+        assert asyncio.iscoroutinefunction(wrapped_function) == True
+
+        with pytest.raises(RuntimeError) as exception:
+            await wrapped_function()
+        assert "This is a test error" in str(exception.value)
+
+        # get the metrics
+        blob = generate_latest()
+        assert blob is not None
+        data = blob.decode("utf-8")
+
+        total_count = f"""function_calls_count_total{{caller="{caller}",function="{function_name}",module="test_decorator",objective_name="",objective_percentile="",result="error"}} 1.0"""
+        assert total_count in data
+
+        for latency in ObjectiveLatency:
+            query = f"""function_calls_duration_bucket{{function="{function_name}",le="{latency.value}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
+            assert query in data
 
-    duration_sum = f"""function_calls_duration_sum{{function="{function_name}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
-    assert duration_sum in data
+        duration_count = f"""function_calls_duration_count{{function="{function_name}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
+        assert duration_count in data
 
-    duration_created = f"""function_calls_duration_created{{function="{function_name}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
-    assert duration_created in data
+        duration_sum = f"""function_calls_duration_sum{{function="{function_name}",module="test_decorator",objective_latency_threshold="",objective_name="",objective_percentile=""}}"""
+        assert duration_sum in data
```

### Comparing `autometrics-0.4/src/autometrics/utils.py` & `autometrics-0.5/src/autometrics/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,12 +36,20 @@
     for key, value in urls.items():
         docs = f"{docs}{key} : {value} \n\n"
 
     docs = f"{docs}-------------------------------------------\n"
     return docs
 
 
+def append_docs_to_docstring(func, func_name, module_name):
+    """Helper for appending docs to a function's docstring."""
+    if func.__doc__ is None:
+        return write_docs(func_name, module_name)
+    else:
+        return f"{func.__doc__}\n{write_docs(func_name, module_name)}"
+
+
 def get_caller_function(depth: int = 2):
     """Get the name of the function. Default depth is 2 to get the caller of the caller of the function being decorated."""
     caller_frame = inspect.stack()[depth]
     caller_function_name = caller_frame[3]
     return caller_function_name
```

### Comparing `autometrics-0.4/PKG-INFO` & `autometrics-0.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: autometrics
-Version: 0.4
+Version: 0.5
 Summary: Easily add metrics to your system – and actually understand them using automatically customized Prometheus queries
 Home-page: https://github.com/autometrics-dev/autometrics-py
 License: MIT OR Apache-2.0
 Keywords: metrics,telemetry,prometheus,monitoring,observability,instrumentation
 Author: Fiberplane
 Author-email: info@fiberplane.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: opentelemetry-api (>=1.17.0,<2.0.0)
+Requires-Dist: opentelemetry-exporter-prometheus (>=1.12.0rc1,<2.0.0)
+Requires-Dist: opentelemetry-sdk (>=1.17.0,<2.0.0)
 Requires-Dist: prometheus-client (==0.16.0)
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/autometrics-dev/autometrics-py
 Description-Content-Type: text/markdown
 
 ![GitHub_headerImage](https://user-images.githubusercontent.com/3262610/221191767-73b8a8d9-9f8b-440e-8ab6-75cb3c82f2bc.png)
@@ -35,18 +38,19 @@
 
 ## Features
 
 - ✨ `autometrics` decorator instruments any function or class method to track the
   most useful metrics
 - 💡 Writes Prometheus queries so you can understand the data generated without
   knowing PromQL
-- 🔗 Create links to live Prometheus charts directly into each functions docstrings (with tooltips coming soon!)
-- 📊 (Coming Soon!) Grafana dashboard showing the performance of all
-  instrumented functions
-- 🚨 Enable Prometheus alerts using SLO best practices from simple annotations in your code
+- 🔗 Create links to live Prometheus charts directly into each function's docstring
+- [🔍 Identify commits](#identifying-commits-that-introduced-problems) that introduced errors or increased latency
+- [🚨 Define alerts](#alerts--slos) using SLO best practices directly in your source code
+- [📊 Grafana dashboards](#dashboards) work out of the box to visualize the performance of instrumented functions & SLOs
+- [⚙️ Configurable](#metrics-libraries) metric collection library (`opentelemetry`, `prometheus`, or `metrics`)
 - ⚡ Minimal runtime overhead
 
 ## Using autometrics-py
 
 - Set up a [Prometheus instance](https://prometheus.io/download/)
 - Configure prometheus to scrape your application ([check our instructions if you need help](https://github.com/autometrics-dev#5-configuring-prometheus))
 - Include a .env file with your prometheus endpoint `PROMETHEUS_URL=your endpoint`. If this is not defined, the default endpoint will be `http://localhost:9090/`
@@ -64,14 +68,18 @@
 
 - To access the PromQL queries for your decorated functions, run `help(yourfunction)` or `print(yourfunction.__doc__)`.
 
 - To show tooltips over decorated functions in VSCode, with links to Prometheus queries, try installing [the VSCode extension](https://marketplace.visualstudio.com/items?itemName=Fiberplane.autometrics).
 
 > Note that we cannot support tooltips without a VSCode extension due to behavior of the [static analyzer](https://github.com/davidhalter/jedi/issues/1921) used in VSCode.
 
+## Dashboards
+
+Autometrics provides [Grafana dashboards](https://github.com/autometrics-dev/autometrics-shared#dashboards) that will work for any project instrumented with the library.
+
 ## Alerts / SLOs
 
 Autometrics makes it easy to add Prometheus alerts using Service-Level Objectives (SLOs) to a function or group of functions.
 
 In order to receive alerts you need to add a set of rules to your Prometheus set up. You can find out more about those rules here: [Prometheus alerting rules](https://github.com/autometrics-dev/autometrics-shared#prometheus-recording--alerting-rules). Once added, most of the recording rules are dormant. They are enabled by specific metric labels that can be automatically attached by autometrics.
 
 To use autometrics SLOs and alerts, create one or multiple `Objective`s based on the function(s) success rate and/or latency, as shown below. The `Objective` can be passed as an argument to the `autometrics` macro to include the given function in that objective.
@@ -121,14 +129,36 @@
 ```py
 @autometrics
 @noop
 def api_handler():
   # ...
 ```
 
+#### Metrics Libraries
+
+Configure the crate that autometrics will use to produce metrics by using one of the following feature flags:
+
+- `opentelemetry` - (enabled by default, can also be explicitly set using the AUTOMETRICS_TRACKER="OPEN_TELEMETERY" env var) uses
+- `prometheus` - (using the AUTOMETRICS_TRACKER env var set to "PROMETHEUS")
+
+## Identifying commits that introduced problems
+
+> **NOTE** - As of writing, `build_info` will not work correctly when using the default tracker (`AUTOMETRICS_TRACKER=OPEN_TELEMETRY`).
+> This will be fixed once the following PR is merged on the opentelemetry-python project: https://github.com/open-telemetry/opentelemetry-python/pull/3306
+>
+> autometrics-py will track support for build_info using the OpenTelemetry tracker via #38
+
+Autometrics makes it easy to identify if a specific version or commit introduced errors or increased latencies.
+
+It uses a separate metric (`build_info`) to track the version and, optionally, git commit of your service. It then writes queries that group metrics by the `version` and `commit` labels so you can spot correlations between those and potential issues.
+
+The `version` is read from the `AUTOMETRICS_VERSION` environment variable, and the `commit` value uses the environment variable `AUTOMETRICS_COMMIT`.
+
+This follows the method outlined in [Exposing the software version to Prometheus](https://www.robustperception.io/exposing-the-software-version-to-prometheus/).
+
 ## Development of the package
 
 This package uses [poetry](https://python-poetry.org) as a package manager, with all dependencies separated into three groups:
 
 - root level dependencies, required
 - `dev`, everything that is needed for development or in ci
 - `examples`, dependencies of everything in `examples/` directory
@@ -156,9 +186,11 @@
 ```sh
 # Formatting using black
 poetry run black .
 # Lint using pyright
 poetry run pyright
 # Run the tests using pytest
 poetry run pytest
+# Run a single test, and clear the cache
+poetry run pytest --cache-clear -k test_tracker
 ```
```

